---
title: Panoramica di Activate
description: Scopri come attivare i contenuti con le applicazioni Adobe CX Enterprise e di terze parti.
level: Beginner
feature: Ad Activation
exl-id: 365fe253-d189-467e-a723-f54cd74ff60b
TQID: https://experienceleague.adobe.com/-Nal0YqjTzKw4g2SM3IuMf0a13e87CWdTqBZPd0dBkU
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
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%
---
# Attivazione Adobe GenStudio for Performance Marketing

In GenStudio for Performance Marketing [!DNL Activate] è possibile preparare e inviare esperienze pubblicitarie ai canali di annunci a pagamento, ad esempio Meta o LinkedIn. _Activation_ accetta un&#39;esperienza di annuncio approvata e le relative risorse, applica la configurazione richiesta da un canale specifico, quindi la consegna direttamente a tale canale in uno stato inattivo e disattivato. Da lì, puoi fare una revisione finale nel gestore degli annunci del canale stesso prima che l’annuncio venga pubblicato.

[!DNL Activate] consegna la tua esperienza direttamente al canale, quindi non è necessario esportare i file o caricarli manualmente nel gestore degli annunci del canale.

Un system manager o editor di GenStudio deve collegare l’account dell’annuncio per ogni canale di annuncio a pagamento prima di poter attivare un’esperienza di annuncio su tale canale.

## Attiva funzionalità

Utilizza [!DNL Activate] per preparare esperienze pubblicitarie per i loro canali pubblicitari a pagamento target. [Attiva le esperienze in blocco](create-activation.md) su più canali di annunci a pagamento in un&#39;unica tabella di attivazione. Quindi [gestisci le tue attivazioni](manage-activations.md) per visualizzare lo stato e i dettagli di ogni esperienza attivata.

>[!VIDEO](https://video.tv.adobe.com/v/3503538?learn=on)

### Attiva esperienze approvate dal contenuto

Seleziona una o più esperienze approvate e pubblicate da [!DNL Content] oppure inizia dalla pagina di destinazione [!DNL Activate]. A differenza delle versioni precedenti di [!DNL Activate], una singola tabella di attivazione può includere esperienze per più canali di annunci a pagamento contemporaneamente, organizzati per formato di annunci e canale.

>[!NOTE]
>
>[!DNL Content] chiama una destinazione come Meta o LinkedIn in un **canale**. [!DNL Activate] chiama la stessa destinazione come **piattaforma** (ad esempio, in **[!UICONTROL Configurazione piattaforma]**). I due termini si riferiscono alla stessa cosa.

### Configurare i dettagli di installazione di annunci e piattaforme

Ogni riga nella tabella di attivazione rappresenta un annuncio. Le risorse creative, i titoli e la copia del corpo approvati sono bloccati perché sono già stati sottoposti a revisione e approvazione. Puoi modificare i campi rimanenti, ad esempio il testo di call-to-action, l’URL di destinazione e i dettagli di configurazione della piattaforma, come l’account dell’annuncio, la campagna e il set di annunci. Modificare i campi di una riga alla volta oppure selezionare più righe per modificare i campi condivisi in blocco.

### Rivedere e pubblicare le esperienze sui loro canali pubblicitari

Verificare che ogni riga mostri [!UICONTROL Pronto per l&#39;attivazione]. [!DNL Activate] flag mancanti o non validi, chiamate all&#39;azione non compatibili e ID di tracciamento duplicati come [!UICONTROL Richiede attenzione]. Quando ogni riga è pronta, fai clic su **[!UICONTROL Invia a Platform]** per pubblicare tutti gli annunci nella tabella. [!DNL Activate] segnala lo stato di ogni annuncio quasi in tempo reale e gli annunci pubblicati correttamente includono un collegamento profondo all&#39;annuncio nel gestore di annunci nativo della piattaforma di destinazione. Gli annunci non riusciti restituiscono un messaggio di errore e possono essere ritentati.
