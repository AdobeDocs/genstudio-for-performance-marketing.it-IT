---
title: Attivare un annuncio al Trade Desk
description: Scopri come attivare un’esperienza di visualizzazione e annuncio statica al Trade Desk.
feature: Ad Activation
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
subfeature_v2:
  - id: d87258a7-722c-4afd-b632-adddc447c7aa
    internal-label: Ad activation
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
    internal-label: Experiences
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%
---
# Attivare un annuncio al Trade Desk

Adobe GenStudio for Performance Marketing supporta l’attivazione di esperienze pubblicitarie presso il Trade Desk.

**Formati supportati**: visualizzazione statica (solo per risorsa singola).

L&#39;attivazione di un annuncio al Trade Desk segue [gli stessi passaggi generali](create-activation.md) richiesti per l&#39;attivazione ad altri canali di annunci a pagamento, con una differenza. Il Trade Desk è un servizio aziendale gestito, non una piattaforma pubblicitaria self-service, pertanto l’accesso all’account funziona in modo diverso rispetto ad altri canali. Questa pagina descrive tali differenze, insieme ai prerequisiti e ai campi di configurazione specifici per il Trade Desk.

I system manager e gli editor di GenStudio possono attivare le esperienze pubblicitarie.

## Prerequisiti

* Un account Trade Desk esistente. Configurarlo direttamente con il Trade Desk prima di collegarlo a GenStudio for Performance Marketing.
* Accesso API abilitato dal team dell’account del Trade Desk. Per Trade Desk, il team del tuo account abilita questo accesso per tuo conto utilizzando un token API, anziché l’accesso OAuth utilizzato da altri canali di annunci a pagamento.
* L’inserzionista, la sede e le autorizzazioni corretti abilitati da The Trade Desk per l’integrazione con GenStudio for Performance Marketing.
* Uno o più token API dal team dell’account Trade Desk, con autorizzazioni per pubblicare contenuti creativi sull’account dell’inserzionista di destinazione.
* Campagna di destinazione già esistente nel Trade Desk. GenStudio for Performance Marketing attiva gli annunci nella campagna esistente.

## Collegare l&#39;account del Trade Desk

Prima che la tua organizzazione possa attivare le esperienze, collabora con il team dell’account di Trade Desk per abilitare l’accesso API, quindi un manager di sistema di GenStudio connette l’account a GenStudio for Performance Marketing:

1. Contatta il team dell’account del Trade Desk e richiedi l’accesso per pubblicare i contenuti creativi di GenStudio for Performance Marketing nell’account del Trade Desk. Conferma l’ID inserzionista, la sede o i dettagli del partner da utilizzare per l’attivazione.
1. Ottieni il token API o le credenziali dal team dell’account Trade Desk e conferma che il token supporti le autorizzazioni di pubblicazione creativa per l’account dell’inserzionista di destinazione.
1. In GenStudio for Performance Marketing, vai a **[!UICONTROL Impostazioni]** > **[!UICONTROL Canali]**, quindi fai clic su **[!UICONTROL Connetti]** nella sezione **[!UICONTROL The Trade Desk]**. Immetti il nome account, l’ID inserzionista e il token o le credenziali API, quindi salva la connessione.

Se la connessione non riesce, verifica con il team dell’account The Trade Desk che l’accesso API sia stato abilitato e che il token disponga delle corrette autorizzazioni per inserzionista e postazione.

## Campi di impostazione del Trade Desk

Le risorse approvate sono bloccate e non possono essere modificate durante l&#39;attivazione poiché sono già state sottoposte a revisione e approvazione in [!DNL Content]. Puoi modificare:

* **Campi di testo**: ID di tracciamento (utilizzato come nome creativo della piattaforma)
* **Campi di installazione piattaforma**: account, campagna

Al momento, l’attivazione a The Trade Desk supporta solo annunci di visualizzazione statici a risorsa singola.
