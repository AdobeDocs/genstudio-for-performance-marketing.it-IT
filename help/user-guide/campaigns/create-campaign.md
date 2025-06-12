---
title: Campagne Adobe GenStudio for Performance Marketing
description: Scopri come creare e gestire campagne di marketing digitale che sfruttano risorse ed esperienze di IA generativa.
feature: Campaign Planning, Campaign Brief
badgeBeta: label="Beta" tooltip="Questa funzione è attualmente in Beta, quindi alcune funzionalità potrebbero essere limitate o soggette a modifiche."
exl-id: b7c4194f-fa61-4739-acd6-7acbdd98e9b2
source-git-commit: 5279caaf4651ed81c3cf3d8a4de2f17c3f151ec8
workflow-type: tm+mt
source-wordcount: '859'
ht-degree: 0%

---

# Creare una campagna

Una campagna GenStudio for Performance Marketing definisce le caratteristiche chiave delle campagne digitali ed evolve man mano che le fasi vengono distribuite e valutate. GenStudio for Performance Marketing supporta il processo dinamico di avvio di una campagna, tracciamento delle prestazioni dei singoli componenti della campagna e ridefinizione delle esperienze pubblicitarie in base a metriche delle prestazioni.

Gli elementi chiave della campagna sono memorizzati in un oggetto campagna, che crea un contesto condiviso per tutte le risorse ed esperienze etichettate con lo stesso nome campagna univoco. Questa etichetta identifica la campagna in GenStudio for Performance Marketing.

I responsabili di sistema di GenStudio e gli editor di GenStudio possono creare campagne.

## Definire i dettagli della campagna

{{$include /help/_includes/campaign-details.md}}

**Per immettere i dettagli della campagna**:

1. Da [!DNL Campaigns], fai clic su **[!UICONTROL Aggiungi campagna]**. Verrà aperta la visualizzazione _Crea campagna_.

   I dettagli includono campi facoltativi e obbligatori che definiscono la campagna. Questi dettagli vengono salvati in [!DNL Campaigns] come attributi di metadati della campagna.

1. Fai doppio clic sull&#39;intestazione _Nuova campagna_ e immetti un nome informativo e univoco.

   Questo nome diventa una _etichetta campagna_ in GenStudio for Performance Marketing e consente di associare risorse o esperienze alla campagna durante il caricamento e la creazione.

1. Immetti i valori nei campi _Dettagli_ che descrivono la campagna. Consulta la tabella _Dettagli campagna_ per le definizioni di queste funzioni della campagna.

## Assegna canali e aree geografiche

Le impostazioni relative al canale e all’area geografica determinano dove viene distribuita la campagna e i relativi canali di distribuzione.

GenStudio for Performance Marketing utilizza modelli predefiniti denominati _record_ per rappresentare componenti chiave della campagna, quali canali, aree geografiche, utenti tipo e prodotti. Quando crei una campagna, la associ ai record rilevanti per ciascuno di questi componenti.

* **Impostazioni canale**—Definisce i canali di distribuzione pubblici per la campagna, inclusi gli account multimediali a pagamento, i servizi di marketing e-mail e le reti di annunci di visualizzazione. I dati sulle prestazioni di campagne, risorse ed esperienze in questi canali vengono inseriti in [[!DNL Insights]](/help/user-guide/insights/overview.md) per l&#39;analisi specifica del canale.

* **Impostazioni area geografica** - Specifica le aree geografiche in cui distribuire la campagna. Collegandosi a fonti di dati regionali, GenStudio for Performance Marketing può adattare contenuti e strategia alle preferenze del pubblico locale. Questo consente di eseguire il targeting e l’analisi delle prestazioni in modo più preciso in base a metriche regionali.

**Per selezionare i canali di distribuzione per la campagna**:

1. Fai clic sul segno + (**[!UICONTROL Connetti record +]**) accanto a **[!UICONTROL Canali]**.

   Viene aperto il popup _Seleziona canali_.

1. Seleziona i canali su cui viene distribuita la campagna. I valori validi includono `Email`, `Paid media`, `Web` e `Display ads`.

   Facoltativamente, scegliere **[!UICONTROL Visualizza tutto]** per aprire una visualizzazione di tutti i canali supportati.

**Per assegnare aree alla campagna**:

