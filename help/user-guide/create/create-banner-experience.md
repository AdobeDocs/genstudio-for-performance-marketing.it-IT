---
title: Creare un'esperienza di banner
description: Scopri come creare esperienze banner in Adobe [!DNL GenStudio] for Performance Marketing.
feature: Brands Service, Guidelines, Content Generation, Generative AI, Create, Experiences, Variant Generation
badgeBeta: label="Beta" tooltip="Questa funzione è attualmente in Beta, quindi alcune funzionalità potrebbero essere limitate o soggette a modifiche."
role: User
level: Beginner
recommendations: noDisplay
source-git-commit: e4f552016fe17d2d7eb61792b62859475f107094
workflow-type: tm+mt
source-wordcount: '981'
ht-degree: 0%

---

# Creare un&#39;esperienza di banner

Questa esercitazione mostra come creare [esperienze banner](banner-experiences.md) con il marchio utilizzando GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (icona del pennello nell&#39;area di navigazione a sinistra).

Per progettare un&#39;esperienza di banner coinvolgente, si consiglia di [aggiungere linee guida a GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md) e rivedere le [nozioni di base sui prompt di scrittura](/help/user-guide/effective-prompts.md) prima di iniziare.

## Scegli un modello

Per creare un&#39;esperienza banner, utilizza un modello disponibile per fornire il framework per il contenuto. Consulta [Best practice per i modelli](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines) per informazioni sulle dimensioni del banner supportate.

**Per scegliere un modello di banner**:

1. In _[!DNL Create]_, fare clic su **[!UICONTROL Banner]**in_&quot;Cosa si desidera creare oggi?&quot;_sezione.
1. Utilizza l&#39;opzione di ricerca, adiacente al _filtro_, per trovare un modello di banner specifico.
1. Nella visualizzazione _Seleziona modello_, fare clic su un modello di banner.
1. Fai clic su **[!UICONTROL Usa]**.

   Viene visualizzato Canvas, che è la home base per la creazione di contenuti.

## Aggiungi parametri

L&#39;incorporazione di [linee guida](/help/user-guide/guidelines/overview.md) e risorse in _Parametri_ nel cassetto dei prompt migliora il processo di generazione dei contenuti ed è un passaggio preparatorio fondamentale per la creazione di un&#39;esperienza banner.

**Per aggiungere parametri e risorse**:

1. Fai clic sull&#39;icona _Parametri_ per espandere il cassetto dei prompt.
1. Nella sezione _Parametri_, selezionare linee guida—[!DNL Brands], [!DNL Personas] e [!DNL Products], per informare la creazione dei contenuti.

   Se da questi menu non sono disponibili marchi, utenti tipo o prodotti, [aggiungi linee guida al tuo GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md).

1. Per aggiungere contenuto da utilizzare nell&#39;esperienza *e* per influenzare la generazione del contenuto:
   * Fare clic su **[!UICONTROL Seleziona dal contenuto]** per selezionare le risorse (immagini) dal repository [!DNL Content], filtrare e selezionare una o più immagini.

     Per utilizzare le risorse da un repository [!DNL AEM Assets Content Hub] connesso, scegliere un repository dal menu a discesa _Posizione_. Filtra e seleziona una o più immagini.

   * In alternativa, trascina e rilascia le risorse nella sezione **[!UICONTROL Seleziona da contenuto]** per caricare una o più nuove risorse.
1. Fai clic su **[!UICONTROL Usa]**.

Al termine dell&#39;aggiunta dei parametri, comprimere il cassetto dei prompt facendo nuovamente clic sull&#39;icona _Parametri_.

## Immetti un prompt

Dopo aver selezionato le linee guida, utilizza il linguaggio naturale per creare un prompt per avviare la generazione dei contenuti per la nuova esperienza del banner. Per garantire risultati di alta qualità, è essenziale creare prompt dettagliati e descrittivi.

![Immetti un prompt](/help/assets/prompt-displayad.png){width="650" zoomable="yes"}

Per ulteriori informazioni sulla scrittura dei prompt, vedere [Scrivi prompt effettivi](/help/user-guide/effective-prompts.md).

**Per immettere una richiesta**:

1. Immettere un prompt nella casella di prompt _&quot;Descrivi le esperienze da generare&quot;_.
1. Fai clic su **[!UICONTROL Genera]**.

Per impostazione predefinita, quattro varianti (alimentate dal prompt, dalle linee guida e dal contenuto aggiunto) vengono generate e visualizzate nell’area di lavoro.

## Rivedere i banner generati

Prima di selezionare gli elementi da inviare per l&#39;approvazione o la pubblicazione a [!DNL Content], è possibile modificare sezioni di banner e campi di testo oppure eliminare una variante generata.

**Per rivedere le varianti generate**:

* **Per [modificare il nome della bozza del banner](/help/user-guide/create/manage-variants.md#change-draft-name)**, fare clic nel titolo _Bozza senza titolo_ nella parte superiore dell&#39;area di lavoro e immettere un nuovo titolo.
* **Per [modificare manualmente un banner](/help/user-guide/create/manage-variants.md#manually-edit-text)**, fare doppio clic su una sezione o un campo del banner (ad esempio il titolo o CTA) e modificarlo in base alle esigenze.
* **Per [rigenerare una sezione di una variante](/help/user-guide/create/manage-variants.md#re-generate-sections)**, fai clic su un campo di testo modificabile e utilizza le _[!UICONTROL opzioni di modifica consigliate]_ oppure immetti un nuovo prompt nella _[!UICONTROL Generate new text_ section] e fai clic su **[!UICONTROL Generate]**.
* **Per [aggiungere o scambiare immagini in una variante](/help/user-guide/create/manage-variants.md#swap-image)**, fai clic su una risorsa immagine (o sull&#39;area della risorsa immagine se un&#39;immagine non esiste attualmente) e fai clic sull&#39;icona **[!UICONTROL Scambia da contenuto]**.
* **Per [aggiungere un collegamento a un&#39;immagine in una variante](/help/user-guide/create/manage-variants.md#add-image-link)**, fare clic su una risorsa immagine (o sull&#39;area della risorsa immagine se non esiste attualmente un&#39;immagine) e fare clic sull&#39;icona del collegamento.
* **Per [modificare le dimensioni e le proporzioni dell&#39;annuncio](/help/user-guide/create/manage-variants.md#change-aspect-ratio)**, fare clic sul pulsante _[!UICONTROL Ridimensiona]_ (casella con l&#39;icona di un pulsante sul lato sinistro dell&#39;area di lavoro) e selezionare nuove dimensioni e proporzioni da applicare a tutte le varianti. Le varianti vengono duplicate e ridimensionate.
* **Per [ritagliare o riposizionare le immagini](/help/user-guide/create/manage-variants.md#crop-assets)**, posizionare il puntatore del mouse sull&#39;immagine, fare clic sull&#39;icona di ritaglio visualizzata e modificare le dimensioni e il posizionamento dell&#39;immagine. Fai clic su **[!UICONTROL Applica]**.

<!-- # Preview for device
When revising and preparing email experiences, you can toggle between previews for desktop and mobile views to ensure coherence and visual appeal of draft variants.
**To preview variants for desktop and mobile devices** toggle the device preview option—between **desktop** and **mobile**—in the right menu bar (computer and phone icons) to preview how variants appear. -->

## Invia feedback generazione

Per [inviare un feedback](/help/user-guide/create/manage-variants.md#generation-feedback) sulla qualità dell&#39;output di generazione, fare clic sull&#39;icona delle opzioni (tre punti) e selezionare **[!UICONTROL Output valido]** o **[!UICONTROL Output insufficiente]**.

## Verifica l’allineamento della verifica del contenuto

Per ottimizzare le varianti generate e garantire una rigorosa aderenza all&#39;identità del brand, alle linee guida della piattaforma e agli standard di accessibilità, sfrutta la potenza del pannello [_Verifica contenuto_](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Questo pannello mostra i dettagli completi del controllo dei contenuti e illumina le aree del miglioramento.

**Per eseguire controlli del contenuto su una variante**:

1. Fai clic sull&#39;icona del pannello _Verifica contenuto_ nella barra delle azioni a destra per aprire il pannello [_Verifica contenuto_](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Visualizza un riepilogo delle _verifiche necessarie_ e _verifiche superate_ per vedere quali sezioni e linee guida necessitano di miglioramenti.

   ![_Controllo contenuto_ pannello](/help/assets/content-check-panel.png){height="400" zoomable="yes"}

1. [Rivedi manualmente le varianti](#revise-generated-variants) per assicurarti che siano strettamente allineate con i controlli del contenuto eseguiti.

Consulta [Convalida marchio](/help/user-guide/guidelines/brand-validation.md).

## Ottieni recensioni e approvazioni

Utilizza il pannello _Approvazioni_, accessibile come icona sulla barra delle azioni a destra dell&#39;area di lavoro, per ottenere recensioni, tenere traccia dei commenti di revisione e ottenere le approvazioni delle parti interessate.

**Per ottenere revisioni e approvazioni**:

1. [Avvia una richiesta di approvazione](/help/user-guide/approvals/request-review.md) per richiedere un [approvazione delle esperienze banner bozza](/help/user-guide/approvals/approve-content.md).
1. [Rimuovere o aggiungere revisori](/help/user-guide/approvals/review-and-edit.md#manage-approvals) durante il processo di revisione.
1. [Accedere al contenuto per la revisione](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) e visualizzare le richieste di revisione.
1. Modifica le bozze in base ai commenti di revisione e [pubblica le esperienze del banner](#publish-and-export-experience).

Consulta [Recensioni e approvazioni](/help/user-guide/approvals/overview.md).

## Pubblicare ed esportare esperienze

Per rendere i banner generati disponibili per l&#39;uso corrente e futuro, pubblicarli in [!UICONTROL Contenuto] ed esportarli per utilizzarli nelle campagne di marketing.

1. **Per pubblicare le nuove esperienze banner**, fai clic su **[!UICONTROL Pubblica]** nella barra degli strumenti superiore o nel flusso di approvazioni.
   1. Seleziona _[!UICONTROL [!DNL Campaigns]]_e aggiungi_[!UICONTROL  Ulteriori dettagli ]_, se necessario.
   1. Fai clic su **[!UICONTROL Pubblica]**.

      ![Pubblica un banner](/help/assets/publish-displayad.png){width="450" zoomable="yes"}

1. **Per esportare i nuovi banner**, fai clic su **[!UICONTROL Esporta]** nella barra degli strumenti superiore.
   1. Seleziona il formato (HTML e immagini, PNG o JPG) e fai clic su **[!UICONTROL Esporta]**.

      Il HTML esportato deve trovarsi all&#39;interno di una proprietà Web predefinita, ad esempio un modello o un contenitore `div`. Senza queste dimensioni impostate, le immagini potrebbero apparire distorte se visualizzate in modo indipendente.

Vedere [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content).
