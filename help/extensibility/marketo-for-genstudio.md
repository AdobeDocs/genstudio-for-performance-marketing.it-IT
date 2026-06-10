---
title: Marketo per GenStudio
description: Installa e configura l’app Adobe Exchange Marketo for GenStudio in modo che la tua organizzazione possa utilizzare i modelli Marketo Engage in GenStudio for Performance Marketing.
feature: Extensibility
source-git-commit: e5011c95e9536d73b1f09d6bc76bb83f121573cd
workflow-type: tm+mt
source-wordcount: '955'
ht-degree: 0%

---

# Marketo per GenStudio

Le organizzazioni che utilizzano [!DNL Marketo Engage] e [!DNL GenStudio for Performance Marketing] nella stessa organizzazione [!DNL IMS] possono installare l&#39;app **Marketo per GenStudio** da [!DNL Adobe Exchange]. Dopo che un amministratore di sistema ha approvato l&#39;app e completato la distribuzione, gli autori possono scegliere i modelli di Marketo durante la creazione di esperienze e-mail in GenStudio, accanto ai modelli caricati direttamente in [!DNL Content].

Questo argomento è destinato a **amministratori** che installano l&#39;app, raccolgono le credenziali da Marketo e distribuiscono l&#39;app in Exchange. Per informazioni sul funzionamento della sintassi dei modelli AJO e Marketo con GenStudio, vedere [Modelli da AJO e Marketo](/help/user-guide/templates/use-templates.md#templates-from-ajo-and-marketo).

## Prerequisiti

* Il provisioning di [!DNL Marketo Engage] deve essere eseguito nell&#39;organizzazione in cui si distribuisce l&#39;estensione.
* Gli utenti che distribuiscono l&#39;applicazione hanno bisogno di **credenziali Marketo**. Per creare e recuperare tali credenziali, è necessario disporre dell&#39;accesso **Amministratore prodotto Marketo** (l&#39;area **[!UICONTROL Amministratore]** deve essere disponibile quando si apre Marketo).

## Installare l’app da Adobe Exchange

