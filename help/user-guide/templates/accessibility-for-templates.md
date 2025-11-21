---
title: Creare modelli accessibili
description: Crea in Adobe GenStudio for Performance Marketing modelli in grado di raggiungere più tipi di pubblico e fornire un’esperienza ottimale.
feature: Media Templates
exl-id: eaaa5d9f-ad45-4fd0-826d-c250deb6d238
source-git-commit: 9e51e853542d20f0b90b10071f4f26aaae1d6aad
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 0%

---

# Creare modelli accessibili

Adobe si impegna a fornire un’esperienza ottimale per tutti i tipi di pubblico. Consulta [Iniziative per l&#39;accessibilità in Adobe](https://www.adobe.com/trust/accessibility/initiatives.html) per ulteriori informazioni.

In GenStudio for Performance Marketing, puoi caricare risorse e modelli che consentono la creazione di contenuti per diverse esperienze. Il rispetto degli standard di accessibilità consente ai contenuti di raggiungere il pubblico desiderato.

Utilizza i consigli seguenti per preparare i modelli utilizzando standard di accessibilità ottimali.

## Testo alternativo

Fornisci alternative testuali per il contenuto non testuale, ad esempio le immagini.

```html
<img alt="Collage of ideas, books, man holding giant pencil, computer" src="card-create-assets.png">
```

![Collage di idee, libri, uomo con matita gigante, computer](/help/assets/card-create-assets.png){width="400"}

Durante la personalizzazione del modello, utilizzare i segnaposto di contenuto per gli attributi `alt` e `aria-label`:

- [Testo alternativo](/help/user-guide/templates/customize-template.md#alternative-text)
- [Etichetta di accessibilità](/help/user-guide/templates/customize-template.md#accessibility-label)

## Font

Utilizza caratteri di facile lettura. Ad esempio, i font Sans Serif hanno un aspetto pulito, simile a un blocco, che contribuisce a una maggiore leggibilità.

Fornire un contrasto appropriato tra testo e sfondo. Evitare di utilizzare colori di carattere che producono testo scuro su uno sfondo scuro e testo chiaro su uno sfondo chiaro. Considera le linee guida di contrasto per un rapporto ottimale:

- Testo e immagini di testo: rapporto di contrasto di almeno 4,5:1
- Testo e immagini di grandi dimensioni di testo: rapporto di contrasto di almeno 3:1

## Scopo collegamento (solo collegamento)

Crea un testo di collegamento chiaro che descriva lo scopo e la posizione del collegamento.

Ad esempio, l’utilizzo di testo di collegamento come &quot;Fai clic qui&quot; o &quot;Ulteriori informazioni&quot; non descrive chiaramente lo scopo del collegamento:

```html
<a href="product-site.html">Click here</a>
```

Come best practice, utilizza un testo che descriva chiaramente dove va il collegamento. Un esempio migliore potrebbe utilizzare il titolo della sorgente del collegamento e lo scopo:

```html
<a href="product-site.html">Explore Product Site</a>
```

## Lingua

Molti prodotti e servizi utilizzano il linguaggio in modo creativo o univoco. Evita il gergo, le frasi lunghe e le frasi complesse. Utilizza un linguaggio chiaro, conciso e di facile lettura compatibile con il tuo pubblico di destinazione.

- Se possibile, utilizza descrizioni chiare, definizioni in linea o esempi correlati. Può essere difficile tradurre un vernacolo unico.

- Scrivi o collega a una definizione per le prime istanze di un acronimo o di un’abbreviazione. Può essere difficile tradurre le abbreviazioni.

- Se possibile, utilizza elementi visivi per integrare il testo o le idee complesse.
