---
source-git-commit: c3c6aa86f4f520d020f8928612d1be6be1599652
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 3%

---
# Riferimento: utilizzare le origini di rilascio (MCP)

## Individuazione pagina Cerimonia

| Pattern | Esempio |
|---------|---------|
| Titolo | `YYYY/MM Release Ceremony` nello spazio **GenStudio** |
| Da Jira | Collegamento wiki nel ticket `description` (preferito) |
| Fallback CQL | `title ~ "2026/06 Release Ceremony" AND space = GenStudio` |

## Gruppi di funzioni Cerimonia

I wiki per le cerimonie di rilascio contengono fino a **due** tabelle delle funzioni. Analizza entrambi da **storage** HTML.

### Funzioni della versione GA

- Intestazione sezione: `GA Release Features` (`<h2>`)
- Sottotitolo: `Feature Group:` con collegamento Floodgate facoltativo
- Le colonne della tabella includono **Tipo** (`GA`, `Limited`, `EA`, `Beta` o vuote)
- **Documentazione KT** colonna: `<ac:link><ri:page ri:content-title="..."/></ac:link>`

Estrazione per riga:

| Campo | Origine |
|-------|--------|
| `featureDescription` | Primi `<td>` nella riga di dati |
| `type` | Digita il testo della cella della colonna |
| `ktPageTitle` | `ri:content-title` nella colonna KT |
| `jiraKeys` | `ac:macro ac:name="jira"` → `key` parametro (solo interno) |
| `releaseTier` | `ga` quando Type è `GA`; eredita Type per altri valori di tabella GA |

### Funzioni della versione di Beta

- Intestazione sezione: `Beta Release Features` (potrebbe essere **assente** in alcuni mesi)
- Seconda tabella; **nessuna colonna Tipo** — ogni riga è Beta
- Stessa estrazione KT e Jira della tabella GA
- Imposta `releaseTier: beta` e `requiresBetaBadge: true` su ogni riga della sezione Beta

Se manca la sezione Beta, non registrare righe Beta e continuare.

### Modelli di storage HTML

```html
<ac:link><ri:page ri:content-title="Translation on HZ Canvas" /></ac:link>
<ac:structured-macro ac:name="jira" ...><ac:parameter ac:name="key">GS-23218</ac:parameter></ac:structured-macro>
```

## Utilizzo dello strumento MCP

| Passaggio | Strumento | Parametri |
|------|------|------------|
| Ticket | `jira_getIssue` | `issueKey`, facoltativo `expand: renderedFields` |
| Cerimonia | `confluence_getContent` | `contentId`, `bodyMode: storage` |
| Ricerca KT | `confluence_searchContent` | `cql: title = "<KT title>" AND space = GenStudio` |
| Corpo KT | `confluence_getContent` | `contentId`, `bodyMode: text`, `maxBodyChars: 50000` |

**Non** utilizzare `bodyMode: text` per le pagine di cerimonia durante l&#39;analisi dei collegamenti KT.

## Mappatura campo KT (input di bozza)

Mappa in generate-release-notes; non incollare nelle note sulla versione pubbliche letteralmente.

| Sezione KT | Utilizzo |
|------------|-----|
| Descrizione | Funzionalità di base |
| Piazzola di elevazione | Proposta di valore |
| Funzionalità fornite | Comportamento concreto |
| Dichiarazione di problema | Dolore dell’utente (solo contesto) |
| Tipo di versione e data | GA / Beta / Limitato (interno); decisione di badge delle unità |

## Filtri di inclusione

Conferma l’ambito con l’utente quando non è chiaro. Predefiniti comuni:

| Predefinito | Include |
|--------|----------|
| `ga_only` | Righe tabella GA in cui Tipo = `GA` |
| `ga_and_beta` | **Impostazione predefinita consigliata per i mesi futuri** — Righe GA in cui Tipo = `GA` **più tutte** righe della tabella Caratteristiche di rilascio di Beta |
| `ga_plus_empty` | Tabella GA: Tipo = `GA` o Tipo vuoto |
| `all_except_pilot` | Righe tabella GA tranne `Limited`; più sezione Beta quando si utilizza `ga_and_beta` |
| `all_with_badges` | Tutte le righe della tabella GA; le righe della sezione Beta ricevono sempre il badge Beta |

## Distribuzione dei badge Beta

| Condizione | `requiresBetaBadge` |
|-----------|---------------------|
| Riga dalla tabella **Caratteristiche della versione di Beta** | `true` |
| Riga tabella GA con tipo = `Beta` | `true` |
| Riga tabella GA con tipo = `GA` | `false` |

A valle: [genera-note sulla versione Regole di decisione](../generate-release-notes/SKILL.md#decision-rules) e [snippet di badge Beta](../generate-release-notes/SKILL.md#beta-badge).

## Payload handoff (informale)

Passa a generate-release-notes come elenco di elementi:

```yaml
- featureDescription: "YouTube Shorts"
  releaseTier: ga
  requiresBetaBadge: false
  ktPageTitle: "YouTube Shorts (Create + Activate)"
  # extracted KT fields: description, elevatorPitch, featuresDelivered, ...
```