>[!VIDEO](https://video.tv.adobe.com/v/3483319?captions=ita&learn=on)

1. Apri [Adobe Exchange](https://exchange.adobe.com) e passa a **[!UICONTROL CX Enterprise]**.
1. Apri l&#39;inserzione [Marketo per GenStudio](https://exchange.adobe.com/apps/ec/ab6p21vo8r/marketo-for-genstudio).
   ![Marketo per GenStudio in Adobe Exchange](/help/extensibility/marketo-adobe-exchange.png){width="75%"}
1. Seleziona **[!UICONTROL Gratis]** per richiedere l&#39;app per la tua organizzazione.
1. Dopo che l&#39;organizzazione **ha esaminato e approvato** la richiesta, continuare con [Ottieni credenziali Marketo](#get-marketo-credentials) e [Distribuisci l&#39;applicazione da Exchange](#deploy-the-application-from-exchange).

## Ottieni credenziali Marketo

Usa le credenziali dell&#39;istanza **Marketo** (non Adobe Developer Console). Prima di eseguire la distribuzione in Exchange, raccogli le credenziali seguenti seguendo la procedura descritta di seguito.

>[!NOTE]
>
>Per generare e recuperare le credenziali di Marketo, devi disporre dell’accesso di amministratore di prodotto Marketo, altrimenti la scheda Amministratore non è visibile in Marketo.

### Creare un utente solo API (facoltativo se si riutilizza un utente API esistente)

1. In Marketo, passa a **[!UICONTROL Amministratore]**.
   ![Scheda Amministratore Marketo](/help/extensibility/marketo-admin-global.png){width="80%"}
1. In **[!UICONTROL Sicurezza]**, apri **[!UICONTROL Utenti e ruoli]** e passa alla scheda **[!UICONTROL Ruoli]**.
1. Creare un nuovo ruolo o modificare un ruolo esistente con le seguenti autorizzazioni aggiunte: _Access API_ e _Access Design Studio_.
1. Per un nuovo utente API, fare clic su **[!UICONTROL Crea solo utente API]** (utilizzare un&#39;e-mail univoca per ogni utente API).
1. Selezionare la casella di controllo Ruoli e assegnare il nuovo ruolo creato. Se si dispone già di un utente API che si desidera utilizzare, passare a [Creare o selezionare un servizio LaunchPoint](#create-or-select-a-launchpoint-service).

![Utenti e ruoli con solo API Ruoli utente e API](/help/extensibility/marketo-users-roles-api-user.png){width="80%"}

### Creare o selezionare un servizio LaunchPoint

1. In **[!UICONTROL Admin]**, in **[!UICONTROL Integration]**, aprire **[!UICONTROL LaunchPoint]**.
1. Fai clic su **[!UICONTROL Crea]** per creare un nuovo servizio (o utilizzare un servizio personalizzato esistente).
   ![Servizio personalizzato LaunchPoint](/help/extensibility/marketo-launchpoint-custom-service.png){width="80%"}
1. Per il tuo servizio, fai clic su **[!UICONTROL Visualizza dettagli]** e copia **[!UICONTROL ID client]** e **[!UICONTROL Segreto client]**. Immetterai questi in Adobe Exchange **[!UICONTROL Configurazione]**.

### Prendi nota dell’URL di base dell’API REST di Marketo.

1. In **[!UICONTROL Admin]**, in **[!UICONTROL Integration]**, aprire **[!UICONTROL Servizi Web]**.
1. Trova l&#39;endpoint **[!UICONTROL REST API]**. Copiare solo l&#39;**URL di base** (host), nel formato `https://###-XXX-###.mktorest.com`. **non** includere segmenti di percorso come `/rest` o `/identity`. Questo valore è univoco per ogni istanza di Marketo.

![URL base endpoint REST API servizi Web](/help/extensibility/marketo-web-services-rest-endpoint.png){width="80%"}

Sarà inoltre necessario l&#39;**[!UICONTROL URL Marketo Engage Identity]** richiesto dalla schermata di distribuzione di Exchange, insieme all&#39;URL REST di base e all&#39;ID client e al segreto client di LaunchPoint.

## Distribuire l&#39;applicazione da Exchange

Per rendere l&#39;estensione disponibile in GenStudio, distribuisci l&#39;app da Adobe Exchange.

1. Torna a [Adobe Exchange](https://exchange.adobe.com).
1. Seleziona **[!UICONTROL Gestisci]** e apri l&#39;app **Marketo per GenStudio** (ad esempio in **[!UICONTROL applicazioni App Builder]** o nelle app gestite della tua organizzazione).
1. In **[!UICONTROL Ambienti]**, scegli un ambiente esistente dal menu a discesa oppure seleziona **[!UICONTROL Aggiungi ambiente]** per crearne uno.
1. Apri **[!UICONTROL Configurazione]** per l&#39;ambiente selezionato.
1. Immettere **[!UICONTROL ID client]** e **[!UICONTROL Segreto client]** da [LaunchPoint](#create-or-select-a-launchpoint-service), **[!UICONTROL URL identità Marketo Engage]** e **[!UICONTROL URL di base API REST Marketo Engage]** (host di base da [Servizi Web](#note-your-marketo-rest-api-base-url)) sia per l&#39;URL identità Marketo Engage &#x200B;e per l&#39;URL di base API REST Marketo Engage.
1. Fare clic su **[!UICONTROL Distribuisci]**. Al termine della distribuzione, l&#39;azione diventa **[!UICONTROL Annulla distribuzione]**.

### Aggiorna configurazione

Per modificare i valori di configurazione per un ambiente, **[!UICONTROL Annulla la distribuzione]**, aggiorna i campi, quindi **[!UICONTROL Ridistribuisci]**.

### Configurazione Workspace (opzionale)

È possibile saltare questo passaggio se si desidera utilizzare l&#39;area di lavoro predefinita. Per impostazione predefinita, i campi **Workspace ID** e **Dimensioni pagina elenco modelli** sono preconfigurati.

Tuttavia, se devi recuperare i modelli da un’area di lavoro diversa:

1. In Marketo, passa a **[!UICONTROL Admin]** → **[!UICONTROL Security]** → **[!UICONTROL Workspace e partizioni]**.
1. La colonna **Workspace ID** è nascosta per impostazione predefinita. Per abilitarla, fai clic con il pulsante destro del mouse sulla riga di intestazione (dove vengono visualizzati i nomi delle colonne).
1. Seleziona **[!UICONTROL Colonne]**.
1. Abilita **[!UICONTROL ID]** dall&#39;elenco.
   ![Aree di lavoro e partizioni con colonna Workspace ID abilitata](/help/extensibility/marketo-workspace-id.png){width="80%"}

Una volta visualizzato, usa il **Workspace ID** appropriato per la configurazione.

## Accedere ai modelli di Marketo in GenStudio

Dopo l&#39;installazione e la configurazione di Marketo for GenStudio, viene visualizzata una scheda **[!UICONTROL Modelli Marketo]** quando si crea un&#39;esperienza **E-mail** in GenStudio. Utilizza quella scheda per sfogliare i modelli da Marketo Engage.

>[!IMPORTANT]
>
>Crea e-mail nel flusso di esperienza **E-mail standard** in GenStudio for Performance Marketing. Questa integrazione NON supporta le e-mail create con la nuova esperienza di editor e-mail.

![Configurazione di Exchange con credenziali Marketo](/help/extensibility/marketo-exchange-configuration.png){width="80%"}

## Risoluzione dei problemi

### La scheda Modelli di Marketo non è visibile

* Verificare che l&#39;app sia **Approvata** in Exchange e che l&#39;ambiente sia **distribuito** con ID client, segreto client e URL di base Marketo validi.
* Chiedi all&#39;amministratore di verificare che sia stato utilizzato l&#39;accesso **Amministratore di prodotto Marketo** durante la creazione delle credenziali.

### I modelli non si caricano

* Ricarica la pagina oppure esci e accedi di nuovo a GenStudio.
* Nel pannello degli strumenti di sviluppo del browser **[!UICONTROL Rete]**, cerca le chiamate API non riuscite all&#39;istanza di Marketo e verifica che l&#39;URL della base REST corrisponda a **[!UICONTROL Servizi Web]** in Marketo (nessun percorso aggiuntivo dopo l&#39;host).

### Errore &quot;Nessun modello trovato&quot;

Se l’estensione viene installata correttamente e la scheda Modelli di Marketo è visibile ma viene visualizzato &quot;Nessun modello trovato&quot;, il problema potrebbe essere causato dal superamento dei limiti di dimensione da parte dell’applicazione durante il rendering dei modelli, con conseguente arresto anomalo.
Per risolvere il problema:

1. Annulla la distribuzione dell&#39;applicazione da Exchange.
1. Riduci le dimensioni della pagina dell’elenco di modelli (ad esempio, impostalo su 1 o 2).
1. Ridistribuire l&#39;applicazione.
