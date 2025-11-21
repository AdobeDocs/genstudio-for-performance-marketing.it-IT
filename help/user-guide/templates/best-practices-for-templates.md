---
title: Best practice per i modelli
description: Segui le best practice per l’utilizzo dei modelli con Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates, Content Generation, Brand Personalization
exl-id: 3ff24fec-e836-4202-80f8-ba165e173b75
source-git-commit: 71b46454fa6fe2037ea6b103c0dfeedad74b8919
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 0%

---

# Best practice per l’utilizzo dei modelli

I modelli riducono in modo significativo il tempo e l’impegno necessari per generare nuovi contenuti, fornendo un punto di partenza che include layout preconfigurati ed elementi di progettazione.

Quando utilizzi i modelli con GenStudio for Performance Marketing, attieniti alle seguenti raccomandazioni:

1. Informazioni su [elementi modello](#know-about-template-elements)
1. Configura le [linee guida per i canali](#configure-channel-guidelines) per una personalizzazione efficace dei contenuti
1. Progettazione con [standard di accessibilità](accessibility-for-templates.md) per un&#39;esperienza ottimale
1. Segui [linee guida per modelli specifici per canale](#follow-channel-specific-template-guidelines)

>[!TIP]
>
>Scopri le nozioni di base sugli elementi e sulle procedure dei modelli in [Operazioni con i modelli](use-templates.md). Approfondisci [la personalizzazione di un modello](customize-template.md) per istruzioni specifiche da utilizzare nella prossima campagna.

## Utilizzare gli elementi di modello corretti

Ogni tipo di modello utilizza elementi diversi per creare una struttura per la creazione di contenuti specifici per il canale. [Acquisisci familiarità con le parti di un modello](use-templates.md#template-elements) e includi gli elementi migliori per il contenuto e il tipo di modello.

Quando personalizzi il modello, utilizza i nomi dei campi al posto di questi elementi dove è necessario GenStudio for Performance Marketing per generare il contenuto.

Vedi [Elementi modello](use-templates.md#template-elements).

## Utilizzo del testo segnaposto nei modelli

Il testo segnaposto può essere utile per definire la sintassi o la struttura del contenuto da compilare successivamente in un modello da parte di un utente. Ad esempio, {first_name}.{last_name}@email.etc. per definire un indirizzo e-mail. Tuttavia, alcuni delimitatori comuni sono già riservati ad altri significati in GenStudio for Performance Marketing:

❌ &lt; > - In uso per i tag HTML.
❌ {{ }}{{ }} - In uso per le espressioni Handlebar.

Utilizzare parentesi uniche (rette o ricce) per indicare il testo segnaposto per evitare confusione con i tag esistenti.

✅ {first_name} - Segnaposto per nome.

## Configurare le linee guida per i canali

Definire linee guida chiare per il canale è essenziale per garantire che i contenuti generati siano in linea con i requisiti e gli obiettivi del tuo marchio. Le linee guida per il canale consentono di specificare regole per elementi quali il tono, la lunghezza e lo stile utilizzati nel modello. Ad esempio, puoi impostare un numero massimo di caratteri per il corpo o richiedere uno stile call-to-action specifico. Impostando queste linee guida in anticipo, riduci la necessità di scrivere istruzioni dettagliate in ogni prompt di IA, semplificando il processo di generazione dei contenuti e garantendo coerenza nelle e-mail.

Rivedi e definisci le [linee guida per il canale](/help/user-guide/guidelines/brands.md#channel-guidelines) del tuo marchio per tutti i campi chiave nel modello. Se non definisci le linee guida, vengono applicate le [linee guida predefinite per il canale](/help/user-guide/guidelines/brands.md#default-channel-guidelines), che potrebbero non riflettere completamente i requisiti del brand.

![Specifiche del corpo](/help/assets/channel-email-body.png)

Scopri in che modo [Marchi, Prodotti e Linee guida per Personas](/help/user-guide/guidelines/overview.md) influenzano i contenuti generati e come adattarli agli obiettivi di marketing.

## Caricamento immagini per modelli

Le immagini utilizzate nei modelli devono provenire dall’archivio dei contenuti e devono essere caricate correttamente per garantire una visualizzazione accurata.

Quando un modello presenta un&#39;immagine da spigolo a spigolo (full bleed), l&#39;immagine selezionata viene automaticamente ridimensionata per adattarsi alle dimensioni complete del modello. Tuttavia, se l’immagine non corrisponde alle proporzioni del modello, viene ritagliata per adattarla alle dimensioni del modello e potrebbe non essere visualizzata come previsto.

Non è disponibile la funzionalità di adattamento automatico per le immagini incluse nei modelli.

Per risolvere il ritaglio di immagini, gli utenti devono definire le proporzioni dell’immagine da utilizzare nel modello quando viene caricata nell’archivio dei contenuti. Durante il caricamento di un modello approvato:

1. [Procedi attraverso il processo di caricamento del modello](/help/user-guide/templates/use-templates.md#add-a-template) fino a raggiungere la pagina **[!UICONTROL Aggiungi dettagli]**.

2. Definisci le proporzioni dell&#39;immagine da utilizzare nel modello in **[!UICONTROL Larghezza annuncio (px)]** e **[!UICONTROL Altezza annuncio (px)]**. In questo modo viene definita la finestra immagine per la sezione del modello che visualizza l&#39;immagine.

3. Nella sezione **[!UICONTROL Ulteriori dettagli]**, seleziona il menu a discesa **[!UICONTROL Dimensioni immagine]** e scegli _Ritaglia a dimensioni fisse_.
   ![Ritagliato a dimensioni fisse](images/crop-to-fixed-size.png "Ritagliato a dimensioni fisse"){width="80%"}

Per determinare le dimensioni e le proporzioni di un&#39;immagine nel browser:

1. Ispezionare l&#39;immagine.
   - Su Windows/Linux:
      - Premere F12.
   - Su macOS:
      - Premere Command + Option + I.

1. Passa il puntatore sull&#39;immagine.

1. Osserva le proporzioni. Utilizzate questa opzione per definire le proporzioni dell&#39;immagine nel modello.

Se questi dettagli non vengono applicati durante il caricamento, si presume che l’immagine corrisponda all’intera proporzione del modello e che le immagini che non corrispondono esattamente a tale proporzione verranno ritagliate.

![Immagine ritagliata in un annuncio](images/cropped-display.png "Ritaglio immagine"){width="60%"}

**❌immagine ritagliata in un modello di annuncio visualizzato**

![Immagine visualizzata in un annuncio pubblicitario](images/full-fit.png "Immagine visualizzata in un annuncio pubblicitario"){width="60%"}

**✅immagine completamente visualizzata**

## Segui le linee guida dei modelli specifiche per il canale

Quando crei i modelli, accertati che soddisfino i requisiti specifici del canale previsto. Crea modelli che soddisfino i requisiti di layout e di visualizzazione per ogni canale. Esistono linee guida generali applicabili a qualsiasi modello, ad esempio:

- Utilizzare HTML e CSS in linea puliti e reattivi
- Utilizzare i caratteri Adobe o Google
- **non** utilizza JavaScript

{{note-css-effects}}

Per prestazioni ottimali, consulta ulteriori suggerimenti e vincoli durante l’utilizzo di ciascun tipo di modello:

- [E-mail](/help/user-guide/templates/email-template.md)
- [Visualizzazione e banner pubblicitari](/help/user-guide/templates/display-template.md)
- [LinkedIn](/help/user-guide/templates/linkedin-template.md)
- [Meta ads](/help/user-guide/templates/meta-template.md)
