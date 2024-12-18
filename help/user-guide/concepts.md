---
title: Concetti di Adobe GenStudio for Performance Marketing
description: Scopri i concetti e la terminologia di Adobe GenStudio for Performance Marketing.
feature: Workflow, Generative AI
exl-id: 7dd00b4c-f429-499b-851d-3606c82c09dc
source-git-commit: bfe961a06f62e55f3207088f6f390204b12e7142
workflow-type: tm+mt
source-wordcount: '698'
ht-degree: 0%

---

# Concetti

GenStudio for Performance Marketing è un prodotto aziendale indipendente che incorpora la catena di fornitura dei contenuti di Adobe per semplificare le campagne di marketing. È difficile creare contenuti personalizzati e approvati dal marchio su larga scala, monitorare l’efficacia e adattarsi rapidamente a un mercato in continua evoluzione. GenStudio for Performance Marketing riunisce Creative Cloud e Experience Cloud in un’unica applicazione che sfrutta l’intelligenza artificiale generativa come moltiplicatore delle prestazioni per i team di marketing aziendali.

Con GenStudio for Performance Marketing è possibile:

* Creazione di contenuti on-brand utilizzando prompt in linguaggio naturale per i canali digitali a priorità alta, come media a pagamento, e-mail e annunci di visualizzazione

* Collaborare con le parti interessate per rivedere e approvare i contenuti generati
* Salva i contenuti generati e approvati per accedere alle campagne di marketing future
* Valutare l’efficacia dei contenuti analizzando le prestazioni delle risorse e identificando gli attributi chiave dei contenuti con prestazioni migliori

## Tecnologia di intelligenza artificiale generativa

GenStudio for Performance Marketing sfrutta la potenza dell’intelligenza artificiale generativa per accelerare il processo di creazione dei contenuti e garantire una generazione di contenuti di alta qualità. Il ciclo di vita iterativo delle risorse creative consente di ottenere contenuti sempre più precisi e allineati al brand, in linea con il pubblico di destinazione.

Inizia acquisendo il marchio della tua organizzazione, gli utenti tipo e le descrizioni dei prodotti attraverso la potente funzione delle linee guida per il brand. Per informazioni su come preparare e caricare queste linee guida, consulta la [panoramica delle linee guida](../user-guide/guidelines/overview.md).

{{in-academy}}

## Modelli in lingue di grandi dimensioni

GenStudio for Performance Marketing sfrutta la piattaforma di intelligenza artificiale generativa di Adobe, che offre servizi di intelligenza artificiale e apprendimento automatico (ML) fondamentali. Questa piattaforma semplifica l’utilizzo dei modelli LLM (Large Language Model), consentendo alle funzionalità GenAI di Adobe di creare esperienze coinvolgenti.

GenStudio for Performance Marketing utilizza la serie GPT di LLM di terze parti tramite Azure OpenAI.<!-- Claude, and Gemini models. -->

## [!DNL Generative Actions]

