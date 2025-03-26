---
title: Funzioni immagine
description: Scopri la funzione per immagini delle categorie di attributi utilizzate in GenStudio for Performance Marketing.
level: Intermediate
feature: Reporting and Insights, Image Attributes, Generative AI
exl-id: b7e3d202-4085-48a4-a6ba-c950dfd52233
source-git-commit: 8a5d15df7a347c4ee7767610fc9bb23fc7b71db4
workflow-type: tm+mt
source-wordcount: '1044'
ht-degree: 0%

---

# Funzioni immagine

Le funzionalità immagine rappresentano elementi o pattern distinti e informativi all&#39;interno di un&#39;immagine utilizzati per l&#39;analisi con [!DNL Insights]. Queste funzioni consentono di classificare e comprendere il contenuto visivo, consentendo di ottenere informazioni più precise e dettagliate. Identificando vari attributi, come stile, colore e oggetti, l’intelligenza artificiale può fornire un’analisi completa dell’immagine, contribuendo a migliorare il processo decisionale e la formulazione della strategia.

## Rilevamento degli stili

La determinazione dello _stile immagine_ funge da base per l&#39;identificazione di altre caratteristiche immagine. L’intelligenza artificiale può applicare le tecniche di analisi appropriate e riconoscere le funzioni rilevanti, consentendo una comprensione più completa dell’immagine. Ogni stile ha caratteristiche visive distinte che influenzano il modo in cui l&#39;immagine viene percepita e analizzata.

Se lo stile dell&#39;immagine è identificato come `photograph`, l&#39;intelligenza artificiale analizza caratteristiche aggiuntive per `camera settings`, `camera proximity` e `Photography genres`. Queste caratteristiche sono specifiche delle fotografie e forniscono informazioni più approfondite sulla composizione e sulla qualità dell’immagine. Consulta [28 tipi di stili di fotografia](https://www.adobe.com/creativecloud/photography/discover/types-of-photography.html) in _Scopri la fotografia_ di Adobe e scopri i tipi popolari di fotografia e la terminologia fondamentale.

Se lo stile dell&#39;immagine è identificato come `sketch` o `digital cartoon`, può essere rilevante un diverso insieme di caratteristiche. Questo approccio gerarchico garantisce che l’analisi sia contestualmente accurata e personalizzata in base al tipo specifico di immagine esaminata.

## Funzioni per la ricerca delle immagini

**Per visualizzare le immagini in una categoria di attributi specifica**:

1. In _[!DNL Insights]_, selezionare la visualizzazione **[!UICONTROL Attributi]**.

1. Modificare la visualizzazione della tabella selezionando **[!UICONTROL Immagini]**.

1. Selezionare una funzionalità immagine dall&#39;elenco **[!UICONTROL Categoria attributo]**, ad esempio `Scenes`.

1. Selezionare un attributo per una visualizzazione dettagliata delle immagini che condividono tale categoria.

   Ad esempio, la categoria `Scenes` può avere `restaurant` come attributo.

1. Nella pagina _Dettagli attributo_ sono elencate tutte le immagini con questo attributo.

Nella tabella seguente sono elencate le categorie di funzioni immagine riconosciute da GenStudio for Performance Marketing AI. L’elenco degli attributi rilevati per il contenuto multimediale non è esaustivo. I contenuti multimediali che contengono un set completo di funzioni possono essere limitati alle tre funzioni più dominanti identificate dall’intelligenza artificiale.

<!-- For the writer: turn off word wrap to work with these tables. Option + Z -->

