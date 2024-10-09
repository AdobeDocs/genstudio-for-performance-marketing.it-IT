---
title: Panoramica sulle esperienze
description: Guarda una panoramica del coinvolgimento dei clienti, del budget e delle spese per esperienze e prestazioni di posizionamento degli annunci in Adobe GenStudio for Performance Marketing.
feature: Insights, Experiences
source-git-commit: ce08231cb723bec3d80a732837b72a435d3b552d
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 0%

---

# Panoramica sulle esperienze

La visualizzazione [!DNL Insights] _[!UICONTROL Esperienze]_ mostra un elenco di esperienze per l&#39;account annuncio del canale connesso. Per Facebook, le esperienze sono nomi di Meta Ad.

La tabella _[!UICONTROL Esperienze]_ è organizzata utilizzando [!UICONTROL Nomi annuncio]. Fai clic sull’icona delle impostazioni (cog) sopra il lato destro della tabella per attivare/disattivare le colonne visualizzabili. L&#39;icona del filtro (funnel) sopra il lato sinistro della tabella apre il menu **[!UICONTROL Filtro]** in cui è possibile selezionare gli elenchi [!UICONTROL Account] e [!UICONTROL Campaign] per filtrare i nomi degli annunci nella tabella.

![Filtro esperienze e tabella](/help/assets/insights-experiences-filter.png){zoomable="yes"}

## Dettagli esperienza

Una _esperienza_ è una risorsa promozionale che include contenuti visivi e interattivi destinati alla distribuzione a un pubblico specifico nell&#39;ambito di una campagna di marketing.

Seleziona un’esperienza (nome annuncio) e visualizza le metriche delle prestazioni, gli attributi di testo e i posizionamenti associati a ciascun annuncio. Nella vista dei dettagli, puoi analizzare le metriche di un’esperienza in base al posizionamento degli annunci e alle attività di marketing all’interno di un intervallo di date specificato.

La visualizzazione dei dettagli include una metrica complessiva dell&#39;annuncio `click-through rate`, `cost per click` e la quantità di budget `spent` presente nell&#39;annuncio. Poiché gli annunci possono avere più posizionamenti, ad esempio un feed o un banner, puoi visualizzare un raggruppamento delle stesse metriche per ogni posizionamento di annuncio. Utilizza le frecce sinistra e destra in **[!UICONTROL Prestazioni per posizionamento annuncio]** per scorrere le metriche di posizionamento dell&#39;annuncio.

![Dettagli annuncio con metriche e posizionamenti annuncio](/help/assets/insights-experience-details.png){zoomable="yes"}

### Attributi di testo

Sotto l&#39;anteprima dell&#39;esperienza è riportato un elenco di [!UICONTROL attributi di testo] associati all&#39;annuncio. Quando le risorse e le esperienze vengono approvate e memorizzate in [!DNL Content], GenStudio for Performance Marketing genera i tag in base alle caratteristiche intrinseche. Per informazioni dettagliate sui metadati di sistema, consulta [Dettagli risorsa](../content/asset-details.md#system-metadata).

### Posizionamenti di annunci

