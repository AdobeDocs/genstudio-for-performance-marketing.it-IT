---
title: Integrazione di Workfront Proof con revisione e approvazioni
description: Integrazione di Workfront Proof con Adobe GenStudio for Performance Marketing.
feature: Content Review, Content Management
source-git-commit: f8508ee9440714137141e933cfe0f5761a510c7a
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 0%

---

# Integrazione di Workfront Proof con GenStudio for Performance Marketing

L&#39;integrazione con Workfront Proof migliora il ciclo di vita di revisione e approvazione di GenStudio for Performance Marketing con funzioni avanzate, tra cui modelli di approvazione, flussi di lavoro in più fasi e la possibilità di [confrontare le versioni della bozza](https://experienceleague.adobe.com/it/docs/workfront/using/workfront-proof/work-with-proofs-in-wf-proof/review-proofs-web-proofing-viewer/compare-proofs). Questo controllo delle versioni strutturato garantisce trasparenza, responsabilità e collaborazione semplificata durante l&#39;intero ciclo di revisione dei contenuti.

>[!BEGINSHADEBOX]

**Prerequisiti**:

Installa l&#39;estensione [Adobe Workfront Web Viewer](https://experienceleague.adobe.com/it/docs/workfront/using/review-and-approve-work/proofing/review-proofs-in-workfront/review-a-proof/review-proof-in-web-viewer-extension)

>[!ENDSHADEBOX]

[!DNL Proofing Viewer] di Workfront Proof è un&#39;area di lavoro avanzata per la visualizzazione, il commento e il confronto delle bozze. Da [!DNL Proofing Viewer], puoi

* Confrontare diverse versioni del contenuto
* Aggiungere commenti e disegnare markup in una bozza
* Approva la bozza

[!DNL Proofing Viewer] viene caricato quando si fa clic sull&#39;URL della bozza nell&#39;e-mail della richiesta di approvazione o nella notifica interna al prodotto. Viene aperta la visualizzazione [!DNL Proofing Viewer] _La mia nuova approvazione_. Da questa visualizzazione è possibile esaminare il contenuto e fornire commenti utilizzando gli strumenti di annotazione [!DNL Proofing Viewer] di base.

Per uscire da [!DNL Proofing Viewer], fare clic su **[!UICONTROL Torna a GenStudio]**.

## Genstudio per Performance Marketing e Workfront Proof: confronto delle funzioni

La tabella seguente confronta le funzioni standard di revisione e approvazione di GenStudio for Performance Marketing con le funzionalità più avanzate disponibili tramite l’integrazione di Workfront Proof.

| Funzionalità        | GenStudio for Performance Marketing                                                                 | Workfront Proof                                                                 |
|-------------------------------|------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|
| **Ciclo di vita bozza/bozza**        | Il contenuto della bozza scade al momento della pubblicazione. | Catene di approvazione in più fasi basate su ruoli con registri permanenti con marca temporale.<br> Tutte le versioni vengono mantenute indefinitamente. |
| **Commenti**                | I commenti vengono associati all&#39;ID bozza e vengono eliminati dopo la pubblicazione.                                           | I commenti e le annotazioni persistenti vengono conservati per scopi di audit e conformità.     |
| **Versioni**           | Le bozze vengono trattate come istanze univoche.<br>Nessun confronto affiancato.                                      | Controllo completo della versione con strumenti di confronto affiancati e sovrapposti.        |
| **Gestione dei progetti** | Gestione di base delle campagne. | Gestione completa del ciclo di vita delle campagne, compresi personalizzazione, modelli, reporting e audit dettagliati. |

### Licenze e ruoli utente

