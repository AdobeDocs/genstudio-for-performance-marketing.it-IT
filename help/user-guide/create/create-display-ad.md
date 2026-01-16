---
title: Creare un’esperienza di visualizzazione annuncio
description: Scopri come creare esperienze di annunci display in Adobe [!DNL GenStudio] for Performance Marketing.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
recommendations: noDisplay
exl-id: 7d5e777b-7a30-48f4-b253-9823e38eecce
source-git-commit: 4172d58660b0242976f73d7575142456ae8c4ae1
workflow-type: tm+mt
source-wordcount: '1135'
ht-degree: 0%

---

# Creare un’esperienza di visualizzazione annuncio

Questo tutorial illustra come generare [esperienze pubblicitarie con marchio](display-ad-experiences.md) utilizzando GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (icona del pennello nell&#39;area di navigazione a sinistra).

Per progettare un&#39;esperienza di visualizzazione coinvolgente, si consiglia di [aggiungere linee guida a GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md) e rivedere le [nozioni di base sui prompt di scrittura](/help/user-guide/effective-prompts.md) prima di iniziare.

## Scegli un modello

Per creare un’esperienza di visualizzazione annuncio, utilizza un modello disponibile per fornire il framework per il contenuto. Consulta [Linee guida per la visualizzazione dei modelli di annunci](/help/user-guide/templates/display-template.md) per informazioni sulle dimensioni di visualizzazione supportate.

**Per scegliere un modello di annuncio visualizzato**:

1. In _[!DNL Create]_, fai clic su **[!UICONTROL Annunci visualizzati]**.
1. Utilizza l&#39;opzione di ricerca, adiacente a _Filtro_, per trovare un modello di annuncio visualizzato specifico.
1. Nella visualizzazione _Seleziona modello_, fai clic su un modello di annuncio visualizzato.
1. Fai clic su **[!UICONTROL Usa]**.

   Viene visualizzato Canvas, che funge da hub centrale per la creazione dei contenuti.

## Aggiungi parametri

L&#39;aggiunta di [linee guida](/help/user-guide/guidelines/overview.md) e risorse in _Parametri_ nel cassetto dei prompt sovrascrive il processo di generazione del contenuto ed è un passaggio preparatorio integrale per la generazione di un&#39;esperienza di visualizzazione annuncio.

Se utilizzi un modello con linee guida predefinite (come [!DNL Brands], [!DNL Personas] o [!DNL Products]), queste linee guida si applicano alle tue varianti. Puoi modificarli se lo desideri.

![Immettere i parametri nel cassetto delle richieste](/help/assets/prompt-displayad2.png){width="50%" align="center"}

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

Dopo aver selezionato le linee guida, crea un prompt utilizzando il linguaggio naturale per iniziare a generare contenuti per la nuova esperienza di visualizzazione degli annunci. Per migliorare la qualità delle esperienze e dei display generati, è fondamentale creare prompt dettagliati e descrittivi.

Per ulteriori informazioni sulla scrittura dei prompt, vedere [Scrivi prompt effettivi](/help/user-guide/effective-prompts.md).

**Per immettere una richiesta**:

1. Immettere un prompt nella casella di prompt _&quot;Descrivi le esperienze da generare&quot;_.
2. Fai clic su **[!UICONTROL Genera]**.

Per impostazione predefinita, quattro varianti (alimentate dal prompt, dalle linee guida e dal contenuto aggiunto) vengono generate e visualizzate nell’area di lavoro.

## Rivedi varianti generate

Prima di selezionare gli elementi da inviare per l&#39;approvazione o la pubblicazione a [!DNL Content], è possibile modificare sezioni di annunci di visualizzazione e campi di testo oppure eliminare una variante generata.

Per evidenziare un singolo livello da rivedere, fare clic su un campo o un&#39;immagine modificabile e quindi su _[!UICONTROL Visualizza livelli]_.

**Per rivedere le varianti generate**:

* **Per [modificare il nome della bozza dell&#39;annuncio visualizzato](/help/user-guide/create/manage-variants.md#change-draft-name)**, fare clic sul titolo _Bozza senza titolo_ nella parte superiore dell&#39;area di lavoro e immettere un nuovo titolo.
* **Per [modificare manualmente un annuncio di visualizzazione](/help/user-guide/create/manage-variants.md#manually-edit-text)**, fare doppio clic in una sezione o in un campo dell&#39;annuncio di visualizzazione (ad esempio l&#39;oggetto, l&#39;intestazione o la copia del corpo) e modificarlo in base alle esigenze.
* **Per [applicare la formattazione del testo](/help/user-guide/create/manage-variants.md#manually-edit-text)** in una variante, fare clic sul testo nell&#39;immagine o sul collegamento in linea per una variante e quindi fare clic su **[!UICONTROL Formattare il testo]**.
* **Per [rigenerare una sezione di una variante](/help/user-guide/create/manage-variants.md#re-generate-sections)**, fai clic su un campo di testo modificabile e utilizza le _[!UICONTROL opzioni di modifica consigliate]_ oppure immetti un nuovo prompt nella _[!UICONTROL Generate new text_ section] e fai clic su **[!UICONTROL Generate]**.
* **Per [aggiungere o scambiare immagini in una variante](/help/user-guide/create/manage-variants.md#swap-image)**, fai clic su una risorsa immagine (o sull&#39;area della risorsa immagine se un&#39;immagine non esiste attualmente) e fai clic sull&#39;icona **[!UICONTROL Scambia da contenuto]**.
* **Per [aggiungere un collegamento a un&#39;immagine in una variante](/help/user-guide/create/manage-variants.md#add-image-link)**, fare clic su una risorsa immagine (o sull&#39;area della risorsa immagine se non esiste attualmente un&#39;immagine) e fare clic sull&#39;icona del collegamento.
* **Per [aggiungere testo alternativo per le immagini in una variante](/help/user-guide/create/manage-variants.md#add-alt-text-for-images)**, fare clic su una risorsa immagine e utilizzare l&#39;opzione _Testo alternativo_ per aggiungere o generare manualmente testo alternativo per immagine.
* **Per [aggiungere etichette di accesso facilitato](/help/user-guide/create/manage-variants.md#add-accessibility-labels) alle varianti**, fai clic su un&#39;immagine o su un collegamento a call-to-action, quindi fornisci una breve descrizione che spieghi il funzionamento del collegamento o del pulsante.
* **Per [modificare le dimensioni e le proporzioni dell&#39;annuncio](/help/user-guide/create/manage-variants.md#change-aspect-ratio)**, fare clic sul pulsante _[!UICONTROL Ridimensiona]_ (casella con l&#39;icona di un pulsante sul lato sinistro dell&#39;area di lavoro) e selezionare nuove dimensioni e proporzioni da applicare a tutte le varianti. Le varianti vengono duplicate e ridimensionate.
* **Per [ritagliare o riposizionare le immagini](/help/user-guide/create/manage-variants.md#crop-assets)**, fare clic su un&#39;immagine, fare clic su **[!UICONTROL Modifica]** (icona matita) e quindi su **[!UICONTROL Ritaglia]**. Regola le dimensioni e il posizionamento dell&#39;immagine.
* **Per [utilizzare l&#39;opzione di espansione generativa per ridimensionare e adattare le immagini](/help/user-guide/create/manage-variants.md#use-generative-expand) al modello di lavoro**, fare clic su un&#39;immagine, fare clic su **[!UICONTROL Modifica]** (icona a forma di matita) e quindi su **[!UICONTROL Espandi]**. Regola l’immagine per adattarla alle proporzioni e al modello necessari.

<!-- # Preview for device
When revising and preparing email experiences, you can toggle between previews for desktop and mobile views to ensure coherence and visual appeal of draft variants.
**To preview variants for desktop and mobile devices** toggle the device preview option—between **desktop** and **mobile**—in the right menu bar (computer and phone icons) to preview how variants appear. -->

## Invia feedback generazione

Per [inviare un feedback](/help/user-guide/create/manage-variants.md#generation-feedback) sulla qualità dell&#39;output di generazione, fare clic sull&#39;icona delle opzioni (tre punti) e selezionare **[!UICONTROL Output valido]** o **[!UICONTROL Output insufficiente]**.

## Verifica l’allineamento della verifica del contenuto

Per ottimizzare le varianti generate e garantire una rigorosa aderenza all&#39;identità del brand, alle linee guida della piattaforma e agli standard di accessibilità, sfrutta la potenza del pannello [_Verifica contenuto_](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Questo pannello mostra i dettagli completi del controllo dei contenuti e illumina le aree del miglioramento.

**Per eseguire controlli del contenuto su una variante**:

1. Fai clic sull&#39;icona del pannello _Verifica contenuto_ nella barra delle azioni a destra per aprire il pannello [_Verifica contenuto_](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Visualizza un riepilogo delle *verifiche necessarie* e *verifiche superate* per vedere quali sezioni e linee guida necessitano di miglioramenti.

   ![_Controllo contenuto_ pannello](/help/assets/content-check-panel.png){width="300"}

2. [Rivedi manualmente le varianti](#revise-generated-variants) per assicurarti che siano strettamente allineate con i controlli del contenuto eseguiti.

Consulta [Convalida marchio](/help/user-guide/guidelines/brand-validation.md).

## Ottieni recensioni e approvazioni

Utilizza il pannello Approvazioni, accessibile come icona sulla barra delle azioni a destra dell’area di lavoro, per ottenere revisioni, tenere traccia dei commenti di revisione e ottenere approvazioni dalle parti interessate.

**Per ottenere revisioni e approvazioni**:

1. [Avvia una richiesta di approvazione](/help/user-guide/approvals/request-review.md) per richiedere un [approvazione delle bozze di esperienze pubblicitarie](/help/user-guide/approvals/approve-content.md).
1. [Rimuovere o aggiungere revisori](/help/user-guide/approvals/review-and-edit.md#manage-approvals) durante il processo di revisione.
1. [Accedere al contenuto per la revisione](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) e visualizzare le richieste di revisione.
1. Modifica le bozze in base ai commenti di revisione e [pubblica le esperienze degli annunci di visualizzazione](#publish-and-export-experience).

Consulta [Recensioni e approvazioni](/help/user-guide/approvals/overview.md).

## Pubblicare ed esportare esperienze

Per rendere gli annunci di visualizzazione generati disponibili per l&#39;uso corrente e futuro, pubblicarli in [!UICONTROL Contenuto] ed esportarli per utilizzarli nelle campagne di marketing.

1. **Per pubblicare le nuove esperienze degli annunci visualizzati**, fai clic su **[!UICONTROL Pubblica]** nella barra degli strumenti superiore o nel flusso di approvazioni.
   1. Seleziona _[!UICONTROL [!DNL Campaigns]]_e aggiungi_[!UICONTROL  Ulteriori dettagli ]_, se necessario.
   1. Fai clic su **[!UICONTROL Pubblica]**.

      ![Pubblica un annuncio visualizzato](/help/assets/publish-displayad.png){width="450" zoomable="yes"}

1. **Per esportare le nuove esperienze degli annunci visualizzati**, fai clic su **[!UICONTROL Esporta]** nella barra degli strumenti superiore.
   1. Seleziona il formato (HTML e immagini, PNG o JPG) e fai clic su **[!UICONTROL Esporta]**.

      Il HTML esportato deve trovarsi all&#39;interno di una proprietà Web predefinita, ad esempio un modello o un contenitore `div`. Senza queste dimensioni impostate, le immagini potrebbero apparire distorte se visualizzate in modo indipendente.

Vedere [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content).
