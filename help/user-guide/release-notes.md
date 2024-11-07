---
title: Note sulla versione di Adobe GenStudio for Performance Marketing
description: Scopri le funzioni e i miglioramenti più recenti di Adobe GenStudio for Performance Marketing.
recommendations: noDisplay
source-git-commit: b502e0a558cbc26c70d813938734a2f6f230dc8e
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 1%

---

# Note sulla versione di GenStudio for Performance Marketing

Queste informazioni sulla versione descrivono gli ultimi aggiornamenti dell’applicazione GenStudio for Performance Marketing.

## 2024.11.07 {#latest}

### Correzioni

* Lo spinner _Salva in corso_ non viene più visualizzato quando un utente fa clic su **[!UICONTROL Carica nuova immagine]** e quindi annulla l&#39;operazione prima del completamento del caricamento. <!-- GS-6780 -->

* I titoli delle esperienze ora vengono creati correttamente durante la rigenerazione dell’esperienza. <!-- GS-7006 -->

* Sono stati risolti i problemi relativi allo sfarfallio delle barre di scorrimento durante il caricamento delle bozze. <!-- GS-5587 -->

* Il collegamento `View documentation` nel [!DNL Content] _Aggiungi il modello approvato_ ora funziona come previsto. <!-- GS-6881 -->

* L’eliminazione di un’immagine dal riquadro dei prompt durante un’operazione di ridimensionamento non genera più un errore. <!-- GS-7115 7009 -->

* La selezione di **[!UICONTROL Elimina]** dal menu azioni [!DNL Create] (...) ora funziona come previsto. <!-- GS-6871 -->

* Gli utenti possono ora controllare tutti gli elementi interattivi del modello di Meta Ad con la sola tastiera. <!-- GS-4066 -->

* È stata aggiunta l’estrazione di dimensioni immagine dai campi immagine del modello per visualizzare i modelli di annunci. Le richieste di ritaglio avanzato vengono ora inviate per la dimensione effettiva dell’immagine e non per l’intero modello. <!-- GS-6926 -->

* La stringa `Zoom to fit to screen` è stata localizzata negli annunci e-mail e meta generati. <!-- GS-5063 -->

* Il cassetto dei prompt di [!DNL Create] ora si chiude come previsto quando un utente fa clic in un altro punto. <!-- GS-5254 -->

* L’esportazione dei metadati ora include l’etichetta di invito all’azione selezionata, come previsto. <!-- GS-6504 -->

* Il punteggio del marchio ora viene aggiornato e mantenuto come previsto per le esperienze rigenerate. <!-- GS-6535 -->

* L&#39;esportazione HTML di annunci Meta e di annunci di visualizzazione non include più il wrapper `div` e gli elementi `chrome`. <!-- GS-7116 -->

* I problemi relativi al rendering delle bozze e-mail durante la pubblicazione ora sono risolti. <!-- GS-6394 -->

* Il pulsante Canvas **[!UICONTROL Brand]** è ora disabilitato quando non viene generato un punteggio di marchio. <!-- GS-6429 -->

* L&#39;interruttore Facebook/Instagram sulla barra delle azioni Area di lavoro ora aggiorna i rendering delle esperienze come previsto quando l&#39;impostazione Area di lavoro `ReadOnly` è abilitata. <!-- GS-7039 -->

#### Rigenerazione immagine

* Il ridimensionamento di più varianti di annunci Meta ora funziona come previsto. In precedenza, l’area di lavoro non presentava varianti rigenerate, ma rimaneva vuota. <!-- GS-7010 -->

* La rigenerazione dei frammenti ora funziona come previsto per le esperienze ridimensionate. <!-- GS-6836 -->

* La rigenerazione delle metaimmagini degli annunci dopo il ridimensionamento non genera più un errore. In precedenza, il ridimensionamento delle immagini prima della rigenerazione modificava i metadati del canale da `meta` a `facebook`. <!-- GS-7042 -->

## 2024.10.31.

### Nuove funzioni

* Il filtro di ricerca **[!DNL Content]** ora supporta la ricerca per tag colore. <!-- GS-5501 -->

* L&#39;area di lavoro **[!DNL Create]** visualizza ora il numero di caratteri per i frammenti di posta elettronica. <!-- GS-5819 -->

### Correzioni

* Le etichette per gli assistenti vocali mancanti sono state aggiunte agli elementi `view` per dispositivi mobili e desktop. <!-- GS-5624 4729 -->

* L&#39;oggetto dell&#39;e-mail dell&#39;area di lavoro **[!DNL Create]** e le aree di testo pre-intestazione sono ora di altezza dinamica. <!-- GS-6258 -->

* Sono stati risolti i problemi di layout relativi ai bordi delle e-mail. <!-- GS-6631 -->

* Lo stato attivo sulla tastiera ora funziona come previsto sul pulsante **[!DNL Content]** **[!UICONTROL Elimina]**. In precedenza, questo pulsante non poteva essere raggiunto o utilizzato dalla tastiera.  <!-- GS-4065 -->

## Versione di disponibilità generale 2024.10.14

Questa versione introduce Adobe GenStudio for Performance Marketing, un’applicazione generativa basata sull’intelligenza artificiale che accelera la pianificazione, lo sviluppo e l’analisi delle campagne di marketing. GenStudio for Performance Marketing consente ai team di marketing di creare contenuti multicanale e on-brand per annunci, e-mail e campagne, fornendo al contempo informazioni in tempo reale per ottimizzare le prestazioni dei contenuti.

### Funzioni

Le principali caratteristiche del prodotto includono:

**[!DNL Create]** introduce Canvas, che offre un&#39;esperienza di richiesta strutturata che consente agli editor di contenuto di generare rapidamente contenuti e varianti. I responsabili di sistema addestrano il prodotto in base alle linee guida del marchio dell’organizzazione. [!DNL Create] garantisce che tutti i contenuti generati dall&#39;intelligenza artificiale siano in linea con le linee guida del tuo marchio (branding, utenti tipo e descrizioni dei prodotti) e semplifica la produzione di contenuti di marketing di forte impatto e coerenti con il marchio.

**[!DNL Content]** archivia risorse ed esperienze approvate e curate, conformi al brand. Gli utenti di GenStudio for Performance Marketing possono trovare, modificare, riutilizzare e condividere facilmente le risorse approvate, riducendo la necessità di ricreare contenuti da zero per ogni campagna.

**[!DNL Reviews and Approvals]** stabilisce un framework per consentire alle parti interessate di rivedere e approvare le varianti generate prima di salvarle in **[!DNL Content]** o esportarle.

**[!DNL Campaigns]** organizza e gestisce le campagne di marketing, garantendo esecuzione e tracciamento semplificati. I collaboratori possono visualizzare, pianificare e tenere traccia delle campagne per gestire in modo efficace più iniziative e garantire una distribuzione tempestiva.

**[!DNL Insights]** offre la valutazione in tempo reale delle prestazioni dei contenuti, aiutando gli addetti al marketing a ottimizzare le strategie e a prendere decisioni basate sui dati.

GenStudio for Performance Marketing si integra con altri prodotti Adobe Experience Cloud, tra cui Adobe Express e Adobe AEM Assets.

### Informazioni aggiuntive

Consulta le seguenti risorse utili:

* [Guida utente di Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/en/docs/genstudio/user-guide/home)

* [Adobe GenStudio Academy](genstudioacademy.md), piattaforma di apprendimento online di Adobe per l&#39;utilizzo di tecnologie di intelligenza artificiale generative nel processo creativo. [Registrati a GenStudio Academy](http://adobe.ly/genstudioacademyregistration).
