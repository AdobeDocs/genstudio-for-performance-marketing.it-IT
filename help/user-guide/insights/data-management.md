---
title: Gestione dei dati
description: Scopri come acquisire e memorizzare dati per approfondimenti in GenStudio for Performance Marketing.
feature: Insights
level: Experienced
role: Admin
last-substantial-update: 2025-1-7
source-git-commit: 5dbe645f2ccf033f515da22ffdcce86edcb9fb24
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 0%

---

# Gestione dei dati

GenStudio for Performance Marketing utilizza Adobe Experience Platform (AEP) per l&#39;acquisizione dei dati e l&#39;archiviazione delle metriche e dei metadati che alimentano [!DNL Insights]. AEP utilizza _schemi_ per definire le strutture di dati e _set di dati_ per l&#39;archiviazione e la gestione delle raccolte di dati.

## Connessioni dati

GenStudio for Performance Marketing utilizza Customer Journey Analytics (CJA) per aggregare più origini dati creando una connessione a uno o più set di dati AEP. CJA utilizza queste connessioni dati per creare visualizzazioni dati per analizzare le metriche con [!DNL Insights].

>[!BEGINSHADEBOX]

**Informazioni importanti sulle connessioni dati**

Se sei un [amministratore di Adobe](/help/user-guide/user-roles.md#adobe-system-administrator-vs-genstudio-system-manager), potresti disporre di diritti che consentono l&#39;accesso alla gestione sandbox di AEP e ai componenti del data lake che supportano GenStudio for Performance Marketing.

>[!WARNING]
>
>Il ripristino della sandbox di produzione in AEP elimina tutte le connessioni dati e impedisce il funzionamento di [!DNL Insights].

Presta attenzione e non eliminare le seguenti connessioni dati necessarie per il funzionamento affidabile di GenStudio for Performance Marketing:

- Set di dati AEP con prefisso `GS Insights`
- Schemi, classi e gruppi di campi AEP con prefisso `GS Insights`
- Gruppo di campi personalizzato `timestamp for metadata`
- Connessioni AEP: flussi di dati con prefisso `GS Insights`
- Connessioni AEP: account GS Insights

Consulta [Eliminare le implicazioni](https://experienceleague.adobe.com/en/docs/analytics-platform/using/technotes/deletion) nella guida _Customer Journey Analytics_ prima di eliminare qualsiasi componente dati in AEP.

>[!ENDSHADEBOX]

## Criteri di conservazione dei dati

GenStudio for Performance Marketing conserva i dati del canale per 13 mesi. Questo criterio di conservazione include i 6 mesi di dati acquisiti durante la connessione iniziale, garantendo analisi e rapporti completi sui dati storici.

Consulta [Connetti account annuncio canale](/help/user-guide/insights/connect-channel.md).
