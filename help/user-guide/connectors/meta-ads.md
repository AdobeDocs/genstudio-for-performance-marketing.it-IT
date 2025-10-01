---
title: Connetti a Meta Ads
description: Connetti un account Meta Ads per attivare e monitorare annunci e contenuti multimediali con Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Admin, Data Engineer
recommendations: noDisplay
feature: Reporting and Insights
exl-id: 78110edf-947b-4e05-a3f1-de4b1eabda44
source-git-commit: fb5fe4885340639f8179c8de6944ac21bfe009ec
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 0%

---

# Connetti a Meta Ads

Questa pagina spiega come collegare e gestire l’account del profilo Meta Ads a GenStudio for Performance Marketing per gestire campagne, esportare contenuto e accedere ai dati pubblicitari per le campagne attive.

>[!BEGINSHADEBOX]

**Prerequisiti**:

- Accesso a Facebook/Meta che può accedere a tutti i servizi Meta

- _Controllo completo_ sugli account Meta Business Portfolio e Ad, inclusi:

   - Gestire le campagne
   - Visualizza prestazioni
   - Gestire i modelli dell’hub Creative
   - Analisi avanzata

- Disattiva eventuali blocchi popup nel browser

>[!ENDSHADEBOX]

## Connettere un account Meta ads

1. Fai clic su **[!UICONTROL Altro]** > **[!UICONTROL Impostazioni]**.

1. Nella sezione _Connettori dati_, fai clic su **[!UICONTROL Connetti]** nella scheda _Meta Ads_.

1. Accedi al tuo account Facebook.

   Potrebbe essere necessario rimuovere i blocchi popup e quindi utilizzare **[!UICONTROL Aggiorna]** per riprovare.

1. Segui le istruzioni di autenticazione di Facebook, verifica le informazioni sull&#39;account e fai clic su **[!UICONTROL Continua come ...]**

1. In _[!UICONTROL Accesso a Facebook per le aziende]_ (simbolo da Meta ad Adobe), effettuare le seguenti operazioni per concedere l&#39;accesso a GenStudio for Performance Marketing:

   - Seleziona uno o più profili aziendali di Meta e fai clic su **[!UICONTROL Continua]**
   - Seleziona una o più pagine Meta e fai clic su **[!UICONTROL Continua]**
   - Seleziona uno o più account Instagram e fai clic su **[!UICONTROL Continua]**
   - Rivedi le selezioni e fai clic su **[!UICONTROL Salva]**

     ![Rivedi selezioni](/help/assets/meta/meta-review-selections.png "Rivedi selezioni"){width="400" zoomable="yes"}

1. Dopo aver ricevuto la verifica della connessione dell&#39;account, fare clic su **[!UICONTROL Ottieni]**.

   Questo passaggio garantisce a GenStudio for Performance Marketing l’accesso a tutti gli annunci, i metadati e le metriche per prestazioni ottimali.

1. In _[!UICONTROL Meta Ads]_, selezionare uno o più account da includere in [!DNL Insights] e fare clic su **[!UICONTROL Seleziona]**.

1. Dopo aver ricevuto la conferma della connessione a _Platform_, fai clic su **[!UICONTROL Visualizza account]**.

   Nella visualizzazione _[!UICONTROL Account Meta Ads]_ sono elencati `Account name`, `Added by`, `Date added` e `Status`.

   ![Elenco account Meta](/help/assets/meta/meta-accounts-list.png "Elenco degli account Meta connessi"){zoomable="yes"}

Utilizza **[!UICONTROL Aggiungi account]** per aggiungere altri account all&#39;elenco. Il flusso di autorizzazione può variare leggermente quando si aggiungono account collegati allo stesso profilo aziendale di Meta. Durante il processo di connessione vengono selezionati solo i nuovi account Meta Ads.

## Disconnessione e risoluzione dei problemi relativi a un’integrazione di Meta Ads

A volte un’istanza di GenStudio for Performance Marketing è connessa a un account Meta Ads in modo errato. Le impostazioni comuni che possono causare problemi includono:

- Un account Instagram viene selezionato senza selezionare la pagina Facebook associata
- Autorizzazioni revocate per un utente che ha eseguito la connessione iniziale

In queste situazioni, è meglio riconnettere l’account Meta Ad all’istanza GenStudio for Performance Marketing. Innanzitutto, l’utente deve rimuovere l’integrazione dell’app direttamente dal proprio Meta Business Manager, creando una lavagna per il ripristino delle autorizzazioni. A tal fine è necessario disporre dell&#39;accesso amministratore a Meta Business Manager.

Questi passaggi cancellano le autorizzazioni memorizzate nella cache e reimpostano il flusso di integrazione:

1. Accedere a [Meta Business Manager](https://business.facebook.com) visitando il sito Web di Facebook.
1. Accedi con il tuo account. L&#39;account deve avere accesso come amministratore a Business Manager.
1. Fai clic sull&#39;icona **[!UICONTROL Impostazioni]** in basso a sinistra per passare alle impostazioni di Business Portfolio.
1. Nel menu a sinistra, fai clic su **[!UICONTROL Integrazioni]**.
1. Selezionare **[!UICONTROL App collegate]**. Vedrai Adobe GenStudio nell’elenco delle app collegate.
   ![App collegate a Meta Business Manager](./meta-connected-apps.png "Riquadro App collegate a Meta Business Manager")
1. Fai clic sul nome dell’app.
1. Fai clic su **[!UICONTROL Rimuovi]**.
1. Quando richiesto, confermare la rimozione.

Ora puoi riconnettere i tuoi account Meta, i profili Instagram e le pagine Facebook.
