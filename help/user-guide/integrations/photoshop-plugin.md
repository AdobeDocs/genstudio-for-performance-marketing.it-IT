---
title: Plug-in Photoshop per Adobe GenStudio for Performance Marketing
description: Scopri come installare, configurare e utilizzare il plug-in Photoshop per GenStudio for Performance Marketing.
feature: Generative AI
role: User
source-git-commit: bb6b8de80bdf6089e70756bea5dbf3e6a7945052
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 1%

---

# Plug-in Photoshop per GenStudio for Performance Marketing

Il plug-in Photoshop di GenStudio for Performance Marketing aggiunge un pannello ad Adobe Photoshop che consente di generare contenuti per il brand.

Questa pagina descrive come installare e configurare il plug-in e come utilizzarlo.

Le funzioni di questo plug-in includono:

* Accedi a un’istanza di GenStudio for Performance Marketing con un Adobe ID
* Mappatura dei campi di generazione dei contenuti di GenStudio for Performance Marketing ai livelli di testo di un documento Photoshop
* Specifica un marchio, un prodotto, un utente tipo e un prompt di testo per la generazione del contenuto
* Se necessario, aggiungi un’immagine in sostituzione dell’immagine modello
* Anteprima delle varianti di contenuto on-brand generate
* Applica il contenuto generato ai livelli mappati nel documento corrente
* Creare traduzioni di contenuti sul marchio
* Esporta [!DNL Experiences] generato in GenStudio for Performance Marketing

