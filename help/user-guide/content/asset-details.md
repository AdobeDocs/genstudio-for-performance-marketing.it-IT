---
title: Dettagli risorsa
description: Adobe GenStudio for Performance Marketing archivia i contenuti approvati con metadati avanzati per ricercare e monitorare le prestazioni.
feature: Generative AI, Content Attributes, Content Management
exl-id: 2be5cfee-f315-4ad6-8cf0-a8d3929b9ba3
source-git-commit: c0f45fb0ffc61d20611693498f1b12d3946ca6ca
workflow-type: tm+mt
source-wordcount: '726'
ht-degree: 1%

---

# Dettagli risorsa

Adobe GenStudio for Performance Marketing archivia i contenuti approvati con metadati avanzati per il discovery e il tracciamento delle prestazioni.

A ogni risorsa (inclusi esperienze e modelli) sono associati _dettagli_ (metadati) che consentono di identificare, tenere traccia, utilizzare e apprendere dalle prestazioni dei contenuti.

**Per visualizzare i dettagli della risorsa**:

1. In _[!DNL Content]_, seleziona una risorsa, un&#39;esperienza o un modello. Facendo clic su una risorsa si apre una sua visualizzazione mirata.

1. Nella visualizzazione delle risorse, controlla la sezione _[!UICONTROL Dettagli]_ a destra.

1. Se la sezione _[!UICONTROL Dettagli]_ non è visibile, fare clic sull&#39;icona **[!UICONTROL Informazioni]** (i).

