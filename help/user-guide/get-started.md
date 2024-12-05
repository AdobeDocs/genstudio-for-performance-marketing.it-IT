---
title: Introduzione ad Adobe GenStudio for Performance Marketing
description: Scopri come iniziare a utilizzare GenStudio for Performance Marketing per generare nuovi contenuti di marketing allineati al brand.
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
exl-id: bcb03198-bbcb-45ae-af01-25c1e834b563
source-git-commit: 088bc6df481fb1e961a7df3c79515642ec39767d
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 0%

---

# Introduzione ad Adobe GenStudio for Performance Marketing

Adobe GenStudio for Performance Marketing offre una suite completa di strumenti progettati per semplificare la creazione, la gestione e l’analisi dei contenuti. Infonde il ciclo di vita della creazione dei contenuti con funzionalità di intelligenza artificiale generative che trasformano il modo in cui i contenuti di marketing vengono creati, revisionati, condivisi e analizzati.

## Inizia a creare, condividere e rivedere i contenuti

Se sei un nuovo utente di strumenti generativi basati sull&#39;intelligenza artificiale o sei semplicemente curioso dei principi di base di GenStudio for Performance Marketing, consulta [Concetti](concepts.md) e [Scrivi prompt efficaci](effective-prompts.md). Consulta [Adobe GenStudio Academy](https://learningmanager.adobe.com/genstudioacademy), la piattaforma di apprendimento online di Adobe sull’utilizzo di tecnologie di intelligenza artificiale generative nel processo creativo.

## Addestra GenStudio for Performance Marketing

GenStudio for Performance Marketing utilizza le informazioni sul tuo marchio e sui tuoi mercati per migliorare la creazione di contenuti conformi al brand. I materiali per la formazione includono esempi, descrizioni di [utenti tipo](/help/user-guide/guidelines/personas.md) e [prodotti](/help/user-guide/guidelines/products.md) del cliente e [linee guida per il marchio](/help/user-guide/guidelines/overview.md).

I responsabili di sistema configurano Adobe GenStudio for Performance Marketing immettendo o caricando informazioni specifiche per l’organizzazione. Questa preparazione garantisce che gli editor di contenuti e i collaboratori possano utilizzare in modo efficace le funzioni di intelligenza artificiale generative per creare e rivedere le risorse della campagna. Quando un amministratore di Adobe esegue il provisioning dell’istanza di prodotto della tua organizzazione e assegna le autorizzazioni di GenStudio GenStudio System Manager, quest’ultimo può preparare il framework generativo di IA del prodotto utilizzando le linee guida.

### Passaggio 1: aggiungere linee guida

Configurare gli elementi costitutivi chiave dell’identità del brand della tua organizzazione è un prerequisito essenziale per il lavoro degli editor di contenuti e dei collaboratori. [Linee guida](./guidelines/overview.md) acquisiscono le caratteristiche del brand come loghi, tono di voce e palette di colori. Puoi caricare [[!DNL Brands] documenti di linee guida](./guidelines/brands.md) o immettere manualmente le informazioni sul marchio. Anche [[!DNL Personas] linee guida](./guidelines/personas.md) e [[!DNL Products] linee guida](./guidelines/products.md) sono importanti. Le funzionalità di intelligenza artificiale generative di GenStudio for Performance Marketing utilizzano queste linee guida per stabilire protezioni che guidano la generazione dei contenuti.

#### Preparare la documentazione sulle linee guida

Le linee guida complete e mirate di [[!DNL Brands]](./guidelines/brands.md), [[!DNL Products]](./guidelines/products.md) e [[!DNL Personas]](./guidelines/personas.md) definiscono gli aspetti principali delle campagne di marketing della tua organizzazione. GenStudio for Performance Marketing estrae informazioni da queste linee guida per iniziare a creare il tuo marchio.

Segui queste best practice durante la preparazione delle linee guida:

* Utilizza un linguaggio specifico.

* Includi i migliori esempi che puoi trovare dello stile e del tono che le risorse della campagna devono incorporare.

* Evita la ridondanza. Potresti essere tentato di ripetere una direttiva più volte, ma la ridondanza nelle linee guida non aiuta l’acquisizione LLM sottostante e l’implementazione delle linee guida del brand.

* Identificare gli elementi che si desidera escludere dal modulo LLM durante la generazione del contenuto (ad esempio, punti esclamativi nel testo).

È possibile caricare i documenti delle linee guida o consultarli quando si immettono manualmente le informazioni in GenStudio for Performance Marketing. Consulta [Aggiungi linee guida](./guidelines/overview.md) per informazioni su come caricare o immettere queste informazioni.

#### Rivedere le linee guida

Un manager di sistema GenStudio può preparare il framework generativo di intelligenza artificiale del prodotto inserendo o caricando manualmente i requisiti specifici del marchio della tua organizzazione. Anche se l’impostazione delle linee guida per il marchio di un’organizzazione è un’azione da intraprendere una tantum, è possibile rivedere e migliorare tali linee guida in base alla volatilità, alla crescita e alle mutevoli circostanze di mercato della propria organizzazione.

## Passaggio 2: configurare un progetto Adobe Admin Console per GenStudio [!DNL Brands]

Gli amministratori di sistema devono completare ulteriori attività di configurazione prima che i collaboratori possano modificare o creare [!DNL Brands]. Gli amministratori di Adobe eseguono queste attività in Adobe Admin Console:

* Crea un nuovo gruppo di utenti che include tutti gli utenti che necessitano di modifica e crea [!DNL Brands] adesioni.

* Crea un nuovo progetto in Adobe Admin Console.

Consulta [Assegnare le autorizzazioni del marchio](configure-brand-permissions.md).

### Passaggio 3: Caricare i modelli

I modelli accelerano la creazione dei contenuti. Un modello contiene funzioni approvate, come intestazioni e piè di pagina, ed è ottimizzato per canali specifici. In genere, i responsabili di sistema caricano e gestiscono i modelli per la propria organizzazione. Gli editor di contenuti utilizzano i modelli per avviare rapidamente il processo di creazione dei contenuti entro i limiti stabiliti del brand organizzativo.

Vedi [Utilizzare i modelli](./content/use-templates.md).

### Passaggio 4: caricare le risorse approvate

Le risorse approvate in [!DNL Content] sono disponibili per tutti gli editor di GenStudio for Performance Marketing. È possibile popolare [!DNL Content] con risorse da utilizzare per gli editor di contenuti nella creazione di nuove esperienze o risorse.

Consulta [Caricare risorse approvate](./content/manage-assets.md).

### Passaggio 5: connettersi a un account Meta (Facebook)

Configura una connessione tra GenStudio for Performance Marketing e gli account social della tua organizzazione per ricevere dati da campagne di marketing, risorse ed esperienze attive. [[!DNL Insights]](./insights/overview.md) fornisce gli strumenti per analizzare i dati derivati dal canale. Vedi [Connetti a un account Meta (Facebook)](./insights/connect-channel.md#meta-ads-connect).
