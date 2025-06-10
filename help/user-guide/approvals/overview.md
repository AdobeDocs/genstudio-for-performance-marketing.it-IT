---
title: Recensioni e approvazioni di Adobe GenStudio for Performance Marketing
description: Scopri il processo di revisione e approvazione di GenStudio for Performance Marketing.
level: Beginner
feature: Content Review, Content Management
exl-id: c83f47c0-e8ae-4c54-84b3-c50f67d6b3c2
source-git-commit: 7955796949c17f7cd877b115cba45c58cdd614a7
workflow-type: tm+mt
source-wordcount: '860'
ht-degree: 0%

---

# Recensioni e approvazioni di Adobe GenStudio for Performance Marketing

Il flusso di lavoro di revisione e approvazione assicura che tutte le parti interessate, dai team creativi agli esperti legali, possano rivedere e approvare in modo efficiente le risorse e le esperienze delle campagne, incluse le risorse di marchio generate dall’intelligenza artificiale.

>[!NOTE]
>
> Questa funzione è disponibile anche come integrazione [con Adobe Workfront Proof](/help/user-guide/approvals/proof-integration.md). Questa integrazione offre funzionalità di verifica nell’area di lavoro di GenStudio for Performance Marketing. Con l’integrazione di Workfront Proof, GenStudio for Performance Marketing ottiene un processo di revisione più strutturato, trasparente e collaborativo, che aiuta i team a passare dalla bozza alla versione finale con maggiore sicurezza e chiarezza.

## Vantaggi del flusso di lavoro di revisione e approvazione

* **Supporto per la creazione di contenuti di IA generativa e affidabile**. La creazione e l’implementazione di contenuti allineati al brand in un’organizzazione è un processo altamente iterativo. Le funzionalità di intelligenza artificiale generative di GenStudio for Performance Marketing supportano la creazione rapida di centinaia di varianti di risorse. Ogni revisore può richiedere più modifiche a una bozza di risorsa prima di approvarla. Maggiore è il numero di revisori potenziali prima che tutte le parti interessate concordino su una variante finale.

* **Supporto per integrità creativa**. Le approvazioni salvaguardano l’integrità creativa delle risorse del brand mantenendo i creatori di contenuti coinvolti nel processo di approvazione. Coinvolgendo i soggetti creativi (ad esempio, creatori di contenuti e direttori creativi) nel processo di revisione e approvazione, assicurati che il risultato finale sia allineato alla tua visione e alla tua identità del marchio.

* **Rispetto degli obiettivi e dei requisiti legali della campagna**. Il processo di approvazione consente di verificare che il contenuto supporti gli obiettivi della campagna. Garantisce che tutto il materiale di marketing sia conforme agli standard legali e normativi, riducendo al minimo i rischi e i potenziali problemi legali.

