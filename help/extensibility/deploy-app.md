---
title: Distribuire l’app App Builder
description: Distribuisci l’app App Builder, o il componente aggiuntivo, per GenStudio for Performance Marketing.
feature: Extensibility
exl-id: 51888ab7-7772-4ac8-838d-26db3019e9b0
source-git-commit: 7fdd3f54a0a031bfe26b48983de9cd24baad2f62
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 0%

---

# Distribuire l’app

L’esecuzione dell’app offre un’istantanea preliminare del comportamento del componente aggiuntivo prima della distribuzione. Queste informazioni possono facilitare il debug.

**Per eseguire l&#39;app**:

Esegui l&#39;app in `https://localhost:9080`:

```bash
aio app run
```

**Per distribuire l&#39;app**:

1. Passa all’area di lavoro di implementazione:

   ```bash
   aio app use -w [deployment_workspace]
   ```

2. Distribuire l’app:

   ```bash
   aio app deploy
   ```

**Per forzare la ridistribuzione**:

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

**Per generare e distribuire contemporaneamente**:

```bash
aio app deploy --force-build --force-deploy
```

**Per visualizzare l&#39;app**:

Dopo la distribuzione, puoi visualizzare l&#39;app in GenStudio for Performance Marketing aggiungendo un parametro `query` all&#39;URL di GenStudio for Performance Marketing:

```txt
https://experience.adobe.com/?ext=https://<my-deployed-add-on>.adobeio-static.net/index.html#/@<ims-org>/genstudio/create
```

Se si è soddisfatti del componente aggiuntivo, è possibile distribuirlo senza il parametro `query`.

Ora puoi [distribuire la tua app](distribute-app.md).
