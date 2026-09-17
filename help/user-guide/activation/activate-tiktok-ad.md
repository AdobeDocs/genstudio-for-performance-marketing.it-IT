---
title: Attivare un annuncio TikTok
description: Scopri come attivare un’esperienza di annuncio video in-feed di TikTok.
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
source-wordcount: '294'
ht-degree: 1%
---
# Attivare un annuncio TikTok

Adobe GenStudio for Performance Marketing supporta l’attivazione delle esperienze pubblicitarie TikTok.

**Formati supportati**: Annunci video in-feed.

Puoi [creare un&#39;esperienza TikTok](/help/user-guide/create/tiktok-experiences.md) in GenStudio for Performance Marketing, quindi selezionarla per l&#39;attivazione.

L&#39;attivazione di un annuncio TikTok segue gli [stessi passaggi generali](create-activation.md) richiesti per l&#39;attivazione ad altri canali di annunci a pagamento. Questa pagina descrive i prerequisiti e i campi di configurazione specifici per TikTok. Dopo aver attivato un’esperienza TikTok in GenStudio for Performance Marketing, utilizza TikTok Ads Manager per eseguire i controlli finali e avviare l’annuncio.

I system manager e gli editor di GenStudio possono attivare le esperienze pubblicitarie.

## Prerequisiti

* Un account TikTok Ads con accesso come operatore o amministratore.
* Almeno un account TikTok Ad abilitato per l&#39;uso, connesso da un gestore o editor di sistema GenStudio.
* La campagna TikTok di destinazione deve esistere già in TikTok Ads Manager. TikTok Ads Manager, non GenStudio for Performance Marketing, definisce il budget, l’offerta, l’ottimizzazione e il targeting del gruppo di annunci.

## Connetti il tuo account TikTok

Prima che la tua organizzazione possa attivare le esperienze, un manager di sistema di GenStudio deve collegare il tuo account TikTok Ads a GenStudio for Performance Marketing:

1. Vai a **[!UICONTROL Impostazioni]** > **[!UICONTROL TikTok]** > **[!UICONTROL Connetti]**.
1. Accedi all’account TikTok Ads Manager nella finestra che si apre e completa l’accesso OAuth. Il tuo account deve avere accesso come operatore o amministratore all’account dell’annuncio.

Al termine della connessione, verifica che almeno un account TikTok Ad sia abilitato per l’uso.

## Campi di configurazione TikTok

Le risorse approvate e il testo principale sono bloccati e non possono essere modificati durante l&#39;attivazione, poiché sono già stati sottoposti a revisione e approvazione in [!DNL Content]. Puoi modificare:

* **Campi di testo**: Call-to-action, URL di destinazione, ID di tracciamento (utilizzato come nome dell&#39;annuncio della piattaforma)
* **Campi installazione piattaforma**: account TikTok Ads, Campaign, gruppo di annunci
