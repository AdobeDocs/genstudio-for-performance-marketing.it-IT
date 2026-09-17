---
title: Gestione attivazioni
description: Scopri come gestire le esperienze attivate con Adobe GenStudio for Performance Marketing.
feature: Ad Activation
exl-id: 7cf340d4-37ab-4906-9aad-088a26db0818
TQID: https://experienceleague.adobe.com/ird0IiW8L5Axjj2FmEjlUcD1sPaNCNfxj9XNqGfQWiI
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 1%
---
# Gestire le attivazioni

Le tabelle di attivazione vengono visualizzate nella pagina di destinazione [!DNL Activate]. Ogni tabella elenca i propri annunci e il relativo stato:

| Stato | Significato |
|---|---|
| [!UICONTROL Richiede Attenzione] | Almeno un annuncio nella tabella di attivazione contiene un campo mancante o non valido, ad esempio un call to action non compatibile o un ID di tracciamento duplicato. |
| [!UICONTROL Pronto ad attivare] | Tutti gli annunci nella tabella di attivazione superano la convalida e sono pronti per la pubblicazione. |
| [!UICONTROL In Attesa] | L’intera tabella di attivazione è stata inviata ed è in fase di elaborazione da parte della piattaforma di destinazione. |
| [!UICONTROL Pubblicato] | L&#39;intera tabella di attivazione è stata pubblicata correttamente. |
| [!UICONTROL Non riuscito] | La piattaforma di destinazione ha rifiutato almeno uno degli annunci nella tabella. Passa il puntatore del mouse sulla descrizione dello stato per visualizzare il messaggio di errore della piattaforma. |

Puoi riprovare automaticamente le attivazioni non riuscite facendo clic su **[!UICONTROL Riprova]** in alto a destra.

Le righe pubblicate non possono essere inviate nuovamente e includono un collegamento profondo all’annuncio nel gestore di annunci nativo della piattaforma di destinazione, in modo da potervi passare direttamente per rivederlo o avviarlo.

## Visualizzazione dettagli

Fai clic su una riga di annuncio per aprire una visualizzazione mirata dei relativi dettagli di attivazione. La visualizzazione dei dettagli di sola lettura acquisisce i dettagli di definizione di un annuncio attivato, comprese le attivazioni non riuscite, con informazioni derivate sia da GenStudio for Performance Marketing che dalla piattaforma di destinazione:

* **Data e ora di pubblicazione**: ora e data di pubblicazione dalla piattaforma di destinazione
* **ID annuncio**: ID assegnato dalla piattaforma di destinazione e utilizzato per il tracciamento, con un collegamento diretto all&#39;annuncio pubblicato nel gestore di annunci nativo della piattaforma
* **Dettagli annuncio**: le risorse, la copia e i metadati approvati utilizzati per l&#39;annuncio
* **Configurazione piattaforma**: i campi account, campagna e altre impostazioni piattaforma utilizzati per attivare l&#39;annuncio

La visualizzazione dei dettagli di un&#39;attivazione non riuscita include il motivo dell&#39;errore.
