---
name: consume-release-sources
description: ""
source-git-commit: c3c6aa86f4f520d020f8928612d1be6be1599652
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 1%

---


# Consumare le fonti di rilascio (Jira + Confluence MCP)

**Redazione a valle:** [generate-release-notes](../generate-release-notes/SKILL.md) → [polish-release-notes](../polish-release-notes/SKILL.md) opzionale

**Riferimento di analisi:** [reference.md](reference.md)

**File di output di destinazione (solo a valle):** [help/user-guide/release-notes.md](../../help/user-guide/release-notes.md)

## Prerequisiti

- **Jira MCP** (`jira_getIssue`, `jira_searchIssues`) autenticato
- **Autenticazione MCP** (`confluence_getContent`, `confluence_searchContent`)
- Chiave ticket Jira dal nome della filiale (`GS-#####`), input utente o descrizione ticket

## Elenco di controllo del flusso di lavoro

1. [ ] **Risolvi ticket Jira** — `jira_getIssue` con `issueKey`. Leggi `description` per il collegamento wiki della cerimonia e il mese di rilascio.
2. [ ] **Individua pagina cerimonia**. Utilizzare l&#39;URL wiki del ticket. CQL di fallback: `title ~ "YYYY/MM Release Ceremony" AND space = GenStudio`.
3. [ ] **Recupero del corpo della cerimonia** - `confluence_getContent` con `bodyMode: storage` (obbligatorio; `text` perde i collegamenti KT e la struttura della tabella).
4. [ ] **Analizza gruppi di funzionalità** — Estrai righe da **Funzionalità rilascio GA** e **Funzionalità rilascio Beta** (vedi [reference.md](reference.md#ceremony-feature-groups)).
5. [ ] **Applica filtro di inclusione** — per ambito utente (vedi [reference.md](reference.md#inclusion-filters)); conferma conteggio righe Beta (potrebbe essere zero).
6. [ ] **Risolvi pagine KT** — `confluence_searchContent` per titolo KT; `confluence_getContent` con `bodyMode: text`.
7. [ ] **Estrai campi KT** — Descrizione, passo di elevazione, funzionalità distribuite, istruzione di problema, tipo di rilascio e data.
8. [ ] **Imposta flag Beta** - `requiresBetaBadge: true` per righe di sezione Beta o righe di tabella GA con tipo `Beta`.
9. [ ] **Scollegare** a [generate-release-notes](../generate-release-notes/SKILL.md) con elenco di righe strutturato (nessun riferimento wiki/Jira nella copia spedita).

## Etichettatura Beta (handoff per generare abilità)

Quando `requiresBetaBadge: true`, la sezione `###` a valle deve includere immediatamente sotto l&#39;intestazione:

```markdown
[!BADGE Beta]{type=Informative tooltip="This feature is currently in Beta, so some functionality may be limited or subject to change."}
```

Non aggiungere liberatoria per la pianificazione in corsivo per Beta; il badge è il pattern supportato.

## Non consentito nelle note sulla versione spedite

Gli ID interni, gli URL wiki, le citazioni KT e le chiavi Jira rimangono solo in questa fase di acquisizione. Riepiloga i risultati rivolti all&#39;utente nella pagina pubblica per [contenuto non consentito](../generate-release-notes/SKILL.md#prohibited-content) generato-note sulla versione.

## Regresso

Se le chiamate MCP non riescono, chiedi all&#39;utente di incollare la cerimonia e il contenuto KT, quindi continua con generate-release-notes utilizzando [reference.md KT field mapping](../generate-release-notes/reference.md#internal-sources-kt-and-release-wikis).

## Risorse aggiuntive

- [reference.md](reference.md) — analisi delle cerimonie, CQL, filtri di inclusione, parametri MCP
- [generate-release-notes](../generate-release-notes/SKILL.md) — archivia, bozza, collegamenti, controlli di qualità
- [polish-release-notes](../polish-release-notes/SKILL.md) — passaggio editoriale sul nuovo `###` in `{#latest}`
