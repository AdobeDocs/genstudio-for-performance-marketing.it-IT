---
title: Preparare un modello di e-mail per Adobe GenStudio for Performance Marketing
description: Scopri come creare un modello e-mail personalizzato per Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Templates, Content
exl-id: 8b1e8d32-5a23-45ce-a2d4-ae6de3698c45
source-git-commit: ce08231cb723bec3d80a732837b72a435d3b552d
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# Preparare il modello e-mail per Adobe GenStudio for Performance Marketing

In genere, una finestra di progettazione crea la progettazione visiva di un modello in un programma di progettazione come Adobe XD. Dopo aver progettato, codificato e testato un modello e-mail, puoi prepararlo per il caricamento e l’utilizzo in GenStudio for Performance Marketing.

Vedi [Elementi modello](use-templates.md#template-elements).

## Aggiungi linee guida

Prima di preparare un Meta Ad Template, assicurati di aver aggiunto [linee guida](/help/user-guide/guidelines/overview.md) al tuo GenStudio for Performance Marketing e di averle compilate con informazioni complete per i brand rilevanti. Le [linee guida per il brand](/help/user-guide/guidelines/brands.md) influenzano direttamente i contenuti generati.

**Esempio**: se desideri che il corpo di un modello di posta elettronica non superi i 500 caratteri, aggiungi tale requisito alle [linee guida del canale](/help/user-guide/guidelines/brands.md#channel-guidelines) per il campo &quot;body&quot;.

Se non si aggiungono linee guida a GenStudio for Performance Marketing, vengono utilizzati i valori predefiniti.

## Codificare un modello e-mail

Dopo che un modello è stato progettato, viene codificato utilizzando HTML e CSS in linea. Il codice deve essere pulito e reattivo per vari dispositivi.

Vedi [Esempi di modelli](/help/user-guide/content/customize-template.md#template-examples).

### E-mail con più sezioni

È possibile utilizzare [prompt strutturati](/help/user-guide/effective-prompts.md#structured-prompts) durante la generazione del contenuto per istruire GenStudio for Performance Marketing a generare contenuti diversi per sezione di un messaggio e-mail.

Ad esempio, se le sezioni nel modello e-mail hanno il prefisso `Pod`—`Pod1` e `Pod2`, il prompt strutturato per la generazione del contenuto può includere direttive specifiche per tali sezioni e-mail. GenStudio for Performance Marketing corrisponde alla direttiva specifica della sezione nella richiesta inviata alla sezione e-mail correlata e genera contenuto allineato con le direttive.

Visualizza [prompt strutturati](/help/user-guide/effective-prompts.md#structured-prompts).

## Testare un modello e-mail

Utilizza la piattaforma di consegna e-mail o di verifica per testare l’e-mail e verificare che venga riprodotta correttamente tra client e dispositivi e-mail diversi.

Esegui un test per verificare che il modello e-mail soddisfi quanto segue:

* Il layout si adatta a diverse dimensioni dello schermo utilizzando query multimediali CSS
* È possibile fare clic sui pulsanti e passare alla posizione desiderata
* Il modello e-mail è leggibile e utilizzabile sui dispositivi mobili

## Definire le aree di contenuto generato

Definisci le aree nel modello e-mail che devono essere compilate dinamicamente con il contenuto di GenStudio for Performance Marketing.

Per definire le aree di contenuto generato:

* Identifica gli elementi di testo nel modello che GenStudio for Performance Marketing deve generare automaticamente, ad esempio il titolo o CTA.
* Adatta il modello di HTML inserendo segnaposto al suo interno utilizzando la sintassi Handlebars.

Vedi [Segnaposto contenuto](/help/user-guide/content/customize-template.md#content-placeholders).

## Visualizzare l’anteprima del modello

Controlla la visibilità di specifiche aree di contenuto con Helper integrati. Ad esempio, puoi includere parametri di tracciamento per i collegamenti in un modello esportato mantenendo collegamenti di anteprima puliti.

Vedi [Anteprima modello](/help/user-guide/content/customize-template.md#template-preview).

## Caricare e utilizzare il modello

Dopo aver progettato, codificato, testato e visualizzato in anteprima il modello, puoi caricarlo in GenStudio for Performance Marketing per utilizzarlo nella generazione di nuovi contenuti di marketing.

Vedi [Utilizzo dei modelli](use-templates.md).
