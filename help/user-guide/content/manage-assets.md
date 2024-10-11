---
title: Gestire risorse ed esperienze
description: Semplifica e migliora la gestione delle risorse approvate dal marchio da utilizzare e riutilizzare nel percorso di marketing digitale.
feature: Content, Assets, Experiences
exl-id: e2ce8797-6d3b-46d4-b12f-f5f80e26c669
source-git-commit: 600d4a37be22bd057074b4dd3773b75f0273a567
workflow-type: tm+mt
source-wordcount: '786'
ht-degree: 0%

---

# Gestire risorse ed esperienze

Adobe GenStudio for Performance Marketing [!DNL Content] semplifica e migliora la gestione delle risorse approvate dal marchio da utilizzare e riutilizzare nel percorso di marketing digitale.

## Galleria Assets

La raccolta [!UICONTROL Assets] mostra un inventario delle risorse approvate. L&#39;icona del filtro (funnel) sopra il lato sinistro della tabella apre il menu **[!UICONTROL Filtro]** in cui è possibile selezionare diverse categorie per filtrare le risorse visualizzate nella raccolta. Fai clic sull’icona di ricerca (lente di ingrandimento) per trovare una risorsa con una parola chiave.

Di seguito è riportata una ricerca per il termine `dog` nella raccolta [!UICONTROL Assets]:

![Visualizzazione Assets con ricerca su cane](../../assets/content-assets.png)

### Posizione Assets

Per impostazione predefinita, le risorse aggiunte a [!DNL Content] tramite il processo [!DNL Create] o il caricamento vengono archiviate nell&#39;archivio `GenStudio assets`. L&#39;archivio `GenStudio assets` è di lettura/scrittura in GenStudio for Performance Marketing. Ciò significa che è possibile salvare, modificare ed eliminare le risorse nell&#39;archivio `GenStudio assets`.

L&#39;elenco **[!UICONTROL Posizione]** sopra la raccolta sul lato destro consente di selezionare dagli archivi Adobe Experience Manager (AEM) [!DNL Assets Content Hub] connessi. Quando selezioni un archivio AEM, la galleria mostra un inventario delle risorse provenienti da tale archivio, che ti consente di sfruttare le risorse approvate provenienti da tali archivi come input per la creazione di contenuti. Le opzioni del filtro cambiano per riflettere le categorie configurate in [!DNL AEM Assets Content Hub].

Per istruzioni sull&#39;aggiunta dell&#39;archivio [!DNL AEM Assets Content Hub] a GenStudio for Performance Marketing, vedere [Connettere un archivio AEM](connect-aem-repo.md).

L’archivio AEM è di sola lettura, il che significa che non è possibile salvare bozze, nuove risorse o metadati nell’archivio AEM. Tutte le bozze e gli aggiornamenti finali per risorse, esperienze e modelli vengono salvati nell&#39;archivio `GenStudio assets` con i nuovi [metadati di sistema](asset-details.md#system-metadata).

{{note-aem-assets}}

## Gestione di Assets

In [!UICONTROL Content], Performance Marketing può archiviare, recuperare e gestire facilmente le risorse digitali. Sfruttando sia l&#39;archivio `GenStudio assets` che gli archivi AEM, gli utenti possono garantire che le proprie risorse siano ben organizzate e accessibili per varie campagne di marketing. Questo approccio con più repository offre flessibilità e controllo sull’utilizzo delle risorse in ambienti diversi, garantendo che solo le risorse approvate e aggiornate vengano utilizzate nelle attività di marketing.

### Aggiungere risorse

Per impostazione predefinita, quando si aggiungono risorse a [!DNL Content], queste vengono memorizzate nell&#39;archivio `GenStudio assets`. Il pulsante _[!UICONTROL Aggiungi risorse]_ è disponibile solo quando _[!UICONTROL Posizione]_ è l&#39;archivio `GenStudio assets`.

![Campo posizione](../../assets/content-location.png){width="350" align="center"}

**Per aggiungere una o più risorse**:

