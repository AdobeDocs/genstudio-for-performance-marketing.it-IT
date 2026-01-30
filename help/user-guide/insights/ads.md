---
title: Panoramica sugli annunci e sul posizionamento degli annunci
description: Guarda una panoramica del coinvolgimento dei clienti, del budget e delle spese per annunci e prestazioni di posizionamento degli annunci in Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Ad Performance, Text Attributes, Reporting and Insights
exl-id: e3827b1a-53d0-465c-8125-15b0e298ef3a
source-git-commit: 8bdfe52173b93e55f627f37cb1d6c5b16827d899
workflow-type: tm+mt
source-wordcount: '1458'
ht-degree: 0%

---

# Panoramica sugli annunci e sul posizionamento degli annunci

La visualizzazione [!DNL Insights] _[!UICONTROL Annunci]_ mostra un elenco di annunci per l&#39;account dell&#39;annuncio del canale connesso. Un _annuncio_ è una risorsa promozionale che include contenuti visivi e interattivi destinati alla distribuzione a un pubblico specifico nell&#39;ambito di una campagna di marketing.

{{connect-insights}}

La tabella _[!UICONTROL Ads]_ è organizzata utilizzando [!UICONTROL Ad names]. Fai clic sull’icona delle impostazioni (cog) sopra il lato destro della tabella per attivare/disattivare le colonne visualizzabili.

![Filtro annunci e tabella](/help/assets/insights-ads-filter.png){zoomable="yes"}

La visualizzazione della galleria _[!UICONTROL Ad]_ mostra un collage di anteprime di annunci e una metrica, ad esempio il tasso di click-through. Fai clic sull&#39;icona delle impostazioni (cog) sopra il lato destro della galleria per aprire **[!UICONTROL Impostazioni scheda]** e attivare/disattivare una delle tre metriche visualizzabili:

- CPA (Costo per azione)
- CTR (tasso di click-through)
- CPC (costo per clic)
- Spesa

{{filter-table}}

## Dettagli annuncio

