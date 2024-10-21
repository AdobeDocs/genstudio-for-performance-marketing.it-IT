---
title: Panoramica sugli attributi
description: Scopri come valutare le prestazioni di attributi specifici in Adobe GenStudio for Performance Marketing.
feature: Insights, Assets
source-git-commit: 87a8833549569aaeaa60f5760b4e9a8b710a6033
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 0%

---

# Panoramica sugli attributi

La visualizzazione [!DNL Insights] _[!UICONTROL Attributi]_ mostra un elenco di attributi utilizzati nelle campagne pubblicitarie per l&#39;account canale selezionato.

La tabella _[!UICONTROL Attributes]_ è organizzata utilizzando il nome [!UICONTROL Attribute]. Puoi passare da un tipo di elenco all&#39;altro utilizzando il pulsante **[!UICONTROL Immagini]** e il pulsante **[!UICONTROL Video]**. Fai clic sull’icona delle impostazioni (cog) sopra il lato destro della tabella per attivare/disattivare le colonne visualizzabili.

L&#39;icona del filtro (funnel) sopra il lato sinistro della tabella apre il menu **[!UICONTROL Filtro]** in cui è possibile selezionare la [!UICONTROL Categoria account] e la [!UICONTROL Categoria attributo] per filtrare gli attributi nella tabella. Nell&#39;esempio seguente viene illustrato un elenco di attributi nella categoria `Lighting Condition`.

![Filtro attributi e tabella](/help/assets/insights-attributes-filter.png){zoomable="yes"}

## Dettagli attributo

Gli attributi consentono di identificare le risorse in base ai relativi dettagli, ad esempio colore, composizione, elementi visivi e altre proprietà.

Nella visualizzazione dei dettagli dell’attributo, puoi vedere quali esperienze utilizzano l’attributo selezionato. I dettagli includono le prestazioni totali degli attributi e una suddivisione delle metriche delle prestazioni relative a ogni esperienza.

![Metriche delle prestazioni degli attributi](/help/assets/insights-attribute-details.png){zoomable="yes"}

