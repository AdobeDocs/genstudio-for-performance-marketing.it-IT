---
title: Utilizzare i modelli
description: Scopri come utilizzare i modelli in modo efficace per semplificare il processo creativo in Adobe GenStudio for Performance Marketing.
feature: Templates, Content
exl-id: 7705bb79-19ca-4c16-8f8b-95bf8687e96d
source-git-commit: e9c398cc81413fc22746d85abd6444c6bd42efe4
workflow-type: tm+mt
source-wordcount: '929'
ht-degree: 0%

---

# Utilizzare i modelli

GenStudio for Performance Marketing consente ai creatori di contenuti di produrre rapidamente contenuti di marketing coerenti nel brand utilizzando _modelli_. Un modello riduce in modo significativo il tempo e l’impegno necessari per generare nuovi contenuti, fornendo un punto di partenza che include layout preconfigurati ed elementi di progettazione.

Anche se GenStudio for Performance Marketing non supporta la creazione diretta di modelli all’interno dell’applicazione, è possibile progettare e preparare facilmente i modelli utilizzando i più diffusi strumenti di progettazione, come Adobe InDesign, Illustrator o Express. Una volta completato il progetto, puoi adattarlo per l’utilizzo in GenStudio for Performance Marketing. Per iniziare a utilizzare i modelli, segui questi passaggi:

