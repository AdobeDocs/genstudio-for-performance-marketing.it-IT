---
title: Panoramica sugli annunci e sul posizionamento degli annunci
description: Guarda una panoramica del coinvolgimento dei clienti, del budget e delle spese per annunci e prestazioni di posizionamento degli annunci in Adobe GenStudio for Performance Marketing.
feature: Ad Performance, Text Attributes, Reporting and Insights
exl-id: e3827b1a-53d0-465c-8125-15b0e298ef3a
source-git-commit: 3448392bc3f1496dafdbed2995f40bdba9c91c31
workflow-type: tm+mt
source-wordcount: '1237'
ht-degree: 0%

---

# Panoramica sugli annunci e sul posizionamento degli annunci

La visualizzazione [!DNL Insights] _[!UICONTROL Annunci]_ mostra un elenco di annunci per l&#39;account dell&#39;annuncio del canale connesso. Un _annuncio_ è una risorsa promozionale che include contenuti visivi e interattivi destinati alla distribuzione a un pubblico specifico nell&#39;ambito di una campagna di marketing. Per Facebook, gli annunci sono Meta Ad Name.

{{connect-insights}}

La tabella _[!UICONTROL Ads]_ è organizzata utilizzando [!UICONTROL Ad names]. Fai clic sull’icona delle impostazioni (cog) sopra il lato destro della tabella per attivare/disattivare le colonne visualizzabili. L&#39;icona del filtro (funnel) sopra il lato sinistro della tabella apre il menu **[!UICONTROL Filtro]** in cui è possibile selezionare più elenchi. Seleziona **[!UICONTROL Cancella tutto]** sopra la tabella per rimuovere tutti i filtri.

![Filtro annunci e tabella](/help/assets/insights-ads-filter.png){zoomable="yes"}

{{$include /help/_includes/download-insights.md}}

## Dettagli annuncio

