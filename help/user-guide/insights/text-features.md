---
title: Funzioni testo
description: Scopri la funzione testo delle categorie di attributi utilizzate in GenStudio for Performance Marketing.
feature: Reporting and Insights, Text Attributes, Generative AI
exl-id: 7b81b0ae-0c62-468f-965c-fd8070644fb3
source-git-commit: ac2e18899f910a47ec5013a13c2ee2771684ddad
workflow-type: tm+mt
source-wordcount: '1290'
ht-degree: 1%

---

# Funzioni testo

Le caratteristiche del testo includono conteggi per alcuni elementi di testo, quali parole, frasi, emoticon e classificazioni per semantica, emozione e tono, utilizzati per l&#39;analisi con [!DNL Insights]. Il testo può inoltre ricevere un punteggio di leggibilità.

GenStudio for Performance Marketing utilizza le funzionalità di intelligenza artificiale e machine learning di Adobe per studiare il testo e applicare [!UICONTROL attributi multimediali] in base ai toni di testo associati e alla narrazione di marketing. Il processo convalida il testo di input per verificare che contenga caratteri alfanumerici, rimuovendo gli spazi vuoti aggiuntivi e i caratteri non stampabili e troncando il testo fino al massimo consentito di 1500 parole. Prima di applicare i tag attributo rilevati, l’intelligenza artificiale prevede il tono prevalente.

## Tono della voce

Il tono rappresenta un carattere generale, un atteggiamento o un&#39;atmosfera esibita attraverso il linguaggio. Una semplice scelta di parole e punteggiatura, struttura della frase e stile può alterare il tono del messaggio. Ad esempio, considera i seguenti messaggi urgenti utilizzando i tre livelli di tono di base:

| Tono | Descrizione | Esempio |
| -------------- | ----------------------------------- | --------------------------------------------------------- |
| Formale | Linguaggio lucido e professionale. | `Take advantage of this distinctive and exceptional opportunity!` |
| Conversazionale | Linguaggio amichevole e informale. | `Don't miss out on this great opportunity!` |
| Diretto | Diretto e diretto al punto. | `Don't miss the chance!` |

Altri valori secondari per il tono forniscono una distinzione più precisa del carattere e dell&#39;atteggiamento del messaggio. In linea con l&#39;esempio precedente di un messaggio urgente, GenAI potrebbe rilevare un tono _poetico_ in questo esempio stravagante: `Embrace the moment, without delay, for this occasion won't always stay.`

Nella tabella seguente sono elencati i valori tonali riconosciuti da GenStudio for Performance Marketing AI.

| Tono | Descrizione | Esempio |
| -------------- | ------------------------------------------------ | --------------------------------------------------------- |
| Assertivo | Fiducia e forza nell&#39;espressione. | `You need to act now to secure this deal!` |
| Diretto | Diretto e diretto al punto. | `Don't miss the chance!` |
| Empatico | Mostrare comprensione e sensibilità. | `We understand your needs, and this is perfect for you.` |
| Entusiasta | Mostrare piacere, interesse o approvazione intensi e desiderosi. | `This is an amazing opportunity you can't miss!` |
| Umoristico/spiritoso | Leggero e intelligente. | `Why wait? Grab this deal before it's gone!` |
| Ispirativo | Incoraggiante e incoraggiante. | `Believe in yourself and seize this opportunity!` |
| Poetico | Artistico ed espressivo. | `Embrace the dawn of a new opportunity.` |
| Quantitativo | In base a dati numerici. | `99% of users loved this offer, and you will too.` |
| Sensoriale | Coinvolgere i sensi. | `Feel the excitement with this incredible offer!` |
| Narrazione | Narrazione di una storia per trasmettere un messaggio. | `Once upon a time, there was an offer you couldn't refuse.` |

## Appello emotivo

Gli addetti al marketing sfruttano il potere delle emozioni umane per creare una forte connessione tra il pubblico e il brand. Attingendo ai sensi come la felicità, la paura, l’eccitazione o la nostalgia, gli esperti di marketing possono creare messaggi che risuonano a un livello più profondo, guidando il coinvolgimento e influenzando il comportamento dei consumatori. L&#39;attrattiva emotiva aiuta a fornire contenuti più affidabili e memorabili, in ultima analisi promuovendo la brand loyalty e incoraggiando le azioni desiderate.

Le tattiche di persuasione, le emozioni di marketing e gli stili narrativi collaborano per eseguire il targeting dei segmenti di clienti.

- **Gli stili narrativi**, come autenticità, celebrazione e community, aiutano a trasmettere i valori e l&#39;identità che risuonano con il pubblico di destinazione, creando un messaggio più convincente e correlabile.
- **Le tattiche di persuasione**, come la scarsità, la prova sociale e la reciprocità, sono progettate per influenzare il comportamento dei consumatori facendo appello alle loro emozioni e preferenze.
- **Le emozioni di marketing** mirano a stimolare sentimenti che migliorano il coinvolgimento e la connessione con il brand.

