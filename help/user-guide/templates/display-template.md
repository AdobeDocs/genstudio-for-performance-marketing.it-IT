---
title: Visualizzare le linee guida per i modelli di annunci
description: Segui le best practice per l’utilizzo di annunci display e modelli di banner con Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 076239b3-9444-48f9-bdd6-ef2b757bdf0d
source-git-commit: 4760da26d20e91489a74bb238e07f0d3b426c0a1
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 1%

---

# Visualizzare le linee guida per i modelli di annunci

I modelli di visualizzazione sono layout predefiniti utilizzati per creare banner e annunci di visualizzazione visivamente coinvolgenti. Offrono un framework flessibile per incorporare immagini, testo e call to action, garantendo coerenza ed efficienza nella produzione di più varianti di annunci. Quando prepari il modello per l’utilizzo in GenStudio for Performance Marketing, accertati che tutte le risorse siano ottimizzate per la visualizzazione web e soddisfino i formati e le dimensioni di file richiesti.

Segui queste best practice per la progettazione quando personalizzi i modelli di banner e annunci display per lavorare con GenStudio for Performance Marketing:

- Utilizzare i caratteri Adobe o Google
- Prepara le risorse che vengono visualizzate correttamente in dimensioni sottili
- È richiesto un solo campo immagine
- **non** utilizza immagini di sfondo incorporate o codificate
- Usa immagini di sfondo (campo `image`) caricate nell&#39;archivio dei contenuti di GenStudio for Performance Marketing
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

Consulta [Segnaposto di contenuto](/help/user-guide/content/customize-template.md#content-placeholders) per ulteriori informazioni sull&#39;utilizzo dei nomi dei campi nei modelli.

## Dimensioni supportate

È necessario impostare la larghezza x l&#39;altezza (pixel).

| Orientamento | Dimensioni (pixel) | Note |
|--------------|-------------------------------------------------------------|------------------------------------------------------------------|
| Verticale | 300 x 600<br>160 x 600 | Comune per grattacieli e banner a mezza pagina |
| Orizzontale | 300 x 250<br>728 x 90<br>336 x 280<br>320 x 50<br>970 x 250 | Classifica standard, rettangolo medio e dimensioni banner |
| Personalizzato | Da 50 x 50 a 2000 x 2000 | Utilizza per posizionamenti non standard o univoci; controlla i limiti della piattaforma |

<!-- Potentially add an example

## Template example

+++Example: Display ad template

+++

-->
