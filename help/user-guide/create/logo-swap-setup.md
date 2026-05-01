---
title: Configurare lo scambio di logo nei modelli
description: Configura i segnaposto del logo del brand nei modelli per abilitare lo scambio di logo in [!DNL GenStudio for Performance Marketing].
feature: Create Canvas
role: User
level: Intermediate
source-git-commit: 98cb7ba338878495e6d7b68f3b8c620abae10127
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 2%

---

# Configurare lo scambio di logo nei modelli

In questa guida viene illustrato come configurare i segnaposto per i logo del brand nei modelli per abilitare la [funzionalità di scambio logo](/help/user-guide/create/logo-swap.md) in [!DNL GenStudio for Performance Marketing]. Utilizza queste linee guida per garantire che il segnaposto venga visualizzato correttamente nelle varie dimensioni e proporzioni dell’immagine.

## Configurazione rapida

Utilizza il seguente codice modello di base per l&#39;immagine del logo:

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="my-logo"
>
```

Obbligatorio:

- `src="{{brand_logo}}"` - Abilita la funzionalità di scambio logo.
- `style="{{defaultLogo}}"` - Applica lo stile del bordo segnaposto.

Facoltativo:

- `class="my-logo"`—La classe CSS personalizzata per il dimensionamento e lo stile.

## Comprendere il bordo segnaposto

Se non è selezionato alcun logo, `{{brand_logo}}` contiene un&#39;immagine trasparente da 1×1 pixel. Lo stile `{{defaultLogo}}` applica automaticamente una struttura in modo che il segnaposto sia visibile:

```css
outline: clamp(1px, 0.1em, 5px) dashed #FFF;
```

Comportamento bordo:

- Viene visualizzato quando viene visualizzato il segnaposto predefinito.
- Scompare automaticamente dopo lo scambio di un logo.
- Ridimensiona in base alla dimensione del carattere padre.

### Ridimensionamento bordo

La funzione `clamp()` adatta lo spessore della struttura alle dimensioni del modello:

| Dimensione font principale | Dimensione struttura |
| --- | --- |
| 10px | 1 px (min) |
| 16px | 1.6px |
| 24px | 2.4px |
| 32px | 3.2px |
| 50px+ | 5 px (max) |

Formula: `0.1em` è uguale al 10% della dimensione del carattere ereditato, bloccata tra `1px` e `5px`.

## Personalizzare il bordo segnaposto

È possibile modificare la struttura predefinita utilizzando le classi CSS. Lo stile `{{defaultLogo}}` applica il profilo di base e la classe può personalizzare colore, larghezza e stile.

HTML modello:

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-custom-border"
>
```

CSS modello:

```css
.logo-custom-border {
  outline-color: #0066CC !important;
  outline-width: 2px !important;
  outline-style: dotted !important;
}
```

>[!NOTE]
>Gli stili di struttura personalizzati influiscono solo sul segnaposto. Una volta scambiato il logo, tutti gli stili di struttura vengono rimossi automaticamente.

## Imposta dimensioni logo consigliate

Per garantire che il segnaposto sia visibile e impedisca spostamenti del layout, imposta il dimensionamento esplicito nella classe CSS:

HTML modello:

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-standard"
>
```

CSS modello:

```css
.logo-standard {
  width: 120px;
  height: 60px;
}
```

## Controllo del posizionamento del logo

Utilizza `object-fit` e `object-position` per controllare il ridimensionamento del logo all&#39;interno del relativo contenitore.

### Logo centrato (più comune)

Il logo viene ridimensionato in modo da rientrare in 150×80 pixel, centrato sia orizzontalmente che verticalmente.

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-centered"
>
```

```css
.logo-centered {
  width: 150px;
  height: 80px;
  object-fit: contain;
  object-position: center center;
}
```

### Logo allineato a sinistra

Il logo viene ridimensionato per adattarsi, allineato al bordo sinistro, centrato verticalmente.

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-left"
>
```

```css
.logo-left {
  width: 200px;
  height: 60px;
  object-fit: contain;
  object-position: left center;
}
```

### Logo in alto a destra

Il logo viene adattato in scala, posizionato nell&#39;angolo superiore destro.

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-top-right"
>
```

```css
.logo-top-right {
  width: 100px;
  height: 100px;
  object-fit: contain;
  object-position: right top;
}
```

## Esempi completi

### Configurazione minima

```html
<img src="{{brand_logo}}" style="{{defaultLogo}}">
```