Seleziona un annuncio e visualizza le metriche delle prestazioni, gli attributi di testo e i posizionamenti associati a ciascun annuncio. La _[!UICONTROL pagina dei dettagli dell&#39;annuncio]_ include le metriche per l&#39;annuncio `click-through rate`, `cost per action` e `spend`, ovvero la quantità di budget spesa per l&#39;annuncio. Poiché gli annunci possono avere più posizionamenti, ad esempio un feed o un banner, puoi visualizzare un raggruppamento delle stesse metriche per ogni posizionamento di annuncio. Utilizza le frecce sinistra e destra in **[!UICONTROL Prestazioni per posizionamento annuncio]** per scorrere le metriche di posizionamento.

![Dettagli annuncio con metriche e posizionamenti annuncio](/help/assets/insights-ad-details.png){zoomable="yes"}

### Attributi annuncio

Di seguito è riportato un elenco di attributi associati all’annuncio.

{{$include /help/_includes/generated-attributes.md}}

### Formati degli annunci

I formati degli annunci si riferiscono ai vari elementi creativi e layout utilizzati per allinearsi agli obiettivi della campagna, coinvolgere il pubblico target e aiutare a tracciare le metriche delle prestazioni.

[!DNL Insights] in GenStudio for Performance Marketing attualmente supporta i seguenti formati di annunci disponibili.

| Canale | Funzione supportata | Non supportato |
|---|---|---|
| Meta | <ul><li>Annunci dinamici</li><li>Link Ads</li><li>Annunci immagine semplici</li><li>Annunci video semplici</li><li>Acquista annunci</li></ul> | <ul><li>Advantage+ Annunci catalogo</li><li>Annunci carosello</li><li>Messenger Ads</li><li>Annunci lead</li><li>Annunci raccolta</li><li>Call Ads</li><li>Annunci post pagina di proprietà</li><li>Annunci partnership</li><li>Annunci flessibili</li></ul> |
| LinkedIn | <ul><li>Annunci immagine singola</li><li>Annunci video singoli</li><li>Annunci articolo</li></ul> | <ul><li>Annunci carosello</li><li>Annunci documento</li><li>Annunci evento</li><li>Thought Leader Ads</li><li>Annunci lead gen.</li><li>Follower Ads</li><li>Annunci conversazione</li><li>Annunci in evidenza</li><li>Annunci di lavoro</li><li>Annunci contenuto</li><li>Annunci messaggio</li></ul> |
| TikTok | <ul><li>Annunci immagine singola</li><li>Annunci video singoli</li></ul> | <ul><li>Annunci In-Feed (Video, Spark, Carosello)</li><li>Annunci di consapevolezza Premium (TopView, Brand Takeover)</li><li>Annunci interattivi (sfide dell&#39;hashtag, effetti del marchio)</li><li>Commerce Ads (Acquisti, Catalogo, LIVE)</li><li>Annunci lead e messaggi</li><li>È difficile categorizzare perché non disponiamo delle risorse per determinare il tipo di annuncio</li></ul> |
| DV360 | <ul><li>DISPLAY_AND_VIDEO_ADS</li><li>YOUTUBE_AND_PARTNERS_AD</li></ul> | Difficile da categorizzare. Non disponiamo delle risorse per determinare il tipo di annuncio. |
| Innovid | N/D | È difficile categorizzare perché non disponiamo delle risorse per determinare il tipo di annuncio. |

### Posizionamenti di annunci

I posizionamenti di annunci si riferiscono alle posizioni o alle piattaforme specifiche in cui gli annunci compaiono all’interno di una campagna. Questi posizionamenti determinano come e dove il pubblico interagisce con il contenuto. I posizionamenti di annunci ampliano la portata del pubblico, che consente di massimizzare la visibilità, il coinvolgimento e l’efficacia complessiva della campagna.

Quando crei una campagna, potresti aver selezionato dove eseguire gli annunci in base alla [finalità](campaigns.md#objectives) della campagna.

Di seguito è riportato un elenco dei posizionamenti di annunci supportati da Meta:

| Audience Network | Facebook/Meta \* | Instagram | Messenger |
|--------------------|--------------------|-------------------------|---------------------|
| Video premiato | Feed<br>Feed video<br>Storie<br>Marketplace<br>Colonna destra<br>Bobine<br>Sovrapposizione bobine<br>Video in streaming<br>Ricerca<br>Feed disco aziendale<br>Feed profilo | Storie<br>Feed<br>Esplora<br>Rulli<br>Esplora griglia Home<br>Feed profilo<br>Cerca<br>Flusso | Storie<br>Posta in arrivo |

\* Consulta [Informazioni sui posizionamenti di annunci nelle tecnologie Meta](https://www.facebook.com/business/help/407108559393196?id=369787570424415) nel _Centro assistenza aziendale Meta_.

## Prestazioni annuncio

Le metriche di Insights possono aiutarti a valutare quali annunci contribuiscono al successo di una campagna e quali posizionamenti di annunci sono più efficaci.

La tabella seguente fornisce definizioni e informazioni approfondite per le metriche di marketing digitale chiave nella visualizzazione per tabella [!UICONTROL Ads]. Ogni metrica include una breve definizione relativa ai nomi degli annunci, al modo in cui viene calcolata la metrica e una o più informazioni per comprenderne il significato e l’impatto su un annuncio.

| Metrica | Definizione | Insight |
| ---------------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Nome annuncio]** | Un elenco di annunci per l’account del canale connesso. Filtra gli annunci selezionando una campagna. | Ordina l’elenco degli annunci facendo clic su una qualsiasi delle metriche chiave. |
| **[!UICONTROL Campagna]** | Una campagna è un insieme di annunci progettati per raggiungere un obiettivo specifico. | Quando si filtra la tabella Annunci per campagna, le metriche di riepilogo di tutti gli annunci per la campagna potrebbero essere diverse dalla riga di riepilogo della campagna nella visualizzazione [!UICONTROL Canali]. Questa discrepanza può verificarsi se l’origine del canale, ad esempio Meta, e GenStudio utilizzano calcoli di riepilogo leggermente diversi. |
| **[!UICONTROL Posizionamenti]** | Un conteggio di [posizionamenti](#ad-placements) di annunci, posizioni in cui un annuncio è apparso nella campagna. | I posizionamenti aumentano la portata del pubblico.<p>Gli annunci che mostrano zero posizionamenti e nessun contenuto multimediale possono indicare un tipo di annuncio [non supportato](#unsupported-placements).</p> |
| **[!UICONTROL File multimediali]** | Numero di risorse utilizzate negli annunci e nei posizionamenti di annunci | Il conteggio nella tabella Annunci potrebbe essere diverso dal conteggio nella visualizzazione Dettagli annuncio. Questa discrepanza può verificarsi se l’origine del canale, ad esempio Meta, e GenStudio utilizzano calcoli di riepilogo leggermente diversi. |
| **[!UICONTROL Impression]** | Un conteggio di ogni volta che il posizionamento o l’annuncio viene caricato nel canale, indipendentemente dall’interazione o dalla visualizzazione. | Un conteggio elevato delle impression può indicare un’ampia visibilità, ma per insight con prestazioni reali, consideralo in relazione ad altre metriche di coinvolgimento. |
| **[!UICONTROL Clic]** | Il numero di volte in cui gli utenti interagiscono con un elemento cliccabile, ad esempio un collegamento o un pulsante call-to-action, in un posizionamento annuncio. | Un numero elevato di clic indica un forte interesse e coinvolgimento per il contenuto, che può essere efficace e raggiungere il pubblico giusto. |
| **[!UICONTROL CTR &#x200B;]**<br>_Percentuale di click-through_ | Percentuale (%) di impression che hanno generato clic sull’annuncio all’interno di una campagna.<br>**Calcolo**: `clicks` diviso per `impressions` | Un elevato tasso di click-through indica che il contenuto è altamente pertinente e motivante per il pubblico nella messaggistica e nella progettazione, e sta mirando in modo efficace agli interessi del pubblico. |
| **[!UICONTROL CPM &#x200B;]**<br>_Costo per mille_ | Il costo medio per ogni mille ad impression.<br>**Calcolo**: importo totale `spent` diviso per la portata, quindi moltiplicato per 1000 | Un valore basso può indicare una visibilità a costi contenuti, soprattutto se associata a un elevato tasso di click-through. |
| **[!UICONTROL CPA &#x200B;]**<br>_Costo per azione_ | Il costo medio speso per ottenere un’azione specifica del cliente, ad esempio un acquisto o un abbonamento.<br>**Calcolo**: importo totale `spent` diviso per il numero di azioni cliente completate | Utilizza per monitorare la spesa per gli annunci pubblicitari che si traducono in azioni preziose per i clienti. |
| **[!UICONTROL CPC &#x200B;]**<br>_Costo per clic_ | Il costo medio associato a ogni clic in un posizionamento pubblicitario.<br>**Calcolo**: importo totale `spent` diviso per `clicks` | Costi medi più bassi possono indicare una spesa pubblicitaria efficiente in termini di costi, soprattutto se confrontata con un aumento delle conversioni. |
| **[!UICONTROL Spesa]** | L’importo speso dal budget della campagna in un dato periodo di tempo per inserire questo annuncio. | Un importo di spesa elevato in un breve periodo può indicare un utilizzo rapido, che potrebbe portare a un precoce esaurimento delle risorse. Monitora l’importo speso rispetto alle metriche delle prestazioni chiave per monitorare il ritorno complessivo sull’investimento. |
| **Attributi** | Elenco delle funzioni inerenti presenti in questo annuncio. | Gli attributi aiutano a identificare gli elementi creativi che risuonano di più con il tuo pubblico. Vedi [Categorie](/help/user-guide/insights/attributes.md#categories). |

## Prestazioni di posizionamento

Nella visualizzazione _[!UICONTROL Pagina dettagli annuncio]_, le tre metriche principali riflettono le prestazioni complessive dell&#39;annuncio selezionato. Tuttavia, la sezione _Prestazioni per posizionamento_ mostra le metriche dettagliate per ciascun posizionamento dell&#39;annuncio. Utilizza le frecce destra e sinistra per spostarti tra i diversi posizionamenti di annunci.

La tabella seguente fornisce le definizioni per le metriche delle prestazioni di posizionamento degli annunci:

| Metrica | Definizione | Insight |
| ---------------------------- | ----------------------------- | --------------------------------- |
| **[!UICONTROL CTR &#x200B;]**<br>_Percentuale di click-through_ | La percentuale (%) di impression per un singolo posizionamento di annuncio che ha generato clic.<p>**Calcolo**:`clicks` diviso per `impressions`<p>Questa metrica aiuta a determinare l’efficacia del posizionamento dell’annuncio nel coinvolgere il pubblico. | Un CTR elevato indica che il posizionamento dell’annuncio è rilevante e convincente per il pubblico, portando a più interazioni. |
| **[!UICONTROL CPA &#x200B;]**<br>_Costo per azione_ | Il costo medio speso per un singolo posizionamento pubblicitario per ottenere l’azione desiderata dal cliente, ad esempio un acquisto o un abbonamento.<p>**Calcolo**: importo totale `spent` diviso per il numero di azioni cliente completate<p>Questa metrica consente di valutare il rapporto costi-efficacia del posizionamento dell’annuncio nella promozione di azioni di valore. | Un CPA più basso suggerisce che il posizionamento dell’annuncio è efficace nel convertire le interazioni del pubblico in azioni desiderate a un costo inferiore. |
| **[!UICONTROL CPC &#x200B;]**<br>_Costo per clic_ | Il costo medio associato a ogni clic in un singolo posizionamento pubblicitario.<p>**Calcolo**: importo totale `spent` diviso per `clicks`<p>Questa metrica consente di valutare il rapporto costi/efficacia del posizionamento dell’annuncio nella generazione dei clic. | Un CPC inferiore indica che il posizionamento dell’annuncio genera clic a un costo inferiore, il che può essere utile per massimizzare il ritorno sull’investimento. |
| **[!UICONTROL Spesa]** | L’importo speso per un singolo posizionamento pubblicitario, che rappresenta una frazione dell’importo totale speso per l’intero annuncio. Questa metrica consente di tenere traccia dell’allocazione del budget e dell’efficienza della spesa per ciascun posizionamento di annunci. | Il monitoraggio della spesa può contribuire a garantire che le risorse vengano utilizzate in modo efficace tra posizionamenti diversi. |
| **Attributi** | Elenco delle funzioni intrinseche presenti in questo posizionamento pubblicitario. | Gli attributi aiutano a identificare gli elementi creativi che risuonano di più con il tuo pubblico. Vedi [Categorie](/help/user-guide/insights/attributes.md#categories). |
