---
source-git-commit: 8ed1e6853c9f844c72431dc692b556ece9c215a8
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---
## Scopo

Aiuta gli assistenti alla codifica IA a apportare piccole modifiche sicure all’archivio della documentazione di GenStudio for Performance Marketing.

## Architettura di alto livello (breve)
- Questo repository è un sito di documentazione composto da Markdown in `help/` con inclusioni condivise in `help/_includes/` e immagini curate in `help/_includes/assets/`.
- Le note sulla versione, la guida utente e il contenuto di estensibilità sono disponibili in `help/`. Le modifiche di grandi dimensioni ai contenuti devono preservare la materia prima e la struttura di intestazione esistente.
- Il sito viene creato utilizzando Jekyll e ospitato su GitHub Pages. Il processo di build utilizza le convenzioni Jekyll standard con alcuni plug-in personalizzati.

## Convenzioni specifiche per il progetto
- Regole cursore: l&#39;automazione personalizzata e la guida risiedono in `.cursor/rules/*.mdc`. Esempi: `.cursor/rules/docs-lint.mdc` (processo lint), `.cursor/rules/generate-release-notes.mdc` (formato note sulla versione). Segui questi passaggi per le attività automatizzate.
- Nomi di file e contenuti anteriori:
   - Le note sulla versione richiedono un frontmatter specifico (vedere `.cursor/rules/generate-release-notes.mdc`).
   - Utilizza kebab-case per i file di regole e l&#39;estensione `.mdc`.
- Convenzioni di formattazione: i documenti utilizzano Markdown aromatizzato su GitHub. I titoli seguono generalmente lettere maiuscole e minuscole e brevi paragrafi. Preferisci i punti elenco `*` per gli elenchi nelle note sulla versione e `###` per le sezioni delle funzionalità.

## Linee guida sullo stile della documentazione
- Segui la [Guida allo stile di scrittura di Microsoft](https://learn.microsoft.com/en-us/style-guide/) per le best practice per la documentazione tecnica:
   - Scrivere frasi chiare e concise incentrate sulle azioni degli utenti
   - Usa la voce attiva e il presente teso
   - Suddividere il testo in blocchi brevi e analizzabili
   - Mantenere un tono caldo e diretto mantenendo la precisione tecnica
- Authoring Markdown:
   - Usa maiuscole/minuscole per le intestazioni (solo prima parola in maiuscolo)
   - Mantieni i paragrafi brevi (2-3 frasi) per maggiore leggibilità
   - Aggiungere righe vuote prima e dopo intestazioni ed elenchi
   - Utilizzare i backtick per elementi dell’interfaccia utente, percorsi di file e codice
   - Includi testo alternativo per tutte le immagini
   - Collegamento a sezioni specifiche tramite testo descrittivo

## Norme di sicurezza per le modifiche (cosa dovrebbe fare l’intelligenza artificiale)
- Non aggiungere mai Jira ID, collegamenti interni o riferimenti ai soli documenti pubblici all’interno dell’azienda. Consulta la sezione &quot;Tracciamento dei problemi&quot; di `generate-release-notes.mdc`.
- Mantenere YAML come frontmatter durante la modifica di file che lo includono. Molti modelli e note sulla versione si basano su chiavi fisse (titolo, descrizione, ruolo, exl-id).
- Per le correzioni di testo, preferisci modifiche automatizzate e idempotenti da `.cursor/rules/docs-lint.mdc` (rimuovi gli spazi finali, assicurati che la nuova riga sia finale). Comandi di esempio utilizzati dagli esseri umani:

```sh
sed -i '' 's/ $//' <file>
sed -i '' '$ { /^$/d; }' <file> && echo "" >> <file>
```

## Esempi (cosa modificare e come)
- Correzioni di piccole copie: aggiorna il testo all&#39;interno di `help/` file Markdown, mantieni intatte le intestazioni e gli ancoraggi.
- Aggiornamenti immagine: immagini di riferimento in `help/_includes/assets/`. Non spostare o rinominare le immagini senza aggiornare tutti i riferimenti.

## Dove cercare per primo
- `help/_includes/`: frammenti e immagini condivisi.
- `.cursor/rules/` - guida all&#39;automazione e alla stampa; utilizzare queste regole come regole autorevoli per la formattazione e i processi.
- `markdownlint_custom.json` — sostituzioni markdownlint locali.
- `.github/pull_request_template.md` - Previsioni PR.

## Quando chiedere all&#39;uomo
- Se una modifica richiede l’esecuzione o la modifica di strumenti basati su Docker (la regola di collegamento menziona Docker) o influisce sulle pipeline di creazione del sito.
- Se un file fa riferimento a una configurazione esterna sconosciuta (ad esempio `markdownlint.json`), chiedere se creare o ignorare.

## Comandi minimi per gli esseri umani

```sh
# Install linter (if not present)
npm install -g markdownlint-cli

# Run lint locally using project config
markdownlint --config markdownlint_custom.json "help/**/*.md"

# Project lint via yarn (preferred if available in environment)
yarn lint
```

---
Se lo desideri, posso unirlo in `.github/copilot-instructions.md` nell&#39;archivio (o modificare la formulazione/lunghezza). Cosa devo modificare o aggiungere?
