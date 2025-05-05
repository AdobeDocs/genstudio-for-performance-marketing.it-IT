---
title: Gestione dei dati
description: Scopri sull'assimilazione e l'archiviazione dei dati in [!DNL Insights] GenStudio for Performance Marketing.
feature: Reporting and Insights
level: Experienced
role: Admin, Data Architect
last-substantial-update: 2025-1-7
exl-id: a5ab44d6-75c0-405b-82ad-9c65f6094bd6
source-git-commit: 8e61fa5c08102c5dd9905e693d7f129105d9f633
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---

# Gestione dei dati

GenStudio for Performance Marketing utilizza Adobe Experience Platform (AEP) per l&#39;inserimento dei dati e l&#39;archiviazione delle metriche e dei metadati che alimentano [!DNL Insights]. AEP utilizza _schemi_ per definire le strutture dei dati e _i set di dati per l&#39;archiviazione e la gestione delle_ raccolte di dati.

## Connessioni dati

GenStudio for Performance Marketing utilizza Customer Journey Analytics (CJA) per aggregato più origini dati creando una connessione a uno o più set di dati AEP. CJA utilizza queste connessioni dati per creare visualizzazioni dati per l&#39;analisi delle metriche con [!DNL Insights].

>[!BEGINSHADEBOX]

**Informazioni importanti sulle connessioni dati**

Se sei un [amministratore](/help/user-guide/user-roles.md#adobe-system-administrator-vs-genstudio-system-manager) di sistema Adobe Systems, puoi disporre di adesioni che accesso consentono alla gestione sandbox AEP e ai componenti del data lake che supportano GenStudio per il Performance Marketing.

>[!WARNING]
>
>Il ripristino della sandbox di produzione in AEP elimina tutte le connessioni dati e causa [!DNL Insights] l&#39;interruzione del funzionamento.

Prestare attenzione e non eliminare le seguenti connessioni dati necessarie affinché GenStudio for Performance Marketing funzioni in modo affidabile:

- Set di dati AEP con prefisso `GS Insights`
- Schemi, classi e gruppi di campi AEP con prefisso `GS Insights`
- Gruppo di campi personalizzato `timestamp for metadata`
- Connessioni AEP: flussi di dati con prefisso `GS Insights`
- Connessioni AEP: GS Insights account

Consulta [Elimina implicazioni](https://experienceleague.adobe.com/it/docs/analytics-platform/using/technotes/deletion) nella _guida Customer Journey Analytics_ prima di eliminare qualsiasi componente dati in AEP.

>[!ENDSHADEBOX]

## Conservazione dei dati regola

GenStudio for Performance Marketing conserva i dati di canale per 13 mesi. Questo regola di conservazione include i 6 mesi di dati acquisiti durante la connessione iniziale, garantendo un&#39;analisi e un reporting completi dei dati storici.

Consulta [Connetti canale annuncio account](/help/user-guide/connectors/connect-channel.md).