* **Integrazione con Adobe Workfront Proof**. Gli utenti possono accedere alle solide funzionalità di revisione e approvazione di Workfront Proof direttamente da GenStudio for Performance Marketing. I contenuti esaminati in GenStudio for Performance Marketing vengono sincronizzati con Workfront Proof e i commenti e lo stato di revisione vengono mantenuti. [Elementi di rilievo dell&#39;integrazione](/help/user-guide/approvals/proof-integration.md) identifica come Proof estende il flusso di lavoro di approvazione di GenStudio for Performance Marketing.

## Ciclo di vita di revisione e approvazione

Le fasi principali del flusso di lavoro di revisione e approvazione includono:

* [Richiedi revisione e approvazione del contenuto creato](/help/user-guide/approvals/request-review.md). GenStudio for Performance Marketing semplifica il processo di richiesta delle approvazioni e di gestione degli approvatori. I modelli di approvazione di Workfront Proof possono semplificare ulteriormente questa attività.

* [Rivedere e modificare il contenuto](/help/user-guide/approvals/review-and-edit.md). Le notifiche mantengono i creatori di contenuto nel loop per quanto riguarda le modifiche e le approvazioni richieste. La revisione del contenuto attiva un nuovo ciclo di approvazione automatico.

* [Approva contenuto](/help/user-guide/approvals/approve-content.md). Gli approvatori designati contrassegnano il contenuto come approvato o pronto per la pubblicazione.

* [Pubblica contenuto](/help/user-guide/approvals/publish-content.md). La pubblicazione di contenuti approvati in [!DNL Content] ne rende disponibile l&#39;utilizzo o l&#39;utilizzo da parte di altri utenti dell&#39;organizzazione.

## Informazioni sulle bozze di contenuto

_Le bozze_ sono versioni preliminari di risorse o esperienze che non hanno completato il processo di revisione e approvazione. Lo stato Bozza indica dove si trova la bozza nel processo di revisione e approvazione. Ogni bozza è identificata da un ID di bozza univoco. Questo ID è valido finché una bozza non viene approvata e pubblicata in [!DNL Content]. I commenti di revisione e le approvazioni per una bozza sono associati a questo singolo ID bozza. Non è disponibile il controllo delle versioni per le bozze di contenuto di GenStudio.

Quando una bozza completa il processo di revisione e approvazione e viene pubblicata in [!DNL Content], l&#39;ID della bozza scade. GenStudio for Performance Marketing non salva i commenti associati e lo stato di approvazione. L’URL della bozza non è più valido.

Lo stato Bozza acquisisce lo stato della bozza di contenuto durante il processo di revisione e approvazione. All’editor dei contenuti di GenStudio for Performance Marketing che ha creato la risorsa in revisione vengono notificate tutte le modifiche richieste alla bozza o alle approvazioni. Gli approvatori cambiano lo stato di bozza per indicare se una bozza necessita di ulteriore revisione o può essere approvata. Tutti gli approvatori designati devono approvare una risorsa o un’esperienza prima di poterla pubblicare.

Stati bozza disponibili:

**Notifica**: l&#39;editor di contenuto ha avviato il processo di revisione e approvazione notificando agli approvatori che una bozza è pronta per la revisione.
**Operazione necessaria**: indica che uno o più approvatori hanno richiesto modifiche alla bozza di contenuto. Impossibile salvare il contenuto in questo stato in [!DNL Content].
**Approvato**: tutti gli approvatori designati hanno approvato la risorsa o l&#39;esperienza. L&#39;editor dei contenuti può ora aggiungere metadati alla risorsa o all&#39;esperienza e salvarla in [!DNL Content].

>[!NOTE]
>
> Le bozze corrispondono a _bozze_ per gli utenti dell&#39;integrazione Workfront Proof. [Le bozze e le bozze](/help/user-guide/approvals/proof-integration.md#drafts-and-proofs) differiscono in termini di persistenza e controllo delle versioni.

## Ruoli di approvazione

_I revisori_ possono aggiungere commenti ma non possono approvare il contenuto. La partecipazione del revisore è utile ma non essenziale. _Gli approvatori_ devono approvare il contenuto prima che possa avanzare nel processo di approvazione. L’integrazione di Workfront Proof supporta una gamma più ampia di ruoli utente.

## Notifiche

Le notifiche interne al prodotto di GenStudio for Performance Marketing aggiornano in tempo reale gli approvatori e gli editor di contenuti in merito alle modifiche di stato delle risorse e `@mention` commenti. Le notifiche supportano una rapida iterazione attraverso più cicli di revisione, modifica e approvazione.

Gli editor di contenuti e gli approvatori possono registrarsi per ricevere queste notifiche in Slack. Vedi [Abbonati ai servizi in Experience Cloud](https://experienceleague.adobe.com/it/docs/core-services/interface/services/customer-attributes/subscription).

Le azioni intraprese dai partecipanti all’approvazione attivano le notifiche automatiche interne al prodotto e le notifiche e-mail. Quando avvii un processo di approvazione, gli approvatori designati ricevono sia le notifiche e-mail che quelle interne al prodotto. L&#39;utente viene tenuto costantemente aggiornato con notifiche interne ed e-mail ogni volta che un approvatore aggiunge `@mention` commenti o prende una decisione. Le notifiche includono collegamenti alla bozza di contenuto.

Se hai avviato il processo di revisione e approvazione per il contenuto, riceverai una notifica di tutte le approvazioni e dei commenti di revisione. Tuttavia, agli approvatori vengono notificati solo i commenti che li includono con `@mention`.
