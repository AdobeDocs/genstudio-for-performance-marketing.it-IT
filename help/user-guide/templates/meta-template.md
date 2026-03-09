---
title: Linee guida per il modello di annunci Meta
description: Segui le best practice quando utilizzi i modelli di annunci Meta con Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: e69039b0-272d-4f39-b0e4-916be710fd5f
TQID: https://experienceleague.adobe.com/-WHH1xjWFaizXTKjuF-K9UtaR12V3QpMezSqRfwbMIU
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
subfeature_v2:
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 376
ht-degree: 1%

---

# Linee guida per i modelli di annunci Meta

I modelli di annunci Meta consentono di creare annunci coerenti ed efficaci dal punto di vista visivo per le piattaforme Meta. Seguendo le procedure di progettazione consigliate e utilizzando i campi supportati, puoi garantire che i modelli siano ottimizzati per GenStudio for Performance Marketing. Questa guida spiega come strutturare, personalizzare e preparare modelli di annunci Meta per un’integrazione fluida e risultati di forte impatto.

Segui queste best practice per la progettazione quando personalizzi i modelli di annunci Meta per lavorare con GenStudio for Performance Marketing:

- Utilizza una larghezza di 360 pixel per i layout di colonna
- Risoluzione minima di 1080 x 1080 pixel per le immagini
- È richiesto un solo campo immagine
- **non** utilizza la dimensione font relativa
- **non** definire il riquadro di visualizzazione
- **non** utilizza JavaScript
- **not** esegue l&#39;override di un elemento HTML nel CSS
- Utilizza il tag `<img>` invece di `background-image`
- Utilizza il mascheramento per migliorare la leggibilità del testo rispetto alle immagini di sfondo
- È possibile utilizzare una sola sezione, generando un singolo set di elementi modello

## Nomi di campi riconosciuti

Quando personalizzi il modello di annunci Meta, applica segnaposto di contenuto per i campi obbligatori:

- `image` (obbligatorio, selezionato da Content JPEG, PNG o GIF)
- `on_image_text` (testo visualizzato sopra l&#39;immagine)

GenStudio for Performance Marketing genera automaticamente i campi seguenti. Non è necessario applicare segnaposto di contenuto per:

- `headline`
- `body`
- `cta`

Consulta [Segnaposto di contenuto](/help/user-guide/templates/customize-template.md#content-placeholders) per ulteriori informazioni sull&#39;utilizzo dei nomi dei campi nei modelli.

## Proporzioni supportate

| Proporzioni | Dimensioni (pixel) | Note |
|------------------|----------------------------|-----------------------------------------------------------------------|
| Quadrato 1:1 | 1080 x 1080 | Standard per la maggior parte dei posizionamenti Meta; consigliato per un’ampia compatibilità. |
| Verticale 4:5 | 1080 x 1350 | Ottimizzato per feed mobili; fornisce più spazio verticale. |
| Storia 9:16 | 1080 x 1920 | Ideale per storie e rulli; riempie l&#39;intero schermo mobile. |
| Orizzontale 1.91:1 | 1080 x 566 | Consigliato per annunci di collegamento e posizionamenti di feed di notizie; formato ampio. |
| Personalizzato | Minimo 50 x 50 (larghezza) | Usare solo se necessario; può causare ritaglio o ridimensionamento. |

Se l’annuncio non è progettato in uno di questi rapporti di formato, GenStudio for Performance Marketing ritaglia automaticamente l’immagine nelle dimensioni appropriate.

## Esempio di modello

+++Esempio: modello di annuncio Meta

<!-- Does this need to be a precise size? -->

Di seguito è riportato un esempio di base di un modello di annuncio Meta. L’intestazione contiene CSS in linea per lo stile. Il corpo utilizza [segnaposto contenuto](#content-placeholders), ad esempio `image` e `on_image_text`, per indicare dove GenStudio for Performance Marketing può generare il contenuto.

```html {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title>Adobe</title>
        <style>
            .ad-container {
            font-family: Helvetica, sans-serif;
            position: relative;
            text-align: center;
            height: 100%;
            }
            .ad-image {
            width: 100%;
            height: 100%;
            object-fit: cover;
            }
            .ad-text {
            position: absolute;
            top: 0;
            left: 0;
            margin: 1em;
            background-color: rgba(0, 0, 0, 0.5);
            color: white;
            padding: 1em;
            font-size: 75px;
            }
        </style>
    </head>
    <body>
        <div class="ad-container">
            <img src="{{image}}" alt="Ad Image" class="ad-image" />
            <div class="ad-text">{{on_image_text}}</div>
        </div>
    </body>
</html>
```

+++
