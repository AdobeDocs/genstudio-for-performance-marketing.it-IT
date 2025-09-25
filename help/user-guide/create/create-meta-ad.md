---
title: Creare un’esperienza Meta Ad
description: Scopri come creare esperienze pubblicitarie on-brand Meta (per Facebook o Instagram) con Adobe GenStudio for Performance Marketing.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
recommendations: noDisplay
exl-id: 42111bbf-70cd-4fd2-a7a9-15abe072d720
source-git-commit: 47195c08f500e50a01db127c6badc461c10afaf9
workflow-type: tm+mt
source-wordcount: '1392'
ht-degree: 0%

---

# Creare un’esperienza di annuncio Meta

Questo tutorial illustra come generare [esperienze pubblicitarie Meta](/help/user-guide/create/meta-experiences.md) con il marchio utilizzando GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (icona del pennello nell&#39;area di navigazione a sinistra).

Prima di iniziare a generare un&#39;esperienza pubblicitaria di Meta, è importante [incorporare le linee guida](/help/user-guide/guidelines/add-guidelines.md) in GenStudio for Performance Marketing e acquisire familiarità con le nozioni di base sulla [creazione di un prompt](/help/user-guide/effective-prompts.md).

## Scegli un modello

Per iniziare a generare una nuova esperienza pubblicitaria in Meta, utilizza un modello disponibile per fornire il framework per il contenuto. Consulta [Linee guida per i modelli di annunci Meta](/help/user-guide/templates/meta-template.md) per informazioni sulle proporzioni degli annunci Meta supportati.

Quando selezioni un modello, puoi utilizzare uno dei modelli caricati o un modello iniziale.

**Per scegliere un modello di annuncio Meta**:

1. In _[!DNL Create]_, fai clic su **[!UICONTROL Meta ads]**.
1. Seleziona **[!UICONTROL Modelli personalizzati]** per sfogliare i modelli caricati oppure **[!UICONTROL Modelli iniziali]** per sfogliare i modelli predefiniti.

   Se prevedi di aggiungere risorse video alle varianti di Meta, devi scegliere un modello iniziale. Vengono precaricate con aree di contenuto definite dal sistema che facilitano l’utilizzo dei video.

1. Fare clic per selezionare un modello e fare clic su **[!UICONTROL Usa]**.

   Questa azione apre Canvas, l’hub centrale per la creazione dei contenuti.

## Aggiungi parametri

L&#39;aggiunta di [linee guida](/help/user-guide/guidelines/overview.md) e risorse in _Parametri_ nel cassetto dei prompt migliora il processo di generazione dei contenuti ed è un passaggio fondamentale nella preparazione alla generazione di un annuncio Meta.

Se si utilizza un modello con linee guida predefinite, [!DNL Brands], [!DNL Personas] o [!DNL Products], queste linee guida si applicano alle varianti. Puoi modificarli se lo desideri.

**Per aggiungere parametri e risorse**:

1. Fai clic sull&#39;icona _Parametri_ per espandere il cassetto dei prompt.
1. Nella sezione _Parametri_, selezionare linee guida—[!DNL Brands], [!DNL Personas] e [!DNL Products], per informare la creazione dei contenuti.

   ![Scegli utente tipo](/help/assets/persona-select.png){width="600" zoomable="yes"}

   Se da questi menu non sono disponibili marchi, utenti tipo o prodotti, [aggiungi linee guida al tuo GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md).

1. Aggiungi contenuto (immagini o video) da utilizzare nell&#39;esperienza *e* per influenzare la generazione di contenuti:
   * Fare clic su **[!UICONTROL Seleziona dal contenuto]** per selezionare le risorse dal repository [!DNL Content], filtrare e selezionare una o più immagini.

     Se utilizzi un modello con una sezione per video, il contenuto video (.mp4) verrà preselezionato e filtrato automaticamente. Passa il cursore del mouse su un video per visualizzare un’anteprima riprodotta automaticamente.

     ![Scegli contenuto visivo](/help/assets/content-select-meta.png){width="500" zoomable="yes"}

     Per utilizzare le risorse da un repository [!DNL AEM Assets Content Hub] connesso, scegliere un repository dal menu a discesa _Posizione_. Filtra e seleziona una o più immagini.

   * In alternativa, trascina le immagini nella sezione **[!UICONTROL Seleziona da contenuto]** per caricare una o più nuove risorse.

1. Fai clic su **[!UICONTROL Usa]**.

Dopo aver aggiunto i parametri, è possibile comprimere il cassetto dei prompt facendo nuovamente clic sull&#39;icona _Parametri_.

## Immetti un prompt

Dopo aver selezionato le linee guida, crea un prompt utilizzando il linguaggio naturale per iniziare a generare contenuti per la nuova esperienza pubblicitaria Meta. I prompt dettagliati producono un output di qualità superiore rispetto ai prompt vaghi o ambigui.

Per ulteriori informazioni sulla scrittura dei prompt, vedere [Scrivi prompt effettivi](/help/user-guide/effective-prompts.md).

**Per immettere una richiesta**:

1. Immettere un prompt nella casella di prompt _&quot;Descrivi le esperienze da generare&quot;_.
1. Fai clic su **[!UICONTROL Genera]**.

   Consulta [Gestire i video](#manage-videos) per capire come vengono generati e come gestirli.

Per impostazione predefinita, quattro varianti (tutte alimentate dal prompt, dalle linee guida e dal contenuto aggiunto) vengono generate e visualizzate nell’area di lavoro.

Il contenuto generato viene caricato progressivamente, man mano che vengono generate, le esperienze Meta vengono visualizzate nell’area di lavoro. Consulta [Esperienze Meta](/help/user-guide/create/meta-experiences.md#progressive-loading) per scoprire come vengono caricate le modifiche nell&#39;area di lavoro.

## Scegli il canale degli annunci Meta

Durante la generazione di un annuncio Meta, puoi scegliere tra annunci Facebook o Instagram.

Attiva/disattiva l&#39;opzione del canale Meta ads (tra **Facebook** e **Instagram**) nella barra dei menu a destra (icone Facebook e Instagram) per visualizzare e gestire le varianti di ogni canale.

Quando [rivedi gli annunci Meta](#revise-generated-variants), puoi modificare le proporzioni degli annunci Facebook e Instagram.

## Rivedi varianti generate

Prima di selezionare gli elementi da inviare per l&#39;approvazione o la pubblicazione a [!DNL Content], è possibile modificare gli annunci di Meta o eliminare una variante dal set di annunci generati.

Per evidenziare un singolo livello da rivedere, fare clic su un campo o un&#39;immagine modificabile e quindi su _[!UICONTROL Visualizza livelli]_.

**Per rivedere le varianti generate**:

* **Per [modificare il nome della bozza dell&#39;annuncio di Meta](/help/user-guide/create/manage-variants.md#change-draft-name)**, fare clic sul titolo _Untitled Draft_ nella parte superiore dell&#39;area di lavoro e immettere un nuovo titolo.
* **Per [modificare manualmente un annuncio di Meta](/help/user-guide/create/manage-variants.md#manually-edit-text)**, fare clic in una delle sezioni dell&#39;annuncio (ad esempio l&#39;oggetto,
o body copy) e modificarli in base alle esigenze.
* **Per modificare o selezionare call to action**, fare clic sul pulsante call-to-action e selezionare le opzioni di testo disponibili per il pulsante. In _Collegamento_, immettere un URL per il testo di call-to-action.
* **Per [applicare la formattazione del testo](/help/user-guide/create/manage-variants.md#manually-edit-text)** in una variante, fare clic sul testo nell&#39;immagine o sul collegamento in linea per una variante e quindi fare clic su **[!UICONTROL Formattare il testo]**.
<!-- **To [change or select the Call to action](/help/user-guide/create/manage-variants.md#revise-call-to-action)**, click the call-to-action button and select _[!UICONTROL Rephrase]_ or _[!UICONTROL Add link]_. -->
* **Per [aggiungere un collegamento a un&#39;immagine in una variante](/help/user-guide/create/manage-variants.md#add-image-link)**, fare clic su una risorsa immagine (o sull&#39;area della risorsa immagine se non esiste attualmente un&#39;immagine) e fare clic sull&#39;icona del collegamento.
* **Per [modificare le dimensioni e le proporzioni dell&#39;annuncio](/help/user-guide/create/manage-variants.md#change-aspect-ratio)**, fare clic sul pulsante _[!UICONTROL Ridimensiona]_ (casella con l&#39;icona di un pulsante sul lato sinistro dell&#39;area di lavoro) e selezionare nuove dimensioni e proporzioni da applicare a tutte le varianti. Le varianti vengono duplicate e ridimensionate.
* **Per [rigenerare una sezione di una variante](/help/user-guide/create/manage-variants.md#re-generate-sections)**, fare clic su un campo di testo modificabile e utilizzare le _[!UICONTROL opzioni di modifica consigliate]_ oppure immettere un nuovo prompt e fare clic su **[!UICONTROL Genera]**.
* **Per [aggiungere o scambiare immagini in una variante](/help/user-guide/create/manage-variants.md#swap-image)**, fai clic su una risorsa immagine (o sull&#39;area della risorsa immagine se un&#39;immagine non esiste attualmente) e fai clic sull&#39;icona **[!UICONTROL Scambia da contenuto]**.
* **Per [ritagliare o riposizionare le immagini](/help/user-guide/create/manage-variants.md#crop-assets)**, fare clic su un&#39;immagine, fare clic su **[!UICONTROL Modifica]** (icona matita) e quindi su **[!UICONTROL Ritaglia]**. Regola le dimensioni e il posizionamento dell&#39;immagine.
* **Per [utilizzare l&#39;opzione di espansione generativa per ridimensionare e adattare le immagini](/help/user-guide/create/manage-variants.md#use-generative-expand) al modello di lavoro**, fare clic su un&#39;immagine, fare clic su **[!UICONTROL Modifica]** (icona a forma di matita) e quindi su **[!UICONTROL Espandi]**. Regola l’immagine per adattarla alle proporzioni e al modello necessari.
* **Per [aggiungere testo alternativo per le immagini in una variante](/help/user-guide/create/manage-variants.md#add-alt-text-for-images)**, fare clic su una risorsa immagine e utilizzare l&#39;opzione _Testo alternativo_ per aggiungere o generare manualmente testo alternativo per immagine.
* **Per [aggiungere etichette di accesso facilitato](/help/user-guide/create/manage-variants.md#add-accessibility-labels) alle varianti**, fai clic su un&#39;immagine o su un collegamento a call-to-action, quindi fornisci una breve descrizione che spieghi il funzionamento del collegamento o del pulsante.
* **Per [eliminare un annuncio di Meta](/help/user-guide/create/manage-variants.md#delete-variant)**, fare clic sul menu delle opzioni per una variante e quindi su **[!UICONTROL Elimina variante]**.

### Gestire i video

Passa il puntatore del mouse su ciascuno dei video per visualizzare la riproduzione automatica ciclica.

I video vengono riorganizzati per adattarsi alle proporzioni selezionate durante la generazione. Ripristinare il video originale non riformattato facendo clic su **[!UICONTROL Rielabora video]** e disattivandolo.

## Invia feedback generazione

Per [inviare un feedback](/help/user-guide/create/manage-variants.md#generation-feedback) sulla qualità dell&#39;output di generazione, fare clic sull&#39;icona delle opzioni (tre punti) e selezionare **[!UICONTROL Output valido]** o **[!UICONTROL Output insufficiente]**.

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

1. [Avvia una richiesta di approvazione](/help/user-guide/approvals/request-review.md) per richiedere un [approvazione delle bozze di esperienze pubblicitarie di Meta](/help/user-guide/approvals/approve-content.md).

   ![Invia bozze per revisione e approvazione](/help/assets/send-approval-meta.png){width="450" zoomable="yes"}

1. [Rimuovere o aggiungere revisori](/help/user-guide/approvals/review-and-edit.md#manage-approvals) durante il processo di revisione.
1. [Accedere al contenuto per la revisione](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) e visualizzare le richieste di revisione.
1. Modifica le bozze in base ai commenti di revisione e [pubblica le esperienze degli annunci Meta](#publish-and-export-experience).

Per ulteriori informazioni, vedere [Recensioni e approvazioni](/help/user-guide/approvals/overview.md).

## Pubblicare ed esportare esperienze

Per rendere gli annunci Meta generati disponibili per l&#39;uso corrente e futuro, pubblicarli in [!UICONTROL Contenuto] ed esportarli per utilizzarli nelle campagne di marketing.

1. **Per pubblicare le nuove esperienze pubblicitarie di Meta**, fai clic su **[!UICONTROL Pubblica]** nella barra degli strumenti superiore o nel flusso di approvazioni.
1. **Per esportare le nuove esperienze pubblicitarie di Meta**, fai clic su **[!UICONTROL Esporta]** nella barra degli strumenti superiore.
   1. Seleziona il formato: HTML e immagini o CSV e immagini (JPG o PNG). Fai clic su **[!UICONTROL Esporta]**.

Per ulteriori informazioni, vedere [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content).

## Connetti Meta

Puoi collegare GenStudio for Performance Marketing a Meta per ricevere analisi avanzate e approfondimenti sulle prestazioni dei contenuti.

Vedi [Connessione annunci Meta](/help/user-guide/connectors/meta-ads.md).