>[!VIDEO](https://video.tv.adobe.com/v/3478808?learn=on)

## Installare il plug-in

Seguire queste istruzioni per installare il plug-in.

### Prerequisiti

* applicazione desktop Creative Cloud
* Photoshop, versione minima 25.6.0

### Passaggi per l’installazione

1. Scarica e aggiorna il plug-in da Creative Cloud Marketplace in Adobe Exchange.
1. Cerca il **plug-in GenStudio per Photoshop** in Adobe Exchange.
1. Seguire le istruzioni per installare il plug-in.

### Disinstallare il plug-in

1. Avviare l&#39;applicazione desktop Creative Cloud.
1. Fare clic sull&#39;opzione **[!UICONTROL Plugin]**.
1. Per visualizzare le opzioni, fai clic sui puntini di sospensione **[!UICONTROL (...)]** nella scheda GenStudio for Creative Cloud.
1. Scegliere **Disinstalla**.

## Creare un modello

Per generare il contenuto è necessario un modello GenStudio for Performance Marketing creato dal documento Photoshop.

Per creare un modello compatibile con GenStudio:

1. Aprire un documento in Photoshop.
1. Identifica un livello di testo per il contenuto generato.
1. Rinominare il livello con il formato di convenzione del nome campo: `{<name_of_generated_field>}`. Ad esempio, `{body}`, `{headline}` e `{cta}`.
1. Rinominare i livelli per tutti i [&#x200B; campi richiesti dal canale previsto per il tipo di modello](../../user-guide/templates/customize-template.md#recognized-field-names).

| Canale | Campi obbligatori per la generazione | Campi facoltativi per la generazione |
| --- | --- | --- |
| LinkedIn | `{on_image_text}`, `{image}` | `{headline}`, `{introductory_text}`, `{cta}`, `{website_url}` |
| Meta | `{on_image_text}`, `{image}` | `{body}`, `{headline}`, `{cta}`, `{website_url}`, `{display_link}` |
| Visualizzazione | `{body}`, `{image}` | `{headline}`, `{cta}`, `{website_url}` |

Si noti che più livelli possono condividere la stessa designazione di campo, ma ogni livello può specificare un solo campo. Ad esempio, se nel documento sono presenti più tavole da disegno:

* È possibile specificare un livello `{headline}` in ogni tavola da disegno.
* È possibile specificare più livelli `{headline}` in una singola tavola da disegno.
* Impossibile specificare che un singolo livello riceva sia i nomi di campo `{headline}` che quelli di campo `{cta}`.

### Requisiti per la dimensione del modello

#### Modelli Meta

Per i post su Instagram e Facebook:

* Larghezza: 1080 px (fissa)
* Altezza: 1080 px o 1350 px

Per le storie su Instagram e Facebook:

* Larghezza: 1080 px (fissa)
* Altezza: 1920 px

Il plug-in determina il cromo dell’esperienza generata in base all’altezza del modello.

#### Visualizza modelli

Non esiste alcun requisito di dimensione fissa. I modelli di visualizzazione supportano qualsiasi dimensione.

#### Modelli LinkedIn

* Larghezza: 1200 px (fissa)
* Altezza: 1200 px, 628 px, 2292 px, 1800 px o 1500 px

Il documento è ora pronto per essere utilizzato con il plug-in.

## Genera nuovo contenuto

1. Apri Photoshop.
1. Aprire un documento di modello predisposto per GenStudio creato (vedere le istruzioni precedenti) oppure utilizzare il modello iniziale di GenStudio for Performance Marketing: `branding-template-acrobat-handlebars.psd`.
1. Apri il pannello dei plug-in in **[!UICONTROL Plugin]** > **[!UICONTROL GenStudio]**.
1. Fai clic sul pulsante **[!UICONTROL Accesso]**. Se viene richiesta l&#39;autorizzazione per aprire un URL, selezionare **Ricorda la scelta**, quindi fare clic su **[!UICONTROL Consenti]**.
1. Utilizza il browser web per accedere con un profilo che abbia accesso a GenStudio for Performance Marketing.
1. Seleziona il canale (Meta, LinkedIn o Display) applicabile al modello aperto.
   ![Selezione canale](./ps-select-channel.png){width="300" zoomable="yes"}
1. Selezionare il contesto [!DNL Brand], [!DNL Persona] e [!DNL Product] per la generazione del contenuto.
   ![Selezione marchio, persona e prodotto](./ps-select-box.png){width="300" zoomable="yes"}
1. Seleziona il numero di varianti da produrre.
1. Utilizza il pulsante in **[!UICONTROL Seleziona contenuto]** per sfogliare e scegliere le immagini dalle risorse. Le 40 risorse aggiunte più di recente vengono visualizzate per prime e puoi cercare altre risorse. Le immagini selezionate vengono automaticamente ridimensionate in base ai modelli.
1. Fornisci un prompt di testo per il contenuto nella casella **[!UICONTROL Prompt di testo]**.
1. Fare clic sul pulsante **[!UICONTROL Genera]**. Le varianti vengono visualizzate sulle schede nel pannello plugin.

I nuovi documenti vengono aggiunti all’area di lavoro Photoshop con il contenuto generato applicato ai campi del modello. Questi documenti sono denominati con un suffisso di variante numerato.

## Tradurre il contenuto

Dopo la generazione della copia, gli utenti possono tradurre i contenuti nelle lingue supportate.

1. Fai clic su **[!UICONTROL Traduci]** dopo aver generato la copia annuncio con il plug-in.
1. Seleziona una o più lingue per la traduzione.
1. Fare clic sul pulsante **[!UICONTROL Traduci]**.

I nuovi documenti vengono aggiunti all’area di lavoro Photoshop con il contenuto generato applicato ai campi del modello. Questi documenti sono denominati con un suffisso di variante numerato.

## Esportare esperienze in GenStudio

Gli utenti possono selezionare l’esportazione dopo la generazione o la traduzione del contenuto. Le esperienze esportate vengono compilate nella sezione dei contenuti di GenStudio for Performance Marketing.

![Risorse esportate visualizzate nella sezione Contenuto](./content-assets.png){width="90%"}

## Risoluzione dei problemi

Prendi in considerazione queste best practice e suggerimenti se testo o immagini non vengono sostituiti nelle varianti generate.

### Campi mappati

Se il testo o le immagini non vengono sostituiti, i campi di conferma vengono mappati correttamente con parentesi graffe `{}` (non parentesi `()`).

### Conferma che i font siano disponibili

Affinché la sostituzione venga eseguita durante la generazione, è necessario che nel computer sia disponibile un tipo di carattere per il campo di testo. Verificare che tutti i tipi di carattere utilizzati nel file siano disponibili nel computer, soprattutto se il file è stato creato nel computer di un altro utente.

### Eccezioni di mappatura campi

{{$include /help/_includes/field-mapping-exceptions.md}}