Seleziona un annuncio e visualizza le metriche delle prestazioni, gli attributi di testo e i posizionamenti associati a ciascun annuncio. La _[!UICONTROL pagina dei dettagli dell&#39;annuncio]_ include le metriche per l&#39;annuncio `click-through rate`, `cost per action` e `spend`, ovvero la quantità di budget spesa per l&#39;annuncio. Poiché gli annunci possono avere più posizionamenti, ad esempio un feed o un banner, puoi visualizzare un raggruppamento delle stesse metriche per ogni posizionamento di annuncio. Utilizza le frecce sinistra e destra in **[!UICONTROL Prestazioni per posizionamento annuncio]** per scorrere le metriche di posizionamento.

![Dettagli annuncio con metriche e posizionamenti annuncio](/help/assets/insights-ad-details.png){zoomable="yes"}

### Attributi di testo

Sotto l&#39;anteprima dell&#39;annuncio è riportato un elenco di [!UICONTROL attributi di testo] associati all&#39;annuncio. Quando le risorse e gli annunci vengono approvati e memorizzati in [!DNL Content], GenStudio for Performance Marketing genera i tag in base alle caratteristiche intrinseche. Per informazioni dettagliate sui metadati di sistema, consulta [Dettagli file multimediali](/help/user-guide/content/asset-details.md#system-metadata).

### Posizionamenti di annunci

Al momento della creazione di una campagna con annunci Meta, potresti aver selezionato dove eseguire gli annunci in base alla campagna [obiettivo](channels.md#objectives). I posizionamenti di annunci ampliano la portata del pubblico per l’annuncio.

GenStudio for Performance Marketing supporta formati di annunci, come feed di risorse, annunci di collegamenti e immagini singole o video. Di seguito è riportato un elenco di formati di annunci per piattaforma:

| Instagram | Facebook/Meta | Messenger | Audience Network |
| ------------ | ---------------- | ------------ | ---------------- |
| Esplora<br>Esplora la home<br>Esplora la griglia Home<br>Feed<br>Rulli<br>Feed profilo<br>Cerca<br>Acquista<br>Storie | Business Explore<br>Feed<br>Video in-stream<br>Marketplace<br>Reels<br>Sovrapposizione bobine<br>Colonna destra<br>Risultati ricerca<br>Storie<br>Feed video<br>Annunci su bobine Facebook | Casella in entrata<br>Storie | Video nativo, banner e interstiziale<br>Premiato |

#### Posizionamenti non supportati

GenStudio for Performance Marketing non supporta i seguenti posizionamenti di annunci:

- Collaborativo
- Catalogo/Vantaggio+ catalogo
- Esperienza istanza
- Carosello

## Prestazioni annuncio

Le metriche di Insights possono aiutarti a valutare quali annunci contribuiscono al successo di una campagna e quali posizionamenti di annunci sono più efficaci.

La tabella seguente fornisce definizioni e informazioni approfondite per le metriche di marketing digitale chiave nella visualizzazione per tabella [!UICONTROL Ads]. Ogni metrica include una breve definizione relativa ai nomi degli annunci, al modo in cui viene calcolata la metrica e una o più informazioni per comprenderne il significato e l’impatto su un annuncio.

| Metrica | Definizione | Insight |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Nome annuncio]** | Un elenco di annunci per l’account del canale connesso. Filtra gli annunci selezionando una campagna. | Ordina l’elenco degli annunci facendo clic su una qualsiasi delle metriche chiave. |
| **[!UICONTROL Campagna]** | Una campagna è un insieme di annunci progettati per raggiungere un obiettivo specifico. | Quando si filtra la tabella Annunci per campagna, le metriche di riepilogo di tutti gli annunci per la campagna potrebbero essere diverse dalla riga di riepilogo della campagna nella visualizzazione [!UICONTROL Canali]. Questa discrepanza può verificarsi se l’origine del canale, ad esempio Meta, e GenStudio utilizzano calcoli di riepilogo leggermente diversi. |
| **[!UICONTROL Posizionamenti]** | Un conteggio di [posizionamenti](#ad-placements) di annunci, posizioni in cui un annuncio è apparso nella campagna. | I posizionamenti aumentano la portata del pubblico.<p>Gli annunci che mostrano zero posizionamenti e nessun contenuto multimediale possono indicare un tipo di annuncio [non supportato](#unsupported-placements).</p> |
| **[!UICONTROL File multimediali]** | Il numero di risorse utilizzate nell’annuncio o nell’annuncio. | Il conteggio nella tabella Annunci potrebbe essere diverso dal conteggio nella visualizzazione Dettagli annuncio. Questa discrepanza può verificarsi se l’origine del canale, ad esempio Meta, e GenStudio utilizzano calcoli di riepilogo leggermente diversi. |
| **[!UICONTROL Impression]** | Un conteggio di ogni volta che il posizionamento o l’annuncio viene caricato nel canale, indipendentemente dall’interazione o dalla visualizzazione. | Un conteggio elevato delle impression può indicare un’ampia visibilità, ma per informazioni approfondite sulle prestazioni, consideralo in relazione ad altre metriche di coinvolgimento. |
| **[!UICONTROL Clic]** | Il numero di volte in cui gli utenti interagiscono con un elemento cliccabile, ad esempio un collegamento o un pulsante di invito all’azione, in un posizionamento di annuncio. | Un numero elevato di clic indica un forte interesse e coinvolgimento per il contenuto, che può essere efficace e raggiungere il pubblico giusto. |
| **[!UICONTROL CTR ]**<br>_Percentuale di click-through_ | Percentuale (%) di impression che hanno generato clic sull’annuncio all’interno di una campagna.<br>**Calcolo**: `clicks` diviso per `impressions` | Un elevato tasso di click-through indica che il contenuto è altamente pertinente e motivante per il pubblico nella messaggistica e nella progettazione, e sta mirando in modo efficace agli interessi del pubblico. |
| **[!UICONTROL CPM ]**<br>_Costo per mille_ | Costo per ogni mille ad impression.<br>**Calcolo**: importo totale `spent` diviso per la portata, quindi moltiplicato per 1000 | Un valore basso può indicare una visibilità a costi contenuti, soprattutto se associata a un elevato tasso di click-through. |
| **[!UICONTROL CPA ]**<br>_Costo per azione_ | Costo medio speso per ottenere un’azione specifica del cliente, ad esempio un acquisto o un abbonamento.<br>**Calcolo**: importo totale `spent` diviso per il numero di azioni cliente completate | Utilizza per monitorare la spesa per gli annunci pubblicitari che si traducono in azioni preziose per i clienti. |
| **[!UICONTROL CPC ]**<br>_Costo per clic_ | Costo medio associato a ogni clic in un posizionamento pubblicitario.<br>**Calcolo**: importo totale `spent` diviso per `clicks` | Costi medi più bassi possono indicare una spesa pubblicitaria efficiente in termini di costi, soprattutto se confrontata con un aumento delle conversioni. |
| **[!UICONTROL Spesa]** | L’importo speso dal budget della campagna in un dato periodo di tempo per inserire questo annuncio. | Un importo di spesa elevato in un breve periodo può indicare un utilizzo rapido, che potrebbe portare a un precoce esaurimento delle risorse. Monitora l’importo speso rispetto alle metriche delle prestazioni chiave per monitorare il ritorno complessivo sull’investimento. |

## Prestazioni di posizionamento

Nella visualizzazione _[!UICONTROL Pagina dettagli annuncio]_, le tre metriche principali riflettono le prestazioni complessive dell&#39;annuncio selezionato. Tuttavia, la sezione _Prestazioni per posizionamento_ mostra le metriche dettagliate per ciascun posizionamento dell&#39;annuncio. Utilizza le frecce destra e sinistra per spostarti tra i diversi posizionamenti di annunci.

La tabella seguente fornisce le definizioni per le metriche delle prestazioni di posizionamento degli annunci:

| Metrica | Definizione | Insight |
| ---------------------- | ----------------------------- | ----------- |
| **[!UICONTROL CTR ]**<br>_Percentuale di click-through_ | La percentuale (%) di impression per un singolo posizionamento di annuncio che ha generato clic.<p>**Calcolo**:`clicks` diviso per `impressions`<p>Questa metrica aiuta a determinare l’efficacia del posizionamento dell’annuncio nel coinvolgere il pubblico. | Un CTR elevato indica che il posizionamento dell’annuncio è rilevante e convincente per il pubblico, portando a più interazioni. |
| **[!UICONTROL CPA ]**<br>_Costo per azione_ | Il costo medio speso per un singolo posizionamento pubblicitario per ottenere l’azione desiderata dal cliente, ad esempio un acquisto o un abbonamento.<p>**Calcolo**: importo totale `spent` diviso per il numero di azioni cliente completate<p>Questa metrica consente di valutare il rapporto costi-efficacia del posizionamento dell’annuncio nella promozione di azioni di valore. | Un CPA più basso suggerisce che il posizionamento dell’annuncio è efficace nel convertire le interazioni del pubblico in azioni desiderate a un costo inferiore. |
| **[!UICONTROL CPC ]**<br>_Costo per clic_ | Il costo medio associato a ogni clic in un singolo posizionamento pubblicitario.<p>**Calcolo**: importo totale `spent` diviso per `clicks`<p>Questa metrica consente di valutare il rapporto costi/efficacia del posizionamento dell’annuncio nella generazione dei clic. | Un CPC inferiore indica che il posizionamento dell’annuncio genera clic a un costo inferiore, il che può essere utile per massimizzare il ritorno sull’investimento. |
| **[!UICONTROL Spesa]** | L’importo speso per un singolo posizionamento pubblicitario, che rappresenta una frazione dell’importo totale speso per l’intero annuncio. Questa metrica consente di tenere traccia dell’allocazione del budget e dell’efficienza della spesa per ciascun posizionamento di annunci. | Il monitoraggio della spesa può contribuire a garantire che le risorse vengano utilizzate in modo efficace tra posizionamenti diversi. |
