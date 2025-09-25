---
title: Linee guida per il modello di annunci Meta
description: Segui le best practice quando utilizzi i modelli di annunci Meta con Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: e69039b0-272d-4f39-b0e4-916be710fd5f
source-git-commit: c0f45fb0ffc61d20611693498f1b12d3946ca6ca
workflow-type: tm+mt
source-wordcount: '375'
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

Consulta [Segnaposto di contenuto](/help/user-guide/content/customize-template.md#content-placeholders) per ulteriori informazioni sull&#39;utilizzo dei nomi dei campi nei modelli.

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
