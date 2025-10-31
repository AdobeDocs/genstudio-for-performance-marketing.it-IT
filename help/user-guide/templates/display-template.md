---
title: Visualizzare le linee guida per il modello di annuncio
description: Segui le best practice per l’utilizzo di annunci display e modelli di banner con Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 076239b3-9444-48f9-bdd6-ef2b757bdf0d
source-git-commit: f4bc3442678e6366e185d0c7a91c784d43b8e455
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Visualizzare le linee guida per i modelli di annunci

I modelli di visualizzazione sono layout predefiniti utilizzati per creare banner e annunci di visualizzazione visivamente coinvolgenti. Offrono un framework flessibile per incorporare immagini, testo e call to action, garantendo coerenza ed efficienza nella produzione di più varianti di annunci. Quando prepari il modello per l’utilizzo in GenStudio for Performance Marketing, accertati che tutte le risorse siano ottimizzate per la visualizzazione web e soddisfino i formati e le dimensioni di file richiesti.

Segui queste best practice per la progettazione quando personalizzi i modelli di banner e annunci display per lavorare con GenStudio for Performance Marketing:

- Utilizzare i caratteri Adobe o Google
- Prepara le risorse che vengono visualizzate correttamente in dimensioni sottili
- È richiesto un solo campo immagine
- **non** utilizza immagini di sfondo incorporate o codificate
- Utilizza le immagini di sfondo (campo `image`) caricate nell&#39;archivio dei contenuti di GenStudio for Performance Marketing. Per ottenere risultati ottimali, attieniti alle linee guida in [Caricamento di immagini per annunci di visualizzazione](#uploading-images-for-display-ads)
- **non** utilizza JavaScript
- È possibile utilizzare una sola sezione, generando un singolo set di elementi modello

## Nomi di campi riconosciuti

Quando personalizzi il banner o il modello di annuncio visualizzato, utilizza segnaposto di contenuto per i seguenti campi obbligatori:

- `headline`
- `sub_headline`
- `body`
- `image` (obbligatorio, selezionato da Content JPEG, PNG o GIF)

GenStudio for Performance Marketing genera automaticamente i campi seguenti. Non è necessario applicare segnaposto di contenuto per:

- `cta`

Consulta [Segnaposto di contenuto](/help/user-guide/content/customize-template.md#content-placeholders) per ulteriori informazioni sull&#39;utilizzo dei nomi dei campi nei modelli.

## Dimensioni supportate

È necessario impostare la larghezza x l&#39;altezza (pixel).

| Orientamento | Dimensioni (pixel) | Note |
|--------------|-------------------------------------------------------------|------------------------------------------------------------------|
| Verticale | 300 x 600<br>160 x 600 | Comune per grattacieli e banner a mezza pagina. |
| Orizzontale | 300 x 250<br>728 x 90<br>336 x 280<br>320 x 50<br>970 x 250 | Classifica standard, rettangolo medio e dimensioni banner. |
| Personalizzato | Da 50 x 50 a 2000 x 2000 | Da utilizzare per posizionamenti non standard o univoci; controlla i limiti della piattaforma. |

## Caricamento di immagini per annunci display

Le immagini utilizzate negli annunci di visualizzazione devono provenire dall’archivio dei contenuti e devono essere caricate correttamente per garantire che vengano visualizzate con precisione nel modello.

Quando un modello di visualizzazione presenta un&#39;immagine da spigolo a spigolo (pagina al vivo completa), l&#39;immagine selezionata viene automaticamente ridimensionata per adattarsi alle dimensioni del modello complete. Tuttavia, se l’immagine non corrisponde alle proporzioni del modello, viene ritagliata per adattarla alle dimensioni del modello e potrebbe non essere visualizzata come previsto.

Non è disponibile la funzionalità di adattamento automatico per le immagini nei modelli di annunci di visualizzazione.

Per risolvere il ritaglio di immagini, gli utenti devono definire le proporzioni dell’immagine nel modello quando viene caricata nell’archivio dei contenuti. Durante il caricamento di un modello di annuncio visualizzato approvato:

1. [Procedi attraverso il processo di caricamento del modello](/help/user-guide/content/use-templates.md#add-a-template) fino a raggiungere la pagina **[!UICONTROL Aggiungi dettagli]**.

1. Definisci le proporzioni dell&#39;immagine da utilizzare nel modello in **[!UICONTROL Larghezza annuncio (px)]** e **[!UICONTROL Altezza annuncio (px)]**. In questo modo viene definita la finestra immagine per la sezione del modello che visualizza l&#39;immagine.

1. Nella sezione **[!UICONTROL Ulteriori dettagli]**, seleziona il menu a discesa **[!UICONTROL Dimensioni immagine]** e scegli _Ritaglia a dimensioni fisse_.
   ![Ritagliato a dimensioni fisse](./crop-to-fixed-size.png "Ritagliato a dimensioni fisse"){width="80%"}

Per determinare le dimensioni e le proporzioni di un&#39;immagine nel browser:

1. Ispezionare l&#39;immagine.
   - Windows/Linux:
      - Premere F12.
   - macOS:
      - Premere Command + Option + I.

1. Passa il puntatore sull&#39;immagine.

1. Osserva le proporzioni. Utilizzate questa opzione per definire le proporzioni dell&#39;immagine nel modello.

Se questi dettagli non vengono applicati durante il caricamento, si presume che l’immagine corrisponda all’intera proporzione del modello e che le immagini che non corrispondono esattamente a tale proporzione verranno ritagliate.

![Immagine ritagliata in un annuncio](./cropped-display.png "Ritaglio immagine"){width="60%"}

**❌immagine ritagliata in un modello di annuncio visualizzato**

![Immagine visualizzata in un annuncio pubblicitario](./full-fit.png "Immagine visualizzata in un annuncio pubblicitario"){width="60%"}

**✅immagine completamente visualizzata**
