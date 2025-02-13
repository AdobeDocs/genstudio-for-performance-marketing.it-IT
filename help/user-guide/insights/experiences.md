---
title: Panoramica sulle esperienze
description: Guarda una panoramica del coinvolgimento dei clienti, del budget e delle spese per esperienze e prestazioni di posizionamento degli annunci in Adobe GenStudio for Performance Marketing.
feature: Insights, Experiences, Attributes
exl-id: e3827b1a-53d0-465c-8125-15b0e298ef3a
source-git-commit: 2abd2d874fb9ce515c9ec15bd6130b5a4dc8bd48
workflow-type: tm+mt
source-wordcount: '1092'
ht-degree: 0%

---

# Panoramica sulle esperienze

La visualizzazione [!DNL Insights] _[!UICONTROL Esperienze]_ mostra un elenco di esperienze per l&#39;account annuncio del canale connesso. Per Facebook, le esperienze sono dei Meta Ad Name.

{{connect-insights}}

La tabella _[!UICONTROL Esperienze]_ è organizzata utilizzando [!UICONTROL Nomi annuncio]. Fai clic sull’icona delle impostazioni (cog) sopra il lato destro della tabella per attivare/disattivare le colonne visualizzabili. L&#39;icona del filtro (funnel) sopra il lato sinistro della tabella apre il menu **[!UICONTROL Filtro]** in cui è possibile selezionare gli elenchi [!UICONTROL Account] e [!UICONTROL Campaign] per filtrare i nomi degli annunci nella tabella.

![Filtro esperienze e tabella](/help/assets/insights-experiences-filter.png){zoomable="yes"}

{{$include /help/_includes/download-insights.md}}

## Dettagli esperienza

Una _esperienza_ è una risorsa promozionale che include contenuti visivi e interattivi destinati alla distribuzione a un pubblico specifico nell&#39;ambito di una campagna di marketing.

Seleziona un’esperienza (nome annuncio) e visualizza le metriche delle prestazioni, gli attributi di testo e i posizionamenti associati a ciascun annuncio. Nella vista dei dettagli, puoi analizzare le metriche di un’esperienza in base al posizionamento degli annunci e alle attività di marketing all’interno di un intervallo di date specificato.

La visualizzazione dei dettagli include una metrica complessiva dell&#39;annuncio `click-through rate`, `cost per action` e `spend`, ovvero la quantità di budget presente nell&#39;annuncio. Poiché gli annunci possono avere più posizionamenti, ad esempio un feed o un banner, puoi visualizzare un raggruppamento delle stesse metriche per ogni posizionamento di annuncio. Utilizza le frecce sinistra e destra in **[!UICONTROL Prestazioni per posizionamento annuncio]** per scorrere le metriche di posizionamento.

![Dettagli annuncio con metriche e posizionamenti annuncio](/help/assets/insights-experience-details.png){zoomable="yes"}

### Attributi di testo

Sotto l&#39;anteprima dell&#39;esperienza è riportato un elenco di [!UICONTROL attributi di testo] associati all&#39;annuncio. Quando le risorse e le esperienze vengono approvate e memorizzate in [!DNL Content], GenStudio for Performance Marketing genera i tag in base alle caratteristiche intrinseche. Per informazioni dettagliate sui metadati di sistema, consulta [Dettagli risorsa](../content/asset-details.md#system-metadata).

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

## Prestazioni dell’esperienza

Le metriche di Insights possono aiutarti a valutare quali esperienze contribuiscono al successo di una campagna e quali posizionamenti di annunci sono più efficaci.

La tabella seguente fornisce definizioni e informazioni approfondite per le metriche chiave del marketing digitale nella visualizzazione per tabella [!UICONTROL Esperienze]. Ogni metrica include una breve definizione relativa ai nomi degli annunci, al modo in cui viene calcolata la metrica e una o più informazioni utili per comprenderne il significato e l’impatto su un’esperienza.

