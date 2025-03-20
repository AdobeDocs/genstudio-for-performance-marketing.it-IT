---
title: Funzioni testo
description: Scopri la funzione testo delle categorie di attributi utilizzate in GenStudio for Performance Marketing.
feature: Reporting and Insights, Text Attributes, Generative AI
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: 7b81b0ae-0c62-468f-965c-fd8070644fb3
source-git-commit: 3448392bc3f1496dafdbed2995f40bdba9c91c31
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 1%

---

# Funzioni testo

Le caratteristiche del testo includono conteggi per alcuni elementi di testo, quali parole, frasi, emoticon e classificazioni per semantica, emozione e tono, utilizzati per l&#39;analisi con [!DNL Insights]. Il testo può inoltre ricevere un punteggio di leggibilità.

GenStudio for Performance Marketing utilizza le funzionalità di intelligenza artificiale e machine learning di Adobe per studiare il testo e applicare [!UICONTROL attributi multimediali] in base ai toni di testo associati e alla narrazione di marketing. Il processo convalida il testo di input per verificare che contenga caratteri alfanumerici, rimuovendo gli spazi vuoti aggiuntivi e i caratteri non stampabili e troncando il testo fino al massimo consentito di 1500 parole. Prima di applicare i tag attributo rilevati, l’intelligenza artificiale prevede il tono prevalente.

## Tono della voce

Il tono rappresenta un carattere generale, un atteggiamento o un&#39;atmosfera esibita attraverso il linguaggio. Una semplice scelta di parole e punteggiatura, struttura della frase e stile può alterare il tono del messaggio. Ad esempio, considera i seguenti messaggi urgenti utilizzando i tre livelli di tono di base:

- `Formal`

  ```
  Take advantage of this distinctive and exceptional opportunity!
  ```

- `Conversational`

  ```
  Don't miss out on this great opportunity!
  ```

- `Direct`

  ```
  Don't miss the chance!
  ```

L’intelligenza artificiale rileva ulteriormente un tono più sfumato. Utilizzando la stessa istruzione urgente dell&#39;esempio precedente, la seguente versione utilizza un tono `poetic` stravagante:

- `Poetic`

  ```
  Embrace the moment, without delay, for this occasion won't always stay.
  ```

Altri valori secondari per il tono includono: `Enthusiastic`, `Assertive`, `Humorous/Witty`, `Inspirational`, `Empathetic`, `Sensory`, `Storytelling`, `Poetic`, `Quantitative`, `Personal`

## Narrativa

Gli attributi narrativi consentono di identificare i media che comunicano i valori, lo scopo o l’identità che risuonano con il pubblico di destinazione.

| Narrativa | Descrizione | Esempio |
| ----------------- | ----------- | ------- |
| `Authenticity` |             |         |
| `Celebration` |             |         |
| `Community` |             |         |
| `Convenience` |             |         |
| `Empowerment` |             |         |
| `Exploration` |             |         |
| `Futuristic` |             |         |
| `Hype` |             |         |
| `Indulgence` |             |         |
| `Peace of mind` |             |         |
| `Personalization` |             |         |
| `Prestige` |             |         |
| `Timelessness` |             |         |
| `Versatility` |             |         |
| `Well-being` |             |         |

## Punteggio di leggibilità

Il punteggio di leggibilità valuta la facilità di lettura e comprensione di un testo. Ti aiuta a garantire che il contenuto sia appropriato per il pubblico di destinazione. I punteggi si basano su vari fattori, tra cui la lunghezza della frase e la complessità delle parole.

| Punteggio | Livello scolastico | Note |
| ----------- | ------------------ | ------------------------------------------------------------------------- |
| 100,00-90,00 | Quinta elementare | Molto facile da leggere. Facilmente comprensibile per uno studente di 11 anni. |
| 90,0-80,0 | 6° grado | Facile da leggere. Inglese conversazionale per i consumatori. |
| 80,0-70,0 | 7° grado | Abbastanza facile da leggere. |
| 70,0-60,0 | 8° e 9° grado | Inglese semplice. Facilmente comprensibile per gli studenti dai 13 ai 15 anni. |
| 60,0-50,0 | dal 10° al 12° grado | Abbastanza difficile da leggere. |
| 50,0-30,0 | Collegio | Difficile da leggere. |
| 30,0-0,0 | Laureato | Molto difficile da leggere. Meglio compresa dai laureati. |

## Conteggi parole

Da definire

Nella tabella seguente sono elencate le categorie di funzioni immagine riconosciute da GenStudio for Performance Marketing AI.

| Categoria | Descrizione | Esempio |
| -------------------- | ------------- | --------------------- |
| Conteggio emoticon |             |        |
| Conteggio hashTags |             |        |
| Parole chiave |             |        |
| Emozioni marketing | Le emozioni sono mirate nei messaggi di marketing per evocare sentimenti e risposte specifici da parte del pubblico, che possono migliorare il coinvolgimento e la connessione con il brand. | `Aspiration`, `Challenge`, `Curiosity`, `Exclusivity`, `Fascination`, `Gratification`, `Recognition`, `Trust`, `Urgency` |
| Strategie di persuasione | Tecniche utilizzate per influenzare il comportamento dei consumatori e stimolare le azioni desiderate. Queste strategie sono mirate a specifici trigger psicologici e segmenti di clienti per migliorare l’efficacia dei messaggi di marketing. | `Social identity`, `Social proof`, `Endorsement`, `Concreteness`, `Foot in the door`, `Overcoming reactance`, `Reciprocity`, `Comparison`, `Social impact`, `Scarcity`, `Anthropomorphism` |
| Tono della voce | Il carattere generale, l’atteggiamento o l’atmosfera veicolati in un messaggio di marketing attraverso la scelta delle parole, la punteggiatura, la struttura della frase e lo stile. | `Enthusiastic`, `Assertive`, `Humorous/Witty`, `Inspirational`, `Empathetic`, `Sensory`, `Storytelling`, `Poetic`, `Quantitative`, `Personal` |
