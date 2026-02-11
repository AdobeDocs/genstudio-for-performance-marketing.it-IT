---
title: Plug-in Figma per Adobe GenStudio for Performance Marketing
description: Scopri come configurare e utilizzare il plug-in Figma per GenStudio for Performance Marketing.
feature: Generative AI
role: User
exl-id: 232fbbc6-c523-4525-8d26-a8ac8d62c035
source-git-commit: e585c6ff70198fe572b21252ab00b9b1ad368d02
workflow-type: tm+mt
source-wordcount: '1181'
ht-degree: 0%

---

# Plug-in Figma per GenStudio for Performance Marketing

Il plug-in GenStudio for Performance Marketing Figma aggiunge un nuovo pannello all’applicazione Figma che consente di generare contenuti on-brand.

Questa pagina descrive come configurare e utilizzare il plug-in.

Le funzioni di questo plug-in includono:

* Mappare gli elementi di testo Figma ai campi di GenStudio for Performance Marketing, ad esempio `headline`, `body`, `on_image_text` e altro ancora.
* Genera un nuovo Meta, LinkedIn o Annuncio di visualizzazione [!DNL Experiences] per marchio, persona, prodotto e prompt di testo.
* Creare [!DNL Experiences] direttamente nel documento Figma sostituendo il testo negli elementi Figma mappati con i valori generati da GenStudio for Performance Marketing.
* Riformula, accorcia, allunga o traduci il contenuto esistente in base a un prompt.
* Traduci [!DNL Experiences] generato in più lingue.
* Esporta [!DNL Experiences] generato in un&#39;origine locale come immagini appiattite.
* Esporta [!DNL Experiences] generato in GenStudio for Performance Marketing.
* Utilizza le opzioni del plug-in che si adattano agli elementi selezionati nell’area di lavoro di Figma.

