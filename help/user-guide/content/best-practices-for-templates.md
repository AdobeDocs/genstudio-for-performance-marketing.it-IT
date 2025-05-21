---
title: Best practice per i modelli
description: Segui le best practice per l’utilizzo dei modelli con Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates, Content Generation, Brand Personalization
exl-id: 3ff24fec-e836-4202-80f8-ba165e173b75
source-git-commit: dc958a831e3fa26cfc18f7c1a5febd0662102d43
workflow-type: tm+mt
source-wordcount: '982'
ht-degree: 0%

---

# Best practice per l’utilizzo dei modelli

I modelli riducono in modo significativo il tempo e l’impegno necessari per generare nuovi contenuti, fornendo un punto di partenza che include layout preconfigurati ed elementi di progettazione.

Utilizza i seguenti consigli quando utilizzi i modelli con GenStudio for Performance Marketing:

1. Informazioni su [elementi modello](#know-about-template-elements)
1. Configura le [linee guida per i canali](#configure-channel-guidelines) per una personalizzazione efficace dei contenuti
1. Progettazione con [standard di accessibilità](accessibility-for-templates.md) per un&#39;esperienza ottimale
1. Segui [linee guida per modelli specifici per canale](#follow-channel-specific-template-guidelines)

>[!TIP]
>
>Ulteriori informazioni sugli elementi e sulle procedure di base del modello in [Operazioni con i modelli](use-templates.md). Approfondisci [la personalizzazione di un modello](customize-template.md) da utilizzare nella prossima campagna.

## Informazioni sugli elementi del modello

Come best practice, è consigliabile acquisire familiarità con le parti di un modello. Ogni tipo di modello utilizza elementi diversi per creare una struttura per la creazione di contenuti specifici per il canale. Per personalizzare il modello, utilizza i nomi dei campi al posto di questi elementi in cui è necessario che GenStudio for Performance Marketing generi contenuto.

Vedi [Elementi modello](use-templates.md#template-elements).

## Configurare le linee guida per i canali

Configura le linee guida per il canale per ogni marchio prima di utilizzare i modelli in GenStudio for Performance Marketing. Le linee guida per il canale influenzano direttamente il tipo di contenuto generato quando si utilizza il modello. Ad esempio, puoi impostare i limiti dei caratteri per il corpo di un’e-mail.

![Specifiche del corpo](/help/assets/channel-email-body.png)

Consulta [linee guida per i canali](/help/user-guide/guidelines/brands.md#channel-guidelines).

## Segui le linee guida dei modelli specifiche per il canale

Quando crei i modelli, accertati che soddisfino i requisiti specifici del canale previsto. Crea modelli che soddisfino i requisiti di layout e di visualizzazione per ogni canale. Esistono linee guida generali applicabili a qualsiasi modello, ad esempio:

- Utilizzare HTML e CSS in linea puliti e reattivi
- Utilizzare i caratteri Adobe o Google
- **non** utilizza JavaScript

{{note-css-effects}}

Quando si lavora con ciascun tipo di modello, tenere presenti i suggerimenti e i vincoli riportati di seguito per garantire prestazioni e compatibilità ottimali.

>[!BEGINTABS]

>[!TAB E-mail]

Segui queste best practice per la progettazione quando personalizzi i modelli e-mail per l’utilizzo con GenStudio for Performance Marketing:

- Utilizzare i caratteri Adobe o Google
- Utilizzare HTML e CSS in linea puliti e reattivi
- **non** utilizza JavaScript
- **not** utilizza la larghezza fissa nel corpo o nel contenitore
- **not** utilizza la codifica base64 per le immagini perché può aumentare notevolmente le dimensioni del modello

**Vincoli**:

- Le e-mail di marketing possono avere 0, 2 o 3 [sezioni](customize-template.md#sections-or-groups):
   - Un modello di base (zero sezioni) può generare un singolo set di elementi modello, che non richiede la convenzione di denominazione del gruppo.
   - Un modello complesso (più sezioni) può generare fino a tre set di elementi modello, che richiedono l&#39;adesione alla convenzione di denominazione del gruppo: (`groupname_fieldname`)
- Il numero massimo di campi consentiti in un modello è 20
- La dimensione massima del file HTML è 102 KB

**Nomi di campi riconosciuti**:

Per l&#39;e-mail, il campo `subject` viene incluso automaticamente. Utilizza i segnaposto di contenuto per i campi seguenti:

- `pre_header` (Rich Text non abilitato)
- `headline`
- `sub_headline`
- `body`
- `cta`
- `image` (selezionato da Content JPEG, PNG o GIF)

Consulta [Segnaposto di contenuto](customize-template.md#content-placeholders) per ulteriori informazioni sull&#39;utilizzo dei nomi dei campi nei modelli.

>[!TAB Meta annuncio]

Segui queste best practice per la progettazione quando personalizzi i modelli di annunci multimediali per lavorare con GenStudio for Performance Marketing:

- Utilizza una larghezza di 360 pixel per i layout di colonna
- Risoluzione minima di 1080 x 1080 pixel per le immagini
- **non** utilizza la dimensione font relativa
- **non** definire il riquadro di visualizzazione
- **non** utilizza JavaScript
- **not** esegue l&#39;override di un elemento HTML nel CSS
- Utilizza il tag `<img>` invece di `background-image`
- Utilizza il mascheramento per migliorare la leggibilità del testo rispetto alle immagini di sfondo

**Vincoli**:

- Utilizzo di [sezioni](customize-template.md#sections-or-groups):
   - È possibile utilizzare una sola sezione, generando un singolo set di elementi modello.
- È richiesto un solo campo immagine.

**Proporzioni supportate**:

Le proporzioni devono essere impostate:

- Quadrato 1:1 (1080 x 1080 pixel)
- Verticale 4:5 (1080 x 1350 pixel)
- Storia 9:16 (1080 x 1920 pixel)
- Orizzontale: 1,91:1 (larghezza 1080 pixel)
- Dimensioni immagine personalizzate: (larghezza minima immagine 50 x 50 pixel)

**Nomi di campi riconosciuti**:

Per i metadati, i campi `headline`, `body` e `CTA` vengono generati automaticamente. Utilizza i segnaposto di contenuto per i campi seguenti:

- `image` (selezionato da Content JPEG, PNG o GIF)
- `on_image_text`

Consulta [Segnaposto di contenuto](customize-template.md#content-placeholders) per ulteriori informazioni sull&#39;utilizzo dei nomi dei campi nei modelli.

>[!TAB Banner e annuncio visualizzato]

Segui queste best practice per la progettazione quando personalizzi i modelli di banner e annunci display per lavorare con GenStudio for Performance Marketing:

- Utilizzare i caratteri Adobe o Google
- Prepara le risorse che vengono visualizzate correttamente in dimensioni sottili
- **non** utilizza immagini di sfondo incorporate o codificate
- Usa immagini di sfondo (campo `image`) caricate nell&#39;archivio dei contenuti di GenStudio for Performance Marketing
- **non** utilizza JavaScript

**Vincoli**:

- Utilizzo di [sezioni](customize-template.md#sections-or-groups):
   - È possibile utilizzare una sola sezione, generando un singolo set di elementi modello.
- È richiesto un solo campo immagine.

**Dimensioni supportate**:

- È necessario impostare la larghezza x l&#39;altezza (pixel)
- Verticale:
   - 300 x 600
   - 160 x 600 &#x200B;
- Orizzontale
   - 300 x 250
   - 728 x 90
   - 336 x 280
   - 320 x 50
   - 970 x 250 &#x200B;
- Personalizzato: da 50 x 50 a 2000 x 2000

**Nomi di campi riconosciuti**:

Per gli annunci tramite banner e display, il campo `CTA` viene generato automaticamente. Utilizza i segnaposto di contenuto per i campi seguenti:

- `headline`
- `sub_headline`
- `body`
- `image` (selezionato da Content JPEG, PNG o GIF)

Consulta [Segnaposto di contenuto](customize-template.md#content-placeholders) per ulteriori informazioni sull&#39;utilizzo dei nomi dei campi nei modelli.

>[!TAB Annuncio LinkedIn]

[!BADGE Beta]{type=Informative tooltip="Questa funzione è attualmente in Beta, quindi alcune funzionalità potrebbero essere limitate o soggette a modifiche."}

Segui queste best practice per la progettazione quando personalizzi i modelli di annunci LinkedIn per lavorare con GenStudio for Performance Marketing:

**Vincoli**:

- Utilizzo di [sezioni](customize-template.md#sections-or-groups):
   - È possibile utilizzare una sola sezione, generando un singolo set di elementi modello.
- È richiesto un solo campo immagine.
- Dimensione massima dell&#39;immagine: 5 MB
- Massimo 70 caratteri per titolo
- Testo introduttivo massimo 150 caratteri

**Proporzioni supportate**:

- Quadrato 1:1
   - desktop o dispositivo mobile
   - Min: 360 x 360 pixel
   - Max: 4320 x 4320 pixel
- Orizzontale 1,91:1
   - desktop
   - Min: 640 x 360 pixel
   - Max: 7680 x 4320 pixel
- Verticale 1:1,91
   - mobile
   - Min: 360 x 640 pixel
   - Max: 2430 x 4320 pixel
- Verticale 2,3
   - mobile
   - Min: 360 x 640 pixel
   - Max: 2430 x 4320 pixel
- Verticale 4,5 (consigliato)
   - mobile
   - Min: 360 x 640 pixel
   - Max: 2430 x 4320 pixel

**Nomi di campi riconosciuti**:

Per gli annunci LinkedIn, i campi `headline`, `introductory_text` e `CTA` vengono generati automaticamente. Utilizza i segnaposto di contenuto per i campi seguenti:

- `image` (selezionato da Content JPEG, PNG o GIF)
- `on_image_text`

Consulta [Segnaposto di contenuto](customize-template.md#content-placeholders) per ulteriori informazioni sull&#39;utilizzo dei nomi dei campi nei modelli.

>[!ENDTABS]