GenStudio for Performance Marketing AI rileva e distingue queste caratteristiche analizzando il testo per segnali emotivi, toni e stili narrativi. L’intelligenza artificiale utilizza algoritmi di elaborazione del linguaggio naturale (NLP) e di apprendimento automatico per identificare i pattern e classificare il testo in base ad attributi emotivi e persuasivi predefiniti.

### Stile narrativo

Gli attributi narrativi, o fattore di richiamo, aiutano a identificare i media che comunicano i valori, lo scopo o l’identità che risuonano con il pubblico di destinazione. Nella tabella seguente sono elencati gli stili narrativi riconosciuti da GenStudio for Performance Marketing AI.

| Fattore di appello | Descrizione | Esempio |
| ----------------- | --------------------------------------------------------------------- | ------------------------------------------ |
| Autenticità | Genuina e reale, che spesso sottolinea la trasparenza e l&#39;onestà. | `A behind-the-scenes look at how our products are made.` |
| Festeggiamento | Segnalare occasioni speciali o realizzazioni con gioia e festa. | `Join us in celebrating our 10th anniversary with special offers!` |
| Community | Promuovere un senso di appartenenza e di unione in un gruppo. | `Our brand is built on the strength of our community.` |
| Comodità | Enfatizzare la facilità d&#39;uso e i vantaggi in termini di risparmio di tempo. | `Get what you need with just one click.` |
| Potenziamento | Incoraggiare e consentire alle persone di assumere il controllo e prendere decisioni. | `Empower yourself with our latest tools and resources.` |
| Esplorazione | Scoperta e avventura stimolanti, spesso associate a nuove esperienze. | `Discover new horizons with our travel packages.` |
| Futuristico | Evidenziare l&#39;innovazione e le idee lungimiranti. | `Experience the future of technology today.` |
| Hype | Generare emozioni e anticipazioni su un prodotto o un evento. | `Don't miss out on the most anticipated event of the year!` |
| Indulgenza | Appellarsi a fantasie, desideri o piaceri. | `Treat yourself to the finest gourmet chocolates.` |
| Sicurezza totale | Assicurare sicurezza e sicurezza. | `Rest easy knowing your data is safe with us.` |
| Personalizzazione | Personalizzare esperienze o prodotti in base alle preferenze individuali. | `Get a custom-fit solution just for you.` |
| Prestigio | Associandosi a status ed esclusività elevati. | `Join the elite with our premium membership.` |
| Senza tempo | Enfatizzare la qualità duratura e il fascino classico. | `Our designs are timeless and never go out of style.` |
| Versatilità | Evidenziare adattabilità e molteplici utilizzi. | `Our product fits seamlessly into any lifestyle.` |
| Benessere | Promuovere la salute, la felicità e il benessere generale. | `Enhance your well-being with our holistic approach.` |

### Tattiche di persuasione

Le tecniche di persuasione vengono utilizzate per influenzare il comportamento del consumatore e stimolare le azioni desiderate. Queste strategie sono mirate a specifici trigger psicologici e segmenti di clienti per migliorare l’efficacia dei messaggi di marketing. Nella tabella seguente sono elencate le tattiche di persuasione riconosciute da GenStudio for Performance Marketing AI.

| Tattico | Descrizione | Esempio |
| --------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------- |
| Antropomorfismo | Attribuzione di caratteristiche umane a prodotti o marchi. | `Our friendly chatbot is here to help you.` |
| Confronto | Evidenziare le differenze tra le opzioni per influenzare la scelta. | `See how we compare to the competition.` |
| Concretezza | Fornire dettagli specifici per rendere il messaggio più tangibile. | `Save 20% on your next purchase.` |
| Approvazione | Con l&#39;approvazione di fonti o influencer credibili. | `Recommended by top industry experts.` |
| Piede nella porta | A partire da una piccola richiesta per aumentare la probabilità di accettazione di una richiesta più ampia. | `Try our free trial today.` |
| Superare la reazione | Ridurre le resistenze riconoscendo e affrontando le obiezioni. | `We understand your concerns, and here's how we address them.` |
| Reciprocità | Offrire qualcosa di valore per incoraggiare un favore di ritorno. | `Get a free gift with your purchase.` |
| Scarsità | Creare un senso di urgenza evidenziando la disponibilità limitata. | `Only a few items left in stock!` |
| Identità social | Sfruttare il senso di appartenenza del consumatore a un gruppo. | `Join our community of innovators.` |
| Impatto sociale | Enfatizzare l&#39;impatto positivo sulla società o sull&#39;ambiente. | `Your purchase helps plant a tree.` |
| Bozza social | Utilizzare testimonianze o contenuti generati dagli utenti per creare fiducia. | `See why thousands of users love our product.` |

### Emozioni di marketing

Le emozioni sono mirate nei messaggi di marketing per evocare sentimenti e risposte specifici da parte del pubblico, che possono migliorare il coinvolgimento e la connessione con il brand. Nella tabella seguente sono elencate le emozioni riconosciute da GenStudio for Performance Marketing AI.