Al momento della creazione di una campagna con annunci Meta, potresti aver selezionato dove eseguire gli annunci in base alla campagna [obiettivo](channels.md#objectives). I posizionamenti di annunci ampliano la portata del pubblico per l’annuncio.

GenStudio for Performance Marketing supporta formati di annunci, come feed di risorse, annunci di collegamenti e immagini singole o video. Di seguito è riportato un elenco di formati di annunci per piattaforma:

| Instagram | Facebook/Meta | Messenger | Audience Network |
| ------------ | ---------------- | ------------ | ---------------- |
| Esplora<br>Esplora Home<br>Esplora Home Griglia<br>Feed<br>Rulli<br>Feed Profilo<br>Cerca<br>Acquista<br>Storie | Esplora aziende<br>Feed<br>Video in streaming<br>Marketplace<br>Reels<br>Sovrapposizione bobine<br>Colonna destra<br>Risultati ricerca<br>Storie<br>Feed video<br>Annunci su bobine Facebook | Casella in entrata<br>Storie | Video nativo, banner e interstiziale<br>premiato |

## Metriche delle esperienze

Le metriche di Insights possono aiutarti a valutare quali esperienze contribuiscono al successo di una campagna e quali posizionamenti di annunci sono più efficaci.

<!-- For example, -->

### Dettagli delle metriche

La tabella seguente fornisce definizioni e informazioni approfondite per le metriche chiave del marketing digitale nella visualizzazione [!UICONTROL Esperienze]. Ogni metrica include una breve definizione relativa ai nomi degli annunci, al modo in cui viene calcolata la metrica e una o più informazioni utili per comprenderne il significato e l’impatto su un’esperienza.

| Metrica | Definizione | Insight |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Nome annuncio]** | Un elenco di esperienze per l’account del canale connesso. Filtra gli annunci selezionando una campagna. | Ordina l’elenco degli annunci facendo clic su una qualsiasi delle metriche chiave. |
| **[!UICONTROL Campagna]** | Una campagna è un insieme di esperienze progettate per raggiungere un obiettivo specifico. | |
| **[!UICONTROL Posizionamenti di annunci]** | Un conteggio di [posizionamenti di annunci](#ad-placements), dove eseguire l&#39;annuncio, per l&#39;annuncio o l&#39;esperienza. | Il posizionamento degli annunci aumenta la portata del pubblico. |
| **[!UICONTROL Assets]** | Un conteggio delle risorse utilizzate nell’annuncio o nell’esperienza. | |
| **[!UICONTROL Impression]** | Un conteggio di ogni volta che il posizionamento dell’annuncio o l’esperienza viene caricato nel canale, indipendentemente dall’interazione o dalla visualizzazione. | Un conteggio elevato delle impression può indicare un’ampia visibilità, ma per informazioni approfondite sulle prestazioni, considera con altre metriche di coinvolgimento. |
| **[!UICONTROL Clic]** | Numero di volte in cui gli utenti interagiscono con un elemento cliccabile, ad esempio un collegamento o un pulsante di invito all’azione, in un’esperienza. | Un numero elevato di clic indica un forte interesse e coinvolgimento per il contenuto, che può essere efficace e raggiungere il pubblico giusto. |
| **[!UICONTROL CTR ]**<br>_Percentuale di click-through_ | Percentuale (%) di impression che hanno generato clic sull’esperienza all’interno di una campagna.<br>**Calcolo**: `clicks` diviso per `impressions` | Un elevato tasso di click-through indica che il contenuto è altamente pertinente e motivante per il pubblico nella messaggistica e nella progettazione, e sta mirando in modo efficace agli interessi del pubblico. |
| **[!UICONTROL CPM ]**<br>_Costo per mille_ | Costo ($) per ogni mille ad impression per l’esperienza o il posizionamento dell’annuncio.<br>**Calcolo**: importo totale `spent` diviso per la portata, quindi moltiplicato per 1000 | Un valore basso può indicare una visibilità a costi contenuti, soprattutto se associata a un elevato tasso di click-through. |
| **[!UICONTROL CPC ]**<br>_Costo per clic_ | Costo medio ($) associato a ciascun clic in un’esperienza o posizionamento di annunci.<br>**Calcolo**: importo totale `spent` diviso per `clicks` | Costi medi più bassi possono indicare una spesa pubblicitaria efficiente in termini di costi, soprattutto se confrontata con un aumento delle conversioni. |
| **[!UICONTROL Spesa]** | L&#39;importo ($) speso dal budget per un determinato periodo di tempo. | Un importo di spesa elevato in un breve periodo può indicare un utilizzo rapido, che potrebbe portare a un precoce esaurimento delle risorse. Monitora l’importo della spesa rispetto alle metriche delle prestazioni chiave per monitorare il ritorno complessivo sull’investimento. |
