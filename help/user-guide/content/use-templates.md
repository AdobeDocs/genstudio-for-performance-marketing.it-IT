---
title: Utilizzare i modelli
description: Scopri come utilizzare i modelli in modo efficace per semplificare il processo creativo in Adobe GenStudio for Performance Marketing.
feature: Templates, Content
exl-id: 7705bb79-19ca-4c16-8f8b-95bf8687e96d
source-git-commit: 3a361134a0b56a2973399e38e62f4ab345a3dbc8
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 1%

---

# Utilizzare i modelli

GenStudio for Performance Marketing consente ai creatori di contenuti di produrre rapidamente contenuti di marketing coerenti nel brand utilizzando _modelli_. Un modello riduce in modo significativo il tempo e l’impegno necessari per generare nuovi contenuti, fornendo un punto di partenza che include layout preconfigurati ed elementi di progettazione.

## Elementi modello

Un modello è un insieme di istruzioni definite con HTML e CSS in linea che possono essere utilizzate per produrre un’esperienza di e-mail o metadati.

Di seguito è riportato un elenco di elementi utilizzati nei modelli e alcuni dettagli sulle relative caratteristiche.

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

## Configurare le linee guida per i canali

È consigliabile configurare [linee guida per i canali](../guidelines/brands.md#channel-guidelines) per ogni marchio prima di utilizzare i modelli in GenStudio for Performance Marketing. Le linee guida per il canale influenzano direttamente il tipo di contenuto generato quando si utilizza il modello. Ad esempio, puoi impostare i limiti dei caratteri per il corpo di un’e-mail.

![Specifiche del corpo](/help/assets/channel-email-body.png)

## Personalizza modello

[Personalizza il modello](customize-template.md) per l&#39;utilizzo in GenStudio for Performance Marketing inserendo segnaposto di contenuto o campi utilizzati dall&#39;IA generativa per inserire il contenuto. GenStudio for Performance Marketing riconosce alcuni campi, ad esempio il campo `body`, e rispetta le linee guida di canale configurate per il brand selezionato.

>[!TIP]
>
>Segui le [linee guida sull&#39;accessibilità per la creazione di modelli](accessibility-for-templates.md) in modo da poter raggiungere più tipi di pubblico e fornire un&#39;esperienza ottimale.

## Caricare un modello

Utilizza [Personalizza modelli](customize-template.md) come guida per la preparazione di un modello per GenStudio for Performance Marketing. Consulta le [linee guida per l&#39;accessibilità dei modelli](accessibility-for-templates.md) per informazioni su come fornire un&#39;esperienza migliore a tutti i tipi di pubblico.

**Per aggiungere un modello**:

1. In _[!DNL Content]_, selezionare la sezione **[!UICONTROL Modelli]**.

1. Fare clic su **[!UICONTROL Aggiungi modello]**.

1. Nel riquadro _[!UICONTROL Aggiungi il modello approvato]_, individua il file del modello di HTML o trascina il file del modello di HTML nello spazio di rilascio. Fai clic su **[!UICONTROL Avanti]**.

1. Nel riquadro _[!UICONTROL Rivedi campi individuati]_, controlla i campi rilevati. Verifica di utilizzare il modello corretto e che tutti i dettagli siano come previsto. Fai clic su **[!UICONTROL Avanti]**.

   Esempio di anteprima per un modello e-mail:

   ![Rilevati campi di anteprima](../../assets/template-detected-fields.png){width="650"}

   >[!TIP]
   >
   >Se il modello non è corretto, fare clic su **[!UICONTROL Indietro]** e tornare al passaggio precedente. Carica il file modello corretto.

1. Nel riquadro _[!UICONTROL Fornisci dettagli modello e carica]_, assegna un nome al modello e seleziona un tipo **[!UICONTROL Canale]**.

   Sono richiesti il nome del modello e il tipo di canale. Ulteriori requisiti possono includere:

   - **Meta**: richiede proporzioni
   <!-- - **Display ads**: requires Dimensions -->

1. Aggiungi tutti i dettagli possibili per migliorare l’identificazione dei modelli nelle ricerche e nei filtri.

1. Fai clic su **[!UICONTROL Fine]**.

## Creare con un modello

Trova e utilizza un modello esistente in GenStudio for Performance Marketing per creare più esperienze.

**Per creare un&#39;esperienza con un modello**:

1. In _[!DNL Content]_, selezionare la sezione **[!UICONTROL Modelli]**.

   ![Elenco modelli di contenuto](../../assets/content-templates.png){width="650" zoomable="yes"}

1. Selezionare un modello per una visualizzazione completa e un elenco di dettagli.

1. Fai clic su **[!UICONTROL Crea esperienza]** (pennello) nell&#39;angolo superiore destro per utilizzare il modello.

1. Continua a [Creare](/help/user-guide/create/overview.md) un&#39;esperienza.