_[!DNL Generative Actions]_, come definito nella [descrizione del prodotto Adobe GenStudio for Performance Marketing](https://helpx.adobe.com/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html), sono le unità che quantificano l&#39;utilizzo delle funzionalità di intelligenza artificiale generativa in GenStudio for Performance Marketing.

<!-- Add example about usage mode?
Where users check how many generative actions they have left
How they re-up their genactions
If genactions roll over month to month or not -->

### Tariffe

Ricevi un&#39;assegnazione predefinita di [!DNL Generative Actions] come descritto nella [descrizione del prodotto GenStudio for Performance Marketing](https://helpx.adobe.com/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html).

>[!NOTE]
>
>Le percentuali di utilizzo possono variare. I piani sono soggetti a modifiche. Per informazioni aggiornate sulla tariffa, consulta la [descrizione del prodotto Adobe GenStudio for Performance Marketing](https://helpx.adobe.com/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html).

Le seguenti funzioni utilizzano [!DNL Generative Actions] alla velocità specificata.

| Funzione | Percentuale azioni generative |
| -----------------------  | ------------------ |
| Crea e-mail | 5 per generazione |
| Creare annunci multimediali a pagamento | 5 per generazione |
| Creare annunci di visualizzazione | 5 per generazione |
| Rigenera sezioni | 1 per generazione |

<!-- | Generate on-brand images | 1 per prompt  |
| Translation              | 1 per prompt  |
| Video: ADLS              | 1 per prompt  |
| Video: TTS + Avatar      | 1 per prompt  | -->

[!DNL Generative Actions] _non sono_ utilizzati quando:

* Utilizzo della [convalida del brand](/help/user-guide/guidelines/brand-validation.md) durante la generazione delle varianti
* Estrazione delle informazioni dalle [linee guida caricate](/help/user-guide/guidelines/add-guidelines.md)
* [ricontrolla manualmente le varianti](/help/user-guide/guidelines/brand-validation.md#improve-brand-alignment)
* Alle risorse digitali vengono assegnati automaticamente tag con attributi ([[!DNL Insights]](/help/user-guide/insights/overview.md))

>[!TIP]
>
>Se superi il limite di [!DNL Generative Actions], puoi acquistare altri prodotti direttamente dal rappresentante del tuo account.

## Governance dei dati

Quando si lavora con l’intelligenza artificiale per generare contenuti, è essenziale garantire che l’output sia sicuro e inclusivo per tutti gli utenti. Ciò richiede la valutazione del contenuto per potenziali pregiudizi dannosi, incitamento all&#39;odio, materiale offensivo o volgarità. Adobe testa a fondo la tecnologia di generazione dei contenuti da prospettive diverse, esegue valutazioni etiche complete e implementa efficaci piani di mitigazione per evitare che i contenuti dannosi emergano negli output.

Questo approccio rafforza la responsabilità sociale, riduce al minimo il rischio per la reputazione e garantisce il rispetto delle [politiche di etica e sicurezza di Adobe](https://www.adobe.com/content/dam/cc/en/ai-ethics/pdfs/Adobe-AI-Ethics-Principles.pdf).

GenStudio for Performance Marketing incorpora piani di mitigazione per impedire l’utilizzo di contenuti dannosi o distorti identificati in base agli standard e alle politiche di governance dei dati Adobe. Quando viene rilevato tale contenuto, vieni informato che la generazione di risorse è bloccata con un messaggio &quot;Impossibile generare&quot;.

Quando viene visualizzato questo messaggio, puoi modificare il prompt e riprovare _o_ contrassegnando il contenuto del prompt per la revisione da parte di GenStudio for Performance Marketing. I dati di richiesta per il contenuto contrassegnato per la revisione vengono raccolti a scopo di revisione interna.

## Ciclo di vita dei contenuti

La domanda è elevata per esperienze di qualità su più canali a un ritmo più veloce. GenStudio for Performance Marketing semplifica la catena di distribuzione dei contenuti in un flusso di lavoro ben organizzato per gli esperti di marketing. GenStudio for Performance Marketing sfrutta la tecnologia Adobe in ogni fase del ciclo di vita.

<table style="table-layout:auto">

<tr style="border: 0;">

    <td>

       <p><strong>Flusso di lavoro e pianificazione</strong></p>

    </td>

    <td>

        <p>Brainstorming sulle idee, definizione di linee guida e creazione di una strategia basata sui contenuti per coinvolgere il pubblico.</p>

    </td>

</tr>

<tr style="border: 0;">

    <td>

        <p><strong>Creazione e produzione</strong></p>

    </td>

    <td>

        <p>Produrre il contenuto in base al piano. Collabora in tempo reale, ricevi feedback, apporta modifiche e approva contenuti.</p>

    </td>

</tr>

<tr style="border: 0;">

    <td>

        <p><strong>Gestione dei contenuti</strong></p>

    </td>

    <td>

        <p>Archivia, condividi e trova le risorse creative nell’archivio centralizzato. Riutilizzare e rivitalizzare i contenuti in base alle prestazioni.</p>

    </td>

</tr>

<tr style="border: 0;">

    <td>

        <p><strong>Consegna e attivazione</strong></p>

    </td>

    <td>

        <p>Attiva i contenuti e pubblicali su più canali di marketing.</P>

    </td>

</tr>

<tr style="border: 0;">

    <td>

        <p><strong>Reporting e approfondimenti</strong></p>

    </td>

    <td>

        <p>Raccogli dati e ottieni informazioni approfondite per ottimizzare le prestazioni delle risorse.</p>

    </td>

</tr>

</table>
