---
title: Attivare un annuncio Innovid
description: Scopri come attivare un’esperienza Innovid.
feature: Ad Activation
exl-id: ebb2aa9e-8efb-45b0-9ba2-7b27b8888708
TQID: https://experienceleague.adobe.com/VTzk2CDlTqawM1ckdHPVzs2ES-y0Ui0mkOLnVD88bJk
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
    internal-label: Insights
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
    internal-label: Assets
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
    internal-label: Experiences
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%
---
# Attivare un annuncio Innovid

Adobe GenStudio for Performance Marketing supporta l’attivazione delle esperienze pubblicitarie in Innovid.

**Formati supportati**: visualizzazione statica, visualizzazione ZIP HTML5.

L&#39;attivazione di un&#39;esperienza Innovid segue gli [stessi passaggi generali](create-activation.md) richiesti per l&#39;attivazione ad altri canali di annunci a pagamento. Questa pagina descrive i prerequisiti e i campi di configurazione specifici per Innovid. Dopo aver attivato un’esperienza in GenStudio for Performance Marketing, utilizza Innovid per rivederla e avviare l’annuncio.

I system manager e gli editor di GenStudio possono attivare le esperienze pubblicitarie.

## Prerequisiti

* Accedi all’account Innovid di destinazione.
* Accesso amministratore a tale account, per leggere e scrivere su Innovid.

Innovid organizza campagne e annunci all’interno di account diversi e ogni account dispone di una libreria creativa. La libreria creativa di destinazione deve esistere già in Innovid; GenStudio for Performance Marketing pubblica esperienze pubblicitarie in tale libreria creativa, ma non crea account o librerie creative.

## Connetti il tuo account Innovid

Prima che la tua organizzazione possa pubblicare le risorse in una libreria creativa, un manager di sistema di GenStudio deve collegare il tuo account Innovid a GenStudio for Performance Marketing. Per leggere e scrivere su Innovid è necessario disporre dell’accesso come amministratore a tale account. Consulta [Connessione di account multimediali a pagamento](/help/user-guide/connectors/connect-channel.md).

Al termine della sincronizzazione, puoi visualizzare gli account aggiunti.

## Campi di configurazione Innovid

Le risorse approvate sono bloccate e non possono essere modificate durante l&#39;attivazione poiché sono già state sottoposte a revisione e approvazione in [!DNL Content]. Puoi modificare:

* **Campi di testo**: ID di tracciamento (utilizzato come nome creativo della piattaforma)
* **Campi installazione piattaforma**: account, libreria Creative, nome concetto

Al termine dell’attivazione, l’esperienza creativa viene consegnata alla libreria creativa selezionata in Innovid.
