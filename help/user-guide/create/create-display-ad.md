---
title: Creare un’esperienza di visualizzazione annuncio
description: Scopri come creare esperienze di annunci display in Adobe [!DNL GenStudio] for Performance Marketing.
feature: Brands Service, Guidelines, Content Generation, Generative AI, Create, Experiences, Variant Generation
role: User
level: Beginner
recommendations: noDisplay
source-git-commit: 816aeb55eee92758e7ef022ced0ebc3308d27dc9
workflow-type: tm+mt
source-wordcount: '849'
ht-degree: 0%

---

# Creare un’esperienza di visualizzazione annuncio

Questo tutorial illustra come generare [esperienze pubblicitarie con marchio](display-ad-experiences.md) utilizzando GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (icona del pennello nell&#39;area di navigazione a sinistra).

Per progettare un&#39;esperienza di visualizzazione coinvolgente, si consiglia di [aggiungere linee guida a GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md) e rivedere le [nozioni di base sui prompt di scrittura](/help/user-guide/effective-prompts.md) prima di iniziare.

## Scegli un modello

Per creare un’esperienza di visualizzazione annuncio, utilizza un modello disponibile per fornire il framework per il contenuto.

**Per scegliere un modello di annuncio visualizzato**:

1. In _[!DNL Create]_, fai clic su **[!UICONTROL Annunci visualizzati]**in_&quot;Cosa vuoi creare oggi?&quot;_sezione.
1. Utilizza l&#39;opzione di ricerca, adiacente a _Filtro_, per trovare un modello di annuncio visualizzato specifico.
1. Nella visualizzazione _Seleziona modello_, fai clic su un modello di annuncio visualizzato.
1. Fai clic su **[!UICONTROL Usa]**.

   Viene visualizzato Canvas, che funge da hub centrale per la creazione dei contenuti.

## Aggiungi parametri

L&#39;aggiunta di [linee guida](/help/user-guide/guidelines/overview.md) e risorse in _Parametri_ nel cassetto dei prompt sovrascrive il processo di generazione del contenuto ed è un passaggio preparatorio integrale per la generazione di un&#39;esperienza di visualizzazione annuncio.

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

![Immetti un prompt](/help/assets/prompt-displayad.png){width="650" zoomable="yes"}

Per ulteriori informazioni sulla scrittura dei prompt, vedere [Scrivi prompt effettivi](/help/user-guide/effective-prompts.md).

**Per immettere una richiesta**:

1. Immettere un prompt nella casella di prompt _&quot;Descrivi le esperienze da generare&quot;_.
1. Fai clic su **[!UICONTROL Genera]**.

Per impostazione predefinita, una variante, alimentata dal prompt, dalle linee guida e dal contenuto aggiunto, viene generata e visualizzata nell’area di lavoro.

## Rivedere gli annunci visualizzati generati

Prima di selezionare gli elementi da inviare per l&#39;approvazione o la pubblicazione a [!DNL Content], è possibile modificare sezioni di annunci di visualizzazione e campi di testo oppure eliminare una variante generata.

**Per rivedere le varianti generate**:

* **Per [modificare il nome della bozza dell&#39;annuncio visualizzato](/help/user-guide/create/manage-variants.md#change-draft-name)**, fare clic sul titolo _Bozza senza titolo_ nella parte superiore dell&#39;area di lavoro e immettere un nuovo titolo.
* **Per [modificare manualmente un annuncio di visualizzazione](/help/user-guide/create/manage-variants.md#manually-edit-text)**, fare doppio clic in una sezione o in un campo dell&#39;annuncio di visualizzazione (ad esempio l&#39;oggetto, l&#39;intestazione o la copia del corpo) e modificarlo in base alle esigenze.
* **Per [modificare le dimensioni e le proporzioni dell&#39;annuncio](/help/user-guide/create/manage-variants.md#change-aspect-ratio)**, fare clic sul pulsante _[!UICONTROL Ridimensiona]_ (casella con l&#39;icona di un pulsante sul lato sinistro dell&#39;area di lavoro) e selezionare nuove dimensioni e proporzioni da applicare a tutte le varianti. Le varianti vengono duplicate e ridimensionate.
* **Per [ritagliare o riposizionare le immagini](/help/user-guide/create/manage-variants.md#crop-assets)**, posizionare il puntatore del mouse sull&#39;immagine, fare clic sull&#39;icona di ritaglio visualizzata e modificare le dimensioni e il posizionamento dell&#39;immagine. Fai clic su **[!UICONTROL Applica]**.

<!-- # Preview for device
When revising and preparing email experiences, you can toggle between previews for desktop and mobile views to ensure coherence and visual appeal of draft variants.
**To preview variants for desktop and mobile devices** toggle the device preview option—between **desktop** and **mobile**—in the right menu bar (computer and phone icons) to preview how variants appear. -->

## Invia feedback generazione

Per [inviare un feedback](/help/user-guide/create/manage-variants.md#generation-feedback) sulla qualità dell&#39;output di generazione, fare clic sull&#39;icona delle opzioni (tre punti) e selezionare **[!UICONTROL Output valido]** o **[!UICONTROL Output insufficiente]**.

## Verificare l’allineamento del brand

Per ottimizzare gli annunci generati e garantire una rigorosa aderenza all&#39;identità del brand, sfrutta la potenza del [_pannello di convalida del brand_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel), che mostra dettagli completi sulla convalida del brand e illumina le aree di miglioramento.

**Per verificare l&#39;allineamento del brand**:

1. Fai clic sull&#39;icona di convalida del marchio nella barra dei menu superiore per aprire il [_pannello di convalida del marchio_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel). Puoi visualizzare i dettagli dei frammenti e le linee guida che necessitano di miglioramenti.

1. Passa da un annuncio all’altro per vedere come migliorare i contenuti generati per allinearli maggiormente al marchio.
1. [Rivedi manualmente gli annunci](#revise-generated-display-ads) per assicurarti che le e-mail siano strettamente allineate al tuo marchio.

Consulta [Convalida marchio](/help/user-guide/guidelines/brand-validation.md).

## Ottieni recensioni e approvazioni

Utilizza il pannello Approvazioni, accessibile nella barra dei menu superiore dell’area di lavoro, per ottenere recensioni, tenere traccia dei commenti di revisione e ottenere le approvazioni delle parti interessate.

**Per ottenere revisioni e approvazioni**:

1. [Avvia una richiesta di approvazione](/help/user-guide/approvals/request-review.md) per richiedere un [approvazione delle esperienze e-mail bozze](/help/user-guide/approvals/approve-content.md).
1. [Rimuovere o aggiungere revisori](/help/user-guide/approvals/review-and-edit.md#manage-approvals) durante il processo di revisione.
1. [Accedere al contenuto per la revisione](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) e visualizzare le richieste di revisione.
1. Modifica le bozze in base ai commenti di revisione e [pubblica le esperienze degli annunci di visualizzazione](#publish-and-export-experience).

Consulta [Recensioni e approvazioni](/help/user-guide/approvals/overview.md).

## Esperienza di esportazione e Publish

Per rendere gli annunci di visualizzazione generati disponibili per l&#39;uso corrente e futuro, pubblicarli in [!UICONTROL Contenuto] ed esportarli per utilizzarli nelle campagne di marketing.

1. **Per pubblicare le nuove esperienze di annunci display**, fai clic su **[!UICONTROL Publish]** nella barra degli strumenti superiore o nel flusso di approvazioni.
   1. Seleziona _[!UICONTROL [!DNL Campaigns]]_e aggiungi_[!UICONTROL  Ulteriori dettagli ]_, se necessario.
   1. Fai clic su **[!UICONTROL Pubblica]**.

      ![Publish annuncio visualizzato](/help/assets/publish-displayad.png){width="450" zoomable="yes"}

1. **Per esportare le nuove esperienze degli annunci visualizzati**, fai clic su **[!UICONTROL Esporta]** nella barra degli strumenti superiore.
   1. Seleziona il formato (solo JPG-) e fai clic su **[!UICONTROL Esporta]**.

Vedere [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content).