1. Fai clic sul segno + (**[!UICONTROL Connetti record +]**) accanto a **[!UICONTROL Aree geografiche]**.

   Viene aperto il popup _Seleziona aree_. Puoi cercare una specifica area supportata.

1. Seleziona le aree una o più aree di destinazione per la campagna. Le aree valide includono `AMER`, `LATAM`, `EMEA`, `APAC` e `Japan`.

   Facoltativamente, scegliere **[!UICONTROL Visualizza tutto]** per aprire una visualizzazione di tutte le aree supportate.

## Assegnare utenti tipo e prodotti

[Gli utenti tipo](/help/user-guide/guidelines/personas.md) e [prodotti](/help/user-guide/guidelines/products.md) sono salvati come record. Un record personale definisce le caratteristiche di un segmento di clienti specifico, ossia il pubblico di destinazione per i contenuti generati. Può includere dettagli demografici e una cronologia delle interazioni dei clienti.

I record di prodotto definiscono le specifiche e gli attributi chiave del prodotto nel contesto delle linee guida del brand. Gli attributi possono includere funzioni, immagini associate e posizionamento del prodotto all’interno del tuo marchio.

Le opzioni nei menu a discesa _Personas_ e _Prodotti_ sono definite a livello organizzativo. Durante la creazione di una campagna, puoi scegliere tra questi record predefiniti per garantire una rappresentazione coerente del prodotto e supportare il targeting accurato, la messaggistica e il tracciamento delle prestazioni.

**Per assegnare utenti tipo alla campagna**:

1. Fai clic sul segno + (**[!UICONTROL Connetti record +]**) accanto a **[!UICONTROL Persone]**.

   Viene aperto il popup _Seleziona utenti tipo_. Puoi cercare uno specifico utente tipo supportato.

1. Seleziona gli utenti tipo a cui la campagna è destinata. Gli utenti tipo validi vengono definiti dall&#39;organizzazione durante la [creazione delle linee guida](/help/user-guide/guidelines/personas.md).

   Se necessario, scegli **[!UICONTROL Visualizza tutto]** per aprire una visualizzazione di tutti gli utenti tipo disponibili.

**Per assegnare prodotti alla campagna**:

1. Fai clic sul segno + (**[!UICONTROL Connetti record +]**) accanto a **[!UICONTROL Prodotti]**.

   Viene visualizzata la finestra a comparsa _Seleziona prodotti_. Puoi cercare un prodotto specifico supportato.

1. Seleziona uno o più prodotti. I prodotti sono definiti dall&#39;organizzazione durante la [creazione delle linee guida](/help/user-guide/guidelines/products.md).

   Facoltativamente, scegliere **[!UICONTROL Visualizza tutto]** per aprire una visualizzazione di tutti i prodotti disponibili.

## Completare la creazione della campagna

Fai clic su **[!UICONTROL Crea]** per salvare i valori immessi e creare la campagna.

Il nuovo nome della campagna è ora disponibile come etichetta della campagna in [!DNL Content] e [!DNL Create]. Puoi aggiungere risorse ed esperienze approvate alla campagna tramite [!DNL Content] oppure assegnare una risorsa ed esperienza a una campagna durante la creazione di contenuti.

## Aggiungere contenuto alla campagna

GenStudio for Performance Marketing collega il contenuto alle campagne utilizzando le etichette delle campagne memorizzate nei metadati [!DNL Content]. Un singolo contenuto può essere associato a più campagne.

Le etichette della campagna identificano la campagna e i relativi attributi. L’assegnazione di un’etichetta a una risorsa o esperienza la collega alla campagna corrispondente.

**Per aggiungere risorse ed esperienze da[!DNL Content]**:

1. Dalla raccolta [!DNL Content] _Esperienze_ o _Assets_, scegli l&#39;esperienza o la risorsa approvata.

1. Nella visualizzazione _Dettagli_, seleziona il nome della campagna dal menu a discesa _Campagne_.

**Per aggiungere risorse ed esperienze durante la creazione dei contenuti**:

Durante la creazione del contenuto, puoi pubblicare la risorsa o l&#39;esperienza appena creata in [!DNL Content].

1. Dal popup _Conferma dettagli per il contenuto approvato_, seleziona una campagna dal menu a discesa _Campagne_.

1. Fai clic su **[!UICONTROL Pubblica]**.

Questa campagna è ora disponibile nel dashboard _Campagne_.
