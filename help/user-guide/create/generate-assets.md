---
title: Genera immagini
description: Crea un'immagine corrispondente allo stile di un'immagine di riferimento in Adobe [!DNL GenStudio] for Performance Marketing.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
badgeBeta: label="Beta" tooltip="Questa funzione è attualmente in Beta, quindi alcune funzionalità potrebbero essere limitate o soggette a modifiche."
role: User
level: Beginner
recommendations: noDisplay
source-git-commit: 277731aeea966da3cbd1fdabf015bfab3b907d39
workflow-type: tm+mt
source-wordcount: '795'
ht-degree: 0%

---

# Genera immagini

Utilizzando GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (icona del pennello), è possibile generare _[!DNL On-brand images]_risorse generate che traggono ispirazione da un&#39;immagine scelta, acquisendone l&#39;impatto visivo e l&#39;estetica complessiva.<!-- [two types of images](#image-types) using GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (paintbrush icon)—_[!DNL On-brand images]_ and _[!DNL Similar images]_. -->

Per progettare un&#39;immagine accattivante ed efficace, si consiglia di [aggiungere linee guida a GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md) e rivedere le [nozioni di base sulla scrittura dei prompt](/help/user-guide/effective-prompts.md).

## Tipi di immagini

_[!DNL On-brand images]_sono risorse generate che traggono ispirazione da un&#39;immagine scelta, catturandone l&#39;impatto visivo e l&#39;estetica complessiva. Queste immagini vengono create utilizzando le immagini già disponibili in [!DNL Content] e un prompt creato con cura che ne guida la progettazione. Seguono rigorosamente sia le linee guida del marchio che i parametri scelti durante il processo di generazione.

_[!DNL On-brand images]_<!-- and _[!DNL Similar images]_ --> incorpora linee guida per set, parametri e un [prompt creato con cura](/help/user-guide/effective-prompts.md) per fornire risorse di immagine accattivanti.

<!-- * _[!DNL Similar images]_—Image assets created with strong similarity to an existing selected image available in [!DNL Content]. When generating similar images, GenStudio for Performance Marketing redesigns the selected image, giving slight variations on the content to provide variety and nuance. -->

## Generare immagini nel marchio

Puoi generare [!DNL On-brand images] utilizzando linee guida, parametri e un&#39;immagine di riferimento selezionati. Questi elementi, insieme al prompt, guidano la generazione di varianti [!DNL On-brand image] coerenti.

### Scegli un&#39;immagine di riferimento

Per creare un _[!DNL On-brand images]_, selezionare un&#39;immagine esistente salvata in [!DNL Content]. Consulta [Best practice per i modelli](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines) per informazioni sulle dimensioni [!DNL on-brand image] supportate.

**Per scegliere un&#39;immagine di riferimento**:

1. In _[!DNL Create]_, fai clic su **[!UICONTROL Immagine marchio]**.
1. Utilizza l&#39;opzione di ricerca, adiacente al _filtro_, per trovare un&#39;immagine specifica.

   ![Seleziona immagine di riferimento](/help/assets/select-img.png){width="400" zoomable="yes"}

   Per utilizzare le risorse di un repository [!DNL AEM Assets Content Hub] connesso, scegliere un repository dal menu a discesa _Posizione_. Filtra e seleziona un’immagine.

1. Nella visualizzazione _Seleziona immagine_, fai clic su un&#39;immagine.

   Le dimensioni dell&#39;immagine selezionata non possono superare i 10 MB.

1. Fai clic su **[!UICONTROL Usa]**.

   Viene visualizzato Canvas, che funge da hub centrale per la creazione dei contenuti.

### Aggiungi parametri

L&#39;incorporazione di [linee guida](/help/user-guide/guidelines/overview.md) e parametri migliora il processo di generazione dei contenuti ed è un passaggio preparatorio fondamentale per la produzione di [!DNL on-brand image].

**Per aggiungere linee guida e parametri**:

1. Nella scheda _Base_, seleziona un [!DNL Brand] per informare la creazione dei contenuti.

   Se non sono disponibili marchi da questo menu, [aggiungi le linee guida al tuo GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md).

1. Seleziona una categoria di immagini che si adatta meglio al risultato desiderato da _[!UICONTROL Categoria immagine]_.

   Le categorie di immagini sono disponibili se è stato selezionato [!DNL Brand]. Le opzioni sono determinate dal [!DNL Brand] selezionato.

