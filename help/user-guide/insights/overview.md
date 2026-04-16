---
title: Overview of Insights
description: Learn how to optimize ads based on real-time content performance metrics.
level: Intermediate
feature: Reporting and Insights
exl-id: 26402a06-f776-42be-9d8d-fc498c0f75a8
TQID: https://experienceleague.adobe.com/7ERGkM2wuM8JHYf-bi-SAVMSblhwpkt7NNuUNgCCcfc
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
  - id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
  - id: b03d2162-d906-40a0-9cbd-001391e22d4a
  - id: bb0d2eba-617d-4fdd-b920-2f535b5c031c
  - id: dd48f9df-f2e2-49fe-a918-332a8e240ffe
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 4d6a7fafb895ad1e2429978c8ee58d750fff8970
workflow-type: tm+mt
source-wordcount: 943
ht-degree: 0%

---

# Adobe GenStudio for Performance Marketing Insights

Adobe GenStudio for Performance Marketing [!DNL Insights] provides advanced analytics and insights into content performance that can help you make data-driven decisions.

From the [!DNL Insights] dashboard, you can:

- **Identify the most effective content**: Pinpoint which content performs best for different audiences and tailor future content or campaigns for trending preferences.
- **Optimize low-performing content**: Find content that is not performing well and use the integrated generative AI to create variations immediately, potentially improving its effectiveness without starting from scratch.
- **Revitalize high-performing content**: Take successful content and tweak it to refresh the ad for the audience or adapt hero content for use in new campaigns, potentially extending its lifecycle and performance.

