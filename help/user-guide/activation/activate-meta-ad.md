---
title: Attivare un Meta Ad
description: Scopri come attivare un’esperienza di annuncio multimediale.
feature: Experiences
source-git-commit: a098e053dffe4835a4425252203977dc6ce44713
workflow-type: tm+mt
source-wordcount: '1411'
ht-degree: 1%

---

# Attivare un Meta Ad

Adobe GenStudio for Performance Marketing supporta l’attivazione di Meta ads, o creativi, su Instagram e Facebook.

È possibile [creare un&#39;esperienza Meta](/help/user-guide/create/create-meta-ad.md) in GenStudio for Performance Marketing e selezionarla per l&#39;attivazione oppure creare una nuova esperienza dalle risorse approvate in [!DNL Activate].

L&#39;attivazione di un annuncio Meta segue gli [stessi passaggi generali](create-activation.md) richiesti per l&#39;attivazione ad altri canali a pagamento. Il processo di attivazione supporta la preparazione delle esperienze pubblicitarie per i requisiti specifici di Meta. Dopo aver attivato un&#39;esperienza Meta, o creatività, in GenStudio for Performance Marketing, utilizza [Meta Ads Manager](https://adsmanager.facebook.com/) per perfezionare l&#39;esperienza per posizionamenti di annunci Meta specifici prima della pubblicazione finale.

## Passaggio 1: configurare i metadati

Prima di avviare un&#39;attivazione, [accedi a Meta](https://adsmanager.facebook.com/) per accedere al tuo account di Meta Ads Manager. Conferma che gli account dei Meta Ad collegati includano:

* Pagina Facebook
* Meta campaign
* Metadati set di annunci
* Profilo Instagram (facoltativo)

Devi disporre dell&#39;autorizzazione per pubblicare contenuti su Meta Ads Manager.

## Passaggio 2: collegati ai metadati

Prima che la tua organizzazione possa attivare le esperienze, un manager di sistema GenStudio deve collegare i tuoi account Meta a GenStudio for Performance Marketing. Questa connessione consente il flusso dei dati tra GenStudio e strumenti di marketing esterni come Meta, abilitando i processi di attivazione.

**Per collegare GenStudio for Performance Marketing ai tuoi account Meta**:

1. Da _Impostazioni_, fai clic su **[!UICONTROL Connetti]** nella sezione Meta Ads. Viene aperta la visualizzazione dell&#39;account _Meta ads_.

1. Seleziona **[!UICONTROL Consenti popup]** dal browser, se richiesto.

1. Seleziona uno o più account annuncio da connettere, quindi fai clic su **[!UICONTROL Seleziona]**.

Al termine della sincronizzazione, puoi visualizzare gli account aggiunti. La sincronizzazione di grandi quantità di dati richiede più tempo.

## Passaggio 3: preparare l’esperienza per l’attivazione

I system manager e gli editor di GenStudio possono attivare le esperienze pubblicitarie.

**Per preparare l&#39;esperienza per l&#39;attivazione**:

1. Da _[!DNL Activate]_, fai clic su **[!UICONTROL Nuovo]**nella sezione Prodotto metadati. Verrà aperta la visualizzazione_ Configurazione di Creative _.

   La pagina di configurazione di Creative fornisce una posizione centrale per la preparazione dell’attivazione dei Meta Ad. La preparazione dell’annuncio include le tre attività seguenti:

1. Assegna un nome all&#39;esperienza. Dopo l&#39;attivazione, è possibile utilizzare questo nome per cercare questa esperienza nella tabella _Esperienze attivate_.
1. Seleziona le risorse multimediali. Puoi utilizzare le risorse da Contenuto o caricare risorse esterne, ad esempio da OneDrive o Dropbox.
1. [Aggiungi testo](#add-ad-text).
1. [Aggiungi metadati](#assign-metadata).

   Il _pannello Anteprima_ supporta una visualizzazione interattiva del testo e delle risorse nel contesto di un posizionamento specifico dell&#39;annuncio. Utilizza il menu a discesa _Seleziona posizionamento_ per passare tra i posizionamenti di annunci supportati. Le anteprime offrono l’opportunità di finalizzare le decisioni sugli elementi annuncio per posizionamenti specifici. Quando selezioni un posizionamento nel pannello _Anteprima_, viene interessata solo la visualizzazione dell&#39;annuncio. La selezione del posizionamento nel pannello _Anteprima_ non è stata salvata.

### Seleziona le risorse multimediali

Utilizza la sezione _Media_ per selezionare almeno una risorsa immagine da includere nell&#39;esperienza. I posizionamenti di annunci sono associati alle proporzioni immagine supportate, elencate come opzioni nel menu a discesa _Posizionamenti_. Questo menu mostra i posizionamenti di annunci supportati per i post di Facebook o le storie di Instagram, organizzati per proporzioni.

Dopo il caricamento, le risorse vengono salvate in _[!DNL Content]_. Nell&#39;area_ Media _l&#39;immagine viene visualizzata per impostazione predefinita con proporzioni 1:1. Le proporzioni alternative includono solo i valori supportati dal canale dell’annuncio a pagamento. Sono raggruppati per orientamento verticale e orizzontale. GenStudio for Performance Marketing supporta l’inclusione di un massimo di sei rapporti di aspetto per ogni esperienza attivata.

**Per caricare una risorsa dal contenuto**:

_[!DNL Content]_fornisce una visualizzazione centrale delle risorse e delle esperienze approvate della tua organizzazione. Puoi rendere attiva la[_[!DNL Content]_ raccolta](/help/user-guide/content/manage-assets.md) visualizzata con l&#39;inventario delle risorse utilizzando le opzioni di menu **[!UICONTROL Cerca]** (lente di ingrandimento) e _Filtra_.

1. Da _[!DNL Activate]_, fai clic su **[!UICONTROL Nuovo]**nella sezione Meta Ads. Verrà aperta la visualizzazione_ Configurazione di Creative _.

1. Fai clic su **[!UICONTROL Seleziona]**, quindi seleziona **[!UICONTROL Seleziona dal contenuto]**. Viene aperta la visualizzazione _Seleziona contenuto_, in cui viene visualizzata una raccolta di risorse immagine cercate o filtrate.

1. Utilizza gli strumenti di ricerca e filtro della raccolta _[!DNL Content]_per selezionare almeno una risorsa da caricare.

1. Fai clic su **[!UICONTROL Usa]** per includere nella tua creatività la risorsa selezionata. La finestra _Installazione di Creative_ include la risorsa nelle proporzioni predefinite nell&#39;area _Media_. Il pannello _Anteprima_ visualizza in anteprima la risorsa nel posizionamento dell&#39;annuncio che supporta queste proporzioni.

Se il caricamento non riesce, viene visualizzato un messaggio di errore informativo che include un collegamento alla risorsa in _[!DNL Content]_.

**Per caricare una risorsa esterna**:

È possibile caricare fino a sei immagini statiche esterne alla raccolta _[!DNL Content]_da Microsoft OneDrive o Dropbox.

1. Da _[!DNL Activate]_, fai clic su **[!UICONTROL Nuovo]**nella sezione Meta. Viene visualizzata la finestra_ Installazione di Creative _.

1. Nella sezione _Media_, fai clic su **[!UICONTROL Seleziona]**. In un menu a discesa vengono visualizzate le opzioni per _Seleziona dal contenuto_ o _Carica_.

1. Fai clic su **[!UICONTROL Carica]**. Viene visualizzata la finestra _Aggiungi proporzioni_.

1. Seleziona le immagini nelle proporzioni supportate trascinando i file immagine nell’area di caricamento dell’immagine. In alternativa, puoi cercare le risorse nel dispositivo.

1. (Facoltativo) Per caricare le risorse dal dispositivo, fai clic su **[!UICONTROL Sfoglia]**, quindi seleziona _Sfoglia file_ o _Sfoglia cartelle_ per identificare le risorse da caricare.

1. Nell&#39;area _Aggiungi dettagli_, aggiungi dettagli informativi alle risorse caricate per facilitare la ricerca e il filtraggio in _[!DNL Content]_. Questi dettagli vengono salvati come metadati.

1. Dopo aver caricato le risorse e assegnato i dettagli, fai clic su **[!UICONTROL Aggiungi Assets]** in basso a destra.

### Aggiungi testo annuncio

Utilizza la sezione _Testo_ della pagina _Attiva Meta Ad_ per aggiungere testo convincente e aderente al brand ai campi di testo richiesti. Il testo include il testo principale (corpo) dell’annuncio e del testo dell’invito all’azione.

| Campo | Obbligatorio | Limite di caratteri (max) |
|-----------------|---------------------------|---------------------------------|
| Nome annuncio | sì | 500 |
| Testo principale | sì | 500 |
| Titolo | sì | 255 |
| Descrizione | no | 125 |
| Invito all’azione | sì | solo opzioni del menu a discesa |
| Visualizza URL | no | 1000 |
| URL sito Web | sì | 1000 |
| Immagine | almeno uno richiesto |                                 |

_Il testo principale_ e il _titolo_ sono richiesti solo da GenStudio for Performance Marketing, non da Meta.

### Assegna metadati

I dettagli dell’esperienza vengono salvati come metadati e aiutano gli utenti nella ricerca di un’esperienza. Questi dettagli aumentano la visibilità dell&#39;esperienza in [!DNL Content]. Utilizza questi dettagli facoltativi definiti dall&#39;utente per identificare lo scopo dell&#39;esperienza e il contesto, o le campagne, in cui viene distribuita.

| Dettaglio | Descrizione |
|------------|-------------|
| Campagne | Tutte le campagne GenStudio for Performance Marketing a cui appartiene l’esperienza annuncio |
| Marchio | Linee guida, definite dall’utente o predefinite, che consentono agli utenti di stabilire linee guida per il brand che acquisiscono l’essenza dell’identità di un brand. |
| Prodotti | Prodotti associati alla tua organizzazione e identificati in GenStudio for Performance Marketing |
| Persone | Persone associate alla tua organizzazione e identificate in GenStudio for Performance Marketing |
| Intervallo temporale | Il trimestre, la stagione, l’anno o un’altra unità di tempo definita dall’organizzazione durante la quale è attiva l’esperienza pubblicitaria |
| Regione | Area geografica in cui viene avviata l’esperienza |
| Lingua | Lingue per cui viene utilizzata l’esperienza annuncio |
| Parole chiave | Parole chiave definite dall’utente che facilitano la ricerca e la categorizzazione dell’esperienza dell’annuncio |

Dopo aver assemblato il tuo contenuto creativo, fai clic su **[!UICONTROL Avanti]** per confermare la configurazione di Meta.

## Passaggio 4: conferma impostazione metadati

Dopo aver preparato il contenuto creativo, devi confermare le informazioni sul tuo account Meta e assegnare un ID di tracciamento all’esperienza dell’annuncio. La visualizzazione _Impostazione annuncio metadati_ è compilata con opzioni derivate dagli account metadati configurati.

| Dettaglio | Descrizione |
|------------|-------------|
| Account | Metaaccount connessi a GenStudio for Performance Marketing |
| Pagina Facebook | Pagina Facebook in cui viene pubblicata l’esperienza |
| Account Instagram | Account Instagram connessi a GenStudio for Performance Marketing |
| Campagne | Campagne metadati a cui appartiene l’esperienza annuncio |
| Set di annunci | Meta set di annunci a cui appartiene l’esperienza di annuncio attivato. Le impostazioni determinano il posizionamento finale dell’annuncio. |

### ID tracciamento

Gli ID di tracciamento (nome annuncio) forniscono un meccanismo per raccogliere metriche collegate alle prestazioni dell’esperienza. Immetti il nome dell’annuncio in questo campo.

Fai clic su **[!UICONTROL Avanti]** in alto a destra per visualizzare l&#39;anteprima della tua esperienza pubblicitaria e finalizzare l&#39;attivazione.

## Passaggio 5: visualizzare l’anteprima e attivare l’annuncio

Nella pagina _Revisione_ viene visualizzata l&#39;esperienza pubblicitaria assemblata nella _configurazione di Creative_ e viene fornita un&#39;ultima opportunità per visualizzare e modificare l&#39;esperienza. Fai clic su **[!UICONTROL Modifica sezione]** accanto all&#39;etichetta _Configurazione di Creative_ per apportare le modifiche. Puoi anche fare clic su **[!UICONTROL Indietro]** in alto a destra per tornare alla pagina _Configurazione di Creative_.

### Attivazione completa dell’esperienza pubblicitaria

Fai clic su **[!UICONTROL Pubblica]**. L’esperienza completa dei metadati e i metadati associati vengono inviati direttamente nel set di annunci di Meta Ads Manager selezionato. Le esperienze vengono distribuite a Meta Ads Manager disattivato. Da Meta Ads Manager, puoi gestire i passaggi finali della distribuzione dell’esperienza pubblicitaria e della campagna Meta.

### Accedi a Meta Ads Manager per completare l&#39;attivazione

Al termine dell’attivazione, devi accedere a Meta Ads Manager. Da [Meta Ads Manager](https://adsmanager.facebook.com/), puoi rivedere la tua esperienza pubblicitaria e finalizzare la pubblicazione su canali Meta specifici.
