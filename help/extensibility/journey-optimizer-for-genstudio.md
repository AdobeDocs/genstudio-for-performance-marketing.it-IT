---
title: Journey Optimizer per GenStudio
description: Installa e configura l’app Adobe Exchange Journey Optimizer for GenStudio in modo che la tua organizzazione possa utilizzare i modelli Adobe Journey Optimizer in GenStudio for Performance Marketing.
feature: Extensibility
source-git-commit: fbec4567d960a6e3607c5e5e43057e2f22e9f6ea
workflow-type: tm+mt
source-wordcount: '957'
ht-degree: 0%

---

# Journey Optimizer per GenStudio

Le organizzazioni che utilizzano [!DNL Adobe Journey Optimizer] (AJO) e [!DNL GenStudio for Performance Marketing] nella stessa organizzazione [!DNL IMS] possono installare l&#39;app **Journey Optimizer for GenStudio** da [!DNL Adobe Exchange]. Dopo che un amministratore di sistema ha approvato l&#39;app e completato la distribuzione, gli autori possono scegliere i modelli di contenuto AJO durante la creazione di esperienze e-mail in GenStudio, accanto ai modelli caricati direttamente in [!DNL Content].

Questo argomento è destinato a **amministratori e sviluppatori** che installano l&#39;app, creano credenziali OAuth in [!DNL Adobe Developer Console] e mappano le autorizzazioni account tecnico in [!DNL Adobe Experience Platform]. Per informazioni sul funzionamento della sintassi dei modelli AJO e Marketo con GenStudio, vedere [Modelli da AJO e Marketo](/help/user-guide/templates/use-templates.md#templates-from-ajo-and-marketo).

## Prerequisiti

* Il provisioning di AJO deve essere eseguito nell’organizzazione in cui distribuisci l’estensione.
* Gli utenti che creano modelli in AJO devono disporre dell&#39;autorizzazione per **creare e modificare** modelli di contenuto in Journey Optimizer, come definito dalla tua organizzazione.
* I modelli e-mail in AJO devono includere segnaposto di campo (manubri) in cui deve essere visualizzato il contenuto generato. È possibile selezionare un modello senza tali campi, ma la generazione dell&#39;**esperienza non riesce** se mancano i segnaposto [!DNL GenStudio for Performance Marketing] previsti. Vedi [Personalizzare un modello](/help/user-guide/templates/customize-template.md) e [Nomi di campi riconosciuti](/help/user-guide/templates/customize-template.md#recognized-field-names).

## Installare l’app da Adobe Exchange

