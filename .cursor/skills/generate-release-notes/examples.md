---
source-git-commit: c9b8177a564cfcdfd2b63cd28fa22eb93a52d3a7
workflow-type: tm+mt
source-wordcount: '80'
ht-degree: 0%

---
# Esempi di note sulla versione

Modelli pronti per l&#39;incollamento per [help/user-guide/release-notes.md](../../help/user-guide/release-notes.md). Abbina tono e struttura al file circostante.

## Esempio di frontmatter minimo (solo nuova pagina)

Da usare solo quando **si crea** una nuova pagina di note sulla versione da zero. Se il file esiste già, conservarne l&#39;intera parte anteriore.

```yaml
---
title: Adobe GenStudio for Performance Marketing release notes
description: Learn about the latest features and enhancements to Adobe GenStudio for Performance Marketing.
recommendations: noDisplay
role: User
exl-id: 32f5104e-ae15-4092-8a34-642fc641baf9
---
```

## Sezione delle funzioni (con Beta)

```markdown
### Generative Expand AI functionality

[!BADGE Beta]{type=Informative tooltip="This feature is currently in Beta, so some functionality may be limited or subject to change."}

Now, in GenStudio for Performance Marketing [!DNL Create] you can use [Generative Expand AI capabilities](/help/user-guide/create/manage-variants.md#use-generative-expand) to expand the dimensions of images and add generative content to fit your ad templates in paid media variants.
```

## Sezione sulle funzioni (collegamento alla documentazione in prosa)

```markdown
### Compatible assets filter

A new filter in the [!DNL Insights] module automatically hides [unsupported image and video assets](/help/user-guide/insights/published-experiences.md#ad-formats) from ad previews, eliminating visual clutter and broken tiles. This enhancement ensures users only see media that's actually available and ready to use, creating a cleaner and more reliable experience.
```

## Correzioni e miglioramenti (punti elenco)

```markdown
### Fixes and enhancements

* Added support for [publishing ad experiences](/help/user-guide/activation/activate-linkedin-ad.md) from GenStudio for Performance Marketing into LinkedIn Campaign Manager. [!DNL Activate] supports detailed LinkedIn ad previews before publishing to LinkedIn Campaign Manager.
```

Utilizzare questa sottosezione solo per gli elementi **con etichetta esplicita** correzione o miglioramento nel materiale di origine.

## Blocco archiviato (note sulla versione precedenti)

```markdown
+++Notes from 2025.05.15

### Fixes and enhancements

* Enabled functionality for [adding alternative (alt) text](/help/user-guide/create/manage-variants.md#add-alt-text-for-images) to an image for an individual variant.
* Added a [new Meta aspect ratio](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines) —Landscape 1.19:1 (1080 pixel width).
* Now you can choose more than one experience for export or download. See [Export experiences](/help/user-guide/content/manage-assets.md#export-experiences).

+++
```
