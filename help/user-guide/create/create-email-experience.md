---
title: Creare un’esperienza e-mail
description: Scopri come creare esperienze e-mail in Adobe GenStudio for Performance Marketing.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
recommendations: noDisplay
exl-id: 34446202-da98-45ff-869a-b43496a477f8
source-git-commit: 0db148b99a78714020b0ad4d9c1f71e6ccc945b5
workflow-type: tm+mt
source-wordcount: '1084'
ht-degree: 1%

---

# Creare un’esperienza e-mail

Questo tutorial illustra come generare [esperienze e-mail](/help/user-guide/create/email-experiences.md) con marchio utilizzando GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (icona del pennello nell&#39;area di navigazione a sinistra).

Per creare un&#39;esperienza e-mail efficace, ti consigliamo di [aggiungere linee guida a GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md) e di approfondire le [nozioni di base sulla creazione di un prompt](/help/user-guide/effective-prompts.md) prima di iniziare.

## Scegli un modello

Per creare una nuova esperienza e-mail, utilizza un modello disponibile per fornire il framework per il contenuto.

**Per scegliere un modello di posta elettronica**:

1. In _[!DNL Create]_, fare clic su **[!UICONTROL E-mail]**.
1. Utilizza l&#39;opzione di ricerca, accanto a _Filtro_, per trovare un modello e-mail specifico.
1. Fai clic su per selezionare un modello di e-mail e fai clic su **[!UICONTROL Usa]**.

   Viene visualizzato Canvas, l’epicentro della creazione dei contenuti.

## Aggiungi parametri

L&#39;aggiunta di [linee guida](/help/user-guide/guidelines/overview.md) e risorse in _Parametri_ nel cassetto dei prompt sovrascrive il processo di generazione del contenuto ed è un passaggio preparatorio integrale per la generazione di un&#39;esperienza e-mail.

Se utilizzi un modello con linee guida predefinite (come [!DNL Brands], [!DNL Personas] o [!DNL Products]), queste linee guida si applicano alle tue varianti. Puoi modificarli se lo desideri.

**Per aggiungere parametri e risorse**:

1. Fai clic sull&#39;icona _Parametri_ per espandere il cassetto dei prompt.
1. Nella sezione _Parametri_, selezionare linee guida—[!DNL Brands], [!DNL Personas] e [!DNL Products], per informare la creazione dei contenuti.

   ![Scegli utente tipo](/help/assets/persona-select-email.png){width="300" align="center"}

   Se da questi menu non sono disponibili marchi, utenti tipo o prodotti, [aggiungi linee guida al tuo GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md).

1. Aggiungi contenuto da utilizzare nell&#39;esperienza *e* per influenzare la generazione del contenuto:
   * Fare clic su **[!UICONTROL Seleziona dal contenuto]** per selezionare le risorse (immagini) dal repository [!DNL Content], filtrare e selezionare una o più immagini.

     ![Scegli contenuto visivo](/help/assets/content-select-email.png){width="500" zoomable="yes"}

     Per utilizzare le risorse da un repository [!DNL AEM Assets Content Hub] connesso, scegliere un repository dal menu a discesa _Posizione_. Filtra e seleziona una o più immagini.

   * In alternativa, trascina e rilascia le risorse nella sezione **[!UICONTROL Seleziona da contenuto]** per caricare una o più nuove risorse.
1. Fai clic su **[!UICONTROL Usa]**.

   >[!NOTE]
   >Se il modello di posta elettronica include più sezioni, selezionare [!DNL Products] e contenuto (risorse visive) per ogni sezione di posta elettronica in _Messaggi di posta elettronica con più sezioni_. Le e-mail con più sezioni supportano una risorsa visiva per sezione. È possibile aggiungere solo risorse visive alle e-mail con più sezioni da [!DNL Content]. Non è possibile trascinare e rilasciare o caricare risorse dall&#39;origine locale.
   >![Aggiungi contenuto e parametri per ogni sezione e-mail](/help/assets/parameters-multisection-email.png){width="450" zoomable="yes"}

Dopo aver aggiunto i parametri, è possibile comprimere il cassetto dei prompt facendo nuovamente clic sull&#39;icona _Parametri_.

## Immetti un prompt

Dopo aver selezionato le linee guida, crea un prompt utilizzando il linguaggio naturale per iniziare a generare contenuti per la nuova esperienza e-mail. I prompt dettagliati producono un output di qualità superiore rispetto ai prompt vaghi o ambigui.

Per ulteriori informazioni sulla scrittura dei prompt, vedere [Scrivi prompt effettivi](/help/user-guide/effective-prompts.md).

**Per immettere una richiesta**:

1. Immettere un prompt nella casella di prompt _&quot;Descrivi le esperienze da generare&quot;_.
1. Fai clic su **[!UICONTROL Genera]**.

Per impostazione predefinita, quattro varianti (tutte alimentate dal prompt, dalle linee guida e dal contenuto aggiunto) vengono generate e visualizzate nell’area di lavoro.

Il contenuto generato viene caricato progressivamente, man mano che vengono generate, le esperienze e-mail vengono visualizzate nell’area di lavoro. Consulta [Esperienze e-mail](/help/user-guide/create/meta-experiences.md#progressive-loading) per scoprire come vengono caricate le modifiche nell&#39;area di lavoro.

## Rivedi varianti generate

Prima di selezionare gli elementi da inviare per l&#39;approvazione o la pubblicazione a [!DNL Content], è possibile modificare le sezioni e-mail o eliminare una variante dal set di e-mail generate.

**Per rivedere le varianti generate**:

* **Per [modificare il nome della bozza e-mail](/help/user-guide/create/manage-variants.md#change-draft-name)**, fai clic sul titolo _Bozza senza titolo_ nella parte superiore dell&#39;area di lavoro e immetti un nuovo titolo.
* **Per [modificare manualmente un&#39;e-mail](/help/user-guide/create/manage-variants.md#manually-edit-text)**, fare clic in uno dei campi di testo modificabili (ad esempio l&#39;oggetto, l&#39;intestazione o la copia del corpo) e modificarli in base alle esigenze
* **Per [modificare o selezionare Call to action](/help/user-guide/create/manage-variants.md#revise-call-to-action)**, fare clic sul pulsante call-to-action e selezionare _[!UICONTROL Riformula]_ o _[!UICONTROL Aggiungi collegamento]_.
* **Per [applicare la formattazione del testo](/help/user-guide/create/manage-variants.md#manually-edit-text)** in una variante, fare clic sul testo nell&#39;immagine di una variante e fare clic su **[!UICONTROL Formatta testo]**.
* **Per [rigenerare una sezione di una variante](/help/user-guide/create/manage-variants.md#re-generate-sections)**, fare clic su un campo di testo modificabile e utilizzare le _[!UICONTROL opzioni di modifica consigliate]_ oppure immettere un nuovo prompt e fare clic su **[!UICONTROL Genera]**.
* **Per [aggiungere o scambiare immagini in una variante](/help/user-guide/create/manage-variants.md#swap-image)**, fai clic su una risorsa immagine (o sull&#39;area della risorsa immagine se un&#39;immagine non esiste attualmente) e fai clic sull&#39;icona **[!UICONTROL Scambia da contenuto]**.
* **Per [aggiungere un collegamento a un&#39;immagine in una variante](/help/user-guide/create/manage-variants.md#add-image-link)**, fare clic su una risorsa immagine (o sull&#39;area della risorsa immagine se non esiste attualmente un&#39;immagine) e fare clic sull&#39;icona del collegamento.
* **Per [aggiungere testo alternativo per le immagini in una variante](/help/user-guide/create/manage-variants.md#add-alt-text-for-images)**, fare clic su una risorsa immagine e utilizzare l&#39;opzione _Testo alternativo_ per aggiungere o generare manualmente testo alternativo per immagine.
* **Per [aggiungere etichette di accesso facilitato](/help/user-guide/create/manage-variants.md#add-accessibility-labels) alle varianti**, fai clic su un&#39;immagine o su un collegamento a call-to-action, quindi fornisci una breve descrizione che spieghi il funzionamento del collegamento o del pulsante.
* **Per [eliminare un&#39;e-mail](/help/user-guide/create/manage-variants.md#delete-variant)**, fare clic per selezionare il titolo dell&#39;e-mail (ad esempio, &quot;E-mail 1/4&quot;) e fare clic su **[!UICONTROL Elimina variante]**.

## Invia feedback generazione

Per [inviare un feedback](/help/user-guide/create/manage-variants.md#generation-feedback) sulla qualità dell&#39;output di generazione, fare clic sull&#39;icona delle opzioni (tre punti) e selezionare **[!UICONTROL Output valido]** o **[!UICONTROL Output insufficiente]**.

## Anteprima per dispositivo

Durante la revisione e la preparazione delle esperienze e-mail, puoi [passare da un&#39;anteprima all&#39;altra per le visualizzazioni desktop e mobile](/help/user-guide/create/manage-variants.md#preview-for-device) per garantire la coerenza e l&#39;impatto visivo delle varianti di bozza.

## Verifica l’allineamento della verifica del contenuto

Per ottimizzare le varianti generate e garantire una rigorosa aderenza all&#39;identità del brand, alle linee guida della piattaforma e agli standard di accessibilità, sfrutta la potenza del pannello [_Verifica contenuto_](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Questo pannello mostra i dettagli completi del controllo dei contenuti e illumina le aree del miglioramento.

**Per eseguire controlli del contenuto su una variante**:

1. Fai clic sull&#39;icona del pannello _Verifica contenuto_ nella barra delle azioni a destra per aprire il pannello [_Verifica contenuto_](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Visualizza un riepilogo delle *verifiche necessarie* e *verifiche superate* per vedere quali sezioni e linee guida necessitano di miglioramenti.

   ![_Controllo contenuto_ pannello](/help/assets/content-check-panel.png){height="400" zoomable="yes"}

1. [Rivedi manualmente le varianti](#revise-generated-variants) per assicurarti che siano strettamente allineate con i controlli del contenuto eseguiti.

Consulta [Convalida marchio](/help/user-guide/guidelines/brand-validation.md).

## Ottieni recensioni e approvazioni

Utilizza il pannello Approvazioni, accessibile come icona sulla barra delle azioni a destra dell’area di lavoro, per ottenere revisioni, tenere traccia dei commenti di revisione e ottenere approvazioni dalle parti interessate.

**Per ottenere revisioni e approvazioni**:

1. [Avvia una richiesta di approvazione](/help/user-guide/approvals/request-review.md) per richiedere un [approvazione delle esperienze e-mail bozze](/help/user-guide/approvals/approve-content.md).
1. [Rimuovere o aggiungere revisori](/help/user-guide/approvals/review-and-edit.md#manage-approvals) durante il processo di revisione.
1. [Accedere al contenuto per la revisione](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) e visualizzare le richieste di revisione.
1. Modifica le bozze in base ai commenti di revisione e [pubblica le tue esperienze e-mail](#publish-and-export-experience).

Per ulteriori informazioni, vedere [Recensioni e approvazioni](/help/user-guide/approvals/overview.md).

## Pubblicare ed esportare esperienze

Per rendere le e-mail generate disponibili per l&#39;uso corrente e futuro, pubblicale in [!UICONTROL Contenuto] ed esportalo per utilizzarlo nelle campagne di marketing.

1. **Per pubblicare le nuove esperienze e-mail**, fai clic su **[!UICONTROL Pubblica]** nella barra degli strumenti superiore o nel flusso di approvazioni.
1. **Per esportare le nuove esperienze e-mail**, fai clic su **[!UICONTROL Esporta]** nella barra degli strumenti superiore.
   1. Seleziona il formato (solo CSV e immagini o HTML) e fai clic su **[!UICONTROL Esporta]**.

Per ulteriori informazioni, vedere [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content).
