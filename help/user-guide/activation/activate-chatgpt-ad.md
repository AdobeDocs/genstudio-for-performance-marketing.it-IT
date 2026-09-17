---
title: Attivare un annuncio ChatGPT
description: Scopri come attivare un’esperienza annuncio ChatGPT.
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
source-wordcount: '272'
ht-degree: 0%
---
# Attivare un annuncio ChatGPT

Adobe GenStudio for Performance Marketing supporta l’attivazione delle esperienze pubblicitarie ChatGPT.

**Formati supportati**: Schede chat.

Puoi [creare un&#39;esperienza ChatGPT](/help/user-guide/create/create-chatgpt-ad.md) in GenStudio for Performance Marketing, quindi selezionarla per l&#39;attivazione.

L&#39;attivazione di un annuncio ChatGPT segue gli [stessi passaggi generali](create-activation.md) richiesti per l&#39;attivazione ad altri canali di annunci a pagamento. Questa pagina descrive i prerequisiti e i campi di configurazione specifici per ChatGPT. Dopo aver attivato un’esperienza ChatGPT in GenStudio for Performance Marketing, utilizza OpenAI Ads Manager per eseguire i controlli finali e avviare l’annuncio.

I system manager e gli editor di GenStudio possono attivare le esperienze pubblicitarie.

## Prerequisiti

* Un account OpenAI Ads e una chiave API da tale account.
* La campagna ChatGPT di destinazione e il gruppo di annunci devono già esistere in OpenAI Ads Manager. GenStudio for Performance Marketing non crea nuove campagne o gruppi di annunci.

## Connetti il tuo account ChatGPT

Prima che la tua organizzazione possa attivare le esperienze, un manager di sistema di GenStudio deve collegare il tuo account OpenAI Ads a GenStudio for Performance Marketing:

1. In OpenAI Ads Manager, vai a **[!UICONTROL Impostazioni]** > **[!UICONTROL Chiavi API]** > **[!UICONTROL Crea nuova chiave]**.
1. In GenStudio for Performance Marketing, vai a **[!UICONTROL Altro]** > **[!UICONTROL Impostazioni]** > **[!UICONTROL ChatGPT]** > **[!UICONTROL Connetti]** > **[!UICONTROL Aggiungi account]**.
1. Immetti il nome dell&#39;account OpenAI Ads, incolla la chiave API, quindi fai clic su **[!UICONTROL Aggiungi account]**.

## Campi di configurazione di ChatGPT

Le risorse approvate, i titoli (Titolo) e la copia del corpo sono bloccati e non possono essere modificati durante l&#39;attivazione, poiché sono già stati sottoposti a revisione e approvazione in [!DNL Content]. Puoi modificare:

* **Campi di testo**: URL di destinazione, ID di tracciamento (utilizzato come nome dell&#39;annuncio della piattaforma)
* **Campi installazione piattaforma**: account OpenAI Ads, OpenAI Campaign, gruppo di annunci OpenAI

L&#39;URL di destinazione deve utilizzare un formato `https://` valido, ad esempio `https://www.example.com`.
