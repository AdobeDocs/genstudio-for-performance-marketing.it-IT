---
title: Funzioni video
description: Scopri la funzione video delle categorie di attributi utilizzate in GenStudio for Performance Marketing.
level: Intermediate
feature: Reporting and Insights, Video Attributes, Generative AI
exl-id: 0dfdd735-b365-4a15-a6fd-e981697442cb
source-git-commit: 72cd93d9d6fdd99d5a524d05cba923e9c0191960
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 1%

---

# Funzioni video

Le funzionalità video rappresentano elementi, suoni o pattern distinti e informativi all&#39;interno di un video per l&#39;analisi con [!DNL Insights]. Queste funzioni consentono di suddividere in categorie e comprendere i contenuti video, consentendo di ottenere informazioni più precise e dettagliate. Identificando vari attributi come l’umore audio, il genere musicale e gli oggetti, l’intelligenza artificiale può fornire un’analisi completa del video, contribuendo a migliorare il processo decisionale e la formulazione della strategia.

## Rilevamento audio

Il rilevamento audio in GenStudio for Performance Marketing comporta l’analisi della traccia audio di un video per identificare vari attributi. Questo processo di rilevamento determina l&#39;umore complessivo dell&#39;audio identificando i tipi di audio presenti, assegnando tag a specifici generi o categorie di musica ed estraendo le parole chiave dal discorso. Comprendendo questi elementi audio, l’intelligenza artificiale può fornire informazioni più approfondite sul contenuto e sul contesto del video, migliorando il processo complessivo di analisi e classificazione.

## Funzioni di ricerca video

**Per visualizzare l&#39;anteprima di un video e ascoltare un campione dell&#39;audio**:

1. In _[!DNL Insights]_, selezionare la visualizzazione **[!UICONTROL Attributi]**.

1. Modificare la visualizzazione della tabella selezionando **[!UICONTROL Video]**.

1. Selezionare una funzionalità dall&#39;elenco **[!UICONTROL Categoria attributo]**. Per un esempio audio, selezionare **Genere musicale**.

1. Seleziona un attributo per la visualizzazione dettagliata dei video che condividono tale categoria.

   Ad esempio, la categoria `Music genre` può avere `electronic` come attributo.

1. Nella pagina _Dettagli attributo_ sono elencati tutti i video con questo attributo. Per avviare un&#39;anteprima video, posizionate il puntatore del mouse su un video dell&#39;elenco.

1. Attiva il pulsante **attiva** (situato nell&#39;angolo inferiore sinistro di un&#39;anteprima video) e ascolta l&#39;audio dell&#39;anteprima video.

Nella tabella seguente sono elencate le categorie di funzioni video riconosciute da GenStudio for Performance Marketing AI. L’elenco degli attributi rilevati per un contenuto multimediale non è esaustivo. I contenuti multimediali che contengono un set completo di funzioni possono essere limitati alle tre funzioni più dominanti identificate dall’intelligenza artificiale.

<!-- For the writer: turn off word wrap to work with these tables. Option + Z -->

| Categoria | Descrizione | Esempio |
| ------------------- | ------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------- |
| Modo audio | Determina il tono emotivo complessivo o l&#39;atmosfera della traccia audio, ad esempio `calm`, `upbeat` o `tense`. | `Energetic`, `Happy`, `Emotional Ambient/atmospheric`, `Relaxing`, `Dramatic`, `Expressive/characterful`, `Intense`, `Slow`, `Neutral` |
| Tipi di audio | Aggiunge al video un tag con uno o più tipi di contenuto audio, ad esempio `music` o `speech`. | `Music`, `Speech`, `Silence`, `Special effects`, `Ambience` |
| Categorie | Classifica il video in una o più categorie di contenuto generali. | `Entertainment`, `Sports`, `Music`, `Gaming`, `Howto tutorials`, `Fashion and style`, `Film and animation`, `Science and technology`, `Autos and vehicles`, `Pets and animals`, `People and blogs`, `News and politics`, `Social causes and activism`, `Travel and events`, `Education`, `Sales and offers` |
| Categoria musica | Ampia classificazione del genere musicale quando la musica è presente nel video. Il genere consente di identificare il tipo generale di musica, ad esempio gli stili `contemporary` o `traditional`. | `Contemporary/pop music`, `Traditional/folk-based music`, `Instrumental/orchestral music`, `Rock music`, `Acoustic/unplugged music`, `Specialised/occasional music`, `Experimental/unique music` |
| Genere musicale | Classificazione specifica dello stile musicale quando la musica è presente nel video, che fornisce un&#39;identificazione più dettagliata della musica, ad esempio `electronic` o `jazz`. | `electronic`, `hip-hop`, `dance`, `novelty`, `rock`, `world`, `reggae`, `pop`, `film`, `jazz`, `background`, `latin` |
| Oggetti | Identifica uno o più elementi, entità ed elementi visualizzati nel video. | I valori sono troppo numerosi, ma alcuni esempi includono: `backpack`, `book`, `hawk`, `glasses`, `fish`, `pencil`, `mountain bike`, `soap` |
| Orientamento | L’allineamento del video in relazione alla sua larghezza e altezza. Rileva se è più largo di quanto sia alto (orizzontale), più alto di quanto sia largo (verticale) o uguale in larghezza e altezza (quadrato). | `landscape`, `portrait`, `square` |
| Persone | Se è presente almeno una persona, uno o più attributi possono descrivere la persona o le persone presenti nel video. | `person`, `woman`, `man`, `girl`, `boy`, `social group`, `kid`, `crowd`, `people` |
| Scene | Identifica l’impostazione o l’ambiente all’interno di un video, fornendo contesto su dove è stato fatto il video o sul tipo di posizione rappresentata. | I valori sono troppo numerosi, ma alcuni esempi includono: `lake`, `underwater`, `highway`, `hill`, `log cabin`, `island`, `beach`, `lounge` |
| Stili | Rileva i trattamenti visivi applicati agli elementi video, ad esempio quelli utilizzati in After Effects o Lightroom. | `design`, `illustration`, `logo`, `square`, `cartoon`, `art`, `matte`, `neon` |
| Tag | Rileva altre caratteristiche video che non rientrano in una classificazione specifica. I tag forniscono contesto e metadati aggiuntivi sul video. | I valori sono troppo numerosi, ma alcuni esempi includono: `construction`, `gothic`, `healing`, `military`, `selfie`, `football`, `typing`, `dancer`, `dancing` |
