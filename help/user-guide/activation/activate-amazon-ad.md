---
title: Attivare Amazon Ads
description: Scopri come attivare le esperienze Amazon Ads.
feature: Ad Activation
exl-id: 539cb43c-a9d8-4473-8a7d-e81967111741
TQID: https://experienceleague.adobe.com/4L4JHcYLSsoQ50QbCW7Mof52h5jpz3z8n0UL8CaqLA8
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
subfeature_v2:
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
    internal-label: Experiences
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%
---
# Attivare Amazon Ads

Adobe GenStudio for Performance Marketing supporta l’attivazione delle esperienze pubblicitarie in Amazon Ads.

**Formati supportati**: visualizzazione statica.

L&#39;attivazione di un&#39;esperienza Amazon Ads segue gli [stessi passaggi generali](create-activation.md) richiesti per l&#39;attivazione ad altri canali di annunci a pagamento. Questa pagina descrive i prerequisiti e i campi di configurazione specifici per Amazon Ads. Dopo aver attivato un’esperienza in GenStudio for Performance Marketing, utilizza Amazon Ads per rivederla e avviare l’annuncio.

I system manager e gli editor di GenStudio possono attivare le esperienze pubblicitarie.

## Prerequisiti

* Accedi all’account Amazon Ads di destinazione.
* Accesso amministratore a tale account, per leggere e scrivere in Amazon Ads.

Amazon Ads organizza campagne e annunci all’interno di account diversi e ogni account include una libreria creativa. L’account di destinazione deve già esistere in Amazon Ads; GenStudio for Performance Marketing pubblica esperienze pubblicitarie nella libreria creativa dell’account, ma non crea account.

## Connetti il tuo account Amazon Ads

Prima che la tua organizzazione possa pubblicare le risorse in una libreria creativa, un manager di sistema GenStudio deve collegare il tuo account Amazon Ads a GenStudio for Performance Marketing. Per leggere e scrivere in Amazon Ads, devi disporre dell’accesso di amministratore a tale account. Consulta [Connessione di account multimediali a pagamento](/help/user-guide/connectors/connect-channel.md).

Al termine della sincronizzazione, puoi visualizzare gli account aggiunti.

## Campi di configurazione di Amazon Ads

Le risorse approvate sono bloccate e non possono essere modificate durante l&#39;attivazione poiché sono già state sottoposte a revisione e approvazione in [!DNL Content]. Puoi modificare:

* **Campi di testo**: ID di tracciamento (utilizzato come nome creativo della piattaforma)
* **Campi installazione piattaforma**: Account

Al termine dell’attivazione, l’esperienza creativa viene consegnata alla libreria creativa dell’account selezionato in Amazon Ads.