Le licenze identificano il set di diritti utente all’interno di un prodotto. Workfront Proof fornisce più tipi di licenza o ruoli utente rispetto a GenStudio for Performance Marketing. [Panoramica sui ruoli di bozza](https://experienceleague.adobe.com/it/docs/workfront/using/review-and-approve-work/proofing/proofing-overview/proof-roles) introduce i ruoli utente associati al flusso di lavoro di revisione e approvazione di Workfront Proof.

| Licenza GenStudio for Performance Marketing       | Licenza Workfront                 | Descrizione                                                                                                                                                      |
|---------------------------------------------------|-----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| GenStudio System Manager                          | Amministratore Workfront/utente avanzato | Accesso completo alle funzioni di GenStudio Performance Marketing, ad esempio gestione di marchi, utenti tipo e prodotti. Gestisce flussi di lavoro e impostazioni. Crea modelli di approvazione. |
| Creatore ed editor di contenuti (licenza per utenti esperti)   | Creatore bozza (licenza standard)  | Genera e invia bozze di contenuto. In Proofing Viewer (Visualizzatore di bozze), carica le risorse e avvia le bozze. Richiede una licenza Workfront Proof.                              |
| Revisore/Approvatore (licenza Collaborator)        | Revisore/Approvatore                 | Partecipa a revisioni in più fasi, aggiunge commenti e approva o rifiuta i contenuti.                                                                             |

Gli amministratori di sistema di Adobe gestiscono il provisioning degli utenti e le autorizzazioni per entrambi i prodotti in Adobe Admin Console.

>[!NOTE]
>
> Workfront Proof fornisce [ulteriori ruoli utente](https://experienceleague.adobe.com/it/docs/workfront/using/review-and-approve-work/proofing/proofing-overview/proof-roles). Non tutti i ruoli sono visibili all’interno di Performance Marketing. Tuttavia, il sistema rispetta qualsiasi ruolo impostato all&#39;interno di un modello di Workfront Proof.

### Bozze e bozze

Workfront [!DNL Proofing Viewer] estende il processo di revisione e approvazione di base di GenStudio for Performance Marketing con funzioni di revisione e approvazione più strutturate. Le bozze esaminate in questa integrazione sono limitate ai formati supportati da GenStudio for Performance Marketing.

### Controllo della versione

GenStudio for Performance Marketing non supporta i modelli di approvazione, ma Workfront Proof sì. Le funzionalità di controllo delle versioni di Proof migliorano notevolmente il processo di revisione e approvazione dei contenuti GenStudio. Ogni invio nel flusso di lavoro Bozza viene trattato come una versione distinta della bozza di contenuto o _bozza_. Le bozze vengono salvate automaticamente e possono essere confrontate una accanto all’altra con le iterazioni precedenti. Le parti interessate possono tenere traccia delle modifiche, fornire feedback precisi e mantenere l’allineamento durante l’intero ciclo di revisione. Proof conserva una cronologia completa di tutti i commenti, le decisioni e le versioni, supportando la fattibilità dell’audit e i requisiti di conformità. Ogni versione supporta anche flussi di lavoro di approvazione multifase basati sui ruoli, con ogni azione (approvazione, rifiuto o commento) chiaramente registrata e con marca temporale.

### Modelli di approvazione

I modelli di approvazione di Workfront Proof forniscono passaggi preformattati che possono semplificare il flusso di lavoro di approvazione delle bozze. Questi modelli includono revisori e approvatori selezionati, ruoli della bozza e scadenze, garantendo coerenza ed efficienza. I creatori di contenuti che avviano una revisione possono scegliere tra una serie di modelli predefiniti per i flussi di lavoro di approvazione monofase e multifase.

Ogni fase del modello di workflow identifica i revisori assegnati. Tutti gli aggiornamenti di stato e i commenti del flusso di lavoro di Workfront Proof sono visibili all’interno del Proofing Viewer (Visualizzatore di bozze), migliorando la trasparenza e la collaborazione.

I modelli di approvazione supportano le approvazioni in più fasi, che supportano il coordinamento delle revisioni da parte di diversi gruppi di parti interessate.

### Commenti

I revisori possono fare clic direttamente su specifiche aree della bozza per lasciare commenti precisi e contestuali. Tutti i commenti vengono contrassegnati con marca temporale e salvati come parte della cronologia delle versioni della bozza. La cronologia dei commenti non è disponibile in GenStudio for Performance Marketing.

È possibile [confrontare due versioni di una bozza](https://experienceleague.adobe.com/it/docs/workfront/using/workfront-proof/work-with-proofs-in-wf-proof/review-proofs-web-proofing-viewer/compare-proofs) per valutare i commenti e il contenuto della revisione.

## Notifiche e promemoria

I revisori e gli approvatori ricevono notifiche e-mail quando è disponibile una nuova bozza per la revisione o quando lo stato di una revisione in corso è cambiato.
[Notifiche e promemoria bozza](https://experienceleague.adobe.com/it/docs/workfront/using/workfront-proof/proof-notifications-and-reminders/proof-notifications-and-reminders/proof-notifications-and-reminders) includono un collegamento personalizzato alla bozza, dettagli sulla bozza e il relativo avanzamento nel processo di approvazione e informazioni sul controllo delle versioni.
