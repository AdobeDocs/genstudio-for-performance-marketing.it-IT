---
title: Attivare un annuncio LinkedIn
description: Scopri come attivare un’esperienza di annuncio LinkedIn.
feature: Ad Activation
exl-id: edc95319-36c3-4cbf-a5c0-865b49482b50
TQID: https://experienceleague.adobe.com/1mcxWePqYd8tYp3e1D2UTSeBHSvPj4WrqeSyiUCxD8c
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
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%
---
# Attivare un annuncio LinkedIn

Adobe GenStudio for Performance Marketing supporta l&#39;attivazione delle esperienze degli annunci LinkedIn in [Gestione campagne LinkedIn](https://business.linkedin.com/marketing-solutions).

**Formati supportati**: immagine singola, video singolo.

Puoi [creare un&#39;esperienza LinkedIn](/help/user-guide/create/create-linkedin.md) in GenStudio for Performance Marketing, quindi selezionarla per l&#39;attivazione.

L&#39;attivazione di un annuncio LinkedIn segue gli [stessi passaggi generali](create-activation.md) richiesti per l&#39;attivazione ad altri canali di annunci a pagamento. Questa pagina descrive i prerequisiti e i campi di configurazione specifici di LinkedIn. Dopo aver attivato un’esperienza LinkedIn in GenStudio for Performance Marketing, utilizza LinkedIn Campaign Manager per rivederla e avviare l’annuncio.

I system manager e gli editor di GenStudio possono attivare le esperienze pubblicitarie.

## Prerequisiti

* Un account LinkedIn Campaign Manager con autorizzazioni complete per gestire campagne e annunci. Questo account deve contenere campagne esistenti.
* Account degli annunci LinkedIn con autorizzazioni complete per creare annunci e pubblicare contenuti sulle pagine LinkedIn.

La campagna LinkedIn di destinazione e il set di annunci devono già esistere in LinkedIn Campaign Manager. GenStudio for Performance Marketing non crea campagne o set di annunci.

>[!NOTE]
>
>LinkedIn ha rinominato la propria gerarchia di campagne: ciò che LinkedIn Campaign Manager in precedenza chiamava **gruppo di campagne** è ora denominato **campagna** e ciò che in precedenza chiamava **campagna** è ora denominato **set di annunci**. I campi di installazione **[!UICONTROL LinkedIn campaign]** e **[!UICONTROL LinkedIn ad set]** in [!DNL Activate] utilizzano la terminologia corrente.

GenStudio for Performance Marketing attualmente supporta gli annunci LinkedIn per immagine singola e video singolo, ciascuno dei quali presenta una sola immagine o un solo video per post. Se l&#39;esperienza include più proporzioni, [!DNL Activate] genera una riga distinta per ogni proporzione nella tabella di attivazione in modo che ogni riga possa essere eseguita come proprio annuncio; eliminare le righe non necessarie.

## Collegare gli account LinkedIn

Prima che la tua organizzazione possa attivare le esperienze, un manager di sistema o un editor di GenStudio deve collegare gli account degli annunci LinkedIn a GenStudio for Performance Marketing. Per connettersi correttamente, è necessario disporre dell&#39;accesso completo da parte dell&#39;amministratore sia all&#39;account dell&#39;annuncio che alla pagina del profilo LinkedIn. Devi connettere un account annuncio in **[!UICONTROL Impostazioni]** una sola volta. Dopodiché, sarà disponibile per chiunque possa accedere a tale istanza.

Questa connessione consente il flusso dei dati tra GenStudio for Performance Marketing e LinkedIn, abilitando il processo di attivazione.

Al termine della sincronizzazione, puoi visualizzare gli account aggiunti. La sincronizzazione di grandi quantità di dati richiede più tempo.

## Campi di impostazione LinkedIn

Le risorse approvate, i titoli e il testo introduttivo sono bloccati e non possono essere modificati durante l&#39;attivazione, poiché sono già stati sottoposti a revisione e approvazione in [!DNL Content]. Puoi modificare:

* **Campi di testo**: descrizione, Call-to-action, URL di destinazione, parametri URL, ID di tracciamento (utilizzato come nome dell&#39;annuncio della piattaforma)
* **Campi installazione piattaforma**: account annuncio LinkedIn, campagna LinkedIn, set annunci LinkedIn