GenStudio for Performance Marketing rileva alcune funzioni e applica l’attributo appropriato a una risorsa o esperienza come tag. Consulta [Categorie](#categories) per vedere esempi di questi tag. Per visualizzare tutti gli attributi associati a un&#39;esperienza, fai clic sull&#39;icona delle impostazioni (cog) sopra il lato destro della tabella per selezionare la colonna **[!UICONTROL Attributi]**.

## Categorie

GenStudio for Performance Marketing riconosce alcune funzioni di immagini, video e testo e applica un tag funzione alla risorsa. Una _categoria_ è un insieme di caratteristiche che condividono una caratteristica specifica. Un valore di esempio di _orientamento immagine_ è `landscape`.

Gli attributi rilevati e applicati automaticamente non possono essere modificati.

<!--
Select any of the following to open a detailed list of feature categories:

+++**Image features**

| Category               | Values                              |
| ---------------------- | ----------------------------------- |
| Background Colors      | 14 colors |
| Camera Position        | - `low angle`, `high angle`, `dutch angle`<br>- `overhead view`, `eye level`,`bird's eye view` |
| Camera Proximity       | `close up`, `mid shot`, `long shot` |
| Camera Setting         | - `fast shutter speed`, `long exposure`, `double exposure`<br>- `normal mode`, `flash`, `macro`, `wide-angle`<br>- `black and white`, `surreal`<br>- `bokeh blur`, `motion blur`, `tilt-shift blur` |
| Foreground Colors      | 14 colors |
| Image Type             | `photograph`, `sketch`, `painting`, `digital cartoon`, `infographics`, `graphic design`, `collage`, `screenshot` |
| Lighting Condition     | golden hour, blue hour, midday, overcast, night, high-key, low-key, daylight, incandescent, fluorescent, colorful, studio |
| Objects                | The items, entities, and elements that are visible, such as `lighthouse`, `orchid`, or `tunnel`. |
| Orientation            | Examples: `landscape`, `portrait`, `square` |
| Overall Tone           | `warm`, `cool`, `neutral` |
| People Categories      | Examples: `person`, `social group`, `people`, `kid` |
| Photography Styles     | `aerial photography`, `aerial photography`, `architectural photography`, `astrophotography`, `black and white photography`, `business photography`, `cityscape photography`, `commercial photography`, `composite photography`, `creative photography`, `editorial photography`, `event photography`, `family photography`, `fashion photography`, `fine art photography`, `food photography`, `holiday photography`, `indoor photography`, `landscape photography`, `lifestyle photography`, `macro photography`, `minimalist photography`, `night photography`, `outdoor photography`, `pet photography`, `portrait photography`, `product photography`, `real estate photography`, `seascape photography`, `sports photography`, `still-life photography`, `street photography`, `travel photography`, `underwater photography`, `wildlife photography` |
| Scenes                 | Examples: `city`, `island`, `living room` |
| Tags                   | Examples: `gaming`, `law`, `yoga` |
| Visual Attention Spread| The level of viewer attention spread across an image: `high`, `low` |
| Visual Content Density | The amount of information or detail in an image: `high`, `low` |

+++

+++**Video features**

| Category               | Values                              |
| ---------------------- | ----------------------------------- |
| Audio Genre  | |
| Audio Genre Category  | |
| Audio Mood  | |
| Audio Types| |
| Objects  | |
| Orientation  | |
| People Categories  | |
| Scenes  | |
| Styles  | |
| Tags   | |
| Video Category  | |
| Video Type  | |

+++

+++**Text features**

| Category               | Values                              |
| ---------------------- | ----------------------------------- |
| Emojis Count  | |
| HashTags Count  | |
| Keywords  | |
| Marketing Emotions  | |
| Narratives  |  |
| Persuasion Strategies  |  |
| Readability  | |
| Sentences Count  | |
| Stop Words Ratio  | |
| Text Quotes Count  | |
| Tones  | |
| Words Count  | |
| Words Count Per Sentence  | |

+++

-->

## Metriche degli attributi

Le metriche di Insights possono aiutarti a valutare quali attributi ispirano più coinvolgimento dei clienti.

### Dettagli delle metriche

La tabella seguente fornisce definizioni e informazioni approfondite per le metriche chiave del marketing digitale nella vista tabella [!UICONTROL Attributi]. Ogni metrica include una breve definizione relativa a una risorsa, del modo in cui viene calcolata e una o più informazioni per comprenderne il significato e l’impatto su una campagna pubblicitaria.

| Metrica | Definizione | Insight |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Attributo]** | Nome dell’attributo. | Ordina la tabella facendo clic sull’intestazione di colonna per una qualsiasi delle metriche chiave. |
| **[!UICONTROL Categoria]** | La [categoria](#categories) che rappresenta la qualità intrinseca di un attributo. |  |
| **[!UICONTROL # di immagini]** | Numero di immagini con questo attributo. |  |
| **[!UICONTROL # di video]** | Numero di video con questo attributo. |  |
| **[!UICONTROL Impression]** | Un conteggio di ogni volta che un’immagine o dei video con questo attributo vengono caricati nel canale, indipendentemente dall’interazione o dalla visualizzazione. | Un conteggio elevato delle impression può indicare un’ampia visibilità, ma per informazioni approfondite sulle prestazioni, considera con altre metriche di coinvolgimento. |
| **[!UICONTROL Clic]** | Numero di volte in cui gli utenti interagiscono con un’immagine o un video con questo attributo. | Un numero elevato di clic indica un forte interesse e coinvolgimento per il contenuto, che può essere efficace e raggiungere il pubblico giusto. |
| **[!UICONTROL CTR ]**<br>_Percentuale di click-through_ | Percentuale (%) di impression che hanno generato clic su immagini o video con questo attributo.<br>**Calcolo**: `clicks` diviso per `impressions` | Un elevato tasso di click-through indica che il contenuto è altamente pertinente e motivante per il pubblico nella messaggistica e nella progettazione, e sta mirando in modo efficace agli interessi del pubblico. |
| **[!UICONTROL CPM ]**<br>_Costo per mille_ | Costo ($) per ogni mille ad impression di un&#39;immagine o di un video con questo attributo.<br>**Calcolo**: importo totale `spent` diviso per la portata, quindi moltiplicato per 1000 | Un valore basso può indicare una visibilità a costi contenuti, soprattutto se associata a un elevato tasso di click-through. |
| **[!UICONTROL CPA ]**<br>_Costo per azione_ | Costo medio ($) speso per ottenere un&#39;azione specifica del cliente, ad esempio un acquisto o un abbonamento.<br>**Calcolo**: importo totale `spent` diviso per il numero di azioni cliente completate | Consente di identificare gli attributi che determinano azioni utili per il cliente. |
| **[!UICONTROL CPC ]**<br>_Costo per clic_ | Costo medio ($) associato a ciascun clic su immagini o video con questo attributo.<br>**Calcolo**: importo totale `spent` diviso per `clicks` | Costi medi più bassi possono indicare una spesa pubblicitaria efficiente in termini di costi, soprattutto se confrontata con un aumento delle conversioni. |
| **[!UICONTROL Spesa]** | L&#39;importo ($) speso dal budget in relazione agli attributi in un determinato periodo di tempo. | Un importo di spesa elevato in un breve periodo può indicare un utilizzo rapido, che potrebbe portare a un precoce esaurimento delle risorse. Monitora l’importo della spesa rispetto alle metriche delle prestazioni chiave per monitorare il ritorno complessivo sull’investimento. |