| Categoria | Descrizione | Esempio |
| ----------------------- | ----------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Distribuzione dell&#39;attenzione | Il livello di attenzione dell’osservatore si estende a un’immagine, indicando quanta messa a fuoco possono ricevere diverse aree dell’immagine. Una distribuzione più alta significa che nessuna area singola domina la messa a fuoco dell&#39;osservatore, mentre una distribuzione più bassa significa che uno o due punti focali catturano l&#39;attenzione dell&#39;osservatore. | `high`, `medium`, `low`<p>Esempio di distribuzione `low` a sinistra e di distribuzione `high` a destra:<p>![gioco palla a bassa e alta distribuzione](/help/assets/category/image-attn-lowhigh.png "Differenza nella distribuzione bassa e alta"){width="200" zoomable="yes"} |
| Angolo videocamera | La prospettiva da cui la fotocamera cattura il soggetto, che influenza la percezione e l&#39;interpretazione dell&#39;immagine da parte dello spettatore. Se lo stile dell&#39;immagine è `photograph`, questa caratteristica viene identificata. | `Low angle`, `High angle`, `Eye level`, `Overhead view`, `Dutch angle`, `Bird's eye view`<p>Esempio di `eye level`:<p>![livello degli occhi](/help/assets/category/image-camera-angle.png "Persone sedute da angoli diversi"){width="200" zoomable="yes"} |
| Impostazioni della telecamera | Regolazioni e configurazioni specifiche dei comandi della telecamera che influenzano l&#39;aspetto finale e la qualità dell&#39;immagine. Se lo stile dell&#39;immagine è `photograph`, questa caratteristica viene identificata. | `Fast shutter speed`, `Long exposure`, `Bokeh blur`, `Motion blur`, `Tilt-shift blur`, `Flash`, `Wide-angle`, `Black and white`, `Surreal`, `Double-exposure`, `Macro`, `Normal mode`<p>Esempio di impostazione `macro`:<p>![Macro primo piano](/help/assets/category/image-subject-distance.png "Impostazione macro per fiore primo piano e ape ingioiellata"){width="200" zoomable="yes"} |
| Colore e tonalità | I colori e le qualità tonali di un&#39;immagine. Identifica fino a tre colori da un set predefinito di 40 colori in diversi livelli di immagine:<p>**[!UICONTROL Colori di primo piano]**—colori nel livello anteriore dell&#39;immagine<br>**[!UICONTROL Colori di sfondo ]**—colori nel livello posteriore dell&#39;immagine | Valori colore: `Red`, `Dark Red`, `Green`, `Bright Green`, `Dark Green`, `Light Green`, `Mud Green`, `Blue`, `Dark Blue`, `Light Blue`, `Royal Blue`, `Black`, `White`, `Off White`, `Gray`, `Dark Gray`, `Silver`, `Cream`, `Magenta`, `Cyan`, `Yellow`, `Mustard`, `Khaki`, `Brown`, `Dark Brown`, `Violet`, `Pink`, `Dark Pink`, `Maroon`, `Tan`, `Purple`, `Lavender`, `Turquoise`, `Plum`, `Gold`, `Emerald`, `Orange`, `Beige`, `Lilac`, `Olive` |
| Temperatura del colore | Descrive il calore generale o la freddezza dei colori nell&#39;immagine. | Valori di tonalità o temperatura: `warm`, `cool`, `neutral`<br>![colori e tonalità fredde](/help/assets/category/image-color-temp.png "Temperatura del colore con sfondo fresco e più oggetti colorati"){width="200" zoomable="yes"} |
| Densità dei contenuti | Concentrazione di elementi visivi e dettagli all’interno di un’immagine, che indica quante informazioni vengono inserite nello spazio visivo.<p>A differenza della distribuzione dell&#39;attenzione, che misura il modo in cui l&#39;attenzione degli spettatori viene distribuita tra le diverse aree di un&#39;immagine, la densità del contenuto si concentra sulla quantità di informazioni visive presenti. Una maggiore densità di contenuto significa che sono presenti più elementi. | `high`, `medium`, `low`<p>Esempio di densità `low` a sinistra e di densità `high` a destra:<p>![gioco palla a bassa e alta densità](/help/assets/category/image-attn-lowhigh.png "Differenza tra densità di contenuto bassa e alta"){width="200" zoomable="yes"} |
| Stile immagine | Il trattamento visivo di un’immagine, ad esempio una fotografia o uno schizzo. Una volta che l’intelligenza artificiale determina lo stile dell’immagine, è possibile identificare altre caratteristiche. Ad esempio, se l&#39;immagine è una fotografia, possono essere applicate le impostazioni della fotocamera, la prossimità della fotocamera e le condizioni di illuminazione. | `Photograph`, `Sketch`, `Painting`, `Digital cartoon`, `Infographics`, `Graphic design`, `Collage`, `Software screenshot`<p>Esempio di uno stile di immagine `digital cartoon`![stile di immagine di un cartone animato](/help/assets/category/image-style.png "Stile di immagine di un gatto"){width="200" zoomable="yes"} |
| Condizioni di illuminazione | Descrive la qualità e le caratteristiche della luce in un&#39;immagine, influenzandone l&#39;umore, il tono e la visibilità. | `Golden hour`, `Blue hour`, `Midday`, `Overcast`, `Night`, `High-key`, `Low-key`, `Daylighting`, `Incandescent`, `Fluorescent`, `Colorful`, `Studio`<p>Esempio di condizione `daylighting`:<p>![Persona e cane sul marciapiede in condizioni di illuminazione diurna](/help/assets/category/image-lighting.png "Condizioni di illuminazione diurna"){width="200" zoomable="yes"} |
| Oggetti | Identifica uno o più elementi, entità ed elementi che compongono l&#39;immagine. | I valori sono troppo numerosi, ma alcuni esempi includono: `backpack`, `book`, `hawk`, `glasses`, `fish`, `pencil`, `mountain bike`, `soap`<p>Esempio di `toucan` e `bird` oggetti:<p>![uccello, oggetto touch](/help/assets/category/image-objects-bird.png "Progettazione grafica dell&#39;oggetto uccello touch"){width="200" zoomable="yes"} |
| Orientamento | Allineamento dell&#39;immagine in relazione alla larghezza e all&#39;altezza. Rileva se è più largo di quanto sia alto (orizzontale), più alto di quanto sia largo (verticale) o uguale in larghezza e altezza (quadrato). | `landscape`, `portrait`, `square`<p>Esempio di orientamento `square`:<p>![schizzo quadrato](/help/assets/category/image-orientation-square.png "schizzo di fiore con orientamento quadrato"){width="200" zoomable="yes"} |
| Persone | Se è presente almeno una persona, uno o più attributi possono descrivere la persona o le persone nell&#39;immagine. | `person`, `woman`, `man`, `girl`, `boy`, `social group`, `kid`, `crowd`, `people`<p>Esempio di persone `woman` e `person` categorie:<p>![donna con fotocamera](/help/assets/category/image-people.png "Persona che gestisce una fotocamera"){width="200" zoomable="yes"} |
| Generi fotografici | Rileva l&#39;oggetto e la tecnica utilizzati per acquisire un&#39;immagine, ad esempio `abstract` o `landscape` (diverso dall&#39;orientamento orizzontale). | `Architecture`, `Astro`, `Landscape`, `Pet`, `Interior`, `Wildlife`, `Night`, `Cityscape`, `Seascape`, `Underwater`, `Storm`, `Adventure sports`, `Fashion`, `Portrait`, `Sports`, `Food`, `Street`, `Event`, `Lifestyle`, `Commercial`, `Group`, `Abstract`, `Minimalist`, `Composite`<p>Vedi [Tipi di fotografia](https://www.adobe.com/creativecloud/photography/discover/types-of-photography.html) |
| Scene | Identifica l’impostazione o l’ambiente all’interno di un’immagine, fornendo contesto su dove l’immagine è stata acquisita o sul tipo di posizione rappresentata. | I valori sono troppo numerosi, ma alcuni esempi includono: `lake`, `underwater`, `highway`, `hill`, `log cabin`, `island`, `beach`, `lounge`<p>Esempio `snow`, `sky`, `winter` e `mountain` scene riflesse su un casco:<p>![neve invernale](/help/assets/category/image-scenes.png "Inverno, neve, cielo e riflesso della scena montana"){width="200" zoomable="yes"} |
| Distanza soggetto | La distanza tra la fotocamera e il soggetto di un&#39;immagine. | `close up`, `mid shot`, `long shot`<p>Esempio di `closeup shot`:<p>![inquadratura ravvicinata](/help/assets/category/image-subject-distance.png "Chiudi fiore e ape ingioiellata"){width="200" zoomable="yes"} |
| Stili | Rileva i trattamenti visivi applicati agli elementi immagine, ad esempio quelli utilizzati in Lightroom o Photoshop. | `design`, `illustration`, `logo`, `square`, `cartoon`, `art`, `circle`, `circular`<p>Esempio di stile `circular`:<p>![gateway circolare nella barriera corallina](/help/assets/category/image-styles-circular.png "Portale circolare in una barriera corallina"){width="200" zoomable="yes"} |
| Tag | Rileva altre caratteristiche dell&#39;immagine che non rientrano in una classificazione specifica. I tag forniscono contesto e metadati aggiuntivi sull’immagine. Ad esempio, l&#39;IA potrebbe rilevare `helmet` e `motorobike` oggetti in un&#39;immagine e includere `riding` come tag. | I valori sono troppo numerosi, ma alcuni esempi includono: `construction`, `gothic`, `healing`, `military`, `selfie`, `football`, `typing`, `dancer`, `dancing`<p>Esempio di tag `dancer` e `dancing`:<p>![tag per ballerino e ballerino](/help/assets/category/image-tags.png "Danzatore"){width="200" zoomable="yes"} |
