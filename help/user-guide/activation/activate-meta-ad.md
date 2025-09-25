---
title: Attivare un annuncio Meta
description: Scopri come attivare un’esperienza di annuncio Meta.
feature: Ad Activation
exl-id: 157df612-a774-422c-bca3-2fde9e9d1c88
source-git-commit: 0ccdeb2b3375e9ee72bfc4458eeaff11709768cb
workflow-type: tm+mt
source-wordcount: '1907'
ht-degree: 1%

---

# Attivare un annuncio Meta

Adobe GenStudio for Performance Marketing supporta l’attivazione delle esperienze pubblicitarie Meta su Instagram e Facebook.

È possibile [creare un&#39;esperienza Meta](/help/user-guide/create/create-meta-ad.md) in GenStudio for Performance Marketing e selezionarla per l&#39;attivazione oppure creare una nuova esperienza dalle risorse approvate in [!DNL Activate].

L&#39;attivazione di un annuncio Meta segue gli [stessi passaggi generali](create-activation.md) richiesti per l&#39;attivazione ad altri canali a pagamento. Il processo di attivazione supporta la preparazione dell’esperienza annuncio per i requisiti specifici di Meta. Dopo aver attivato un&#39;esperienza Meta in GenStudio for Performance Marketing, utilizza [Meta Ads Manager](https://adsmanager.facebook.com/) per perfezionare l&#39;esperienza per posizionamenti di annunci Meta specifici prima della pubblicazione finale.

I system manager e gli editor di GenStudio possono attivare le esperienze pubblicitarie.

## Passaggio 1: configurare gli account Meta

Prima di avviare un&#39;attivazione, [accedi a Meta](https://adsmanager.facebook.com/) per accedere al tuo account di Meta Ads Manager.

>[!BEGINSHADEBOX]

**Prerequisiti**:

Conferma che gli account degli annunci Meta connessi dispongano dell’autorizzazione completa per gestire gli annunci in questi componenti della piattaforma pubblicitaria Meta:

* Pagina Facebook
* Campagna Meta
* Set di annunci Meta
* Profilo Instagram (facoltativo)

>[!ENDSHADEBOX]

## Passaggio 2: collegati agli account Meta

Prima che la tua organizzazione possa attivare le esperienze, un manager di sistema di GenStudio deve collegare i tuoi account Meta a GenStudio for Performance Marketing. Questa connessione consente il flusso dei dati tra GenStudio e strumenti di marketing esterni, come Meta, abilitando il processo di attivazione.

Vedi [Connetti a Meta Ads](/help/user-guide/connectors/meta-ads.md).

Al termine della sincronizzazione, puoi visualizzare gli account aggiunti. La sincronizzazione di grandi quantità di dati richiede più tempo.

## Passaggio 3: preparare l’esperienza per l’attivazione

Puoi avviare un’attivazione in due modi:

* **Attiva direttamente da[!DNL Content]**. La selezione di un’esperienza approvata con impostazioni predefinite è il modo più semplice per avviare un’attivazione su un singolo canale.

* **Assembla la tua esperienza annuncio da [!DNL Activate] > _Configurazione esperienza_**. È possibile creare un&#39;esperienza selezionando le risorse visive da [!DNL Content], aggiungendo elementi di testo e selezionando le proporzioni. Questo approccio prevede più passaggi, ma offre maggiore flessibilità nella creazione dell’esperienza creativa.

### Attivare un’esperienza approvata dal contenuto

Puoi selezionare più esperienze da attivare su un singolo canale a pagamento. Potrebbe essere richiesto di selezionare una piattaforma prima di continuare con l&#39;attivazione.

Se hai selezionato più di un&#39;esperienza da attivare come gruppo, utilizza la barra laterale a sinistra per concentrare la visualizzazione _Configurazione esperienza_ sui dettagli dell&#39;esperienza selezionata.

1. Utilizza gli strumenti di ricerca e filtro della raccolta [!DNL Content] per identificare l&#39;esperienza da attivare, quindi fai clic su **[!UICONTROL Attiva]**.

   Per questa esperienza viene aperta la pagina Meta ads _Configurazione esperienza_. È precompilato con i dettagli dell’esperienza selezionata. Puoi modificare i campi **[!UICONTROL Call-to-action]**, **[!UICONTROL URL sito Web]** e **[!UICONTROL Collegamento di visualizzazione]**. Se selezioni più di un&#39;esperienza da attivare, la visualizzazione _Configurazione esperienza_ include una barra laterale a sinistra che visualizza le miniature di tutte le esperienze selezionate. Usa questa barra laterale a sinistra per concentrare la visualizzazione _Configurazione esperienza_ sui dettagli dell&#39;esperienza selezionata.

1. Seleziona una campagna dal menu a discesa **[!UICONTROL Campagne]**.

   Se lavori con più esperienze, passa da un’esperienza all’altra nella barra laterale a sinistra fino a quando non hai completato la preparazione di ciascuna esperienza.

1. Fai clic su **[!UICONTROL Avanti]** per confermare la configurazione degli annunci Meta.

1. Assegna un nome a ogni esperienza. Dopo l&#39;attivazione, è possibile utilizzare questo nome per cercare questa esperienza nella tabella _Esperienze attivate_.

### Assemblare componenti esperienza

Se scegli di non attivare direttamente un&#39;esperienza approvata da [!DNL Content], puoi selezionare le risorse, assegnare le proporzioni e gli elementi di testo in bozza.

**Per preparare l&#39;esperienza per l&#39;attivazione**:

1. Da [!DNL Activate], fai clic su **[!UICONTROL Nuovo]** sull&#39;icona che rappresenta il canale a pagamento scelto. Viene aperta la visualizzazione _Configurazione esperienza_.

   La pagina _Configurazione esperienza_ fornisce una posizione centrale per la preparazione dell&#39;attivazione dell&#39;annuncio. La preparazione dell’annuncio include le tre attività seguenti:

1. Assegna un nome all&#39;esperienza. Dopo l&#39;attivazione, è possibile utilizzare questo nome per cercare questa esperienza nella tabella _Esperienze attivate_.
1. Seleziona le risorse multimediali. È possibile utilizzare le risorse di [!DNL Content] o caricare risorse esterne (ad esempio, da OneDrive o Dropbox).
1. [Aggiungi testo](#add-ad-text).
1. [Aggiungi metadati](#assign-metadata).

   Il _pannello Anteprima_ supporta una visualizzazione interattiva del testo e delle risorse nel contesto di un posizionamento specifico dell&#39;annuncio. Utilizza il menu a discesa _Seleziona posizionamento_ per passare tra i posizionamenti di annunci supportati. Le anteprime offrono l’opportunità di finalizzare le decisioni sugli elementi annuncio per posizionamenti specifici. Quando selezioni un posizionamento nel pannello _Anteprima_, viene interessata solo la visualizzazione dell&#39;annuncio. La selezione del posizionamento nel pannello _Anteprima_ non è stata salvata.

### Seleziona le risorse multimediali

Utilizza la sezione _Media_ per selezionare almeno una risorsa immagine da includere nell&#39;esperienza. I posizionamenti di annunci sono associati alle proporzioni immagine supportate, elencate come opzioni nel menu a discesa _Posizionamenti_. Questo menu mostra i posizionamenti di annunci supportati per i post di Facebook o le storie di Instagram, organizzati per proporzioni.

Dopo il caricamento, le risorse vengono salvate in [!DNL Content]. Nell&#39;area _Media_ l&#39;immagine viene visualizzata per impostazione predefinita con proporzioni 1:1. Le proporzioni alternative includono solo i valori supportati dal canale dell’annuncio a pagamento. Sono raggruppati per orientamento verticale e orizzontale. GenStudio for Performance Marketing supporta l’inclusione di un massimo di sei rapporti di aspetto per ogni esperienza attivata.

**Per caricare una risorsa dal contenuto**:

[!DNL Content] fornisce una visualizzazione centrale delle risorse e delle esperienze approvate della tua organizzazione. Puoi rendere attiva la [[!DNL Content] galleria](/help/user-guide/content/manage-assets.md) visualizzata con l&#39;inventario delle risorse utilizzando le opzioni di menu **[!UICONTROL Cerca]** (lente di ingrandimento) e _Filtra_.

1. Da [!DNL Activate], fai clic su **[!UICONTROL Nuovo]** sulla scheda del canale. Viene aperta la visualizzazione _Configurazione esperienza_.

1. Fai clic su **[!UICONTROL Seleziona]**, quindi seleziona **[!UICONTROL Seleziona dal contenuto]**. Viene aperta la visualizzazione _Seleziona contenuto_, in cui viene visualizzata una raccolta di risorse immagine cercate o filtrate.

1. Utilizza gli strumenti di ricerca e filtro della raccolta [!DNL Content] per selezionare almeno una risorsa da caricare.

1. Fai clic su **[!UICONTROL Utilizza]** per includere la risorsa selezionata nella tua esperienza pubblicitaria. La finestra _Configurazione esperienza_ include la risorsa nelle proporzioni predefinite nell&#39;area _Media_. Il pannello _Anteprima_ visualizza in anteprima la risorsa nel posizionamento dell&#39;annuncio che supporta queste proporzioni.

Se il caricamento non riesce, viene visualizzato un messaggio di errore informativo che include un collegamento alla risorsa in _[!DNL Content]_.

**Per caricare una risorsa esterna**:

È possibile caricare fino a sei immagini statiche esterne alla raccolta [!DNL Content] da Microsoft OneDrive o Dropbox.

1. Da [!DNL Activate], fai clic su **[!UICONTROL Nuovo]** nel riquadro Meta. Viene visualizzata la finestra _Configurazione esperienza_.

1. Nella sezione _Media_, fai clic su **[!UICONTROL Seleziona]**. In un menu a discesa vengono visualizzate le opzioni per _Seleziona dal contenuto_ o _Carica_.

1. Fai clic su **[!UICONTROL Carica]**. Viene visualizzata la finestra _Aggiungi proporzioni_.

1. Seleziona le immagini nelle proporzioni supportate trascinando i file immagine nell’area di caricamento dell’immagine. In alternativa, puoi cercare le risorse nel dispositivo.

1. (Facoltativo) Per caricare le risorse dal dispositivo, fai clic su **[!UICONTROL Sfoglia]**, quindi seleziona _Sfoglia file_ o _Sfoglia cartelle_ per identificare le risorse da caricare.

1. Nell&#39;area _Aggiungi dettagli_, aggiungi dettagli informativi alle risorse caricate per facilitare la ricerca e il filtraggio in _[!DNL Content]_. Questi dettagli vengono salvati come metadati.

1. Dopo aver caricato le risorse e assegnato i dettagli, fai clic su **[!UICONTROL Aggiungi Assets]** in basso a destra.

### Aggiungi testo annuncio

Utilizza la sezione _Testo_ della pagina _Attiva Meta ad_ per aggiungere testo convincente e aderente al brand ai campi di testo richiesti. Il testo include il testo principale (corpo) per l’annuncio e il testo call-to-action. Impossibile modificare i campi _Testo principale_, _Titoli_ e _Descrizione_. Puoi modificare i campi _Call-to-action_, _Collegamento di visualizzazione_ e _URL sito Web_.

| Campo | Obbligatorio | Limite di caratteri (max) |
|-----------------|---------------------------|---------------------------------|
| Nome annuncio | sì | 500 |
| Testo principale | sì | 500 |
| Titolo | sì | 255 |
| Descrizione | no | 125 |
| Call to action | sì | solo opzioni del menu a discesa |
| Visualizza URL | no | 1000 |
| URL sito Web | sì | 1000 |
| Immagine | almeno uno richiesto |                                 |

GenStudio for Performance Marketing richiede _il testo principale_ e _il titolo_, non Meta.

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

Dopo aver assemblato o selezionato la tua esperienza, fai clic su **[!UICONTROL Avanti]** per confermare la configurazione di Meta.

## Passaggio 4: confermare la configurazione dell&#39;account Meta

Dopo aver preparato le esperienze pubblicitarie, devi confermare le informazioni sull’account Meta. La visualizzazione _Impostazione annuncio Meta_ è compilata con opzioni derivate dagli account Meta configurati.

| Dettaglio | Descrizione |
|------------|-------------|
| Account | Account Meta connessi a GenStudio for Performance Marketing |
| Pagina Facebook | Pagina Facebook in cui viene pubblicata l’esperienza |
| Account Instagram | Account Instagram connessi a GenStudio for Performance Marketing |
| Campagne | Campagne Meta a cui appartiene l’esperienza annuncio |
| Set di annunci | Set di annunci Meta a cui appartiene l’esperienza di annuncio attivato. Le impostazioni determinano il posizionamento finale dell’annuncio. |

### Creare un nuovo set di annunci

Puoi creare un nuovo set di annunci durante la configurazione della piattaforma clonando un set di annunci esistente durante la configurazione della piattaforma. I metadati definiscono la tempistica, i dettagli del canale e il pubblico per un annuncio specifico. Una Meta campaign può contenere più set di annunci, ma un set di annunci è associato esclusivamente a una campagna.

**Per creare un nuovo set di annunci**:

1. Seleziona una campagna dal menu a discesa _Campagne Meta_.

   La campagna selezionata determina i set di annunci disponibili come opzioni nel menu a discesa _Set di annunci_.

1. Fare clic su **[!UICONTROL + Crea nuovo set di annunci]**.

   Viene aperto il popup _Crea nuovo set di annunci_, che identifica la campagna Meta in cui viene creato il nuovo set di annunci.

1. Selezionare il set di annunci da clonare dal menu a discesa _Usa configurazione da_.

   GenStudio for Performance Marketing assegna un nome predefinito per il set di annunci aggiungendo `- Copy` al nome del set di annunci selezionato.

1. (Facoltativo ma consigliato) Immetti un nome di annuncio univoco nel campo **[!UICONTROL Nuovo nome set di annunci]** per sostituire il valore predefinito.

1. Fare clic su **[!UICONTROL Crea set di annunci]**.

   Si è tornati alla visualizzazione _Configurazione piattaforma_, in cui il nuovo set di annunci è preselezionato. Viene visualizzato un messaggio di successo che include un collegamento al set di annunci in Meta Ads Manager. Questo set di annunci è disponibile per le attivazioni future.

>[!NOTE]
>
>Se il set di annunci è stato creato correttamente ma non è stato possibile salvarlo, il set di annunci viene salvato in Meta Ads Manager con il nome predefinito (_nome del set di annunci originale - Copia_).

### ID tracciamento

Gli ID di tracciamento (nome annuncio) forniscono un meccanismo per raccogliere metriche collegate alle prestazioni dell’esperienza. Immetti il nome dell’annuncio in questo campo.

Fai clic su **[!UICONTROL Avanti]** in alto a destra per visualizzare l&#39;anteprima della tua esperienza pubblicitaria e finalizzare l&#39;attivazione.

## Passaggio 5: visualizzare l’anteprima e attivare l’annuncio

Nella pagina _Revisione_ viene visualizzata l&#39;esperienza pubblicitaria assemblata nella _Configurazione esperienza_ e viene fornita un&#39;ultima opportunità per visualizzare e modificare l&#39;esperienza. Fai clic su **[!UICONTROL Modifica sezione]** accanto all&#39;etichetta _Configurazione esperienza_ per apportare le modifiche. Puoi anche fare clic su **[!UICONTROL Indietro]** in alto a destra per tornare alla pagina _Configurazione esperienza_.

### Passaggio 6: completa attivazione dell’esperienza pubblicitaria

1. Fai clic su **[!UICONTROL Pubblica]**.

   L’esperienza pubblicitaria completa di Meta e i metadati associati vengono inviati direttamente nel set di annunci di Meta Ads Manager selezionato. Le esperienze vengono distribuite a Meta Ads Manager in stato inattivo. Da Meta Ads Manager, puoi gestire i passaggi finali della distribuzione dell’esperienza pubblicitaria e della campagna Meta.

1. [Accedi a Meta Ads Manager](https://adsmanager.facebook.com/) per rivedere la tua esperienza pubblicitaria e finalizzare la pubblicazione su canali Meta specifici.
