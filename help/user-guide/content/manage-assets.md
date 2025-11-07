---
title: Gestire Assets ed esperienze
description: Semplifica e migliora la gestione delle risorse approvate dal marchio da utilizzare e riutilizzare nel percorso di marketing digitale.
feature: Content Management, Content Attributes
exl-id: e2ce8797-6d3b-46d4-b12f-f5f80e26c669
source-git-commit: 279bf9e1fab24c286df4a0600b472c456231ddb6
workflow-type: tm+mt
source-wordcount: '1509'
ht-degree: 1%

---

# Gestire risorse ed esperienze

Adobe GenStudio for Performance Marketing [!DNL Content] semplifica e migliora la gestione delle risorse approvate dal marchio da utilizzare e riutilizzare nel percorso di marketing digitale.

## [!DNL Content] raccolta

Nella galleria viene visualizzato un inventario delle risorse, esperienze o modelli approvati, a seconda della vista selezionata. L&#39;interruttore del filtro (funnel) sopra il lato sinistro della tabella apre il menu **[!UICONTROL Filtro]**, in cui è possibile selezionare diverse categorie per filtrare il contenuto visualizzato nella raccolta. Nella visualizzazione _[!UICONTROL Assets]_, fare clic sull&#39;icona di ricerca (lente di ingrandimento) per utilizzare una parola chiave per trovare una risorsa.

Di seguito è riportata una ricerca per il termine `space` nella raccolta [!UICONTROL Assets]:

![Visualizzazione Assets con ricerca nello spazio](/help/assets/content-assets-filter.png "Ricerca di risorse con attributo spazio")

### Cerca contenuto

Il filtro e l’interfaccia di ricerca sono rapidi e reattivi e forniscono un’esperienza di ricerca iniziale produttiva. Ogni visualizzazione [!DNL Content] fornisce opzioni filtro per limitare la ricerca della risorsa, dell&#39;esperienza o del modello ideale. Per risorse ed esperienze, puoi selezionare una campagna e linee guida specifiche, ad esempio contenuti creati per un prodotto specifico.

