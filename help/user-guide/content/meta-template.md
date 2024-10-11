---
title: Preparare un Meta Ad Template per Adobe GenStudio for Performance Marketing
description: Scopri come creare un Meta Ad Template personalizzato per Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Templates, Content
exl-id: e69039b0-272d-4f39-b0e4-916be710fd5f
source-git-commit: 478815d74a742cdc05d3f1faebf27d5adc04d417
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# Preparare il Meta Ad Template per Adobe GenStudio for Performance Marketing

La creazione di un modello di metadati implica un approccio strutturato personalizzato per i social media. Dopo aver progettato e testato un modello di Meta Ad, puoi prepararlo per il caricamento e l’utilizzo in GenStudio for Performance Marketing.

## Aggiungi linee guida

Prima di preparare un Meta Ad Template, assicurati di aver aggiunto [linee guida](/help/user-guide/guidelines/overview.md) al tuo GenStudio for Performance Marketing e di averle compilate con informazioni complete per i brand rilevanti. Le [linee guida per il brand](/help/user-guide/guidelines/brands.md) influenzano direttamente i contenuti generati.

**Esempio**: se desideri che il corpo di un modello di annunci multimediali non superi i 500 caratteri, aggiungi tale requisito alle [linee guida per i canali](/help/user-guide/guidelines/brands.md#channel-guidelines) per il campo &quot;body&quot;.

Se non si aggiungono linee guida a GenStudio for Performance Marketing, vengono utilizzati i valori predefiniti.

## Progettare un modello

In genere, una finestra di progettazione crea la progettazione visiva di un modello in un programma di progettazione come Adobe XD.

Vedi [Elementi modello](use-templates.md#template-elements) e [Esempi modello](/help/user-guide/content/customize-template.md#template-examples).

### Specifiche dell’annuncio

GenStudio for Performance Marketing supporta le seguenti proporzioni per gli annunci Meta:

* Quadrato (1:1): 1080 x 1080 pixel
* Verticale (4:5): 1080 x 1350 pixel
* Storia (9:16): 1080 x 1920 pixel

Se l’annuncio non è progettato in uno di questi rapporti di formato, GenStudio for Performance Marketing ritaglia automaticamente l’immagine nelle dimensioni appropriate.

## Testare un modello di metadati

Prova il modello utilizzando il Creative Hub di Meta per vedere come si presenta l’annuncio in posizionamenti diversi, ad esempio in un feed o come una storia.

Utilizza la piattaforma di consegna e-mail o di verifica per testare l’e-mail e verificare che venga riprodotta correttamente tra client e dispositivi e-mail diversi.

## Definire le aree di contenuto generato

Definisci le aree nel modello e-mail che devono essere compilate dinamicamente con il contenuto di GenStudio for Performance Marketing.

Per definire le aree di contenuto generato:

* Identifica gli elementi di testo nel modello che GenStudio for Performance Marketing deve generare automaticamente, ad esempio il titolo o CTA.
* Adatta il modello di HTML inserendo segnaposto al suo interno utilizzando la sintassi Handlebars.

Vedi [Segnaposto contenuto](/help/user-guide/content/customize-template.md#content-placeholders).

## Visualizzare l’anteprima del modello

Controlla la visibilità di specifiche aree di contenuto con Helper integrati. Ad esempio, includi i parametri di tracciamento per i collegamenti in un modello esportato mantenendo collegamenti di anteprima puliti.

Vedi [Anteprima modello](/help/user-guide/content/customize-template.md#template-preview).

## Caricare e utilizzare il modello

Dopo aver progettato, codificato, testato e visualizzato in anteprima il modello, caricalo in GenStudio for Performance Marketing per utilizzarlo nella generazione di nuovi contenuti di marketing.

Vedi [Utilizzo dei modelli](use-templates.md).
