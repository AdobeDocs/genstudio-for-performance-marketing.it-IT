---
title: Linee guida per i modelli LinkedIn
description: Segui le best practice quando utilizzi i modelli LinkedIn con Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 85432185-8311-411b-b57b-f482c3d45854
TQID: https://experienceleague.adobe.com/YyG3WuMkdVAaACX03qLKzzw-fFA3WfT9K2ohjnQNPcI
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 242ab858144fd152fd55645143f869fddf7b6fe0
workflow-type: tm+mt
source-wordcount: 287
ht-degree: 2%

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

Consulta [Segnaposto di contenuto](/help/user-guide/templates/customize-template.md#content-placeholders) per ulteriori informazioni sull&#39;utilizzo dei nomi dei campi nei modelli.

## Proporzioni supportate

Tutte le larghezze dei modelli LinkedIn sono codificate a 1200 pixel.

| Proporzioni | Platform | Dimensioni (px) | Note |
|-------------------|-----------------|------------|-------------------------------------------------------------------------------------|
| Quadrato 1:1 | Desktop, dispositivi mobili | 1200 x 1200 | Più versatile. Ideale per un aspetto coerente tra dispositivi e posizionamenti. |
| Orizzontale 1,91:1 | Desktop | 1200 x 628 | Formato orizzontale standard. Comunemente utilizzato per contenuti sponsorizzati e annunci di news feed. |
| Verticale 1:1,91 | Dispositivi mobili | 1200 x 2292 | Formato verticale alto. Ottimizzato per la visualizzazione mobile, offre maggiore presenza sullo schermo. |
| Verticale 2:3 | Dispositivi mobili | 1200 x 1800 | Leggermente meno alto di 1:1,91. Ideale per le campagne mobile-first. |
| Verticale 4:5 | Dispositivi mobili | 1200 x 1500 | Consigliato per dispositivi mobili. Bilancia visibilità e contenuto, che spesso produce un impatto maggiore. |

<!-- 
Potentially add an example

## Template example

+++Example: LinkedIn template

+++

-->
