---
title: Distribuire l’app App Builder
description: Distribuisci l’app App Builder, o il componente aggiuntivo, per GenStudio for Performance Marketing.
feature: Extensibility
exl-id: 51888ab7-7772-4ac8-838d-26db3019e9b0
TQID: https://experienceleague.adobe.com/7Z4Fb-jPi4FHrTeOgHxxO4fl982sqri-7uEDoylFF-s
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: ad3738c7-91ac-48ed-a914-fd0b03f89396
  - id: bfaa655b-e017-428d-80d0-09de2183b296
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: da3860b0-d637-47df-bef0-273751180266
source-git-commit: ca8bfb11a301697c92e97bad41ea3ba8aa359847
workflow-type: tm+mt
source-wordcount: 622
ht-degree: 0%

---

# Distribuire l’app

L’esecuzione dell’app offre un’istantanea preliminare del comportamento del componente aggiuntivo prima della distribuzione. Questo può essere utile per il debug.

## Eseguire l’app

Esegui l&#39;app in `https://localhost:9080`:

```bash
aio app run
```

## Distribuire l’app

1. Passa all’area di lavoro di implementazione:

   ```bash
   aio app use -w [deployment_workspace]
   ```

2. Distribuire l’app:

   ```bash
   aio app deploy
   ```

## Forza ridistribuzione

Puoi forzare la creazione e la distribuzione dell’app senza inviarla nuovamente per l’approvazione.

>[!NOTE]
>
>L’imposizione di una build e di una distribuzione sovrascrive la distribuzione esistente. **Esegui prima il test completo dell&#39;app** in un ambiente di test.

```bash
aio app build --force-build
```

```bash
aio app deploy --force-deploy
```

## Generazione e distribuzione simultanee

```bash
aio app deploy --force-build --force-deploy
```

## Trova la nuova app

Dopo la distribuzione, puoi visualizzare la nuova app in GenStudio for Performance Marketing.

### Visualizza con un URL

Visualizza la nuova app aggiungendo un parametro `query` all&#39;URL di GenStudio for Performance Marketing:

```txt
https://experience.adobe.com/?ext=https://<my-deployed-add-on>.adobeio-static.net/index.html#/@<ims-org>/genstudio/create
```

### Visualizza nell’interfaccia utente

Le nuove estensioni si trovano in posizioni diverse nell&#39;interfaccia utente, a seconda del tipo di estensione distribuito. I punti di estensione attualmente disponibili sono:

* Estensione della conformità, che include:
   * [*punti di estensione prompt*](#find-prompt-extensions), che consentono ai clienti di aggiungere ulteriore contesto alla generazione LLM e
   * [*punti di estensione di convalida*](#find-validation-extensions), che consentono ai clienti di convalidare il contenuto generato da LLM. La convalida viene spesso associata all’estensione Prompt per assicurarsi che il contenuto generato con un prompt esteso sia in conflitto con i requisiti del cliente (ad esempio, dichiarazioni su medicinali o legali)
* [Estensione Digital Asset Management (DAM)](#find-dam-extensions)
* [Estensione modello](#find-template-extensions)
* [Estensione di traduzione](#find-translation-extensions)
* [Estensione Frammento di contenuto](#find-content-fragment-extension)

### Trova estensioni prompt

Le estensioni dei prompt si trovano nel menu a discesa **Componenti aggiuntivi**, nella **sezione parametri** di un modello.

![Richiedi estensioni](./select-prompt-ext.png){width="600" zoomable="yes"}

Viene visualizzata la finestra di dialogo del componente aggiuntivo, che consente di selezionare il contesto aggiuntivo da aggiungere per la generazione LLM.

![Menu a discesa Prompt extension](./select-prompt-dropdown.png){width="600" zoomable="yes"}

### Trova estensioni di convalida

Le estensioni di convalida si trovano dopo una generazione di prompt, nel lato destro visualizzato con i risultati.

![Estensioni di convalida](./validation-ext.png){width="600" zoomable="yes"}

Esegui l’estensione selezionata per convalidare il contenuto generato.

![Convalida valida valida](./validation-valid.png){width="600" zoomable="yes"}

In caso di errori, puoi utilizzare l’estensione per aggiornare la copia delle esperienze a livello di programmazione. Facendo clic sul pulsante **[!UICONTROL Copia]**, il testo suggerito verrà copiato negli Appunti. Facendo clic sul pulsante **[!UICONTROL Applica]**, il testo verrà applicato a una casella di testo specifica nell&#39;esperienza generata.

![Errore di convalida durante la visualizzazione dei pulsanti Copia e Applica](./validation-copy-apply.png){width="600" zoomable="yes"}

### Trovare estensioni DAM

Le estensioni Digital Asset Management (DAM) si trovano quando si seleziona il contenuto nella **sezione parametri** di un modello. Per visualizzare eventuali componenti aggiuntivi, vedi la parte inferiore del menu a discesa **Seleziona percorso**.

![Estensioni DAM](./dam-ext.png){width="600" zoomable="yes"}

### Trovare le estensioni dei modelli

Le estensioni del modello si trovano nella scheda **External Template App** quando si seleziona un modello. Questa scheda viene visualizzata solo in presenza di app modello da selezionare.

![Estensioni modello](./template-ext.png){width="600" zoomable="yes"}

### Trovare le estensioni di traduzione

Utilizza i punti di estensione della traduzione per portare il tuo servizio di traduzione tramite un proxy invece di utilizzare la traduzione predefinita di GenStudio.
Nessuna posizione dell&#39;interfaccia utente per queste estensioni.

Se l&#39;estensione è registrata, viene utilizzato il servizio di traduzione fornito. In caso contrario, viene utilizzato il servizio di traduzione GenStudio predefinito.

### Trova estensione frammento di contenuto

L&#39;estensione Frammento di contenuto in [!DNL GenStudio for Performance Marketing] sostituisce il testo nelle esperienze e-mail generate nell&#39;area di lavoro [!DNL Create] con le voci di un archivio di terze parti (3P) connesso. Dopo aver configurato e distribuito l’estensione, sostituisci la copia dall’area di lavoro senza uscire dal flusso di lavoro.

>[!NOTE]
>
>Lo scambio di estensioni per frammenti di contenuto è attualmente disponibile per **e-mail** esperienze nell&#39;area di lavoro. Il supporto per il canale **Horizon** sarà presto disponibile.

**Per scambiare il testo utilizzando l&#39;estensione Frammento di contenuto**:

1. Nell’area di lavoro, fai clic su un campo di testo modificabile in una variante e-mail generata.
1. Fai clic su **[!UICONTROL Scambia]**.
   ![Scambia testo](./subject-line-swap.png){width="400" zoomable="yes"}
1. Seleziona l’archivio di terze parti. L’organizzazione controlla quali archivi vengono visualizzati e come si comporta l’interfaccia utente dell’archivio.
1. Selezionare la richiesta di risarcimento da utilizzare come testo sostitutivo per il campo.

Se si è soddisfatti del componente aggiuntivo, è possibile distribuirlo senza il parametro `query`.

Ora puoi [distribuire la tua app](distribute-app.md).
