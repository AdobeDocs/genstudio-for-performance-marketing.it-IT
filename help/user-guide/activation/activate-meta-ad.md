---
title: Attivare un annuncio Meta
description: Scopri come attivare un’esperienza di annuncio Meta.
feature: Ad Activation
exl-id: 157df612-a774-422c-bca3-2fde9e9d1c88
TQID: https://experienceleague.adobe.com/hDR0ngNiGnCXCCOgNhVG8gX4kHGrNvfybPbuMLwYk7U
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
    internal-label: Guidelines
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
source-wordcount: '382'
ht-degree: 0%
---
# Attivare un annuncio Meta

Adobe GenStudio for Performance Marketing supporta l’attivazione delle esperienze pubblicitarie Meta su Instagram e Facebook.

**Formati supportati**: immagine, video, carosello.

[Crea un&#39;esperienza Meta](/help/user-guide/create/create-meta-ad.md) in GenStudio for Performance Marketing, quindi selezionala per l&#39;attivazione.

L&#39;attivazione di un annuncio Meta segue gli [stessi passaggi generali](create-activation.md) richiesti per l&#39;attivazione ad altri canali di annunci a pagamento. Questa pagina descrive i prerequisiti e i campi di configurazione specifici per Meta. Dopo aver attivato un&#39;esperienza Meta in GenStudio for Performance Marketing, utilizza [Meta Ads Manager](https://adsmanager.facebook.com/) per rivedere l&#39;esperienza e avviare l&#39;annuncio.

A differenza di altri canali, un annuncio Meta può includere più proporzioni all’interno di un singolo annuncio. Se l&#39;esperienza presenta più proporzioni, [!DNL Activate] genera comunque una sola riga per ogni proporzione, non una riga per ogni proporzione.

I system manager e gli editor di GenStudio possono attivare le esperienze pubblicitarie.

## Prerequisiti

Conferma che gli account degli annunci Meta connessi dispongano dell’autorizzazione completa per gestire gli annunci in questi componenti della piattaforma pubblicitaria Meta:

* Account Meta Ad
* Pagina Facebook
* Campagna Meta
* Set di annunci Meta
* Profilo Instagram (facoltativo)

La campagna Meta di destinazione e il set di annunci devono già esistere in Meta Ads Manager. Al momento GenStudio for Performance Marketing non crea campagne o set di annunci.

## Connetti i tuoi account Meta

Prima che la tua organizzazione possa attivare le esperienze, un manager di sistema di GenStudio deve collegare i tuoi account Meta a GenStudio for Performance Marketing. Questa connessione consente il flusso dei dati tra GenStudio for Performance Marketing e Meta, abilitando il processo di attivazione. Vedi [Connetti a Meta Ads](/help/user-guide/connectors/meta-ads.md).

Per selezionare un account Instagram, assicurati in Meta Business Manager che [l&#39;account Instagram che desideri utilizzare sia connesso allo stesso account annuncio](/help/user-guide/connectors/meta-ads.md#connect-an-instagram-account) selezionato durante l&#39;onboarding. Se manca questa connessione, l&#39;account Instagram potrebbe non essere visualizzato nel menu a discesa **[!UICONTROL Instagram profile]** durante l&#39;attivazione.

Al termine della sincronizzazione, puoi visualizzare gli account aggiunti. La sincronizzazione di grandi quantità di dati richiede più tempo.

## Campi di configurazione Meta

Le risorse approvate, i titoli e la copia del corpo sono bloccati e non possono essere modificati durante l&#39;attivazione, poiché sono già stati sottoposti a revisione e approvazione in [!DNL Content]. Puoi modificare:

* **Campi di testo**: descrizione, Call-to-action, URL di destinazione, parametri URL, ID di tracciamento (utilizzato come nome dell&#39;annuncio Meta)
* **Campi installazione piattaforma**: account annuncio, pagina Facebook, profilo Instagram, campagna Meta, set di annunci Meta
