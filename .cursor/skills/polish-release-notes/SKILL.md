---
name: polish-release-notes
description: ""
notes: refines only newly added
source-git-commit: 1a33b08048233c5f9a82b5f428082aa5c71b0052
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 0%

---


# Note sulla versione di GenStudio in polacco

**File di destinazione canonico:** [help/user-guide/release-notes.md](../../../help/user-guide/release-notes.md)

**Esempi:** [examples.md](examples.md)

**Flusso di lavoro di Drafting (a monte):** [generate-release-notes](../generate-release-notes/SKILL.md)

## Ambito (obbligatorio)

Contenuto polacco **only** identificato dall&#39;utente come **appena aggiunto** in questo turno:

- **Nel file:** `###` sottosezioni sotto l&#39;intestazione singola `## YYYY.MM {#latest}` in `help/user-guide/release-notes.md`.
- **Non** modificare il titolo della pagina, il paragrafo introduttivo, il frontmatter o il testo in **Note sulla versione precedenti** (blocchi `+++` comprimibili).
- **Non** modificare blocchi precedenti a `##` mensili o blocchi preesistenti di `###` nella stessa sezione `{#latest}` a meno che l&#39;utente **non lo chieda esplicitamente**.
- Se non è chiaro quali `###` siano nuovi, **chiedi** o usa **git diff** / modifica contesto prima di modificare prose.
- **Contenuto incollato:** lucida solo markdown incollato dall&#39;utente quando conferma che corrisponde alle **stesse** nuove sottosezioni (non trattare la funzione incolla non correlata come nell&#39;ambito).

Mantieni differenze **minime**: solo le parole e le interruzioni di paragrafo non vengono reimpostate in un&#39;altra posizione del file.

## Voce e tono

- Scrivi come **copywriter** per le note sulla versione del prodotto: **concise**, **scannable** e **energized** circa **new value**—lead con risultati e &quot;what’s in it for you&quot; (cosa contiene), utilizza verbi forti e un linguaggio dei benefici nitido.
- **Massima accuratezza:** nessuna rivendicazione oltre a quella offerta dalla funzionalità; abbina il tono di Experience League/Adobe (sicuro e chiaro, non sensazionalista).
- **Genera eccitazione** con **specifici** vantaggi e delta (ciò che gli addetti al marketing possono fare ora, ciò che viene rimosso dall&#39;attrito), non hype vuoto o superlativi non comprovati.

## Regole paragrafo

- Ogni paragrafo: **2-3 frasi**. **Non più di tre frasi** in un paragrafo. Se ne hai bisogno, inizia un **nuovo paragrafo**.
- Facoltativo: se un paragrafo continua a essere eseguito per più di **~3 righe** nei documenti sottoposti a rendering alla lunghezza tipica della riga, suddividerlo ulteriormente.

## Non aggiungere

- **Procedura &quot;come&quot;** contenuto: passaggi numerati, &quot;fai clic su **[!UICONTROL ...]**, quindi...&quot;, procedure dettagliate complete dell&#39;interfaccia utente o frasi del tutorial. Le note sulla versione riepilogano **ciò che è stato spedito** e **perché è importante**, non le lezioni pratiche.
- Contenuto che viola [Contenuto vietato](../generate-release-notes/SKILL.md#prohibited-content) per l&#39;abilità generata (nessuna chiave Jira, URL interni, wiki come bozza, ecc.).

## Mantieni (non eliminare o riscrivere strutturalmente)

- `[!DNL …]`, `[!UICONTROL …]`, `[!BADGE …]` e altri codici brevi ExL.
- **relativi** collegamenti alla documentazione e modelli di ancoraggio esistenti: `[phrase](/help/...)` su testo di ancoraggio significativo.
- I blocchi del badge di Beta corrispondono esattamente a quelli utilizzati in [esempi di generazione delle note sulla versione](../generate-release-notes/examples.md).

## Elenco di controllo del flusso di lavoro

1. [ ] Conferma **che** `###` in `## … {#latest}` sono nell&#39;ambito (nuovo questo turno).
2. [ ] Per ogni ambito `###`, stringere la copia per [Regole per voce e tono](#voice-and-tone) e [Regole per paragrafo](#paragraph-rules).
3. [ ] Rimuovi o riduci **istruzioni**; mantieni **risultati utente**.
4. [ ] Verificare che i collegamenti e i codici di scelta rapida siano ancora validi. Eseguire un&#39;analisi rapida per individuare gli ID interni o i pattern non consentiti per [controlli di qualità](#quality-checks).

## Controlli di qualità

- [ ] Solo i blocchi **new** `###` concordati in `{#latest}` sono cambiati; gli archivi e i mesi precedenti non sono stati toccati.
- [ ] Nessun nuovo ID in stile Jira, URL wiki interni o lingua &quot;see ticket&quot;.
- [ ] I paragrafi sono **2-3 frasi** ciascuno (massimo tre frasi per paragrafo).
- [ ] La copia rimane **effettiva** e allineata con la funzionalità descritta.

## Risorse aggiuntive

- [examples.md](examples.md) — pattern prima/dopo.
- [generate-release-notes](../generate-release-notes/SKILL.md): bozza, archiviazione, badge Beta, collegamento.