Esistono filtri basati su [linee guida](/help/user-guide/guidelines/overview.md), [parole chiave](asset-details.md#user-defined-metadata) e [categorie di attributi](/help/user-guide/insights/attributes.md#categories) per limitare i risultati della ricerca. Ad esempio, potresti voler trovare una risorsa di un particolare tipo di file o oggetto per aiutarti a creare una nuova esperienza per la campagna. Oppure puoi filtrare il contenuto in base al tuo nome utente o al nome di un membro del team:

- **[!UICONTROL Caricato da]**: limita l&#39;elenco _[!UICONTROL Assets]_ in modo da visualizzare solo le risorse caricate da te o da una persona specifica.
- **[!UICONTROL Creato da]**: limita l&#39;elenco _[!UICONTROL Esperienze]_ per mostrare solo le esperienze create da te o da una persona specifica.
- **[!UICONTROL Modello]**: limita l&#39;elenco _[!UICONTROL Esperienze]_ in modo da visualizzare solo le esperienze create con il modello selezionato.

Se alcune opzioni di filtro non sono visibili, indica che nessun modello nell’archivio corrisponde ai criteri di metadati corrispondenti. Assicurati che i modelli siano correttamente taggati con metadati per renderli individuabili tramite questi filtri.

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

### Dove si trova

Per impostazione predefinita, le risorse aggiunte a [!DNL Content] tramite il processo [!DNL Create] o il caricamento vengono archiviate nell&#39;archivio `GenStudio assets`. L&#39;archivio `GenStudio assets` è di lettura/scrittura in GenStudio for Performance Marketing. Ciò significa che è possibile salvare, modificare ed eliminare le risorse nell&#39;archivio `GenStudio assets`.

L&#39;elenco **[!UICONTROL Posizione]** sopra la raccolta _[!UICONTROL Assets]_ sul lato destro consente di selezionare dagli archivi connessi di Adobe Experience Manager (AEM) [!DNL Assets Content Hub].

![Elenco percorsi dei repository](/help/assets/content-location-selection.png "Selezionare un repository dei contenuti"){width="350"}

Quando selezioni un archivio AEM, nella galleria viene visualizzato un inventario delle risorse provenienti da tale archivio, che consente di sfruttare le risorse approvate provenienti da tali archivi come input per la creazione di contenuto. Le opzioni del filtro cambiano per riflettere le categorie configurate in [!DNL AEM Assets Content Hub].

Consulta [Connettere un archivio AEM](connect-aem-repo.md) per istruzioni sull&#39;aggiunta del tuo archivio [!DNL AEM Assets Content Hub] a GenStudio for Performance Marketing.

L’archivio AEM è di sola lettura, il che significa che puoi accedere al contenuto ma non salvare le bozze, le nuove risorse o i metadati nell’archivio AEM. Tutte le bozze e gli aggiornamenti finali per risorse, esperienze e modelli vengono salvati nell&#39;archivio `GenStudio assets` con i nuovi [metadati di sistema](asset-details.md#system-metadata).

{{note-aem-assets}}

Un archivio AEM può applicare determinati requisiti di licenza, ad esempio la scadenza delle risorse. Queste risorse potrebbero non essere disponibili per l&#39;utilizzo nei flussi di lavoro [!DNL Create]. Potrebbe essere necessario rinnovare o sostituire le risorse scadute per mantenere la continuità dei progetti. Per assistenza su queste risorse, rivolgiti all&#39;amministratore [!DNL AEM Assets Content Hub].

## Gestione di Assets

In [!UICONTROL Contenuto] puoi archiviare, recuperare e gestire facilmente le risorse digitali. Sfruttando sia l&#39;archivio `GenStudio assets` che gli archivi AEM, puoi garantire che le risorse siano ben organizzate e accessibili per varie campagne di marketing. Questo approccio con più repository offre flessibilità e controllo sull’utilizzo delle risorse in ambienti diversi, garantendo che solo le risorse approvate e aggiornate vengano utilizzate nelle attività di marketing.

Nella tabella seguente sono elencate le attività di gestione disponibili per risorse, esperienze e modelli:

| Attività | Risorse | Esperienze | Modelli |
| --------------------------------------------------------- | :----: | :---------: | :-------: |
| [Visualizza dettagli](/help/user-guide/content/asset-details.md) | ✓ | ✓ | ✓ |
| [Crea esperienza](/help/user-guide/create/overview.md) |        |             | ✓ |
| [Modifica in Adobe Express](#edit-in-express) | ✓ |             |           |
| [Esporta esperienze](#export-experiences) |        | ✓ |           |
| [Aggiorna](/help/user-guide/content/use-templates.md#refresh-template) |   |      | ✓ |
| [Download](#download-assets) | ✓ |             | ✓ |
| [Elimina](#delete-assets) | ✓ | ✓ | ✓ |

### Aggiungere le risorse

Per impostazione predefinita, quando si aggiungono risorse a [!DNL Content], queste vengono memorizzate nell&#39;archivio `GenStudio assets`. Il pulsante _[!UICONTROL Aggiungi risorse]_ è disponibile solo quando _[!UICONTROL Posizione]_ è l&#39;archivio `GenStudio assets`.

![Campo posizione](/help/assets/content-location.png "Campo posizione"){width="350"}

**Per aggiungere una o più risorse**:

1. In _[!DNL Content]_, fai clic su **[!UICONTROL Aggiungi risorse]**.

2. Nella visualizzazione _Aggiungi le risorse approvate_, rilascia uno o più file nello spazio di rilascio. In alternativa, è possibile selezionare i file locali utilizzando **[!UICONTROL Sfoglia]** o importare i file da Dropbox o Microsoft OneDrive.

3. Nella sezione _Aggiungi dettagli_, seleziona un **[!UICONTROL nome campagna]** o immetti un nuovo nome.

4. Per informazioni sull&#39;individuazione, aggiungere dettagli facoltativi come _Brand name_, _Personas_, _Region_ e _Keywords_ nella sezione **More details**.

   Maggiore è il numero di dettagli forniti, maggiori saranno le funzionalità di GenStudio for Performance Marketing. Selezionare uno o più dettagli dall&#39;elenco o immetterne uno nuovo, se applicabile, ad esempio con parole chiave. Ogni dettaglio aggiunto viene visualizzato sotto l&#39;elenco. Fare clic su **`x`** per rimuovere un dettaglio.

   Tutti i dettagli aggiunti vengono applicati a tutte le risorse aggiunte in questa azione.

   Vedi [Dettagli metadati](/help/user-guide/content/asset-details.md#system-metadata).

5. Fai clic su **[!UICONTROL Aggiungi risorse]**.

6. Al termine del caricamento della risorsa, fai clic su **Fine**.

7. Per visualizzare le nuove risorse caricate, fai clic su **[!UICONTROL Aggiorna]** dalla notifica _Nuove risorse disponibili_ nella parte inferiore dell&#39;area di lavoro.

### Scaricare le risorse

**Per scaricare una risorsa**:

1. In _[!DNL Content]_, seleziona una risorsa o un modello. Facendo clic su una risorsa si apre una sua visualizzazione mirata.

1. Nella visualizzazione delle risorse, fai clic sull&#39;icona **[!UICONTROL Scarica]** (freccia rivolta verso il basso) in alto a destra.

1. Il download inizia inserendo una copia della risorsa nel percorso di download predefinito.

### Eliminare risorse

**Per eliminare una risorsa**:

1. In _[!DNL Content]_, seleziona una risorsa, un&#39;esperienza o un modello. Facendo clic su una risorsa si apre una sua visualizzazione mirata.

1. Nella visualizzazione delle risorse, fai clic su **[!UICONTROL Elimina]** (cestino) in alto a destra.

1. Nel popup _Elimina risorsa_, verifica la risorsa e fai clic su **[!UICONTROL Elimina]**.

## Esportare esperienze

Puoi selezionare una o più esperienze approvate da scaricare in un formato compatibile con il tuo canale di destinazione. Il file scaricato è denominato utilizzando la data di esportazione: `2025-06-15-export.zip`. Quando decomprimi il file, esiste una cartella per ogni tipo di canale che include le risorse esportate nei formati selezionati. Ogni risorsa esportata mantiene il nome originale della risorsa come nome del file.

>[!WARNING]
>
>Le risorse recuperate non sono sicure da visualizzare senza bonifica. Tutti gli utenti devono gestire cross-site scripting (XSS) dai modelli utilizzando tecniche di bonifica di input alla fine.

**Per esportare o scaricare esperienze**:

1. In _[!DNL Content]_, selezionare una o più esperienze.

   Viene visualizzato un banner con il numero di esperienze selezionate a sinistra e le opzioni [!UICONTROL Attiva], [!UICONTROL Scarica] o [!UICONTROL Elimina] a destra.

2. (Facoltativo) Se scegli di attivare, ti potrebbe essere chiesto di selezionare una piattaforma e quindi continuare con il flusso di lavoro [!DNL Activate]. Vedi [Attiva](/help/user-guide/activation/overview.md).

3. Fai clic su **[!UICONTROL Scarica]**.

4. Nel popup _Scarica_, seleziona uno dei formati disponibili.

   Se hai selezionato più esperienze da canali diversi, puoi selezionare il formato per ciascun tipo di canale.

   - E-mail, LinkedIn: `HTML`, `CSV`, `PDF`
   - Meta, banner e annuncio di visualizzazione: `HTML`, `JPEG`, `PNG`, `PDF`


## Modifica in Express

Puoi modificare le risorse immagine (JPG o PNG) direttamente in GenStudio for Performance Marketing utilizzando Adobe Express. L&#39;area di lavoro _[!UICONTROL con tecnologia Adobe Express]_ offre funzionalità utili per migliorare le immagini senza uscire dall&#39;applicazione GenStudio. È possibile rimuovere facilmente gli sfondi, applicare riempimenti generativi, regolare gli effetti e ritagliare le immagini.

>[!BEGINSHADEBOX]

Criteri per migliorare le immagini con la funzionalità [!DNL Edit in Adobe Express]:

- I tipi MIME supportati includono `image/png` e `image/jpeg`
- Le dimensioni minime dell&#39;immagine sono di 50x50 pixel
- Le dimensioni massime dell&#39;immagine sono 8000x8000 pixel
- La dimensione massima è di 40 MB (40.000.000 byte)

>[!ENDSHADEBOX]

**Per modificare una risorsa con Express**:

1. In _[!DNL Content]_, seleziona una risorsa immagine. Facendo clic su una risorsa si apre una sua visualizzazione mirata.

1. Nella visualizzazione delle risorse, fai clic sull&#39;icona **[!UICONTROL Modifica in Adobe Express]** in alto a destra.

1. Nell&#39;area di lavoro _[!UICONTROL Con tecnologia Adobe Express]_, utilizza i controlli Rapidi nel pannello sinistro per migliorare l&#39;immagine.

1. Quando sei soddisfatto dell&#39;immagine aggiornata, fai clic su **[!UICONTROL Salva una copia]** in alto a destra.

1. Selezionare il formato del file, JPG o PNG, e fare clic su **[!UICONTROL Salva una copia]**.

1. Nel popup _[!UICONTROL Salva una copia della risorsa]_, aggiorna **[!UICONTROL Nome risorsa]**.

   - Seleziona **[!UICONTROL Stessi dettagli della risorsa originale]** per trasferire i dettagli della risorsa nella nuova immagine.

   - Espandi la sezione **[!UICONTROL Ulteriori dettagli]** per aggiornare le linee guida e altri metadati.

   >[!TIP]
   >
   >Maggiore è il numero di dettagli forniti, maggiori saranno le funzionalità di GenStudio for Performance Marketing. Selezionare uno o più dettagli dall&#39;elenco o immetterne uno nuovo, se applicabile, ad esempio con parole chiave. Ogni dettaglio aggiunto viene visualizzato sotto l&#39;elenco. Fare clic su **`x`** per rimuovere un dettaglio.

1. Fai clic su **[!UICONTROL Salva]**.
