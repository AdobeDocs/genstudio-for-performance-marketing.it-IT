---
title: Linee guida per i modelli LinkedIn
description: Segui le best practice quando utilizzi i modelli LinkedIn con Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
source-git-commit: 35a519a8d28e260bfa6d9ed671bd5bf1cfeda931
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 1%

---

# Linee guida per i modelli LinkedIn

I modelli LinkedIn offrono un modo strutturato per creare e personalizzare contenuti pubblicitari per le campagne LinkedIn. Queste linee guida garantiscono che gli annunci soddisfino le specifiche di LinkedIn semplificando al contempo il processo creativo in GenStudio for Performance Marketing. Questa guida ti aiuta a prepararti per un branding coerente e prestazioni efficaci sulle piattaforme desktop e mobili di LinkedIn.

Segui queste best practice per la progettazione quando personalizzi i modelli di annunci LinkedIn per lavorare con GenStudio for Performance Marketing:

- È richiesto un solo campo immagine
- Dimensione massima dell&#39;immagine: 5 MB
- Massimo 70 caratteri per titolo
- Testo introduttivo massimo 150 caratteri
- È possibile utilizzare una sola sezione, generando un singolo set di elementi modello

## Nomi di campi riconosciuti

Quando personalizzi il modello LinkedIn, applica segnaposto di contenuto per i campi obbligatori seguenti:

- `image` (obbligatorio, selezionato da Content JPEG, PNG o GIF)
- `on_image_text` (testo visualizzato sopra l&#39;immagine)

GenStudio for Performance Marketing genera automaticamente i campi seguenti. Non è necessario applicare segnaposto di contenuto per:

- `headline`
- `introductory_text`
- `cta` (Call to action)

Consulta [Segnaposto di contenuto](/help/user-guide/content/customize-template.md#content-placeholders) per ulteriori informazioni sull&#39;utilizzo dei nomi dei campi nei modelli.

## Proporzioni supportate

| Proporzioni | Platform | Dimensioni minime (px) | Dimensione massima (px) | Note |
|-------------------|-----------------|---------------|----------------|-------------------------------------------------------------------------------------|
| Quadrato 1:1 | Desktop, dispositivi mobili | 360 x 360 | 4320 x 4320 | Più versatile. Ideale per un aspetto coerente tra dispositivi e posizionamenti. |
| Orizzontale 1,91:1 | Desktop | 640 x 360 | 7680 x 4320 | Formato orizzontale standard. Comunemente utilizzato per contenuti sponsorizzati e annunci di news feed. |
| Verticale 1:1,91 | Dispositivi mobili | 360 x 640 | 2430 x 4320 | Formato verticale alto. Ottimizzato per la visualizzazione mobile, offre maggiore presenza sullo schermo. |
| Verticale 2:3 | Dispositivi mobili | 360 x 640 | 2430 x 4320 | Leggermente meno alta di 1:1.91. Ideale per le campagne mobile-first. |
| Verticale 4:5 | Dispositivi mobili | 360 x 640 | 2430 x 4320 | Consigliato per dispositivi mobili. Bilancia visibilità e contenuto, che spesso produce un impatto maggiore. |

<!-- Potentially add an example

## Template example

+++Example: LinkedIn template

+++

-->
