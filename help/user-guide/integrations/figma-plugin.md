---
title: Plug-in Figma per Adobe GenStudio for Performance Marketing
description: Scopri come configurare e utilizzare il plug-in Figma per GenStudio for Performance Marketing.
feature: Generative AI
role: User
exl-id: 232fbbc6-c523-4525-8d26-a8ac8d62c035
source-git-commit: c6080555812fa82a7b71eee7e2deb963a881d9f4
workflow-type: tm+mt
source-wordcount: '2124'
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

>[!VIDEO](https://video.tv.adobe.com/v/3478817?captions=ita&learn=on)

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

## Generare un’immagine

Genera immagini da utilizzare nei modelli utilizzando un prompt di testo.

1. Selezionare **[!UICONTROL Genera immagine]**.
1. Seleziona un modello dal menu a discesa. Puoi anche scegliere qualsiasi modello personalizzato creato.
1. Seleziona l’icona delle impostazioni per regolare le impostazioni di generazione.
1. Facoltativo: selezionare le proporzioni.
1. Facoltativo: regolare lo stile dell&#39;immagine eseguendo una delle operazioni seguenti:
   * Carica un&#39;immagine di riferimento dal dispositivo o da AEM selezionando **[!UICONTROL Carica immagine]**.
   * Scegli una delle immagini stock di Adobe selezionando **[!UICONTROL Sfoglia raccolta]**.
   * Scegliete un valore di forza utilizzando il cursore. L&#39;opzione Forza consente di regolare il livello di aderenza di Firefly allo stile fornito.
1. Selezionare il pulsante **&lt;**.
1. Immetti un prompt.
1. Seleziona l’icona Genera. Le immagini vengono visualizzate nel pannello del plug-in.
1. Applica le immagini all&#39;area di lavoro utilizzando uno dei seguenti metodi:
   * Trascina e rilascia qualsiasi immagine nell’area di lavoro.
   * Selezionate un fotogramma nell&#39;area di lavoro di Figma e selezionate un&#39;immagine da inserire nel fotogramma nella finestra del plug-in.
   * Seleziona l’icona Carica per caricare un’immagine nell’area di lavoro.
   * Selezionare i 3 punti e **[!UICONTROL Scaricare tutto in Figma]**.
1. Facoltativo: selezionare i 3 punti per eseguire ulteriori azioni:
   * Selezionare **[!UICONTROL Genera altro]** per eseguire di nuovo il prompt.
   * Selezionare **[!UICONTROL Copia prompt]** per copiare il prompt.
1. Facoltativo: selezionare l&#39;icona della matita per utilizzare il riempimento Generativo e generare azioni simili su una singola immagine.

## Genera immagini simili

Genera un set di immagini simili.

1. Seleziona la scheda **[!UICONTROL Genera simili]**.
1. Selezionate un&#39;immagine come riferimento effettuando una delle seguenti operazioni:
   * Selezionare un&#39;immagine nell&#39;area di lavoro di Figma.
   * Seleziona **[!UICONTROL Carica immagine]** da caricare dal dispositivo.
   * Seleziona **[!UICONTROL Sfoglia risorse AEM]** da caricare da AEM.
1. Seleziona l’icona Genera. Le varianti vengono visualizzate nel pannello plugin.
1. Applica le immagini all&#39;area di lavoro utilizzando uno dei seguenti metodi:
   * Trascina e rilascia qualsiasi immagine nell’area di lavoro.
   * Selezionate un fotogramma nell&#39;area di lavoro di Figma e selezionate un&#39;immagine da inserire nel fotogramma nella finestra del plug-in.
   * Seleziona l’icona Carica per caricare un’immagine nell’area di lavoro.
   * Selezionare i 3 punti e **[!UICONTROL Scaricare tutto in Figma]**.
1. Facoltativo: selezionare i 3 punti per eseguire ulteriori azioni:
   * Selezionare **[!UICONTROL Genera altro]** per eseguire di nuovo il prompt.
1. Facoltativo: selezionare l&#39;icona della matita per utilizzare il riempimento Generativo e generare azioni simili su una singola immagine.

## Rimuovere lo sfondo

Rimuovere lo sfondo di un&#39;immagine.

1. Selezionare la scheda **[!UICONTROL Rimuovi sfondo]**.
1. Selezionate un&#39;immagine come riferimento effettuando una delle seguenti operazioni:
   * Selezionare un&#39;immagine nell&#39;area di lavoro di Figma.
   * Seleziona **[!UICONTROL Carica immagine]** da caricare dal dispositivo.
   * Seleziona **[!UICONTROL Sfoglia risorse AEM]** da caricare da AEM.
1. Selezionare **[!UICONTROL Rimuovi]**. Se l’immagine è stata selezionata dall’area di lavoro, viene sostituita da quest’ultima. Se l&#39;immagine è stata selezionata da un dispositivo o da AEM, è possibile trascinarla nell&#39;area di lavoro oppure selezionare **[!UICONTROL Inserisci immagine]** per inserire l&#39;immagine nell&#39;area di lavoro.

## Riempimento generativo

Applicare riempimenti generativi per un&#39;area di un&#39;immagine.

1. Selezionare la scheda **[!UICONTROL Riempimento generativo]**.
1. Selezionate un&#39;immagine come riferimento effettuando una delle seguenti operazioni:
   * Selezionare un&#39;immagine nell&#39;area di lavoro di Figma.
   * Seleziona **[!UICONTROL Carica immagine]** da caricare dal dispositivo.
   * Seleziona **[!UICONTROL Sfoglia risorse AEM]** da caricare da AEM.
1. Selezionate lo strumento pennello e create una maschera.
1. Facoltativo: selezionare il punto di inserimento a discesa e regolare la dimensione del pennello.
1. Selezionare il pulsante Reimposta per rimuovere la maschera.
1. Se necessario, seleziona l’icona Rimuovi sfondo per rimuovere lo sfondo.
1. Immetti un prompt per guidare la generazione della maschera selezionata e seleziona il pulsante **[!UICONTROL Genera]**.
1. Applica le immagini all&#39;area di lavoro utilizzando uno dei seguenti metodi:
   * Trascina e rilascia qualsiasi immagine nell’area di lavoro.
   * Selezionate un fotogramma nell&#39;area di lavoro di Figma e selezionate un&#39;immagine da inserire nel fotogramma nella finestra del plug-in.
   * Seleziona l’icona Carica per caricare un’immagine nell’area di lavoro.
   * Selezionare i 3 punti e **[!UICONTROL Scaricare tutto in Figma]**.
1. Facoltativo: selezionare i 3 punti per eseguire ulteriori azioni:
   * Selezionare **[!UICONTROL Copia prompt]** per copiare il prompt.
1. Facoltativo: selezionare l&#39;icona della matita per utilizzare il riempimento Generativo e generare azioni simili su una singola immagine.

## Richiedi modifica

Modifica il contenuto di un’immagine con un prompt di testo.

1. Selezionare la scheda **[!UICONTROL Richiedi modifica]**.
1. Selezionate un&#39;immagine come riferimento effettuando una delle seguenti operazioni:
   * Selezionare un&#39;immagine nell&#39;area di lavoro di Figma.
   * Seleziona **[!UICONTROL Carica immagine]** da caricare dal dispositivo.
   * Seleziona **[!UICONTROL Sfoglia risorse AEM]** da caricare da AEM.
1. Seleziona l’icona delle impostazioni per regolare le impostazioni di generazione.
1. Facoltativo: selezionare le proporzioni e il pulsante **&lt;**.
1. Immetti un prompt per guidare la generazione e seleziona il pulsante **[!UICONTROL Genera]**.
1. Applica le immagini all&#39;area di lavoro utilizzando uno dei seguenti metodi:
   * Trascina e rilascia qualsiasi immagine nell’area di lavoro.
   * Selezionate un fotogramma nell&#39;area di lavoro di Figma e selezionate un&#39;immagine da inserire nel fotogramma nella finestra del plug-in.
   * Seleziona l’icona Carica per caricare un’immagine nell’area di lavoro.
   * Selezionare i 3 punti e **[!UICONTROL Scaricare tutto in Figma]**.
1. Facoltativo: selezionare i 3 punti per eseguire ulteriori azioni:
   * Selezionare **[!UICONTROL Genera altro]** per eseguire di nuovo il prompt.
   * Selezionare **[!UICONTROL Copia prompt]** per copiare il prompt.
1. Facoltativo: selezionare l&#39;icona della matita per utilizzare il riempimento Generativo e generare azioni simili su una singola immagine.

## Espansione generativa

Espandi le dimensioni delle immagini e aggiungi contenuti generativi con Espandi generativo. L’espansione generativa consente di trasformare immagini inadatte nelle proporzioni più adatte per i modelli di banner, annunci Meta, annunci LinkedIn o annunci di visualizzazione.

1. Seleziona la scheda **[!UICONTROL Espandi generativi]**.
1. Seleziona un’immagine nell’area di lavoro.
1. Ridimensionare il fotogramma temporaneo di espansione della generazione in base alle nuove dimensioni desiderate.
1. Facoltativo: spostare l&#39;immagine in qualsiasi punto all&#39;interno della cornice.
1. Immetti un prompt per guidare la generazione e seleziona il pulsante **[!UICONTROL Genera]**.
1. Seleziona un’immagine nell’area di lavoro per sostituire l’immagine originale con il risultato generato.

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