The [!DNL Insights] module includes **[!UICONTROL Insights 2.0]**, a cross-channel performance experience for paid social. It works alongside the detailed table and gallery views in the [Dashboard](#dashboard) section of this article.

## Insights 2.0 {#insights-20}

**[!UICONTROL Insights 2.0]** delivers a performance intelligence layer that gives marketers a clear view of how paid social marketing is performing across connected accounts.

**In [!UICONTROL Insights 2.0], you can:**

- **Review cross-channel or single-channel overviews (Meta and LinkedIn)**: See a consolidated snapshot across both paid social channels, or drill down into one channel.
- **Use the cross-channel performance report**: View each channel&#39;s share of results with a percentage contribution visualization, including total spend (percentage and amount) and performance share metrics such as CTR, CPC, and CPM.
- **Use the ad performance report**: Identify high and low performing ads with rankings and metrics that support optimization decisions.
- **Analyze Meta conversion metrics**: Focus on conversions with visibility into CPA across funnel stages (for example, engaged visits, request for information, app start, prospect, and app complete) and review conversion trends over time, with conversion data available in GenStudio for Performance Marketing.
- **Explore insights from ad tags**: Ad tracking IDs are parsed into structured tags so you can analyze performance by dimensions you define (such as call to action, geography, format, or concept), see budget allocation across those dimensions, and spend less time decoding naming conventions manually.

>[!NOTE]
>
>**[!UICONTROL Insights 2.0]** currently includes ONLY **Meta** and **LinkedIn**. TikTok, DV360, and Innovid are not included in the **[!UICONTROL Insights 2.0]** overview at this time. The **[!UICONTROL Campaigns]**, **[!UICONTROL Ads]**, **[!UICONTROL Media]**, and **[!UICONTROL Attributes]** views in the [Dashboard](#dashboard) section continue to support the broader channel set described under [Channels supported](#channels-supported).

## Data connectors

The first time you open [!DNL Insights], you may see a banner to guide you to connect Adobe GenStudio for Performance Marketing with a channel account.

This connection enables GenStudio for Performance Marketing to receive statistical data from your active marketing campaigns, media, and ads. Initially, GenStudio for Performance Marketing ingests the last 6 months of data so that you have the tools to analyze the latest data and take action.

{{connect-insights}}

## Canali supportati {#channels-supported}

I canali supportati in Insights includono Meta, LinkedIn, TikTok, DV360 e Innovid.

Meta, LinkedIn e TikTok forniscono visibilità completa su campagne, annunci, media e attributi. DV360 e Innovid offrono attualmente una copertura dei dati più limitata.

Al momento, i dati multimediali non sono disponibili per DV360 e Innovid, il che significa che la scheda Attributi non viene visualizzata per questi canali. La scheda Attributi dipende dai dati a livello di elemento multimediale per far emergere le caratteristiche estratte dalle esperienze.

Questa limitazione è dovuta ai vincoli presenti nelle piattaforme di media a pagamento stesse e non a un problema di GenStudio for Performance Marketing.

## Dashboard {#dashboard}

Il dashboard [!DNL Insights] dispone di una tabella configurabile per ogni tipo di contenuto: [!UICONTROL Canali], [!UICONTROL Annunci], [!UICONTROL Media] e [!UICONTROL Attributi].

![[!DNL Insights] dashboard](/help/assets/insights-dashboard.png)

Ogni vista mostra una tabella corrispondente, che puoi cercare per parola chiave, filtro e intervallo di date. Puoi fare clic sull’icona delle impostazioni (cog) sopra il lato destro della tabella per attivare o disattivare i tipi di colonna visualizzabili. La riga _[!UICONTROL Riepilogo]_ può mostrare i totali o le medie di una colonna.

[!UICONTROL Ads], [!UICONTROL Media] e [!UICONTROL Attributes] includono una visualizzazione galleria che consente di analizzare e ordinare le risorse utilizzando schede con una miniatura di immagine o video. È disponibile un&#39;opzione per visualizzare una delle tre metriche chiave su ogni scheda: `Click-through rate`, `Cost per click` e `Spend`.

### Campagne

La visualizzazione predefinita [[!DNL Insights] _[!UICONTROL Campagne &#x200B;]_](campaigns.md) mostra un elenco di dettagli attivi della campagna, quali obiettivi, budget, data di lancio e attività. Assicurati di [collegare un account di canale](/help/user-guide/connectors/connect-channel.md) in modo che GenStudio for Performance Marketing inizi a ricevere i dati statistici.

### Annunci

La visualizzazione [[!DNL Insights] _[!UICONTROL Ads &#x200B;]_](ads.md) si concentra sulla valutazione dell&#39;efficacia di un annuncio. La visualizzazione [!UICONTROL Annunci] consente di analizzare le metriche di un annuncio in base al suo posizionamento all&#39;interno di un intervallo di date specificato. Facendo clic su un&#x200B;_[!UICONTROL &#x200B; Nome annuncio &#x200B;]_, puoi visualizzare le metriche delle prestazioni dell&#39;annuncio, le prestazioni in base al posizionamento dell&#39;annuncio e gli attributi.

### Media

La visualizzazione [[!DNL Insights] _[!UICONTROL Media &#x200B;]_](media.md) è progettata per consentire l&#39;analisi delle prestazioni dei contenuti creativi. Puoi identificare gli attributi multimediali che contribuiscono a migliorare una metrica selezionata, ad esempio clic o impression.

Facendo clic sul contenuto multimediale è possibile ottenere ulteriori informazioni sulle prestazioni tra diversi annunci e posizionamenti di annunci:

![Dettagli file multimediali](/help/assets/insights-media-details.png){width="600" zoomable="yes"}

Nella visualizzazione dei dettagli dei file multimediali, a sinistra vengono visualizzate una miniatura della risorsa e un elenco di attributi. Sono presenti tre metriche evidenziate: `Click-through rate`, `Cost per click` e `Spend`. Gli elementi di rilievo delle prestazioni mostrano il confronto tra i valori effettivi (linea continua) e il valore medio (linea tratteggiata) nel periodo di tempo selezionato (l&#39;impostazione predefinita è `Last 30 days`).

### Attributi

I _attributi_ multimediali consentono di identificare il contenuto creativo in base a dettagli intrinseci, quali colore, tono, composizione (come oggetto, font, elementi visivi) e altri componenti chiave. Gli attributi sono spesso il set di informazioni sul contenuto meno misurato e analizzato.

La visualizzazione [[!DNL Insights] _[!UICONTROL Attributi &#x200B;]_](attributes.md) può aiutarti a indagare e identificare quali attributi offrono prestazioni migliori con alcuni tipi di pubblico, canali e aree geografiche e può aiutarti a evidenziare le tendenze stagionali. Con queste informazioni, puoi utilizzare gli attributi delle prestazioni per creare varianti, rivolgerti a un pubblico specifico o sperimentare diverse strategie per campagne.
