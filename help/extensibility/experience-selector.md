---
title: MFE Selettore esperienza GenStudio
description: Comprendere e implementare Experience Selector Micro FrontEnd per le app e i componenti aggiuntivi GenStudio.
feature: Extensibility, Extensions, Experiences
source-git-commit: e30e43bd8d226628b425c341d19195f7f860e560
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 6%

---

# MFE Selettore esperienza GenStudio

Il selettore esperienza è un Micro Frontend (MFE) che fornisce un componente `ExperienceSelectorDialog` per la selezione di esperienze GenStudio. Utilizzare il componente nell&#39;applicazione importando la funzione `renderExperienceSelectorWithSUSI` dal bundle standalone di JavaScript, che carica automaticamente l&#39;ultima versione distribuita di Micro Frontend e presenta un&#39;interfaccia componente naturale.

Il selettore esperienza MFE di GenStudio consente agli utenti di:

- Sfoglia e seleziona esperienze GenStudio
- Filtrare le esperienze in base a vari criteri
- Supporto di modalità di selezione singola e multipla
- Gestire l’autenticazione tramite l’integrazione SUSI (Sign-On)
- Fornire un’interfaccia utente coerente tra diversi framework

## Opzioni di integrazione

L’MFE può essere integrato utilizzando due approcci diversi:

### ESM (moduli ES) - consigliato

```javascript
import { renderExperienceSelectorWithSUSI } from 'https://experience-stage.adobe.com/solutions/GenStudio-experience-selector-mfe/static-assets/resources/@genstudio/experience-selector/esm/standalone.js';
```

### UMD (Universal Module Definition)

```html
<script src="https://experience-stage.adobe.com/solutions/GenStudio-experience-selector-mfe/static-assets/resources/@genstudio/experience-selector/umd/standalone.js"></script>
```

## Proprietà di configurazione

La funzione `renderExperienceSelectorWithSUSI` accetta un oggetto di configurazione con le seguenti proprietà:

| Proprietà | Tipo | Obbligatorio | Descrizione |
|----------|------|----------|-------------|
| `apiKey` | stringa | Sì | Chiave API per i servizi GenStudio |
| `imsOrg` | stringa | Sì | ID organizzazione IMS |
| `env` | stringa | Sì | Ambiente (`stage`, `prod`) |
| `susiConfig` | oggetto | Sì | [Configurazione autenticazione SUSI](#susi-configuration) |
| `onSelectionConfirmed` | funzione | Sì | Callback quando la selezione viene confermata |
| `onDismiss` | funzione | Sì | Callback quando la finestra di dialogo viene chiusa |
| `locale` | stringa | No | Lingua locale (ad esempio, `en-US`) |
| `isOpen` | booleano | No | Stato della finestra di dialogo iniziale |
| `selectionType` | stringa | No | Modalità di selezione (`single` o `multiple`) |
| `customFilters` | array | No | Criteri di filtro personalizzati |
| `dialogTitle` | stringa | No | Titolo finestra di dialogo personalizzata |

### Configurazione SUSI

L&#39;oggetto `susiConfig` può includere:

```javascript
{
  clientId: 'genstudio',
  environment: 'stg1', // or 'prod'
  scope: 'additional_info.projectedProductContext,additional_info.ownerOrg,AdobeID,openid,session,read_organizations,ab.manage',
  locale: 'en_US',
  modalSettings: {
    width: 500,
    height: 700
  }
}
```

## Guida rapida

1. **Scegli il tuo framework** tra gli esempi disponibili di seguito
1. **Passa alla directory di esempio**
1. **Installa dipendenze** (per esempi di React/Vue)
1. **Aggiorna la configurazione** con le chiavi API e l&#39;organizzazione IMS:

   ```javascript
   const experienceSelectorProps = {
     locale: 'en-US',
     apiKey: 'exc_app',           
     imsOrg: 'your-ims-org@AdobeOrg',  // Replace with your IMS Org
     env: 'stage', // or 'prod'
     susiConfig: {
        clientId: 'genstudio',
        environment: 'stg1', // or 'prod'
        scope: 'additional_info.projectedProductContext,additional_info.ownerOrg,AdobeID,openid,session,read_organizations,ab.manage',
        locale: 'en_US',
        modalSettings: {
          width: 500,
          height: 700,
        },
     },
     customFilters: ['genstudio-channel:email'],
     selectionType: 'single', // or 'multiple'
     dialogTitle: 'Select Email Templates'
   };
   ```

1. **Esegui il server di sviluppo**

### Implementazioni di esempio

Questo archivio include esempi di lavoro per diversi framework:

- [Un **applicazione React completa** che dimostra l&#39;integrazione con il sistema di compilazione Vite](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/react-js).

- [A **Applicazione Vue 3** con integrazione API di composizione](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vue-js).

- [Due **Implementazioni di Vanilla JavaScript**](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vanilla-js):

   - [Questa versione di **Vanilla ESM** utilizza moduli ES6 e JavaScript](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vanilla-js/vanilla-esm) moderni.

   - [Questa versione di **Vanilla UMD** utilizza il bundle UMD caricato tramite tag script](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vanilla-js/vanilla-umd-global-var).

## Flusso di autenticazione

Il selettore esperienza gestisce automaticamente l’autenticazione tramite SUSI:

1. All’apertura della finestra di dialogo, verifica la presenza dell’autenticazione esistente.
1. Se non è autenticato, apre un flusso di accesso SUSI.
1. Dopo l’autenticazione corretta, viene visualizzato il selettore delle esperienze.
1. Gli utenti possono esplorare e selezionare le esperienze.
1. Le esperienze selezionate vengono restituite tramite il callback `onSelectionConfirmed`.
