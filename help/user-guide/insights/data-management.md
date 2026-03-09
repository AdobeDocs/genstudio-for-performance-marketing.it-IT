---
title: Gestione dati
description: Scopri come acquisire e archiviare dati per  [!DNL Insights]  in GenStudio for Performance Marketing.
feature: Reporting and Insights
level: Experienced
role: Admin, Developer
last-substantial-update: 2025-1-7
exl-id: a5ab44d6-75c0-405b-82ad-9c65f6094bd6
TQID: https://experienceleague.adobe.com/HM2e0Yq2uwTpKtK-z8gHs0hDFrsJS6koQBqoNoKJK0Y
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: e0aa398c-6185-4e77-8cf7-2561c578c181
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: d3cdead0-685a-4489-9250-4bb709942f66
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 249
ht-degree: 0%

---

# Gestione dei dati

GenStudio for Performance Marketing utilizza Adobe Experience Platform (AEP) per l&#39;acquisizione dei dati e l&#39;archiviazione delle metriche e dei metadati che alimentano [!DNL Insights]. AEP utilizza _schemi_ per definire le strutture di dati e _set di dati_ per archiviare e gestire le raccolte di dati.

## Connessioni dati

GenStudio for Performance Marketing utilizza Customer Journey Analytics (CJA) per aggregare più origini dati creando una connessione a uno o più set di dati di AEP. CJA utilizza queste connessioni dati per creare visualizzazioni dati per l&#39;analisi delle metriche con [!DNL Insights].

>[!BEGINSHADEBOX]

**Informazioni importanti sulle connessioni dati**

Se sei un [amministratore di sistema di Adobe](/help/user-guide/user-roles.md#adobe-system-administrator-vs-genstudio-system-manager), potresti disporre di diritti che consentono l&#39;accesso alla gestione sandbox di AEP e ai componenti del data lake che supportano GenStudio for Performance Marketing.

>[!WARNING]
>
>Se si ripristina la sandbox di produzione in AEP, tutte le connessioni dati vengono eliminate e [!DNL Insights] non funziona più.

Presta attenzione e non eliminare le seguenti connessioni dati necessarie per il funzionamento affidabile di GenStudio for Performance Marketing:

- Set di dati di AEP con prefisso `GS Insights`
- Schemi, classi e gruppi di campi di AEP con prefisso `GS Insights`
- Gruppo di campi personalizzato `timestamp for metadata`
- Connessioni AEP: flussi di dati con prefisso `GS Insights`
- Connessioni AEP: account GS Insights

Consulta [Eliminare le implicazioni](https://experienceleague.adobe.com/it/docs/analytics-platform/using/technotes/deletion) nella guida _Customer Journey Analytics_ prima di eliminare qualsiasi componente dati in AEP.

>[!ENDSHADEBOX]

## Criteri di conservazione dei dati

GenStudio for Performance Marketing conserva i dati del canale per 13 mesi. Questo criterio di conservazione include i 6 mesi di dati acquisiti durante la connessione iniziale, garantendo analisi e rapporti completi sui dati storici.

Consulta [Connetti account di paid media](/help/user-guide/connectors/connect-channel.md).