>[!VIDEO](https://video.tv.adobe.com/v/3483287?learn=on)

1. Apri [Adobe Exchange](https://exchange.adobe.com) e passa a **[!UICONTROL Experience Cloud]**.
1. Apri l&#39;inserzione [Journey Optimizer per GenStudio](https://exchange.adobe.com/apps/ec/abpopqqr1q/journey-optimizer-for-genstudio).
   ![Journey Optimizer per GenStudio in Adobe Exchange, inclusi requisiti e installazione gratuita](/help/extensibility/ajo-adobe-exchange.png){width="75%"}
1. Seleziona **[!UICONTROL Gratis]** per richiedere l&#39;app per la tua organizzazione.
1. Dopo che l&#39;organizzazione **ha esaminato e approvato** la richiesta, continuare con [Creare le credenziali OAuth in Adobe Developer Console](#create-oauth-credentials-in-adobe-developer-console) e [Distribuire l&#39;applicazione da Exchange](#deploy-the-application-from-exchange).

## Creare credenziali OAuth in Adobe Developer Console

Crea un **progetto** in [Adobe Developer Console](https://developer.adobe.com/console/) che fornisce le credenziali OAuth per l&#39;API Journey Optimizer. Quando configuri l&#39;app in Exchange, saranno necessari valori quali **ID client**, **Segreto client**, **ID organizzazione** e **Ambito**.

1. Accedi a Adobe Developer Console e crea un **nuovo progetto**.
1. Aggiungere l&#39;API **Adobe Journey Optimizer (AJO)** al progetto facendo clic su **[!UICONTROL Aggiungi API]** e selezionando **[!UICONTROL Adobe Journey Optimizer]** dall&#39;elenco delle API del prodotto **[!DNL Experience Cloud]**.
1. Genera le credenziali nell&#39;area di lavoro del progetto e copia **ID client**, **Segreto client**, **ID organizzazione**, **Ambito** e tutti gli altri valori richiesti dal flusso di distribuzione. Conservarli in modo sicuro per la sezione successiva.

>[!NOTE]
>
>Quando esegui l&#39;installazione da Exchange, utilizza l&#39;**ID client OAuth** se vengono visualizzati sia un ID client OAuth che un ID account tecnico.

## Distribuire l&#39;applicazione da Exchange

### Apri l’app in Gestione e aggiungi un ambiente

1. Torna a [Adobe Exchange](https://exchange.adobe.com).
1. Seleziona **[!UICONTROL Gestisci]** e apri **[!UICONTROL applicazioni App Builder]** (o il percorso delle app gestite della tua organizzazione).
1. Seleziona **Journey Optimizer per GenStudio** e conferma che l&#39;app sia **Approvata**.
1. In **[!UICONTROL Ambienti]**, scegli un ambiente esistente dal menu a discesa **Ambienti:** oppure seleziona **[!UICONTROL Aggiungi ambiente]** per crearne uno.
   ![Dettagli applicazione con stato Approvato e Aggiungi ambiente](/help/extensibility/ajo-config-002.png){width="50%"}
1. Nell&#39;ambiente selezionato, selezionare **[!UICONTROL Configurazione]**.
1. Nella scheda **[!UICONTROL Configurazione]**, individua **[!UICONTROL Credenziali AJO]**.
   ![Configurazione con credenziali AJO prima della distribuzione (bozza)](/help/extensibility/ajo-config-004.png){width="80%"}
1. Immetti le credenziali dal progetto Developer Console a cui è stata aggiunta l&#39;API Journey Optimizer (ad esempio, **[!UICONTROL ID client AJO]**, **[!UICONTROL Segreto client AJO]**, **[!UICONTROL Endpoint token AJO]** e altri campi obbligatori).
1. Immetti il nome della sandbox **in lettere minuscole** (ad esempio, `prod`).
1. Fare clic su **[!UICONTROL Distribuisci]**. Al termine della distribuzione, lo stato viene visualizzato come distribuito. Il testo del pulsante verrà modificato in **[!UICONTROL Annulla distribuzione]**.
   ![App implementata con annullamento distribuzione disponibile nella visualizzazione delle applicazioni di App Builder](/help/extensibility/ajo-config-005.png){width="80%"}

Dopo la distribuzione, Adobe Developer Console include un nuovo progetto generato automaticamente denominato **Journey Optimizer for GenStudio &lt;Nome_ambiente>** con API di AJO e Adobe Runtime. Questo progetto è di sola lettura e non può essere modificato o eliminato.
![Progetto Developer Console di sola lettura generato automaticamente dopo la distribuzione](/help/extensibility/ajo-auto-project.png){width="100%"}

### Aggiorna configurazione

Per modificare le variabili di configurazione per un ambiente, **[!UICONTROL Annullare la distribuzione]**, aggiornare i valori, quindi **[!UICONTROL Distribuire]** di nuovo in modo che le modifiche abbiano effetto.

È possibile creare **più ambienti** in Exchange (ad esempio, uno per sandbox). Ogni implementazione può avere un’esperienza separata in GenStudio quando l’organizzazione utilizza più sandbox.

## Mappare le autorizzazioni per l’account tecnico

Gli utenti possono visualizzare l&#39;estensione AJO in GenStudio senza accesso completo a [!DNL Adobe Experience Platform]. Per le chiamate API (ad esempio, caricamento dei modelli), all&#39;account tecnico associato alle credenziali OAuth devono essere concesse le autorizzazioni Journey Optimizer in **[!DNL Adobe Experience Platform]** > **[!UICONTROL Autorizzazioni]**. I nomi esatti dei ruoli e dei set di autorizzazioni dipendono dall’organizzazione.

Visualizza l&#39;estensione in **[!UICONTROL Amministratore di Percorso]** in AJO **[!UICONTROL Autorizzazioni]** > **[!UICONTROL Ruoli]** e aggiungi le **credenziali API** dal progetto Developer Console, le stesse credenziali utilizzate durante la distribuzione da Exchange.

![Credenziali API assegnate al ruolo Architetto di AJO nelle autorizzazioni Adobe Experience Platform](/help/extensibility/ajo-map-permissions.png){width="80%"}

**Vedere anche** (controllo accesso Journey Optimizer):

* [Controllo degli accessi](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/access-control/access-control-landing-page)
* [Autorizzazioni in Journey Optimizer](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/access-control/permissions)
* [Introduzione per gli amministratori di sistema](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/get-started/quick-start/administrator)

## Accedere ai modelli di AJO in GenStudio

Dopo la distribuzione e la mappatura delle autorizzazioni:
1. Apri **[!UICONTROL Crea]** in GenStudio for Performance Marketing e avvia un&#39;esperienza **E-mail**.
1. In **[!UICONTROL Seleziona modello]**, apri la scheda **[!UICONTROL Modello AJO]** accanto a **[!UICONTROL Modelli caricati]** per sfogliare i modelli da Journey Optimizer.

![Seleziona modello con scheda Modello AJO e raccolta modelli](/help/extensibility/ajo-template-tab.png){width="80%"}

## Risoluzione dei problemi

### La scheda Modelli di AJO non è visibile

* Verificare che i valori immessi in Exchange **[!UICONTROL Configurazione]** siano corretti, inclusi **ID client**, **Segreto client**, **Ambito** e **Sandbox**.
* Verificare che il nome della sandbox **sia in minuscolo** (ad esempio, `prod`).
* Durante l&#39;installazione da Exchange, utilizzare l&#39;**ID client** come descritto in [Creare credenziali OAuth](#create-oauth-credentials-in-adobe-developer-console).

### La scheda Modelli di AJO è visibile ma non è presente alcun modello

* Ricarica la pagina o apri di nuovo la scheda **[!UICONTROL Modello AJO]**.
* Nel browser **[!UICONTROL Strumenti di rete]**, esaminare la richiesta **`get-templates`**. Se restituisce **403 Non consentito**, l&#39;account tecnico non verrà assegnato a un ruolo o a un gruppo con le autorizzazioni Journey Optimizer richieste. Aggiorna i mapping in [!DNL Adobe Experience Platform] **[!UICONTROL Autorizzazioni]** e in AJO **[!UICONTROL Autorizzazioni]** come richiesto dalla tua organizzazione.
