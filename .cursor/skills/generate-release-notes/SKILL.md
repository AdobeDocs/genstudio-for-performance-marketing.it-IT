---
name: generate-release-notes
description: ""
source-git-commit: 1a33b08048233c5f9a82b5f428082aa5c71b0052
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---


# Genera note sulla versione di GenStudio

**File di destinazione canonico:** [help/user-guide/release-notes.md](help/user-guide/release-notes.md)

**Esempi completi:** [examples.md](examples.md)

**Mapping campi KT/wiki e percorsi documenti:** [reference.md](reference.md)

## Elenco di controllo del flusso di lavoro

Lavora in questo ordine. Copia l’elenco di controllo e tieni traccia dell’avanzamento per le modifiche in più passaggi.

1. [ ] Aprire `help/user-guide/release-notes.md` e leggere il blocco `## YYYY.MM {#latest}` corrente e l&#39;area **Note sulla versione precedenti**.
2. [ ] Se si aggiunge una versione mensile di **new**: archiviare l&#39;ultima versione corrente (vedere [Archiviare l&#39;ultima versione precedente](#archive-previous-latest)).
3. [ ] Aggiungi o modifica la prima sezione `## YYYY.MM {#latest}` (ultimo mese in cima all&#39;elenco delle versioni).
4. [ ] Per ogni elemento, applica [Regole di decisione](#decision-rules) (funzionalità `###` rispetto a **Correzioni e miglioramenti**, badge Beta o meno).
5. [ ] Aggiungi o verifica i collegamenti alla documentazione sulla frase più rilevante (vedi [reference.md](reference.md#documentation-linking)).
6. [ ] Eseguire [controlli di qualità](#quality-checks) prima di terminare.
7. [ ] Mantenere [frontmatter](reference.md#frontmatter) sulla pagina a meno che l&#39;attività non aggiorni esplicitamente i metadati.

## Regole di decisione

Utilizza queste regole &quot;if/then&quot; per indirizzare il contenuto al posto giusto:

| Se | Then |
|----|------|
| Questa funzionalità è nuova e disponibile in Beta | Aggiungi la riga del badge di Beta immediatamente sotto l&#39;intestazione `###` (vedi [examples.md](examples.md)). |
| Il materiale Source definisce esplicitamente l&#39;elemento come **correzione** o **miglioramento** | Inseriscilo in `### Fixes and enhancements` solo con `*` punti elenco. |
| L&#39;elemento è una nuova funzionalità o una storia di funzionalità | Utilizza una sezione di funzionalità `###` con 1-3 frasi (non l&#39;elenco delle correzioni). |
| Non sei sicuro se qualcosa sia una correzione o una feature | Impostazione predefinita per una sezione di funzionalità `###` a meno che l&#39;origine non indichi chiaramente la correzione/miglioramento. |

**Correzioni della regola di sezione:** Non aggiungere punti elenco a **Correzioni e miglioramenti** a meno che l&#39;origine non sia esplicitamente etichettata come correzione o miglioramento.

## Archivia più recente precedente

Quando si introduce un nuovo `## YYYY.MM {#latest}`:

1. Taglia l&#39;intera sezione `## YYYY.MM {#latest}` precedente (dal titolo fino alla fine del contenuto di quella versione, prima delle `##` o **note sulla versione precedente**).
2. Incollalo in **Note sulla versione precedenti**, all&#39;interno di un blocco comprimibile.
3. Sostituire il titolo precedente con: `+++Notes from YYYY.MM.DD+++` (utilizzare la data di rilascio effettiva; formattare come nelle note esistenti nel file).
4. Rimuovi `{#latest}` dall&#39;intestazione archiviata. La nuova sezione superiore è l&#39;unica con `{#latest}`.
5. Mantieni l&#39;ordine cronologico nelle **note sulla versione precedenti** (i blocchi archiviati più recenti vengono spostati nella parte superiore a meno che il file non utilizzi già un ordine diverso—**corrisponde al file esistente**).

## Struttura richiesta

### Titolo pagina e introduzione

Dopo la materia prima, usare:

```markdown
# GenStudio for Performance Marketing release notes

This release information details the latest updates to the GenStudio for Performance Marketing application.
```

Se il file utilizza già una frase introduttiva leggermente diversa (ad esempio, &quot;fornisce&quot; invece di &quot;dettagli&quot;), assicurati di mantenere la coerenza con il resto della pagina.

### Intestazione ultima versione

- Formato: `## YYYY.MM {#latest}` per il blocco della versione più recente.
- Un solo ancoraggio `{#latest}` sulla pagina.

### Sezioni delle feature

- Utilizza `###` per le categorie di funzionalità principali.
- Il presente è teso, 1-3 frasi, chiarisce cosa/perché e le azioni degli utenti laddove utili.
- Nomi di prodotto: `[!DNL Create]`, `[!DNL Content]`, `[!DNL Insights]`, ecc.
- Interfaccia utente: `[!UICONTROL Control Name]` dove appropriato.
- Enfasi: `_italics_` per aree/sezioni dell&#39;interfaccia utente; `**bold**` per i termini chiave con moderazione.

### Badge Beta

Utilizza esattamente:

```markdown
[!BADGE Beta]{type=Informative tooltip="This feature is currently in Beta, so some functionality may be limited or subject to change."}
```

### Collegamenti alla documentazione

- Pattern: `[link text](/help/user-guide/section/page.md#anchor)`
- Preferisci gli ancoraggi; collega la frase desiderata agli utenti, non &quot;fai clic qui&quot;.

### Correzioni di problemi e miglioramenti

- Le righe punto elenco utilizzano `*`.
- Solo gli elementi etichettati in modo esplicito come correzione/miglioramento nel materiale sorgente.
- Stesse convenzioni di collegamento e terminologia delle funzioni.

## Contenuto vietato

- **non** includere chiavi Jira, numeri di problemi interni, URL interni o collegamenti wiki aziendali nelle note sulla versione pubblicate.
- **not** cita documenti, ticket o strumenti interni per il trasferimento delle conoscenze come prova: riepiloga solo i risultati che l&#39;utente sta ottenendo.
- **non** duplicare `{#latest}` in più sezioni.

## Controlli di qualità

Prima di completare l&#39;attività:

- [ ] Tutti i collegamenti relativi nuovi o modificati vengono risolti in percorsi reali in `help/` dove possibile.
- [ Le funzionalità di Beta ] includono lo snippet di badge Beta, se necessario.
- [ ] La terminologia corrisponde alle note sulla versione esistenti (`[!DNL …]`, `[!UICONTROL …]`).
- [ ] Analizzare la bozza per rilevare ID interni accidentali (`[A-Z]+-\d+`), URL wiki o linguaggio &quot;see Jira&quot;. Rimuoverli.
- [ ] **Correzioni e miglioramenti** contiene solo correzioni/miglioramenti etichettati in modo esplicito.
- [ ] L&#39;ultima sezione precedente è stata archiviata correttamente all&#39;aggiunta di un nuovo mese.

## Origini di contenuto (riepilogo)

Quando si estrae dalla documentazione di Trasferimento conoscenze o si rilasciano wiki internamente, mappare i campi come descritto in [reference.md](reference.md#internal-sources-kt-and-release-wikis). La pagina spedita deve essere letta come documentazione utente autonoma.

## Facoltativo: lucidare le nuove sottosezioni

Dopo aver aggiunto il nuovo contenuto `###` in `{#latest}`, esegui [le note sulla versione polacche](../polish-release-notes/SKILL.md) per un passaggio in stile redattore di testo (tono di avanzamento beneficio, **2-3 frasi per paragrafo**, nessuna procedura guidata) **only** su quelle **nuove** sottosezioni—**not** nelle note sulla versione precedenti o testo preesistente, a meno che non sia esplicitamente richiesto.

## Risorse aggiuntive

- [examples.md](examples.md) — esempi pronti per l&#39;inserimento (funzionalità, correzioni, blocco di archiviazione).
- [reference.md](reference.md) — note di argomento, percorsi di documentazione, strategia di collegamento.
- [Note sulla versione polacca](../polish-release-notes/SKILL.md) — passaggio editoriale facoltativo per `###` appena aggiunto in `{#latest}`.