| Emozione | Descrizione | Esempio |
| ------------- | --------------------------------------------------------------------------- | --------------------------------------------------------- |
| Aspirazione | Ispirare un desiderio di raggiungere o raggiungere qualcosa di più grande. | `Imagine the possibilities with our premium service.` |
| Sfida | Incoraggiare il pubblico a superare un ostacolo o ad abbracciare un nuovo compito. | `Are you ready to take the next step in your career?` |
| Curiosità | Suscitare interesse e desiderio di saperne di più. | `Discover the secrets behind our success.` |
| Esclusività | Creazione dell&#39;impressione di far parte di un gruppo selezionato. | `Join our exclusive club for members-only benefits.` |
| Fascinazione | Catturare l&#39;attenzione del pubblico con contenuti interessanti o accattivanti. | `Be amazed by our latest innovations.` |
| Gratificazione | Soddisfazione e piacere nell&#39;uso del prodotto o del servizio. | `Enjoy the ultimate comfort with our luxury bedding.` |
| Riconoscimento | Riconoscere e valutare i risultati o lo stato del pubblico. | `Get the recognition you deserve with our award-winning service.` |
| Trust | Costruire fiducia e affidabilità nel marchio. | `Trust us to deliver quality and excellence every time.` |
| Urgenza | Promuovere un&#39;azione immediata sottolineando le opportunità che richiedono un intervento tempestivo. | `Act now before this limited-time offer expires!` |

## Punteggio di leggibilità

Il punteggio di leggibilità valuta la facilità di lettura e comprensione di un testo. Ti aiuta a garantire che il contenuto sia appropriato per il pubblico di destinazione. I punteggi si basano su vari fattori, tra cui la lunghezza della frase e la complessità delle parole. Nella tabella seguente sono elencati i livelli di leggibilità riconosciuti da GenStudio for Performance Marketing AI.

| Livello di leggibilità | Descrizione | Esempio |
| ------------------- | ------------------------------------------------------------------ | --------------------------------------------------------- |
| Quinta elementare | Linguaggio molto semplice, adatto ai bambini piccoli. | `The cat sat on the mat.` |
| 6° grado | Linguaggio semplice e chiaro, adatto a un pubblico generico. | `You can find great deals on our website.` |
| 7° grado | Facile da capire, con vocabolario e struttura semplici. | `Our new product is simple to use and very effective.` |
| 8° e 9° grado | Linguaggio chiaro e conciso, adatto agli adolescenti. | `This guide will help you understand the basics of our service.` |
| dal 10° al 12° grado | Linguaggio più complesso, adatto agli adolescenti più grandi e agli adulti. | `The comprehensive manual provides detailed instructions for setup.` |
| Collegio | Linguaggio avanzato, adatto a un pubblico istruito. | `The study explores the multifaceted implications of the new policy.` |
| Laureato | Linguaggio altamente avanzato, adatto a esperti e specialisti. | `The dissertation delves into the intricacies of quantum mechanics.` |

## Conteggi

Comprendere e sfruttare gli attributi di conteggio come i conteggi degli hashtag, il conteggio delle parole, il conteggio delle frasi e il rapporto tra parole non significative può migliorare notevolmente la tua strategia di contenuto. Queste metriche offrono informazioni utili sull’efficacia e la portata delle attività di marketing. Nella tabella seguente sono elencate le categorie di conteggio riconosciute da GenStudio for Performance Marketing AI.

| Categoria | Descrizione | Esempio |
| --------------------- | --------------------------------------------------------------------------- | --------------------- |
| Conteggio emoticon | Il numero di emoji presenti nel testo. Le emoticon possono migliorare il coinvolgimento e trasmettere le emozioni rapidamente. | `😊`, `🚀`, `❤️` |
| Conteggio hashTags | Numero di hashtag utilizzati nel testo. Gli hashtag aiutano a categorizzare i contenuti e ad aumentare la reperibilità sui social media. | `#Marketing`, `#Sale` |
| Conteggio parole per frase | Numero medio di parole per frase nel testo. Frasi più brevi sono spesso più facili da leggere e comprendere. | `10` |
| Conteggio parole | Numero totale di parole nel testo. Un conteggio delle parole più elevato può fornire informazioni più dettagliate, ma può anche richiedere più lavoro di lettura. | `1500 words` |
| Proporzione di parole non significative | Rapporto tra parole non significative e parole significative nel testo. Le parole non significative (come &quot;a&quot; &quot;an&quot; &quot;the&quot;) vengono spesso ignorate nelle query di ricerca e nei risultati. Un elevato tasso di parole non significative può rendere il contenuto meno coinvolgente e più difficile da leggere. | `0.375` |
| Conteggio frasi | Numero totale di frasi nel testo. Più frasi possono indicare contenuti più dettagliati, ma testi troppo lunghi possono perdere l&#39;interesse del lettore. | `75 sentences` |