| Metrica | Definizione | Insight |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Nome esperienza]** | Un elenco di esperienze per l’account del canale connesso. Filtra gli annunci selezionando una campagna. | Ordina l’elenco delle esperienze facendo clic su una qualsiasi delle metriche chiave. |
| **[!UICONTROL Campagna]** | Una campagna è un insieme di esperienze progettate per raggiungere un obiettivo specifico. | Quando si filtra la tabella Esperienze per campagna, le metriche di riepilogo di tutte le esperienze per la campagna potrebbero essere diverse dalla riga di riepilogo della campagna nella visualizzazione [!UICONTROL Canali]. Questa discrepanza può verificarsi se l’origine del canale, ad esempio Meta, e GenStudio utilizzano calcoli di riepilogo leggermente diversi. |
| **[!UICONTROL Posizionamenti]** | Un conteggio di [posizionamenti](#ad-placements) di annunci, posizioni in cui è apparsa un&#39;esperienza nella campagna. | I posizionamenti aumentano la portata del pubblico.<p>Gli annunci che mostrano zero posizionamenti e zero risorse possono indicare un tipo di annuncio [non supportato](#unsupported-placements).</p> |
| **[!UICONTROL Assets]** | Il numero di risorse utilizzate nell’annuncio o nell’esperienza. | Il conteggio nella tabella Esperienze può essere diverso da quello nella visualizzazione Dettagli esperienza. Questa discrepanza può verificarsi se l’origine del canale, ad esempio Meta, e GenStudio utilizzano calcoli di riepilogo leggermente diversi. |
| **[!UICONTROL Impression]** | Un conteggio di ogni volta che il posizionamento dell’annuncio o l’esperienza viene caricato nel canale, indipendentemente dall’interazione o dalla visualizzazione. | Un conteggio elevato delle impression può indicare un’ampia visibilità, ma per informazioni approfondite sulle prestazioni, consideralo in relazione ad altre metriche di coinvolgimento. |
| **[!UICONTROL Clic]** | Il numero di volte in cui gli utenti interagiscono con un elemento cliccabile, ad esempio un collegamento o un pulsante di invito all’azione, in un posizionamento di esperienza. | Un numero elevato di clic indica un forte interesse e coinvolgimento per il contenuto, che può essere efficace e raggiungere il pubblico giusto. |
| **[!UICONTROL CTR ]**<br>_Percentuale di click-through_ | Percentuale (%) di impression che hanno generato clic sul posizionamento dell’esperienza all’interno di una campagna.<br>**Calcolo**: `clicks` diviso per `impressions` | Un elevato tasso di click-through indica che il contenuto è altamente pertinente e motivante per il pubblico nella messaggistica e nella progettazione, e sta mirando in modo efficace agli interessi del pubblico. |
| **[!UICONTROL CPM ]**<br>_Costo per mille_ | Costo ogni mille impression pubblicitarie per il posizionamento dell’esperienza.<br>**Calcolo**: importo totale `spent` diviso per la portata, quindi moltiplicato per 1000 | Un valore basso può indicare una visibilità a costi contenuti, soprattutto se associata a un elevato tasso di click-through. |
| **[!UICONTROL CPA ]**<br>_Costo per azione_ | Costo medio speso per ottenere un’azione specifica del cliente, ad esempio un acquisto o un abbonamento.<br>**Calcolo**: importo totale `spent` diviso per il numero di azioni cliente completate | Utilizza per monitorare la spesa per esperienze che si traducono in azioni preziose per il cliente. |
| **[!UICONTROL CPC ]**<br>_Costo per clic_ | Costo medio associato a ogni clic in un posizionamento esperienza.<br>**Calcolo**: importo totale `spent` diviso per `clicks` | Costi medi più bassi possono indicare una spesa pubblicitaria efficiente in termini di costi, soprattutto se confrontata con un aumento delle conversioni. |
| **[!UICONTROL Spesa]** | L&#39;importo speso dal bilancio in un determinato periodo di tempo. | Un importo di spesa elevato in un breve periodo può indicare un utilizzo rapido, che potrebbe portare a un precoce esaurimento delle risorse. Monitora l’importo della spesa rispetto alle metriche delle prestazioni chiave per monitorare il ritorno complessivo sull’investimento. |

## Prestazioni di posizionamento

Nella visualizzazione _Dettagli esperienza_, le tre metriche principali riflettono le prestazioni complessive dell&#39;esperienza selezionata. Tuttavia, la sezione _Prestazioni per posizionamento_ mostra le metriche dettagliate per ciascun posizionamento dell&#39;annuncio. La tabella seguente fornisce le definizioni per le metriche delle prestazioni di posizionamento:

| Metrica | Definizione | Calcolo |
| ---------------------- | ----------------------------- | ----------- |
| **[!UICONTROL CTR ]**<br>_Percentuale di click-through_ | Percentuale (%) di impression che hanno generato clic nel posizionamento dell’annuncio dell’esperienza. | `clicks` diviso per `impressions` |
| **[!UICONTROL CPA ]**<br>_Costo per azione_ | Costo medio speso per il posizionamento dell’annuncio per ottenere un’azione specifica del cliente, ad esempio un acquisto o un abbonamento. | totale `spent` diviso per il numero di azioni cliente completate |
| **[!UICONTROL CPC ]**<br>_Costo per clic_ | Costo medio associato a ogni clic in un posizionamento esperienza. | totale `spent` diviso per `clicks` |
| **[!UICONTROL Spesa]** | L&#39;importo speso dal bilancio in un determinato periodo di tempo. | |
