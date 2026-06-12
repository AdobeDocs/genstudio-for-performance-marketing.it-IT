---
name: generate-release-notes
description: ""
source-git-commit: c3c6aa86f4f520d020f8928612d1be6be1599652
workflow-type: tm+mt
source-wordcount: '957'
ht-degree: 0%

---


# Genera note sulla versione di GenStudio

**File di destinazione canonico:** [help/user-guide/release-notes.md](help/user-guide/release-notes.md)

**Esempi completi:** [examples.md](examples.md)

**Mapping campi KT/wiki e percorsi documenti:** [reference.md](reference.md)

## Ambito di modifica (rigido)

Quando utilizzi questa abilità, **l&#39;unico luogo** in cui puoi **aggiungere** o **modificare** il contenuto del corpo della nota sulla versione è la sezione con **`## … {#latest}`** (il singolo blocco che contiene l&#39;ancoraggio `{#latest}`).

- **Non** modificare le **Note sulla versione precedenti** (blocchi comprimibili `+++Notes from YYYY.MM.DD+++`) o **qualsiasi** sezione mensile precedente `##` che non contiene più `{#latest}`, anche quando l&#39;argomento sembra correlato, un collegamento non funziona correttamente oppure la copia risulta duplicata o obsoleta.
- **Non** &quot;ritoccare&quot; precedenti a `###` sottosezioni, punti elenco, collegamenti o parole al di fuori del blocco `{#latest}` corrente a meno che l&#39;utente non fornisca una richiesta **esplicita e separata** non coperta da questa abilità.
- **Eccezione:** [Archivia le ultime](#archive-previous-latest) precedenti quando introduci un blocco **new** principale `{#latest}`: **sposta** l&#39;intera sezione `{#latest}` precedente in una **new** comprimibile in **Note sulla versione precedenti** come descritto di seguito. Durante questo passaggio, **non riscrivere o aggiungere** a **altri blocchi di archivio precedenti**.

Se le nuove informazioni appartengono al documento, inserirle nell&#39;intestazione **`{#latest}`** corrente (o archiviarle per prime, quindi aggiungerle solo al nuovo `{#latest}`).

## Elenco di controllo del flusso di lavoro

Lavora in questo ordine. Copia l’elenco di controllo e tieni traccia dell’avanzamento per le modifiche in più passaggi.

&#x200B;0. [ ] Se sono disponibili **Jira** e **Confluence** MCP, esegui [consume-release-sources](../consume-release-sources/SKILL.md) per acquisire prima il ticket di lavoro, i gruppi di funzioni wiki per le cerimonie (GA e Beta) e le pagine KT. Se MCP non è disponibile, utilizza il contenuto KT/wiki incollato e la mappatura del campo [reference.md](reference.md#internal-sources-kt-and-release-wikis).
1. [ ] Aprire `help/user-guide/release-notes.md` e leggere il blocco `## YYYY.MM {#latest}` corrente. Considera le **note sulla versione precedenti** come **contesto di sola lettura** a meno che non si esegua il passaggio di archiviazione nel passaggio 2.
2. [ ] Se si aggiunge una versione mensile di **new**: archiviare l&#39;ultima versione corrente (vedere [Archiviare l&#39;ultima versione precedente](#archive-previous-latest)).
3. [ ] Aggiungi o modifica **solo** la prima sezione `## YYYY.MM {#latest}` (ultimo mese in cima all&#39;elenco delle versioni).
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
2. Incollalo in **Note sulla versione precedenti**, all&#39;interno di un blocco comprimibile **new**.
3. Sostituire il titolo precedente con: `+++Notes from YYYY.MM.DD+++` (utilizzare la data di rilascio effettiva; formattare come nelle note esistenti nel file).
4. Rimuovi `{#latest}` dall&#39;intestazione archiviata. La nuova sezione superiore è l&#39;unica con `{#latest}`.
5. Mantieni l&#39;ordine cronologico nelle **note sulla versione precedenti** (i blocchi archiviati più recenti vengono spostati nella parte superiore a meno che il file non utilizzi già un ordine diverso—**corrisponde al file esistente**).

**non** modificare il corpo di **blocchi preesistenti** `+++Notes from …+++` durante l&#39;esecuzione dell&#39;archivio. Inserire solo il blocco appena archiviato e conservare gli archivi meno recenti così come sono.

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

- [ ] **Ambito:** Solo il blocco `## … {#latest}` è stato aggiunto o modificato; **Le note sulla versione precedenti** e le sezioni mensili precedenti non sono state modificate ad eccezione del [Archivia le versioni precedenti più recenti](#archive-previous-latest) tagliate/incollate del precedente `{#latest}` in un blocco di archivio **nuovo**.
- [ ] Tutti i collegamenti relativi nuovi o modificati vengono risolti in percorsi reali in `help/` dove possibile.
- [ Le funzionalità di Beta ] includono lo snippet di badge Beta, se necessario.
- [ ] La terminologia corrisponde alle note sulla versione esistenti (`[!DNL …]`, `[!UICONTROL …]`).
- [ ] Analizzare la bozza per rilevare ID interni accidentali (`[A-Z]+-\d+`), URL wiki o linguaggio &quot;see Jira&quot;. Rimuoverli.
- [ ] **Correzioni e miglioramenti** contiene solo correzioni/miglioramenti etichettati in modo esplicito.
- [ ] L&#39;ultima sezione precedente è stata archiviata correttamente all&#39;aggiunta di un nuovo mese.

## Origini di contenuto (riepilogo)

Quando **Jira/Confluence MCP** è disponibile, inizia con [consume-release-sources](../consume-release-sources/SKILL.md) (le pagine wiki → KT → handoff strutturato). In caso contrario, mappare i campi wiki di trasferimento o rilascio delle conoscenze incollati come descritto in [reference.md](reference.md#internal-sources-kt-and-release-wikis). La pagina spedita deve essere letta come documentazione utente autonoma.

## Facoltativo: lucidare le nuove sottosezioni

Dopo aver aggiunto il nuovo contenuto `###` in `{#latest}`, esegui [le note sulla versione polacche](../polish-release-notes/SKILL.md) per un passaggio in stile redattore di testo (tono di avanzamento beneficio, **2-3 frasi per paragrafo**, nessuna procedura guidata) **only** su quelle **nuove** sottosezioni—**not** nelle note sulla versione precedenti o testo preesistente, a meno che non sia esplicitamente richiesto.

## Risorse aggiuntive

- [examples.md](examples.md) — esempi pronti per l&#39;inserimento (funzionalità, correzioni, blocco di archiviazione).
- [reference.md](reference.md) — note di argomento, percorsi di documentazione, strategia di collegamento.
- [Note sulla versione polacca](../polish-release-notes/SKILL.md) — passaggio editoriale facoltativo per `###` appena aggiunto in `{#latest}`.