>[!VIDEO](https://video.tv.adobe.com/v/3478809?learn=on)

## Creare un modello

Il plug-in richiede i primi due livelli del documento Figma per seguire questa convenzione:

* **Sezione** - Rappresenta il progetto padre, che può contenere più modelli.
* **Frame** - Rappresenta un modello in un progetto. Il modello può essere riempito con testo, immagini, componenti e altri elementi.

### Modelli Meta

Sono supportate le seguenti dimensioni di modello:

Per i post su Instagram o Facebook:

* Larghezza: 1080 px (fissa)
* Altezza: 1080 px o 1350 px

Per le storie su Instagram o Facebook:

* Larghezza: 1080 px (fissa)
* Altezza: 1920 px

Il plug-in determina il cromo dell’esperienza generata in base all’altezza del modello.

### Visualizza modelli

Non esiste alcun requisito di dimensione fissa. I modelli di visualizzazione supportano qualsiasi dimensione.

### Modelli LinkedIn

* Larghezza: 1200 px (fissa)
* Altezza: 1200 px, 628 px, 2292 px, 1800 px o 1500 px

### Mappatura ruolo campo

Il plug-in deve comprendere i diversi elementi del modello, come titolo, testo del corpo o immagine.

Per assegnare ruoli elemento:

1. Seleziona un elemento nel modello (testo, immagine e così via).
1. Utilizza il menu a discesa per assegnare un ruolo.

Il plug-in ricorda queste mappature da utilizzare per il contenuto generato. Un ruolo di campo\ può essere mappato a più elementi del modello.

![Mappatura ruolo campo](./field-role-mapping.png){width="600"}

### Eccezioni di mappatura campi

{{$include /help/_includes/field-mapping-exceptions.md}}

## Genera nuovo contenuto

Utilizza GenStudio for Performance Marketing AI per generare o apportare varianti agli elementi nei modelli Figma.

1. Se utilizzi GenStudio Plugin Playground o i modelli già preparati, seleziona il nodo di sezione che contiene i modelli di annuncio. Puoi eseguire questa operazione dal pannello **Livelli** o facendo clic direttamente sulla sezione nell&#39;area di lavoro.
   ![Selezione sezione o varianti](./plugin-playground.png){width="500" zoomable="yes"}
1. Nella finestra del plug-in, inserisci il nome di un progetto per le varianti, scegli una piattaforma per il contenuto e compila le altre informazioni richieste. Quindi fare clic sul pulsante **[!UICONTROL Termina installazione]**.
   ![Finestra Imposta progetto](./setup-project.png){width="300" zoomable="yes"}
1. Selezionare [!DNL Brand], [!DNL Persona] e [!DNL Product] da utilizzare per la generazione del contenuto.
1. Seleziona il numero di varianti da produrre (fino a otto).
1. Utilizza il pulsante in **[!UICONTROL Seleziona contenuto]** per sfogliare e scegliere le immagini dalle risorse. Le 40 risorse aggiunte più di recente vengono visualizzate per prime e puoi cercare altre risorse. Le immagini selezionate vengono automaticamente ridimensionate in base ai modelli.
1. Immettere un prompt di testo. Per ogni campo dell&#39;elenco **[!UICONTROL Campi]**, l&#39;opzione **[!UICONTROL Azione]** è impostata su **[!UICONTROL Genera]** per il nuovo contenuto.
1. Mappa tutti i ruoli del campo. Vedi [Mappatura ruolo campo](#field-role-mapping).
1. Fare clic sul pulsante **[!UICONTROL Genera]**.

## Traduci o genera varianti di ad copy da contenuto esistente

Utilizza GenStudio for Performance Marketing AI per generare varianti di ad copy o tradurre modelli Figma.

1. Seleziona il nodo della sezione che contiene i modelli di annuncio. Puoi eseguire questa operazione dal pannello **Livelli** o facendo clic direttamente sulla sezione nell&#39;area di lavoro.
   ![Selezione sezione o varianti](./plugin-playground.png){width="500" zoomable="yes"}
1. Nella finestra del plug-in, inserisci il nome di un progetto per le varianti e scegli una piattaforma per il contenuto.
1. In **[!UICONTROL Qual è l&#39;obiettivo?]**, seleziona **[!UICONTROL Genera varianti]** o **[!UICONTROL Traduci]**, quindi fai clic sul pulsante **[!UICONTROL Termina installazione]**.
   ![Finestra Imposta progetto](./setup-project.png){width="300" zoomable="yes"}
1. Selezionare [!DNL Brand], [!DNL Persona] e [!DNL Product] da utilizzare per la generazione del contenuto.
1. Seleziona il numero di varianti da produrre.
1. Utilizza il pulsante in **[!UICONTROL Seleziona contenuto]** per sfogliare e scegliere le immagini dalle risorse. Le 40 risorse aggiunte più di recente vengono visualizzate per prime e puoi cercare altre risorse. Le immagini selezionate vengono automaticamente ridimensionate in base ai modelli.
1. Immettere un prompt di testo. Per ogni campo dell&#39;elenco **[!UICONTROL Campi]**, l&#39;opzione **[!UICONTROL Azione]** è impostata su **[!UICONTROL Genera]** per il nuovo contenuto.
1. Mappa tutti i ruoli del campo. Vedi [Mappatura ruolo campo](#field-role-mapping).
1. Seleziona ciascun tipo di campo da generare varianti o tradurre nel pannello sul lato sinistro del plug-in e incolla il contenuto iniziale in ogni casella **[!UICONTROL Contenuto iniziale]**.
   ![Testo di esempio nella casella Contenuto iniziale](./initial-content-box.png){width="60%" zoomable="yes"}
1. Fare clic sul pulsante **[!UICONTROL Genera]**.

## Traduci contenuto dopo la generazione

1. Seleziona una generazione da tradurre.
   ![Seleziona generazione](./select-generation.png){width="200" zoomable="yes"}
1. Scegli **[!UICONTROL Traduzione]**, quindi fai clic su **[!UICONTROL Traduci]**.
1. Seleziona la lingua o le lingue di destinazione.
1. Fai clic su **[!UICONTROL Seleziona]**.

I risultati della traduzione includono:

* Viene visualizzata una nuova pagina con il contenuto tradotto.
* Ogni traduzione mostra la lingua o le impostazioni internazionali di destinazione.
* Il contenuto originale rimane invariato nella pagina originale.

![Risultati traduzione](./translation-results.png){width="60%" zoomable="yes"}

## Altre azioni sui campi di contenuto dopo la generazione

Durante la modifica del contenuto esistente in un campo, nel pannello del plug-in vengono visualizzate opzioni utili.

![Opzioni azioni plug-in](./figma-other-actions.png){width="300" zoomable="yes"}

Le opzioni includono:

* Modificare **[!UICONTROL Valore]** per modificare direttamente il testo. La modifica di questo contenuto si applica automaticamente a tutte le varianti selezionate.
* L&#39;IA può eseguire molte opzioni **[!UICONTROL Azione]**, tra cui:

| Azione | Descrizione |
| --- | --- |
| **[!UICONTROL Genera]** | Genera una nuova variante del testo. |
| **[!UICONTROL Riformula]** | Genera una nuova variante del testo. |
| **[!UICONTROL Abbrevia]** | Genera una variante più breve del testo. |
| **[!UICONTROL Allunga]** | Genera una variante più lunga del testo. |

Dopo aver selezionato un&#39;opzione **[!UICONTROL Azione]**, rigenera il contenuto con il pulsante **[!UICONTROL Rigenera]**.

## Esportare esperienze

Le varianti possono essere esportate da Figma come GenStudio for Performance Marketing [!DNL Experiences].

1. Selezionare il contenuto da esportare nell&#39;area di lavoro di Figma eseguendo una delle operazioni seguenti:
   * Seleziona la sezione di generazione nell&#39;area di lavoro, quindi fai clic su **[!UICONTROL Contrassegna tutto per esportazione]** nel pannello dei plug-in.
     ![Selezione sezione generazione](./select-generation-section.png){width="200" zoomable="yes"}
   * Seleziona una singola generazione nell&#39;area di lavoro, quindi fai clic su **[!UICONTROL Contrassegna per esportazione]** nel pannello del plug-in.
     ![Selezione generazione individuale](./select-generation.png){width="200" zoomable="yes"}
1. Seleziona la voce Esporta dal menu della barra laterale.
   ![Pulsante Contrassegna per esportazione visualizzato per un annuncio Meta](./mark-for-export.png){width="60%" zoomable="yes"}
1. Seleziona una destinazione.
1. Fai clic su **[!UICONTROL Esporta]** per esportare il contenuto.

Nel pannello del plug-in viene creato un file ZIP oppure viene visualizzato un collegamento a **[!UICONTROL Apri in GenStudio]**. Utilizza il collegamento ZIP per scegliere dove salvare il file oppure seleziona **[!UICONTROL Apri in GenStudio]**.

## Cronologia della generazione

Il plug-in mantiene una cronologia delle modifiche per ciascun campo. Nella pagina del modello, scegli **[!UICONTROL Cronologia generazione]** nella barra laterale del plug-in.

![Opzione cronologia generazione visualizzata per un annuncio Meta](./generation-history.png){width="80%" zoomable="yes"}

## Risoluzione dei problemi

Prendi in considerazione queste best practice e suggerimenti se testo o immagini non vengono sostituiti nelle varianti generate.

### Campi mappati

Se il testo o le immagini non vengono sostituiti, verifica che i campi siano stati mappati sui ruoli dei campi di GenStudio nell’interfaccia utente del plug-in. Vedi [Mappatura ruolo campo](#field-role-mapping).

### Conferma che i font siano disponibili

Affinché la sostituzione venga eseguita durante la generazione, è necessario che nel computer sia disponibile un tipo di carattere per il campo di testo. Verificare che tutti i tipi di carattere utilizzati nel file siano disponibili nel computer, soprattutto se il file è stato creato nel computer di un altro utente.

### Considerare il supporto per il ruolo del campo

Alcuni canali supportano la sostituzione solo in campi specifici. Tieni presente le eccezioni per il mapping di ruoli del campo [&#128279;](#field-role-mapping).
