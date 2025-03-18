---
title: Distribuire l’app
description: Distribuisci l’app, o il componente aggiuntivo, per GenStudio for Performance Marketing.
exl-id: 4935356b-08df-402c-b1a2-b89627afc188
source-git-commit: 8884f3438a0010119f578ca9a3b7158e2e01cfa3
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# Distribuire l’app

La distribuzione del componente aggiuntivo lo rende disponibile per l&#39;utilizzo da parte dell&#39;organizzazione e potenzialmente di altre organizzazioni.

La distribuzione privata limita la distribuzione del componente aggiuntivo all’organizzazione identificata dall’organizzazione IMS per la quale è stato sviluppato il componente aggiuntivo. La distribuzione pubblica rende il componente aggiuntivo disponibile come app in Adobe Exchange. Il flusso di lavoro di distribuzione dipende dal fatto che il componente aggiuntivo sia destinato alla distribuzione pubblica o privata.

In questo argomento viene illustrata la distribuzione privata. [Distribuzione pubblica](https://developer.adobe.com/app-builder/docs/guides/distribution/public/) nella documentazione per gli sviluppatori _App Builder_ descrive come rendere la tua app disponibile per qualsiasi organizzazione Adobe.

>[!BEGINSHADEBOX]

**Prerequisiti**:

Conferma di disporre delle seguenti autorizzazioni:

* Autorizzazioni per gli sviluppatori nell’organizzazione da cui invii l’app per l’approvazione

* Autorizzazioni di amministratore di sistema per approvare l’app

L&#39;app App Builder deve essere distribuita in un progetto App Builder.

>[!ENDSHADEBOX]

**Distribuire l&#39;app privatamente**:

La distribuzione privata rende l’app disponibile solo ai membri dell’organizzazione.

1. Da [Adobe Developer Console](https://developer.adobe.com/console/), selezionare l&#39;organizzazione, il progetto e l&#39;area di lavoro in cui è distribuita l&#39;app.

1. Seleziona **[!UICONTROL Approvazione]** dall&#39;area _Panoramica di Workspace_. Viene aperto il riquadro _Approvazione app_.

1. Nell&#39;area _Dettagli invio app_, aggiungi informazioni sul componente aggiuntivo. I dettagli includono il nome dell’app, la descrizione e l’e-mail di contatto.

1. Dopo aver completato tutti i campi, fare clic su **[!UICONTROL Invia]**.

1. Accedi a [Adobe Exchange](https://exchange.adobe.com/) utilizzando lo stesso Adobe ID utilizzato per accedere a Developer Console. Se non disponi delle autorizzazioni di amministratore di sistema per questa organizzazione, richiedi l’approvazione di un amministratore di sistema dell’organizzazione.

1. Seleziona **[!UICONTROL Gestisci]** > **[!UICONTROL Applicazioni App Builder]** per accedere a una richiesta di revisione dell&#39;app.

1. Dopo aver esaminato l&#39;app, seleziona **[!UICONTROL Approva]**. È possibile aggiungere note informative.

Il componente aggiuntivo è ora visibile nell’istanza GenStudio for Performance Marketing della tua organizzazione.
