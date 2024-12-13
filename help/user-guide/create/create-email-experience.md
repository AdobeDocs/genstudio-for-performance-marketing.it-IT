---
title: Creare un’esperienza e-mail
description: Scopri come creare esperienze e-mail in Adobe GenStudio for Performance Marketing.
feature: Content, Brands Service, Guidelines, Content Generation, Create, Experiences, Variant Generation
role: User
level: Beginner
recommendations: noDisplay
exl-id: 34446202-da98-45ff-869a-b43496a477f8
source-git-commit: 763c907598d92779483938295a99d640ee3f4d20
workflow-type: tm+mt
source-wordcount: '996'
ht-degree: 0%

---

# Creare un’esperienza e-mail

Questo tutorial illustra come generare [esperienze e-mail](/help/user-guide/create/email-experiences.md) con marchio utilizzando GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (icona del pennello nell&#39;area di navigazione a sinistra).

Per creare un&#39;esperienza e-mail efficace, ti consigliamo di [aggiungere linee guida a GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md) e di approfondire le [nozioni di base sulla creazione di un prompt](/help/user-guide/effective-prompts.md) prima di iniziare.

## Scegli un modello

Per creare una nuova esperienza e-mail, utilizza un modello disponibile per fornire il framework per il contenuto.

**Per scegliere un modello di posta elettronica**:

1. In _[!DNL Create]_, fare clic su **[!UICONTROL E-mail]**in_&quot;Cosa si desidera creare oggi?&quot;_sezione.
1. Utilizza l&#39;opzione di ricerca, accanto a _Filtro_, per trovare un modello e-mail specifico.
1. Fai clic su per selezionare un modello di e-mail e fai clic su **[!UICONTROL Usa]**.

   Viene visualizzato Canvas, l’epicentro della creazione dei contenuti.

## Aggiungi parametri

L&#39;aggiunta di [linee guida](/help/user-guide/guidelines/overview.md) e risorse in _Parametri_ nel cassetto dei prompt sovrascrive il processo di generazione del contenuto ed è un passaggio preparatorio integrale per la generazione di un&#39;esperienza e-mail.

**Per aggiungere parametri e risorse**:

1. Fai clic sull&#39;icona _Parametri_ per espandere il cassetto dei prompt.
1. Nella sezione _Parametri_, selezionare linee guida—[!DNL Brands], [!DNL Personas] e [!DNL Products], per informare la creazione dei contenuti.

   ![Scegli utente tipo](/help/assets/persona-select.png){width="600" zoomable="yes"}

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

Dopo aver selezionato le linee guida, crea un prompt utilizzando il linguaggio naturale per iniziare a generare contenuti per la nuova esperienza e-mail. I prompt dettagliati producono un output di qualità superiore rispetto ai prompt vaghi o non descrittivi.

Per ulteriori informazioni sulla scrittura dei prompt, vedere [Scrivi prompt effettivi](/help/user-guide/effective-prompts.md).

**Per immettere una richiesta**:

1. Immettere un prompt nella casella di prompt _&quot;Descrivi le esperienze da generare&quot;_.
1. Fai clic su **[!UICONTROL Genera]**.

Per impostazione predefinita, quattro varianti (tutte alimentate dal prompt, dalle linee guida e dal contenuto aggiunto) vengono generate e visualizzate nell’area di lavoro.

Il contenuto generato viene caricato progressivamente, man mano che vengono generate, le esperienze e-mail vengono visualizzate nell’area di lavoro. Consulta [Esperienze e-mail](/help/user-guide/create/meta-experiences.md#progressive-loading) per scoprire come vengono caricate le modifiche nell&#39;area di lavoro.

## Rivedere le e-mail generate

Prima di selezionare gli elementi da inviare per l&#39;approvazione o la pubblicazione a [!DNL Content], è possibile modificare le sezioni e-mail o eliminare una variante dal set di e-mail generate.

**Per rivedere le varianti generate**:

* **Per [modificare il nome della bozza e-mail](/help/user-guide/create/manage-variants.md#change-draft-name)**, fai clic sul titolo _Bozza senza titolo_ nella parte superiore dell&#39;area di lavoro e immetti un nuovo titolo.
* **Per [modificare manualmente un&#39;e-mail](/help/user-guide/create/manage-variants.md#manually-edit-text)**, fare clic in uno dei campi di testo modificabili (ad esempio l&#39;oggetto, l&#39;intestazione o la copia del corpo) e modificarli in base alle esigenze
* **Per [rigenerare una sezione di una variante](/help/user-guide/create/manage-variants.md#re-generate-sections)**, fare clic su un campo di testo modificabile e utilizzare le _[!UICONTROL opzioni di modifica consigliate]_ oppure immettere un nuovo prompt e fare clic su **[!UICONTROL Genera]**.
* **Per [aggiungere o scambiare immagini in una variante](/help/user-guide/create/manage-variants.md#swap-image)**, fai clic su una risorsa immagine (o sull&#39;area della risorsa immagine se un&#39;immagine non esiste attualmente), quindi fai clic su **[!UICONTROL Seleziona/scambia dal contenuto]** o su **[!UICONTROL Carica nuova immagine]** per aggiungere o scambiare un&#39;immagine in una singola variante.
* **Per [eliminare un&#39;e-mail](/help/user-guide/create/manage-variants.md#delete-variant)**, fare clic per selezionare il titolo dell&#39;e-mail (ad esempio, &quot;E-mail 1/4&quot;) e fare clic su **[!UICONTROL Elimina variante]**.

## Invia feedback generazione

Per [inviare un feedback](/help/user-guide/create/manage-variants.md#generation-feedback) sulla qualità dell&#39;output di generazione, fare clic sull&#39;icona delle opzioni (tre punti) e selezionare **[!UICONTROL Output valido]** o **[!UICONTROL Output insufficiente]**.

## Anteprima per dispositivo

Durante la revisione e la preparazione delle esperienze e-mail, puoi [passare da un&#39;anteprima all&#39;altra per le visualizzazioni desktop e mobile](/help/user-guide/create/manage-variants.md#preview-for-device) per garantire la coerenza e l&#39;impatto visivo delle varianti di bozza.

## Verificare l’allineamento del brand

Per ottimizzare le e-mail generate e garantire una rigorosa aderenza alla brand identity, sfrutta la potenza del [_controllo delle linee guida per il brand_](/help/user-guide/guidelines/brand-validation.md#brand-guidelines-check), che fornisce un riepilogo dell’allineamento del brand per una variante, e del pannello [_Convalida del brand_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel), che mostra dettagli completi sulla convalida del brand e illustra le aree di miglioramento.

**Per verificare l&#39;allineamento del brand**:

1. Fai clic sull&#39;icona [**[!UICONTROL [!DNL Brand] controllo delle linee guida]**](/help/user-guide/guidelines/brand-validation.md#brand-guidelines-check) per una variante e visualizza un riepilogo delle prestazioni della variante quando questa viene confrontata con il tuo marchio.

   ![Verifica delle linee guida per i marchi](/help/assets/brand-guidelines-check.png){width="350" zoomable="yes"}

1. Per ottenere i dettagli delle sezioni e delle linee guida che necessitano di miglioramenti, fai clic su **[!UICONTROL Rivedi]** _o_ fai clic sull&#39;icona Convalida marchio nella barra dei menu superiore per aprire il [_pannello di convalida marchio_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel).

1. Passa da un’e-mail all’altra per vedere come migliorare il contenuto generato in modo che sia più allineato al brand.

   ![Pannello di convalida del marchio](/help/assets/brand-validation-panel.png){width="600" zoomable="yes"}

1. [Rivedi manualmente le e-mail](#revise-generated-emails) per assicurarti che siano strettamente allineate al tuo marchio.

Consulta [Convalida marchio](/help/user-guide/guidelines/brand-validation.md).

## Ottieni recensioni e approvazioni

Utilizza il pannello Approvazioni, accessibile nella barra dei menu superiore dell’area di lavoro, per ottenere recensioni, tenere traccia dei commenti di revisione e ottenere le approvazioni delle parti interessate.

**Per ottenere revisioni e approvazioni**:

1. [Avvia una richiesta di approvazione](/help/user-guide/approvals/request-review.md) per richiedere un [approvazione delle esperienze e-mail bozze](/help/user-guide/approvals/approve-content.md).
1. [Rimuovere o aggiungere revisori](/help/user-guide/approvals/review-and-edit.md#manage-approvals) durante il processo di revisione.
1. [Accedere al contenuto per la revisione](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) e visualizzare le richieste di revisione.
1. Modifica le bozze in base ai commenti di revisione e [pubblica le tue esperienze e-mail](#publish-and-export-experience).

Per ulteriori informazioni, vedere [Recensioni e approvazioni](/help/user-guide/approvals/overview.md).

## Esperienza di esportazione e Publish

Per rendere le e-mail generate disponibili per l&#39;uso corrente e futuro, pubblicale in [!UICONTROL Contenuto] ed esportalo per utilizzarlo nelle campagne di marketing.

1. **Per pubblicare le nuove esperienze e-mail**, fai clic su **[!UICONTROL Publish]** nella barra degli strumenti superiore o nel flusso di approvazioni.
1. **Per esportare le nuove esperienze e-mail**, fai clic su **[!UICONTROL Esporta]** nella barra degli strumenti superiore.
   1. Seleziona il formato (solo CSV e immagini o HTML) e fai clic su **[!UICONTROL Esporta]**.

Per ulteriori informazioni, vedere [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content).