1. **Progetta modello**: utilizza lo strumento di progettazione preferito per creare il layout visivo del modello [con elementi](#template-elements) quali preintestazione, titolo, corpo, CTA, immagini e piè di pagina.

2. **Codifica il modello**: converti il design in HTML e CSS in linea per assicurarti che sia pulito e reattivo tra i vari dispositivi. Considera le [linee guida per l&#39;accessibilità](accessibility-for-templates.md) per raggiungere il pubblico massimo previsto.

3. **Preparazione per GenStudio for Performance Marketing**: adattare il modello HTML utilizzando il linguaggio di modelli Handlebars. Inserisci segnaposto per indicare dove GenStudio for Performance Marketing deve generare il contenuto in modo dinamico. Scopri come [personalizzare un modello](customize-template.md) per GenStudio for Performance Marketing.

Seguendo questi passaggi, puoi creare modelli professionali ed efficaci pronti per l’uso in GenStudio for Performance Marketing, che consentono di produrre contenuti sul marchio in modo rapido ed efficiente.

## Elementi modello

Un modello è un insieme di istruzioni definite con HTML e CSS in linea che possono essere utilizzate per produrre un’esperienza di e-mail, annuncio social o annuncio di visualizzazione. Gli elementi modello forniscono la struttura per la creazione di contenuti.

Di seguito è riportato un elenco di elementi utilizzati nei modelli e alcuni dettagli sulle relative caratteristiche:

- **Preheader**

   - Funge da oggetto secondario in un messaggio e-mail, migliorando l’oggetto principale
   - Tra 40 e 50 caratteri
   - Visibile nella casella in entrata accanto all’oggetto prima dell’apertura dell’e-mail
   - Utilizzato nei modelli e-mail

- **Intestazione**

   - Sezione superiore dell’e-mail visualizzata dal destinatario all’apertura dell’e-mail
   - Imposta il tono e fornisce il contesto per il contenuto incluso
   - Utilizzato nei modelli e-mail

- **Titolo**

   - Primo contenuto visualizzato dal destinatario
   - Dovrebbe essere convincente per catturare interesse
   - Utilizzato nei metadati e modelli di annunci

- **Corpo**

   - Area del contenuto principale in cui viene trasmesso il messaggio principale
   - Capacità di includere testo, immagini e altri supporti
   - Utilizzato nei modelli di e-mail e metadati

- **CTA (invito all&#39;azione)**

   - Incoraggia il destinatario a intraprendere un’azione specifica, ad esempio fare clic su un collegamento o effettuare un acquisto
   - Utilizzato nei modelli di e-mail e metadati

- **Immagini**

   - Migliora l&#39;impatto visivo
   - Suddividere il testo
   - Supporta il messaggio
   - Deve essere di alta qualità e accattivante
   - Utilizzato nei modelli di e-mail e metadati

- **Piè di pagina**

   - Sezione inferiore che contiene contenuti aggiuntivi come dettagli di contatto, collegamenti ai social media, liberatorie e opzioni di annullamento dell’abbonamento
   - Utilizzato nei modelli e-mail

- **Sovrapposizione testo**

   - Testo su un&#39;immagine
   - Utilizza per supportare e migliorare il titolo e il corpo
   - Utilizzato nei metadati e modelli di annunci

>[!TIP]
>
>Visualizza i [nomi di campo riconosciuti](customize-template.md#recognized-field-names) supportati da GenStudio for Performance Marketing per i modelli di ogni tipo di canale.

## Personalizza modello

[Personalizza il modello](customize-template.md) per l&#39;utilizzo in GenStudio for Performance Marketing inserendo segnaposto di contenuto o campi utilizzati dall&#39;IA generativa per inserire il contenuto. GenStudio for Performance Marketing riconosce alcuni campi, ad esempio il campo `body`, e rispetta le linee guida di canale configurate per il brand selezionato.

>[!TIP]
>
>Segui le [linee guida per l&#39;accessibilità](accessibility-for-templates.md) e le [best practice](/help/user-guide/content/best-practices-for-templates.md) in modo da poter raggiungere più destinatari e fornire un&#39;esperienza ottimale.

## Gestire i modelli

Nella raccolta [!DNL Templates] viene visualizzato l&#39;inventario dei modelli personalizzati per la generazione di esperienze in GenStudio for Performance Marketing. Puoi filtrare i modelli in base al tipo di canale, ad esempio e-mail, annunci di visualizzazione e annunci Meta.

![Elenco modelli di contenuto](/help/assets/content-templates.png){width="650" zoomable="yes"}

### Aggiungi un modello

Prima di caricare un modello, assicurati che sia completamente preparato e pronto per essere utilizzato in GenStudio for Performance Marketing seguendo le indicazioni [Personalizza modelli](customize-template.md).

**Per aggiungere un modello**:

1. In _[!DNL Content]_, selezionare la sezione **[!UICONTROL Modelli]**.

1. Fare clic su **[!UICONTROL Aggiungi modello]**.

1. Nel riquadro _[!UICONTROL Aggiungi il modello approvato]_, individua il file del modello di HTML o trascina il file del modello di HTML nello spazio di rilascio. Fai clic su **[!UICONTROL Avanti]**.

1. Nel riquadro _[!UICONTROL Rivedi campi individuati]_, controlla i campi rilevati. Verifica di utilizzare il modello corretto e che tutti i dettagli siano come previsto. Fai clic su **[!UICONTROL Avanti]**.

   Esempio di anteprima per un modello e-mail:

   ![Rilevati campi di anteprima](/help/assets/template-detected-fields.png){width="650"}

   >[!TIP]
   >
   >Se il modello non è corretto, fare clic su **[!UICONTROL Indietro]** e tornare al passaggio precedente. Carica il file modello corretto.

1. Nel riquadro _[!UICONTROL Fornisci dettagli modello e carica]_, assegna un nome al modello e seleziona un tipo **[!UICONTROL Canale]**.

   Sono richiesti il nome del modello e il tipo di canale. Ulteriori requisiti possono includere:

   - **Meta**: richiede proporzioni
   - **Annunci visualizzati**: richiede Dimension

1. Aggiungi tutti i dettagli possibili per migliorare l’identificazione dei modelli nelle ricerche e nei filtri.

1. Fai clic su **[!UICONTROL Fine]**.

### Aggiorna modello

I modelli possono includere file statici, ad esempio icone o logo. Aggiorna consente di aggiornare l’anteprima del modello con le versioni più recenti di queste risorse.

**Per aggiornare il modello**:

1. In _[!DNL Content]_, selezionare la sezione **[!UICONTROL Modelli]**.

1. Fai clic su un modello per una visualizzazione completa e un elenco di dettagli.

1. Fai clic su **[!UICONTROL Aggiorna]** (frecce circolari) dall&#39;angolo superiore destro per aggiornare tutte le risorse utilizzate nel modello.

### Creare un’esperienza con un modello

Trova e utilizza un modello esistente in GenStudio for Performance Marketing per creare più esperienze.

**Per creare un&#39;esperienza con un modello**:

1. In _[!DNL Content]_, selezionare la sezione **[!UICONTROL Modelli]**.

1. Fai clic su un modello per una visualizzazione completa e un elenco di dettagli.

1. Fai clic su **[!UICONTROL Crea esperienza]** (pennello) nell&#39;angolo superiore destro per utilizzare il modello.

1. Continua a [Creare](/help/user-guide/create/overview.md) un&#39;esperienza.
