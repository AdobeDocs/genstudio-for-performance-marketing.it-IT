---
source-git-commit: f6a305c6a4e700525b570bbe280e5d1049d06537
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 6%

---
# Riferimento: authoring delle note sulla versione

## Frontmatter

La pagina live [help/user-guide/release-notes.md](../../help/user-guide/release-notes.md) include metadati di Experience League oltre a un set minimo (ad esempio `TQID`, `product_v2`, `feature_v2`, ID tassonomia).

**Regole:**

- Durante la modifica del contenuto della nota sulla versione **body**, **mantieni le chiavi e i valori esistenti**, a meno che l&#39;attività non richieda esplicitamente di modificare i metadati.
- Non eliminare la tassonomia o i metadati di prodotto per farli corrispondere a un modello più breve.
- I concetti richiesti per le pagine ExL in genere includono `title`, `description` e `role`; segui [le indicazioni sui metadati di Experience League](https://experienceleague.adobe.com/en/docs/authoring-guide/using/authoring/using-metadata) per le nuove pagine.

## Sorgenti interne (KT e wiki sulla versione)

Utilizza questi campi **solo durante la creazione di**; le note sulla versione pubblicate non devono fare riferimento a documenti interni.

### Documenti di trasferimento delle conoscenze (KT)

Estrai da:

| Campo | Utilizzo |
|-------|-----|
| Descrizione | Spiegazione della funzione core |
| Passo di elevazione | Proposta di valore |
| Funzionalità fornite | Comportamento concreto |
| Dichiarazione di problema | Perplessità dell&#39;utente |
| Tipo di versione e data | Timing |

### Rilasciare pagine wiki

Raggruppa e ambito per:

| Campo | Utilizzo |
|-------|-----|
| Data di rilascio (versione fissa) | Stessa data → stesso batch di note sulla versione |
| Iniziativa | Solo contesto; non collegare internamente nel testo pubblico |
| PM presenta la funzione utilizzando KT | Segnali possono esistere dettagli KT più profondi |

**Regola ambito:** gli elementi che condividono la stessa data di rilascio (versione corretta) appartengono allo stesso blocco di rilascio mensile.

## Collegamento alla documentazione

- Collega alla frase **più rilevante** (ad esempio, collega le &quot;risorse video e immagini non supportate&quot; alla sezione formati annuncio).
- Preferisci `#anchor` collegamenti nella sottosezione a destra.
- Le pagine di panoramica sono accettabili quando non esiste un ancoraggio più profondo.

## Percorsi comuni della documentazione

| Area | Prefisso percorso |
|------|-------------|
| Crea | `/help/user-guide/create/` |
| Contenuto | `/help/user-guide/content/` |
| Attivazione | `/help/user-guide/activation/` |
| Approvazioni | `/help/user-guide/approvals/` |
| Approfondimenti | `/help/user-guide/insights/` |
| Linee guida | `/help/user-guide/guidelines/` |
| Modelli | `/help/user-guide/templates/` |
| Campagne | `/help/user-guide/campaigns/` |
| Estensibilità | `/help/extensibility/` |