>[!NOTE]
>Questa impostazione funziona, ma il segnaposto potrebbe essere quasi invisibile perché l&#39;immagine trasparente da 1×1 pixel si riduce alle dimensioni naturali. Utilizza una classe CSS con `width` e `height` per un segnaposto visibile.

### Configurazione consigliata

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="brand-logo"
>
```

```css
.brand-logo {
  width: 120px;
  height: 60px;
  object-fit: contain;
  object-position: center center;
}
```

### Configurazione avanzata con bordo personalizzato

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="sponsor-logo"
>
```

```css
.sponsor-logo {
  width: 180px;
  height: 90px;
  object-fit: contain;
  object-position: left center;
  outline-color: #0066CC !important;
  outline-width: 2px !important;
  outline-style: solid !important;
}
```

### Configurazione flessibile con limiti di dimensione

Utilizza le proprietà `min-*` e `max-*` per i modelli reattivi o per dimensioni logo diverse.

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-flexible"
>
```

```css
.logo-flexible {
  min-width: 20px;
  min-height: 20px;
  max-width: 200px;
  max-height: 100px;
  object-fit: contain;
  object-position: center center;
}
```

Come funziona:

- `min-width` e `min-height` mantengono visibile il segnaposto.
- `max-width` e `max-height` impediscono ai logo sovradimensionati di interrompere il layout.
- Il logo viene ridimensionato proporzionalmente all&#39;interno di questi limiti.

## Riferimento proprietà CSS

| Categoria | Proprietà | Valore | Scopo |
| --- | --- | --- | --- |
| Obbligatorio (HTML) | `src` | `{{brand_logo}}` | Abilita la funzionalità di scambio dei logo. |
| Obbligatorio (HTML) | `style` | `{{defaultLogo}}` | Applica il profilo del segnaposto. |
| Consigliato (classe CSS) | `width` | `120px` | Imposta la larghezza massima del logo. |
| Consigliato (classe CSS) | `height` | `60px` | Imposta l&#39;altezza massima del logo. |
| Consigliato (classe CSS) | `object-fit` | `contain` | Ridimensiona il logo senza ritagliarlo. |
| Consigliato (classe CSS) | `object-position` | `center center` | Controlla l&#39;allineamento del logo. |
| Facoltativo (classe CSS) | `outline-color` | `#FF0000` | Cambia il colore del contorno. |
| Facoltativo (classe CSS) | `outline-width` | `3px` | Modifica lo spessore del profilo. |
| Facoltativo (classe CSS) | `outline-style` | `solid` | Modifica lo stile della struttura. |
| Dimensionamento flessibile (classe CSS) | `min-width` | `20px` | Garantisce la visibilità dei segnaposto. |
| Dimensionamento flessibile (classe CSS) | `min-height` | `20px` | Garantisce la visibilità dei segnaposto. |
| Dimensionamento flessibile (classe CSS) | `max-width` | `200px` | Impedisce l&#39;overflow. |
| Dimensionamento flessibile (classe CSS) | `max-height` | `100px` | Controlla i limiti del layout. |

## Best practice

Effettua:

- Includi sempre `{{brand_logo}}` e `{{defaultLogo}}`.
- Definisci `width` e `height` in modo che il segnaposto sia visibile.
- Utilizza le classi CSS per ridimensionare e personalizzare la struttura.
- Utilizza `object-fit: contain` per mantenere le proporzioni del logo.
- Prova con logo di dimensioni e rapporti di formato diversi.

Non:

- Utilizza `border` invece di `outline` (il bordo non si nasconderà automaticamente).
- Inserisci le proprietà di ridimensionamento negli stili in linea.
- Ometti i vincoli di dimensione (il segnaposto esegue il rendering a 1×1 pixel).
- Utilizza `object-fit: cover` (potrebbe tagliare i loghi).

## Risoluzione dei problemi

Bordo non visibile:

- Assicurarsi che `style="{{defaultLogo}}"` sia incluso.
- Verificare che `width` e `height` siano definiti nella classe CSS.

Segnaposto troppo piccolo (1 px):

- Aggiungi `width` e `height` espliciti alla classe CSS.

Il bordo non scompare dopo lo scambio:

- Utilizzare le proprietà di struttura nella classe CSS, non `border`.

Il logo viene ritagliato:

- Utilizza `object-fit: contain` invece di `cover`.

Logo troppo piccolo o troppo grande:

- Regola `width` e `height` nella classe CSS.

Bordo personalizzato non visualizzato:

- Conferma `{{defaultLogo}}` nell&#39;attributo `style`.
- Inserisci proprietà `outline-*` personalizzate nella classe CSS.