1. In _[!DNL Content]_, fai clic su **[!UICONTROL Aggiungi risorse]**.

1. Nella visualizzazione _Aggiungi le risorse approvate_, rilascia uno o più file nello spazio di rilascio. In alternativa, è possibile selezionare i file locali utilizzando **[!UICONTROL Sfoglia]** o importare i file da Dropbox o Microsoft OneDrive.

1. Nella sezione _Aggiungi dettagli_, seleziona un **[!UICONTROL nome campagna]** o immetti un nuovo nome.

1. Per migliorare la reperibilità, aggiungi dettagli facoltativi come _Brand name_, _Personas_, _Region_ e _Keywords_ nella sezione **More details**.

   Maggiore è il numero di dettagli forniti, maggiori saranno le funzionalità di GenStudio for Performance Marketing. Selezionare uno o più dettagli dall&#39;elenco o immetterne uno nuovo, se applicabile, ad esempio con parole chiave. Ogni dettaglio aggiunto viene visualizzato sotto l&#39;elenco. Fare clic su **`x`** per rimuovere un dettaglio.

   Tutti i dettagli aggiunti vengono applicati a tutte le risorse aggiunte in questa azione.

   Vedi [Dettagli metadati](/help/user-guide/content/asset-details.md#system-metadata).

1. Fai clic su **[!UICONTROL Aggiungi risorse]**.

1. Al termine del caricamento della risorsa, fai clic su **Fine**.

1. Per visualizzare le nuove risorse caricate, fai clic su **[!UICONTROL Aggiorna]** dalla notifica _Nuove risorse disponibili_ nella parte inferiore dell&#39;area di lavoro.

<!--
In the future, need guidance on template upload errors. For now, the UI just says error.
-->

### Cerca contenuto

Il filtro e l’interfaccia di ricerca sono rapidi e reattivi e forniscono un’esperienza di ricerca iniziale produttiva. Ogni visualizzazione [!DNL Content] fornisce opzioni filtro per limitare la ricerca della risorsa, dell&#39;esperienza o del modello ideale. Per risorse ed esperienze, puoi selezionare una campagna e linee guida specifiche, ad esempio contenuti creati per un prodotto specifico.

Sono presenti filtri basati su [parole chiave](asset-details.md#user-defined-metadata) e [attributi](/help/user-guide/insights/attributes.md) per limitare i risultati della ricerca. Ad esempio, potresti voler trovare una risorsa di un particolare tipo di file o oggetto per aiutarti a creare una nuova esperienza per la campagna.

Durante la ricerca di _Esperienze_, puoi utilizzare il filtro **[!UICONTROL Creato da]** per limitare l&#39;elenco in modo da mostrare solo le esperienze create da te o da una persona specifica.

**Per cercare contenuto da riutilizzare**:

1. In _[!DNL Content]_, selezionare la sezione **[!UICONTROL Assets]**.

1. Selezionare un repository di risorse dall&#39;elenco **[!UICONTROL Posizione]** oppure verificare che si stia cercando il repository di risorse corretto. `GenStudio assets` è l&#39;archivio predefinito.

   >[!IMPORTANT]
   >
   >L&#39;elenco _Posizione_ è disponibile solo quando si esegue la [connessione a un repository AEM](connect-aem-repo.md).

1. Fare clic su **[!UICONTROL Cerca]** (lente di ingrandimento) per immettere una parola chiave o una descrizione.

1. Restringi la ricerca selezionando una categoria dall&#39;elenco _[!UICONTROL Filtro]_. Ad esempio, se stai cercando un file PNG, fai clic su **[!UICONTROL Formato file]** e scegli **PNG**.

   Più si restringe la ricerca, meno opzioni di filtro disponibili. Fare clic su **[!UICONTROL Cancella tutto]** per rimuovere tutti i filtri.

1. Seleziona una risorsa per una visualizzazione completa e un elenco di dettagli.

   Fai clic su **[!UICONTROL Scarica]** (freccia giù) per utilizzare la risorsa nella workstation locale.
