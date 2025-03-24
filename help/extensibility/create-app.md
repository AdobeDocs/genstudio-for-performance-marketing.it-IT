---
title: Creare un’app App Builder per estendere GenStudio for Performance Marketing
description: Inizia a creare un'app o un componente aggiuntivo.
feature: Extensibility
exl-id: 4e757dd4-a02d-472c-bc13-6f27dffa48f2
source-git-commit: 52e8e078bc013fe686b5cc2105089f7098cce575
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Sviluppare un’app App Builder

Gli sviluppatori che estendono le funzionalità native di GenStudio for Performance Marketing utilizzano [Adobe App Builder](https://developer.adobe.com/app-builder/) per creare, inviare e distribuire le proprie app estensibili o i componenti aggiuntivi.

>[!BEGINSHADEBOX]

**Prerequisiti**:

* Node.js (versione 20.x o successiva)

* npm (in pacchetto con Node.js)

* Interfaccia della riga di comando (CLI) di Adobe Developer. Per installare: `npm install -g @adobe/aio-cli`

>[!ENDSHADEBOX]

## Struttura dell’app

I componenti aggiuntivi GenStudio for Performance Marketing sono app App Builder e contengono gli stessi componenti di base di altre app App Builder.

### File di build e configurazione

I componenti chiave delle app App Builder includono questi file di build e configurazione. Questo elenco non include tutti i file di build e configurazione.

* `README.md`: include informazioni generali sull&#39;app.

* File app di Servizi terminal:

   * `package.json`
   * `package-lock.json`
   * `eslint`
   * `tsconfig`
   * `jest test up`

* File di configurazione di App Builder:

   * `app.config.yaml`
   * `ext.config.yaml`: file di configurazione per il componente aggiuntivo
   * `app.config.yaml`: file di configurazione per il componente aggiuntivo (include la definizione dell&#39;app come componente aggiuntivo di GenStudio for Performance Marketing)
   * `.aio`
   * `.env`: non eseguire il commit del file `.env` nel controllo del codice sorgente

### Codice Source

```
- src/
    - genstudiopem/
        - web-src/
            - src/
                - components/
                - utils/
                - Constants.ts
                - index.tsx
                - index.css
                - utils.ts
        - index.html
```

### Componenti codice Source

* `ExtensionRegistration.tsx`: definisce le API necessarie per caricare e visualizzare il componente aggiuntivo dell&#39;app host (GenStudio for Performance Marketing).

* `App.tsx`: componente app principale che definisce il routing ad altri componenti.

* `AdditionalContextDialog.tsx`: componente finestra di dialogo per visualizzare componenti aggiuntivi di contesto aggiuntivi.

* `RightPanel.tsx`: componente finestra di dialogo per un componente aggiuntivo di convalida.

* `Helper` componenti: include `ClaimsChecker`.

## Creare un’app App Builder da un’app esistente

Puoi utilizzare un’app di esempio per iniziare subito a creare il componente aggiuntivo.

**Per creare un&#39;app App Builder da un&#39;app esistente**:

1. Scarica un&#39;app di esempio dall&#39;archivio [GenStudio UIX Examples](https://github.com/adobe/genstudio-uix-examples).

1. Dall&#39;area di lavoro del progetto App Builder in [Adobe Developer Console](https://developer.adobe.com/console/), seleziona **[!UICONTROL Scarica tutto]** per scaricare i dettagli del progetto.

1. Apri l’app di esempio localmente nell’ambiente di sviluppo integrato (IDE) preferito.

1. Esegui l’autenticazione tramite l’interfaccia della riga di comando di Adobe Developer:

   ```bash
   aio login
   ```

1. Scarica il file JSON e crea l’app:

   ```bash
   aio app use '/path/to/your/downloaded/app-builder/project/details/config.json'
   ```

## Aggiungere codice personalizzato al componente aggiuntivo

Il codice del componente aggiuntivo viene definito in `AdditionalContextDialog.tsx` e `RightPanel.tsx` file. Questi due file definiscono l&#39;aspetto e il comportamento dei popup quando gli utenti accedono al componente aggiuntivo.

* `AdditionalContextDialog.tsx`: definire questo componente se si intende utilizzare il componente aggiuntivo _Aggiungi contesto_. Gli utenti interagiscono con questo componente facendo clic su _Componenti aggiuntivi_ nel cassetto delle richieste in [!DNL Create].

* `RightPanel.tsx`: definire questo componente se si intende utilizzare il componente aggiuntivo _Pannello destro_ (convalida dell&#39;esperienza). Gli utenti interagiscono con questo componente facendo clic sul componente aggiuntivo di convalida nel pannello a destra in una bozza di esperienza [!DNL Create].

Ora puoi [distribuire la tua app](deploy-app.md)

## Best practice per lo sviluppo di app

La manutenzione dell’ambiente di sviluppo consente di evitare errori di sviluppo e distribuzione delle app:

* Se utilizzi una versione precedente di un’app di esempio, aggiorna le dipendenze reinstallandole:

  ```bash
  rm -rf node_modules package-lock.json && npm i
  ```

* Aggiornare GenStudio UIX SDK. Conferma di utilizzare la versione più recente di [GenStudio UIX SDK](https://github.com/adobe/genstudio-uix-sdk). Per informazioni su come utilizzare le modifiche di SDK più recenti, consulta l&#39;[archivio di esempio di GenStudio UIX](https://github.com/adobe/genstudio-uix-examples).