I dettagli della risorsa includono i metadati applicati durante il processo di creazione o caricamento. I tipi di metadati delle risorse includono [metadati di sistema](#system-metadata) e [metadati definiti dall&#39;utente](#user-defined-metadata).

La seguente risorsa immagine contiene metadati di sistema che descrivono il tipo di file, le dimensioni e altre caratteristiche, una parola chiave definita dall’utente e diversi attributi e colori rilevati dall’intelligenza artificiale.

![dettagli di una risorsa con più tag](/help/assets/content-asset-details.png)

>[!NOTE]
>
>Gli archivi di Assets di AEM presentano metadati diversi. Consulta [Configurare la visibilità delle risorse](connect-aem-repo.md#step-4-configure-asset-visibility) per scoprire come configurare i dettagli di [!DNL AEM Assets Content Hub] risorse.

## Metadati di sistema

Alcuni metadati di risorse vengono raccolti automaticamente quando una risorsa viene caricata, ad esempio tipo di file, dimensioni, dimensioni, origine e altro ancora. Ad eccezione del nome del file, non è possibile modificare i metadati di sistema predefiniti.

### Tag generati

Quando memorizzi una risorsa approvata in [!DNL Content], GenStudio for Performance Marketing utilizza le funzionalità di intelligenza artificiale e machine learning di Adobe per studiare la risorsa e applicare i tag in base alle funzioni della risorsa. Ad esempio, un&#39;immagine di un gatto può causare tag attributo come `pet photography` o `cat` e tag colore che identificano i colori dominanti nell&#39;immagine. Non è possibile modificare i tag rilevati e applicati automaticamente.

Consulta [!DNL Insights] [Categorie di attributi](/help/user-guide/insights/attributes.md#categories) per un elenco dettagliato delle funzioni immagine, video e testo.

### Metadati del contenuto generato

Le informazioni utilizzate per generare una nuova risorsa o esperienza diventano metadati, ad esempio il prompt utilizzato. Non è possibile modificare la richiesta dopo l’approvazione del contenuto, ma è possibile utilizzarla come punto di partenza per la generazione di qualcosa di nuovo.

## Metadati definiti dall&#39;utente

I metadati definiti dall’utente aggiungono un contesto di marketing al contenuto della risorsa, consentendo agli addetti al marketing di comprendere come utilizzarla e interagire con essa.

Quando [carichi una risorsa](/help/user-guide/content/manage-assets.md#add-assets), puoi definire un set di dettagli facoltativi della risorsa presenti in GenStudio for Performance Marketing come metadati. L’inclusione di ulteriori dettagli può migliorare l’identificazione delle risorse nelle ricerche e nei filtri.

**Per modificare i metadati definiti dall&#39;utente**:

1. In _[!DNL Content]_, seleziona una risorsa, un&#39;esperienza o un modello. Facendo clic su una risorsa si apre una sua visualizzazione mirata.

1. Nella visualizzazione delle risorse, controlla la sezione _[!UICONTROL Dettagli]_ a destra.

1. Fai clic su **[!UICONTROL Modifica dettagli]** (matita) per modificare i metadati della risorsa, dell&#39;esperienza o del modello.

   Maggiore è il numero di dettagli forniti, maggiori saranno le funzionalità di GenStudio for Performance Marketing. Selezionare uno o più dettagli dall&#39;elenco o immetterne uno nuovo, se applicabile, ad esempio con parole chiave. Ogni dettaglio aggiunto viene visualizzato sotto l&#39;elenco. Fare clic su **`x`** per rimuovere un dettaglio.

### Dettagli metadati

La tabella seguente descrive i metadati (dettagli risorsa) che puoi definire durante la creazione di una risorsa.

| Campo | Descrizione |
| -------------- | ----------- |
| Titolo | Nome della risorsa; il titolo predefinito può essere il nome del file originale |
| [!DNL Campaigns] | [[!DNL Campaigns]](/help/user-guide/campaigns/overview.md) include contenuti promozionali con messaggi coerenti allo scopo di raggiungere un obiettivo di business<br>Facendo clic su un collegamento a una campagna si accede alla pagina della panoramica della campagna |
| [!DNL Brands] | [[!DNL Brands]](/help/user-guide/guidelines/brands.md) aggiunto a GenStudio for Performance Marketing e pubblicato per l&#39;utilizzo |
| [!DNL Products] | [[!DNL Products]](/help/user-guide/guidelines/products.md) aggiunti a GenStudio for Performance Marketing per l&#39;utilizzo |
| [!DNL Personas] | [[!DNL Personas]](/help/user-guide/guidelines/personas.md) aggiunti a GenStudio for Performance Marketing per l&#39;utilizzo |
| Canali | Piattaforme per la distribuzione di determinati tipi di contenuto, ad esempio e-mail, banner e annunci di visualizzazione |
| [!UICONTROL Intervallo temporale] | Intervallo di tempo per il quale viene utilizzata la risorsa, ad esempio trimestre, stagione, anno e così via. Esempio: `Winter 2023` |
| Regione | Aree per le quali viene utilizzata la risorsa. Esempi: `North America`, `APAC`, `Italy` |
| Lingua | Lingue per cui viene utilizzata la risorsa. Esempio: `Spanish` |
| Parole chiave | Le parole chiave definite dall&#39;utente vengono utilizzate per identificare ulteriormente le caratteristiche e lo scopo delle risorse |

>[!TIP]
>
>Fai clic su **[!UICONTROL Modifica dettagli]** (matita) per modificare i metadati della risorsa. Ad esempio, puoi modificare il nome della risorsa o aggiungere o rimuovere parole chiave.

## Contesto generativo

La sezione [!UICONTROL Contesto generativo] mostra le informazioni utilizzate per generare l&#39;esperienza, ad esempio `Prompt` utilizzate durante il processo [!DNL Create]. Questo insight può aiutarti a creare varianti ancora più di successo.

Le informazioni possono comprendere:

- Parametri `Brand`, `Product` e `Persona` selezionati durante il processo [!DNL Create]
- `Subject line` e `Preheader` per le esperienze e-mail
- `Headline` e `Body` per annunci Meta

## Cronologia

Espandi la sezione _[!UICONTROL Cronologia]_ in un&#39;esperienza per visualizzare una timeline di approvazioni e attività. Ad esempio, un’esperienza approvata rivela la data, l’ora e il responsabile approvazione:

```
Approved

December 10, 2024 at 6:00 PM by Username
```
