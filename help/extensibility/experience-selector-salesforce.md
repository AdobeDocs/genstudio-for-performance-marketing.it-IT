---
title: Selettore di esperienze MFE in Salesforce
description: Scopri come distribuire e configurare l’MFE di Experience Selector in Salesforce Lightning, inclusi CSP, autenticazione Adobe, modelli e-mail Apex e convalida.
feature: Extensibility, Extensions, Experiences
source-git-commit: 4cac970f46ab08bcec2f23fd882c552af088c4ea
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 0%

---

# Selettore di esperienze MFE in Salesforce

In questo argomento viene illustrato come i clienti e i responsabili dell&#39;implementazione possono distribuire ed eseguire il micro front-end (MFE) di [!DNL GenStudio for Performance Marketing] Experience Selector in un&#39;organizzazione Salesforce. Vengono descritti i passaggi dell’amministratore (senza codice), i passaggi dello sviluppatore (distribuzione e configurazione) e le impostazioni relative alla sicurezza, ad esempio Content Security Policy (CSP).

Per opzioni di integrazione MFE generiche, proprietà di configurazione ed esempi di framework, vedi [MFE del selettore esperienza GenStudio](experience-selector.md).

## Funzionamento di questa integrazione

>[!VIDEO](https://video.tv.adobe.com/v/3491087?captions=ita&learn=on)

Il componente Web Lightning (LWC) `sfgsmfe` carica il bundle UMD di Adobe Experience Selector ed esegue il rendering in un `<dialog>` in modo che gli utenti possano scegliere un&#39;esperienza da [!DNL GenStudio for Performance Marketing].

L’integrazione può anche:

* **Anteprima e decodifica:** Visualizza il payload selezionato come JSON, HTML decodificato e un&#39;anteprima HTML bonificata all&#39;interno di LWC.
* **Modelli e-mail (facoltativi):** Un flusso **[!UICONTROL Crea modello e-mail]** in Salesforce può chiamare Apex (`EmailTemplateController.createEmailTemplate`) per inserire un record `EmailTemplate` (HTML, oggetto e cartella).
* **Caricamento runtime:** lo script GenStudio è caricato dall&#39;URL ospitato di Adobe in `experience.adobe.com`, non da una risorsa statica Salesforce nell&#39;implementazione tipica.

## Prerequisiti

* **Organizzazione Salesforce:** organizzazione sandbox o di produzione in cui è possibile distribuire metadati e utilizzare **[!UICONTROL App Builder Lightning]**.
* **Salesforce CLI:** Salesforce CLI (`sf`) è installato e autenticato, ad esempio:

  ```bash
  sf org login web --alias <your-org-alias>
  ```

* **Autorizzazioni:** gli utenti che creano modelli e-mail devono accedere alla cartella dei modelli e-mail di destinazione e disporre dei diritti per creare modelli in base ai criteri dell&#39;organizzazione. Apex esegue `with sharing`.
* **Adobe / GenStudio:** l&#39;ID organizzazione Adobe IMS e SUSI `clientId` devono corrispondere alla configurazione Adobe (vedi [Configurare i valori di integrazione](#configure-integration-values-developer--implementation)).
* **Browser/CSP:** Salesforce deve consentire il caricamento di script da `https://experience.adobe.com` (vedere [Configurare i criteri di sicurezza del contenuto e l&#39;URL di Adobe](#configure-content-security-policy-and-adobe-url)).

## Distribuire il pacchetto (sviluppatore)

L’integrazione segue un layout in stile Salesforce DX. La directory predefinita del pacchetto è in genere `force-app` nel progetto Salesforce DX.

1. Dalla directory principale del progetto, distribuisci l’origine all’organizzazione di destinazione:

   ```bash
   sf project deploy start --source-dir force-app --target-org <your-org-alias>
   ```

2. Conferma che la distribuzione venga completata senza errori.

I metadati tipici del progetto includono:

* Un bundle LWC denominato `sfgsmfe` (HTML, JavaScript, CSS e meta XML) che ospita l&#39;interfaccia utente del selettore e il caricamento dello script.
* Una classe Apex (ad esempio, `EmailTemplateController`) che crea modelli e-mail quando si utilizza tale flusso facoltativo.

Il progetto può anche definire risorse statiche. Se il caricatore LWC utilizza l&#39;URL CDN di Adobe per `standalone.js`, tali risorse non sono necessarie per il percorso di caricamento a meno che non si modifichi l&#39;implementazione.

## Aggiungere il componente a una pagina Lightning (admin)

Il componente `sfgsmfe` è esposto per:

* Pagine app fulmini
* Home page
* Registra pagine
* Schede (inserendo il componente in una pagina Lightning aperta da una scheda personalizzata)

Per aggiungere il componente:

1. In **[!UICONTROL Setup]**, aprire **[!UICONTROL App Manager]**.
1. Crea una **[!UICONTROL nuova app Lightning]** (o apri un&#39;app esistente che desideri estendere).
   ![Nuova app Lightning modale](./mfe-new-lighting-app.png){width="80%" zoomable="yes"}
1. Apri l&#39;app e seleziona **[!UICONTROL Modifica]**.
   ![Modifica modale app fulmini](./mfe-lightning-edit.png){width="80%" zoomable="yes"}
1. Crea una **[!UICONTROL nuova pagina]** (o modifica una pagina Lightning esistente).
   ![Finestra modale Nuova pagina](./mfe-lightning-new-page.png){width="60%" zoomable="yes"}
1. In **[!UICONTROL Lightning App Builder]**, trascinare il componente **sfgsmfe** nel layout.
1. **[!UICONTROL Salva]**, **[!UICONTROL Attiva]** e assegna la pagina all&#39;app Lightning, ai profili e alla visibilità dell&#39;app corretti in modo che gli utenti desiderati possano aprirla.

## Configurare i criteri sulla sicurezza dei contenuti e l’URL di Adobe

LWC inserisce un tag `<script>` il cui `src` punta al bundle UMD di Adobe, ad esempio:

`https://experience.adobe.com/solutions/GenStudio-experience-selector-mfe/static-assets/resources/@genstudio/experience-selector/umd/standalone.js`

Devi configurare Salesforce in modo che questa origine sia consentita per il caricamento dello script in base ai CSP e alle impostazioni di sicurezza Lightning della tua organizzazione.

Se lo script non viene caricato:

1. Apri gli strumenti per sviluppatori del browser.
1. Controlla le schede **[!UICONTROL Console]** e **[!UICONTROL Rete]** per individuare richieste bloccate o violazioni CSP.
1. Aggiungi o regola **[!UICONTROL Siti attendibili CSP]** (e tutte le impostazioni correlate per la versione di Salesforce in uso) per `https://experience.adobe.com`, seguendo l&#39;attuale documentazione di Salesforce per Lightning.

## Configurare i valori di integrazione (sviluppatore/implementazione)

Diversi valori sono impostati nel JavaScript LWC per `sfgsmfe`. In genere i clienti li sostituiscono a seconda dell’ambiente.

| Valore | Descrizione |
| --- | --- |
| `folderId` | ID cartella Salesforce (`00l...`) per i modelli e-mail in cui vengono creati nuovi modelli. Obbligatorio per Apex; la cartella deve esistere ed essere accessibile all&#39;utente in esecuzione. |
| `imsOrg` | Identificatore organizzazione Adobe IMS passato in `GenStudioExperienceSelector.renderExperienceSelectorWithSUSI`. |
| `susiConfig.clientId` | ID client Adobe SUSI per la registrazione all’app del selettore esperienza. |
| GenStudio `script.src` | URL del bundle UMD `standalone.js`; aggiornalo se Adobe pubblica un nuovo percorso. |

La creazione del modello di posta elettronica associa i campi di GenStudio al modello, ad esempio l&#39;oggetto di `experienceFields`. Regola le mappature nell&#39;LWC se il modello di contenuto è diverso.

Per informazioni dettagliate su `renderExperienceSelectorWithSUSI` e sulle opzioni correlate, vedere [Proprietà di configurazione](experience-selector.md#configuration-properties) nell&#39;argomento MFE del selettore esperienza.

## Apex: EmailTemplateController

`EmailTemplateController.createEmailTemplate` in genere:

* Convalida il nome del modello, l’ID della cartella e il HTML non vuoto.
* Crea un `EmailTemplate` con `TemplateType = 'custom'`, `HtmlValue`, `Subject`, `Body` e assegnazione cartella.
* Rileva gli errori in LWC tramite `AuraHandledException`.

Suggerimenti operativi:

* Rispetta le regole di univocità e denominazione di DeveloperName nell’organizzazione.
* Confermare l&#39;ID della cartella e che l&#39;utente possa creare `EmailTemplate` record in tale cartella.
* Utilizza i registri di debug di Salesforce quando DML non riesce a recuperare l’errore esatto.

## Elenco di controllo per la convalida

Utilizza questo elenco dopo la distribuzione e la configurazione:

* [ La distribuzione di ] viene completata senza errori.
* [ ] Gli utenti possono aprire la pagina Lightning che contiene `sfgsmfe`.
* [ ] Il componente non mostra un errore di caricamento. La scheda Rete restituisce HTTP 200 per `standalone.js`.
* [ ] **[!UICONTROL Seleziona un&#39;esperienza GenStudio]** apre il selettore e i callback di selezione vengono eseguiti.
* [ ] **[!UICONTROL Crea modello e-mail]** riesce quando usi quel flusso e il modello viene visualizzato nella cartella configurata in **[!UICONTROL Configurazione]**.

## Vedi anche

* [Selettore esperienza GenStudio MFE](experience-selector.md)
