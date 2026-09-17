---
title: Attivare un annuncio di Google Campaign Manager 360
description: Scopri come attivare un’esperienza Google Campaign Manager 360.
feature: Ad Activation
exl-id: e4ee4e04-8dd0-4e05-a0f7-0ddca2fbb6be
TQID: https://experienceleague.adobe.com/pQbT2OC7-jK33HhJWgTBBtJrmEvr48mGkl8v-fTkOLQ
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
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%
---
# Attivare un annuncio di Google Campaign Manager 360

Adobe GenStudio for Performance Marketing supporta l’attivazione delle esperienze pubblicitarie in Google Campaign Manager 360.

**Formati supportati**: visualizzazione statica, visualizzazione video, visualizzazione ZIP HTML5.

L&#39;attivazione di un annuncio di Google Campaign Manager 360 segue gli [stessi passaggi generali](create-activation.md) richiesti per l&#39;attivazione ad altri canali di annunci a pagamento. Questa pagina descrive i prerequisiti e i campi di configurazione specifici per Google Campaign Manager 360. Dopo aver attivato un’esperienza in GenStudio for Performance Marketing, utilizza Google Campaign Manager 360 per rivederla e avviare l’annuncio.

I system manager e gli editor di GenStudio possono attivare le esperienze pubblicitarie.

## Prerequisiti

* Un account Google Campaign Manager 360 con accesso all’inserzionista target.
* Accesso amministratore all’inserzionista, per leggere e scrivere in Campaign Manager 360.

Campaign Manager 360 organizza campagne e annunci all’interno di diversi inserzionisti e ogni inserzionista include una libreria creativa. L’inserzionista di destinazione deve esistere già in Campaign Manager 360; GenStudio for Performance Marketing pubblica esperienze pubblicitarie nella libreria creativa dell’inserzionista, ma non crea annunci.

## Collegare l’account Google Campaign Manager 360

Prima che la tua organizzazione possa pubblicare le risorse in una libreria creativa, un manager o editor di sistema di GenStudio deve collegare il tuo account Google Campaign Manager 360 a GenStudio for Performance Marketing. Per leggere e scrivere in Campaign Manager 360, è necessario disporre dell’accesso come amministratore all’inserzionista. Consulta [Connessione di account multimediali a pagamento](/help/user-guide/connectors/connect-channel.md).

Al termine della sincronizzazione, puoi visualizzare gli account aggiunti.

## Campi di configurazione di Google Campaign Manager 360

Le risorse approvate sono bloccate e non possono essere modificate durante l&#39;attivazione poiché sono già state sottoposte a revisione e approvazione in [!DNL Content]. Puoi modificare:

* **Campi di testo**: ID di tracciamento (utilizzato come nome creativo della piattaforma)
* **Campi di installazione piattaforma**: inserzionista

Al termine dell’attivazione, l’esperienza creativa viene consegnata alla libreria creativa dell’inserzionista selezionato in Google Campaign Manager 360.