<!-- 1. _(Optional)_ Select a custom model from _[!UICONTROL Model]_.

   Models are available if you access to [custom models in Firefly](https://adobedx.slack.com/archives/CMF1JGMLY/p1743534402774569). The _Models_ list will be blank if you do not have access. -->

1. Selezionare le proporzioni desiderate tra _[!UICONTROL Proporzioni]_.
1. Fai clic su **[!UICONTROL Seleziona dal contenuto]** in _[!UICONTROL Riferimento stile]_ per aggiungere un&#39;immagine di riferimento. L&#39;immagine selezionata influenza l&#39;estetica visiva e la profondità delle immagini generate.

   Per utilizzare le risorse di un repository [!DNL AEM Assets Content Hub] connesso, scegliere un repository dal menu a discesa _Posizione_. Filtra e seleziona un’immagine.

1. Nella scheda _Avanzate_, seleziona il _tipo di contenuto_.

   È preselezionato in base alla categoria di immagini presente per l&#39;[!DNL Brand]—_Arte_ o la _Foto_ selezionata e non è modificabile.

1. Regola l&#39;intensità complessiva delle caratteristiche visive esistenti dell&#39;immagine in _[!UICONTROL Intensità visiva]_.

### Immetti un prompt

Dopo aver selezionato i parametri, crea un prompt utilizzando il linguaggio naturale per iniziare a generare sulle immagini del brand.

Vedere [Scrivi prompt effettivi](/help/user-guide/effective-prompts.md).

**Per immettere una richiesta**:

1. Immettete un prompt nella casella prompt.
1. Fai clic su **[!UICONTROL Genera]**.

Per impostazione predefinita, quattro varianti (alimentate dal prompt, dai parametri e dal contenuto aggiunto) vengono generate e visualizzate nell’area di lavoro.

### Modifica in Adobe Express

Dopo aver generato le varianti di immagine, puoi modificarle direttamente in Adobe GenStudio for Performance Marketing utilizzando Adobe Express.

**Per modificare una singola immagine con Adobe Express**:

1. Passa il puntatore del mouse su una variante di immagine generata e fai clic su _[!UICONTROL Modifica in Adobe Express]_.

   Viene visualizzata una finestra _con tecnologia Adobe Express_.

1. Eseguire la modifica dell&#39;immagine, ad esempio [ritagliare un&#39;immagine](https://helpx.adobe.com/express/create-and-edit-images/edit-images/crop-images.html), [rimuovere un oggetto](https://helpx.adobe.com/express/create-and-edit-images/create-and-modify-with-generative-ai/remove-objects-generative-fill.html) e applicare effetti.

   Consulta la [documentazione di Adobe Express](https://helpx.adobe.com/express/user-guide.html) per scoprire come rivedere le immagini in GenStudio for Performance Marketing con Adobe Express.

1. Fai clic su _[!UICONTROL Applica modifiche]_ per salvare le modifiche.
1. Continua a modificare le singole varianti di immagine come desiderato e applica le modifiche per salvare l’avanzamento.

### Verifica l’allineamento della verifica del contenuto

Per ottimizzare le varianti generate e garantire una rigorosa aderenza all&#39;identità del brand, alle linee guida della piattaforma e agli standard di accessibilità, sfrutta la potenza del pannello [_Verifica contenuto_](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Questo pannello mostra i dettagli completi del controllo dei contenuti e illumina le aree del miglioramento.

**Per eseguire i controlli del contenuto**:

1. Fai clic sull&#39;icona del pannello _Verifica contenuto_ nella barra delle azioni a destra per aprire il pannello [_Verifica contenuto_](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Visualizza un riepilogo delle *verifiche necessarie* e *verifiche superate* per vedere quali sezioni e linee guida necessitano di miglioramenti.

   ![_Controllo contenuto_ pannello](/help/assets/content-check-img.png){width="500" zoomable="yes"}

1. Rivedi le varianti di immagine per garantire che siano strettamente allineate con i controlli del contenuto eseguiti.

Consulta [Convalida marchio](/help/user-guide/guidelines/brand-validation.md).

<!-- ## Generate Similar images

You can quickly generate images similar to a selected image within [!DNL Content] from the [!DNL Create] home.

**To create _[!DNL Similar images]_**:

1. In _[!DNL Create]_, click **[!UICONTROL Similar images]**.
1. Use the search option, adjacent to _Filter_, to find a specific image.

   To use assets from a connected [!DNL AEM Assets Content Hub] repository, choose a repository from the _Location_ drop-down menu. Filter and select one image.

1. In the _Select image_ view, click on an image.
1. Click **[!UICONTROL Use]**.

   The Canvas, which serves as the central hub for content creation, is displayed. Four image variations similar to the original selected image appear.

   ![Generate similar images](/help/assets/generate-similar.png){width="400" zoomable="yes"} -->

## Pubblicare ed esportare immagini

Le bozze di immagini generate vengono visualizzate nella sezione _Recenti_ della home [!DNL Create].

Per rendere le immagini generate disponibili per l&#39;uso corrente e futuro, pubblicarle in [!UICONTROL Contenuto] ed esportarle per utilizzarle nelle campagne di marketing.

1. **Per pubblicare le nuove immagini**, fai clic su **[!UICONTROL Pubblica]** nella barra degli strumenti superiore.
   1. _[!UICONTROL Aggiungi dettagli]_, ad esempio _[!UICONTROL Campagne]_ o _[!UICONTROL Canali]_, se necessario.
   1. Fai clic su **[!UICONTROL Pubblica]**.

1. **Per esportare le nuove immagini**, fai clic su **[!UICONTROL Esporta]** nella barra degli strumenti superiore.
   1. Seleziona il formato (JPG o PNG) e fai clic su **[!UICONTROL Esporta]**.

Vedere [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content).
