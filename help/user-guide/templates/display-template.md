---
title: Visualizzare le linee guida per il modello di annuncio
description: Segui le best practice per l’utilizzo di annunci display e modelli di banner con Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 076239b3-9444-48f9-bdd6-ef2b757bdf0d
TQID: https://experienceleague.adobe.com/HjkLWiyqK1quHoZB5lEE-qyB3zci12KlRAZC8ME-9Ao
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 300
ht-degree: 1%

---

# Visualizzare le linee guida per i modelli di annunci

I modelli di visualizzazione sono layout predefiniti utilizzati per creare banner e annunci di visualizzazione visivamente coinvolgenti. Offrono un framework flessibile per incorporare immagini, testo e call to action, garantendo coerenza ed efficienza nella produzione di più varianti di annunci. Quando prepari il modello per l’utilizzo in GenStudio for Performance Marketing, accertati che tutte le risorse siano ottimizzate per la visualizzazione web e soddisfino i formati e le dimensioni di file richiesti.

Segui queste best practice per la progettazione quando personalizzi i modelli di banner e annunci display per lavorare con GenStudio for Performance Marketing:

- Utilizzare i caratteri Adobe o Google
- Prepara le risorse che vengono visualizzate correttamente in dimensioni sottili
- È richiesto un solo campo immagine
- **non** utilizza immagini di sfondo incorporate o codificate
- Utilizza le immagini di sfondo (campo `image`) caricate nell&#39;archivio dei contenuti di GenStudio for Performance Marketing. Per ottenere risultati ottimali, attieniti alle linee guida in [Caricamento di immagini per annunci di visualizzazione](#uploading-images-for-display-ads)
- **non** utilizza JavaScript
- È possibile utilizzare una sola sezione, generando un singolo set di elementi modello

## Nomi di campi riconosciuti

Quando personalizzi il banner o il modello di annuncio visualizzato, utilizza segnaposto di contenuto per i seguenti campi obbligatori:

- `headline`
- `sub_headline`
- `body`
- `image` (obbligatorio, selezionato da Content JPEG, PNG o GIF)

GenStudio for Performance Marketing genera automaticamente i campi seguenti. Non è necessario applicare segnaposto di contenuto per:

- `cta`

Consulta [Segnaposto di contenuto](/help/user-guide/templates/customize-template.md#content-placeholders) per ulteriori informazioni sull&#39;utilizzo dei nomi dei campi nei modelli.

## Dimensioni supportate

È necessario impostare la larghezza x l&#39;altezza (pixel).

| Orientamento | Dimensioni (pixel) | Note |
|--------------|-------------------------------------------------------------|------------------------------------------------------------------|
| Verticale | 300 x 600<br>160 x 600 | Comune per grattacieli e banner a mezza pagina. |
| Orizzontale | 300 x 250<br>728 x 90<br>336 x 280<br>320 x 50<br>970 x 250 | Classifica standard, rettangolo medio e dimensioni banner. |
| Personalizzato | Da 50 x 50 a 2000 x 2000 | Da utilizzare per posizionamenti non standard o univoci; controlla i limiti della piattaforma. |

