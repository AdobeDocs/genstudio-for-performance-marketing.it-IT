---
title: Distribuire l’app App Builder
description: Distribuisci l’app App Builder, o il componente aggiuntivo, per GenStudio for Performance Marketing.
source-git-commit: acc54215d980f1f7392401cca9d90ed0ce41b2ec
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 0%

---


# Distribuire l’app

L’esecuzione dell’app fornisce un’istantanea preliminare del comportamento del componente aggiuntivo prima della distribuzione. Queste informazioni possono facilitare il debug. Puoi forzare la creazione e la distribuzione di un’app implementata senza inviarla nuovamente per l’approvazione.


**Per eseguire l&#39;app**:

Esegui l&#39;app in `https://localhost:9080`:

```bash
aio app run
```

**Per distribuire l&#39;app**:

1. Passa all’area di lavoro di distribuzione. Ad esempio, per passare all’area di lavoro Produzione:

   ```bash
   aio app use -w Production
   ```

1. Distribuire l’app:

   ```bash
   aio app deploy
   ```

**Per forzare la ridistribuzione**:

>[!NOTE]
>
>L’imposizione della generazione e della distribuzione sovrascrive la distribuzione esistente. Esegui prima il test completo dell’app in un ambiente di test.

```bash
aio app build --force-build
```

```bash
aio app deploy --force-deploy
```

**Per generare e distribuire contemporaneamente**:

```bash
aio app deploy --force-build --force-deploy
```

**Per visualizzare l&#39;app**:

Dopo la distribuzione, puoi visualizzare l&#39;app in GenStudio for Performance Marketing aggiungendo un parametro `query` all&#39;URL di GenStudio for Performance Marketing:

`https://experience.adobe.com/?ext=https://<my-deployed-add-on>.adobeio-static.net/index.html#/@<ims-org>/genstudio/create`

Se si è soddisfatti del componente aggiuntivo, è possibile distribuirlo senza il parametro `query`.

Ora puoi [distribuire la tua app](distribute-app.md).
