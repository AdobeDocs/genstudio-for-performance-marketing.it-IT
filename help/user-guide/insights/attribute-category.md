---
title: Categorie di attributi
description: Scopri le categorie di attributi utilizzate in GenStudio for Performance Marketing.
feature: Insights, Attributes, Generative AI
recommendations: noDisplay
source-git-commit: 3b5fc55595f766db0327b6aefb0e29c3896e00c0
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 1%

---

# Categorie di attributi

Una categoria di attributi è un gruppo di classificazione che organizza attributi correlati che condividono una caratteristica comune. Queste categorie aiutano a semplificare l&#39;individuazione, l&#39;identificazione e la comprensione di attributi specifici fornendo un contesto più ampio e facilitandone l&#39;applicazione e l&#39;utilizzo.

GenStudio for Performance Marketing utilizza le funzionalità di intelligenza artificiale e machine learning di Adobe per studiare immagini, video e testo e applicare [!UICONTROL attributi di risorse] in base al livello di affidabilità. _Affidabilità_ si riferisce alla probabilità che l&#39;IA assegni a una previsione o classificazione. Nel contesto dell’apprendimento automatico, si tratta di una sorta di punteggio che misura quanto l’intelligenza artificiale sia &quot;sicura&quot; che la classificazione sia corretta. Maggiore è il punteggio di affidabilità, maggiore è la certezza. Ad esempio, durante l’analisi di un’immagine, l’intelligenza artificiale può identificare diverse funzioni e assegnare a ciascuna un punteggio che indica quanto sia sicura che la funzione sia corretta. L’elenco degli attributi di una risorsa non è esaustivo. Assets che contiene un set completo di funzioni può essere limitato a una soglia di affidabilità, ad esempio le tre funzioni più dominanti identificate.

## Funzioni immagine

Le funzionalità immagine rappresentano elementi o pattern distinti e informativi all&#39;interno di un&#39;immagine utilizzati per l&#39;analisi con [!DNL Insights]. Nella tabella seguente sono elencate le categorie di funzioni immagine riconosciute da GenStudio for Performance Marketing AI.

<!-- For the writer: turn off word wrap to work with these tables. Option + Z -->

| Categoria | Descrizione | Esempio |
| ----------------------- | ----------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Angolo videocamera | La posizione e l&#39;angolo della fotocamera rispetto al soggetto. |                                                                                                                                                                                |
| Distanza soggetto | La distanza tra la fotocamera e il soggetto di un&#39;immagine. | `close up`, `mid shot`, `long shot` |
| Impostazioni della telecamera | La configurazione dei controlli della telecamera per produrre l&#39;immagine. |                                                                                                                                                                                |
| Colore e tonalità | Valuta i colori utilizzati negli elementi immagine. Identifica da uno a tre colori da un set di 40 colori predefiniti nei seguenti livelli immagine:<br>**[!UICONTROL Colori di primo piano ]**—elementi nel livello anteriore dell&#39;immagine<br>**[!UICONTROL Colori di sfondo]**—elementi nel livello posteriore di un&#39;immagine<p>**[!UICONTROL Temperatura colore]** descrive il calore generale o la freddezza dei colori nell&#39;immagine.<br>Valori di tono o temperatura: `warm`, `cool`, `neutral` | ![colori e tonalità fredde](../../assets/category/image-color-temp.png){width="200" zoomable="yes"} |
| Stile immagine | Il trattamento visivo di un’immagine. |                                                                                                                                                                                |
| Condizioni di illuminazione | Tipo di luce in un&#39;immagine. |                                                                                                                                                                                |
| Oggetti | Identifica uno o più elementi, entità ed elementi che compongono l&#39;immagine. | ![girasole, piano, oggetto fiore](../../assets/category/image-objects.png){width="200" zoomable="yes"} |
| Orientamento | Posizione dell&#39;immagine rispetto alle proporzioni. | `landscape`, `portrait`, `square` |
| Persone | Se è presente almeno una persona, uno o più attributi possono descrivere la persona o le persone nell&#39;immagine. | ![donna che danza](../../assets/category/image-people.png){width="200" zoomable="yes"} |
| Generi fotografici | Rileva l&#39;oggetto e la tecnica utilizzati per acquisire un&#39;immagine, ad esempio `abstract` o `landscape` (diverso dall&#39;orientamento orizzontale). |           |
| Scene | Rileva l’impostazione o l’ambiente rappresentato in un’immagine. |                                             |
| Tag | Rileva oggetti, elementi e altre caratteristiche dell&#39;immagine che non rientrano in una classificazione specifica. |                                      |

<!-- Not yet approved by legal
| Attention distribution  | The level of viewer attention spread across an image.                                                 | `high`, `medium`, `low`                                                                                                                                                                                                    |
| Content density         | The amount of information or detail in an image.                                                      | `high`, `medium`, `low`                                                                                                                                                                                                    |
-->

## Funzioni video

Le caratteristiche dell&#39;immagine rappresentano elementi, suoni o pattern distinti e informativi all&#39;interno di un video per l&#39;analisi con [!DNL Insights]. Nella tabella seguente sono elencate le categorie di funzioni video riconosciute da GenStudio for Performance Marketing AI.

| Categoria | Descrizione | Esempio |
| ------------------- | ------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------- |
| Genere audio | Quando la musica è presente, il video potrebbe ricevere una classificazione dello stile musicale, ad esempio `electronic` o `classical`. |          |
| Categoria genere audio | In presenza di musica, il video potrebbe ricevere un&#39;ampia classificazione del genere musicale, ad esempio `acoustic` o `traditional`. |          |
| Modo audio | Descrive l&#39;atmosfera generale o il tono dell&#39;audio, ad esempio `relaxing` o `energetic`. |          |
| Tipi di audio | In presenza di audio, il video potrebbe ricevere un tag per uno o più tipi di audio, ad esempio `music` o `speech`. |          |
| Oggetti | Identifica uno o più elementi, entità ed elementi visualizzati nel video. | ![oggetti nel video](../../assets/category/video-objects.png){width="200" zoomable="yes"} |
| Orientamento | La posizione del video rispetto alle proporzioni del fotogramma. | `landscape`, `portrait`, `square` |
| Persone | Se è presente almeno una persona, uno o più attributi possono descrivere la persona o le persone nel video. |        |
| Scene | L’impostazione o l’ambiente illustrato nel video. |        |
| Stili | Rileva i trattamenti visivi applicati agli elementi del video, ad esempio `matte` o `neon`. |        |
| Tag | Rileva oggetti, elementi e altre caratteristiche video che non rientrano in una classificazione specifica. |        |

## Funzioni testo

Le caratteristiche del testo includono conteggi per alcuni elementi di testo, quali parole, frasi, emoticon e classificazioni per semantica, emozione e tono, utilizzati per l&#39;analisi con [!DNL Insights]. Il testo può inoltre ricevere un punteggio di leggibilità. In arrivo.

<!-- Not yet approved by legal

The following table lists the image feature categories recognized by the GenStudio for Performance Marketing AI.

| Category             | Description | Example |
|----------------------|-------------|--------|
| Emojis Count         |             |        |
| HashTags Count       |             |        |
| Keywords             |             |        |
| Marketing Emotions   |             |        |
| Narratives           | Text that represents an overarching situation, theme, or a story. Narratives can communicate values, purpose, or identity that resonates with consumers on many levels.   |        |
| Persuasion Strategies|             |        |
| Readability          |             |        |
| Tone of voice        | | |
-->
