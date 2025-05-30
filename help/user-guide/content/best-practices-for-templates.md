---
title: Best practice per i modelli
description: Segui le best practice per l’utilizzo dei modelli con Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates, Content Generation, Brand Personalization
exl-id: 3ff24fec-e836-4202-80f8-ba165e173b75
source-git-commit: adf987b016825861b5522b44b61263000eb63859
workflow-type: tm+mt
source-wordcount: '386'
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

Definire linee guida chiare per il canale è essenziale per garantire che i contenuti generati siano in linea con i requisiti e gli obiettivi del tuo marchio. Le linee guida per il canale consentono di specificare regole per elementi quali il tono, la lunghezza e lo stile utilizzati nel modello. Ad esempio, puoi impostare un numero massimo di caratteri per il corpo o richiedere uno stile call-to-action specifico. Impostando queste linee guida in anticipo, riduci la necessità di scrivere istruzioni dettagliate in ogni prompt di IA, semplificando il processo di generazione dei contenuti e garantendo coerenza nelle e-mail.

Rivedi e definisci le [linee guida per il canale](/help/user-guide/guidelines/brands.md#channel-guidelines) del tuo marchio per tutti i campi chiave nel modello. Se non definisci le linee guida, vengono applicate le [linee guida per il canale predefinite](/help/user-guide/guidelines/brands.md#default-channel-guidelines), che potrebbero non riflettere completamente i requisiti del brand.

![Specifiche del corpo](/help/assets/channel-email-body.png)

Scopri in che modo [Marchi, Prodotti e Linee guida per Personas](/help/user-guide/guidelines/overview.md) influenzano i contenuti generati e come adattarli agli obiettivi di marketing.

## Segui le linee guida dei modelli specifiche per il canale

Quando crei i modelli, accertati che soddisfino i requisiti specifici del canale previsto. Crea modelli che soddisfino i requisiti di layout e di visualizzazione per ogni canale. Esistono linee guida generali applicabili a qualsiasi modello, ad esempio:

- Utilizzare HTML e CSS in linea puliti e reattivi
- Utilizzare i caratteri Adobe o Google
- **non** utilizza JavaScript

{{note-css-effects}}

Per prestazioni e compatibilità ottimali, consulta ulteriori suggerimenti e vincoli durante l’utilizzo di ciascun tipo di modello:

- [E-mail](/help/user-guide/templates/email-template.md)
- [Visualizzazione e banner pubblicitari](/help/user-guide/templates/display-template.md)
- [LinkedIn](/help/user-guide/templates/linkedin-template.md)
- [Meta annunci](/help/user-guide/templates/meta-template.md)
