---
title: Flusso di lavoro di attivazione
description: Scopri il flusso di lavoro di attivazione per le esperienze pubblicitarie.
feature: Ad Activation
exl-id: 17e1bade-d52a-4953-a85c-c10d093e73d6
TQID: https://experienceleague.adobe.com/HSwFeL1qCzgFao2Ii64Hx-kaADRnd3dxaswFMzJ7nfA
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
    internal-label: Insights
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
    internal-label: Guidelines
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
    internal-label: Assets
  - id: dd48f9df-f2e2-49fe-a918-332a8e240ffe
    internal-label: Channels
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
source-git-commit: db0cebfe795569d9913757d190db853097a00405
workflow-type: tm+mt
source-wordcount: '1233'
ht-degree: 1%
---
# Flusso di lavoro attivazione

[!DNL Activate] attiva le esperienze pubblicate sulle loro piattaforme di annunci a pagamento. Un’esperienza GenStudio for Performance Marketing è un componente di una campagna di marketing, ad esempio un annuncio, che viene preparato per un pubblico specifico su una piattaforma di annunci a pagamento. Le esperienze per l’attivazione contengono tre componenti principali:

* **Risorse multimediali**: immagini o video nell&#39;esperienza pubblicitaria, in tipi di file e proporzioni che variano in base alla piattaforma e al formato.

* **Testo**: tutti i moduli di testo inclusi nell&#39;annuncio, inclusi titoli, corpo del testo ed elementi di call-to-action.

* **Metadati**: attributi definiti dall&#39;utente, in genere non visibili al pubblico dell&#39;annuncio, che migliorano l&#39;analisi delle prestazioni, il filtraggio e il tracciamento.

Questi componenti vengono preparati e approvati in [!DNL Content] prima dell&#39;attivazione. [!DNL Activate] non crea né modifica le risorse approvate, i titoli o la copia del corpo. Applica solo la configurazione di cui ogni piattaforma ha bisogno, quindi pubblica l’esperienza.

Una singola tabella di attivazione può includere esperienze per più piattaforme di annunci a pagamento e formati di annunci.

>[!VIDEO](https://video.tv.adobe.com/v/3503538?learn=on)

## Collegare gli account della piattaforma

Un system manager o editor di GenStudio deve collegare gli account annuncio per ogni piattaforma di annunci a pagamento prima di poter attivare un’esperienza su tale piattaforma. Per visualizzare i passaggi per questo processo, consulta [Connessione di account multimediali a pagamento](/help/user-guide/connectors/connect-channel.md).

## Avviare un’attivazione

Avvia un&#39;attivazione da uno dei due punti di ingresso:

* **Da[!DNL Content]**: filtra in esperienze, seleziona una o più esperienze pubblicate, quindi fai clic su **[!UICONTROL Attiva]** nella barra delle azioni superiore.

  ![Selezione di esperienze pubblicate nel contenuto e clic su Attiva per avviare un&#39;attivazione](./images/content-select-activate.png)

* **Da[!DNL Activate]**: nella pagina di destinazione [!DNL Activate], fare clic su **[!UICONTROL + Nuova attivazione]**. Viene aperta la stessa galleria di esperienze, in cui puoi selezionare le esperienze da attivare.

In entrambi i casi, cerca per nome esperienza o filtra per più canali per trovare le esperienze desiderate.

Se la selezione include esperienze in formato display, specifica la piattaforma di visualizzazione da utilizzare: Google Campaign Manager 360, Innovid, Amazon Ads o The Trade Desk. Quindi fare clic su **[!UICONTROL Avvia attivazione]**. Per altri formati, come Meta, LinkedIn, TikTok, YouTube e ChatGPT, [!DNL Activate] deduce la piattaforma dal canale dell&#39;esperienza e ignora questo passaggio.

[!DNL Activate] genera quindi una tabella di attivazione che elenca tutte le esperienze selezionate.

![Una tabella di attivazione appena generata raggruppata in tabelle secondarie Meta e LinkedIn, con ogni annuncio contrassegnato Richiede attenzione fino al completamento dei relativi campi](./images/activation-table.png)

[!DNL Activate] organizza la tabella in tabelle secondarie in base al formato e alla piattaforma dell&#39;annuncio, ad esempio immagine singola Meta o immagine singola LinkedIn. Ogni riga rappresenta un annuncio. Per la maggior parte delle piattaforme, come LinkedIn, TikTok e di visualizzazione, un’esperienza con proporzioni multiple genera una riga per proporzione; elimina le righe non necessarie. Meta è l&#39;eccezione. Un annuncio Meta può includere più proporzioni all’interno di un singolo annuncio, pertanto un’esperienza Meta con più proporzioni genera ancora una sola riga.

## Gestire la tabella di attivazione

La tabella di attivazione viene salvata automaticamente come bozza all&#39;apertura. Potete lasciare e riprendere la bozza in qualsiasi momento prima di pubblicarla.

Per aggiungere altre esperienze a una tabella di attivazione già aperta, fai clic su **[!UICONTROL Aggiungi altre esperienze]** in alto a destra nella tabella. Verrà riaperta la raccolta esperienze, in modo da poter selezionare altre esperienze, che [!DNL Activate] aggiunge alla tabella esistente.

**[!UICONTROL Aggiungi più esperienze]** ti consente inoltre di attivare più piattaforme di visualizzazione nella stessa tabella. Le esperienze in formato visualizzazione ti richiedono di scegliere prima una singola piattaforma di visualizzazione, ma puoi fare clic su **[!UICONTROL Aggiungi altre esperienze]**, selezionare più esperienze in formato visualizzazione e scegliere una piattaforma di visualizzazione diversa da quella già presente nella tabella. Ad esempio, puoi aggiungere gli annunci di Trade Desk a una tabella che contiene già annunci Innovid.

Una volta che la tabella ha le esperienze giuste, configura i campi di ogni annuncio accanto.

## Configurare i dettagli di installazione di annunci e piattaforme

Modificare i campi in linea per riga oppure selezionare più righe all&#39;interno della stessa tabella di formato e fare clic su **[!UICONTROL Modifica dettagli]** sulla barra degli strumenti che consente di modificare questi campi in blocco contemporaneamente.

![Selezione di più annunci in una tabella di attivazione per la modifica in blocco di dettagli o impostazioni della piattaforma](./images/bulk-edit-action-bar.png)

Le risorse approvate, i titoli e la copia del corpo sono bloccati e non possono essere modificati nella tabella di attivazione poiché sono già stati sottoposti a revisione e approvazione in [!DNL Content]. I campi rimanenti possono essere modificati e variano a seconda della piattaforma. [!DNL Activate] mostra solo le colonne relative alle piattaforme e ai formati selezionati. Utilizza la tabella seguente come riferimento per gli elementi modificabili in base alla piattaforma.

**Campi modificabili per piattaforma**

| Platform | Formati supportati | Copia bloccata | Campi di testo modificabili | Campi di configurazione della piattaforma modificabili |
|---|---|---|---|---|
| Meta | Immagine, video, carosello | Titolo, corpo | Descrizione, Call-to-action, URL di destinazione, parametri URL, ID tracciamento | Account annuncio, pagina Facebook, profilo Instagram, campagna Meta, set di annunci Meta |
| LinkedIn | Immagine singola, video singolo | Titolo, testo introduttivo | Descrizione, Call-to-action, URL di destinazione, parametri URL, ID tracciamento | Account, campagna e set di annunci dell’annuncio |
| Google Campaign Manager 360 | Display statico, display video, display Zip HTML5 | n/d | ID tracciamento | Inserzionista |
| Amazon Ads | Visualizzazione statica | n/d | ID tracciamento | Account |
| Innovid | Schermo statico, HTML5 Zip | n/d | ID tracciamento | Account, libreria Creative, nome concetto |
| TikTok | Annunci video in-feed | Testo principale | Call-to-action, URL di destinazione, ID tracciamento | Account annuncio, campagna, gruppo di annunci |
| YouTube | Shorts nelle campagne Google Ads Demand Gen | Descrizione | Call-to-action, nome aziendale, URL di destinazione, parametri URL, ID di tracciamento | Account, campagna, gruppo di annunci, logo |
| ChatGPT | Schede chat | Titolo, corpo | URL di destinazione, ID di tracciamento | Account annuncio OpenAI, Campagna OpenAI, Gruppo annunci OpenAI |
| Il Trade Desk | Visualizzazione statica | n/d | ID tracciamento | Account, Campagna |

Per configurare i campi di installazione della piattaforma per un gruppo di formati di annunci, fai clic su **[!UICONTROL Gestisci impostazioni piattaforma]** e modifica i campi nella finestra di dialogo risultante.

![Finestra di dialogo Gestisci impostazioni piattaforma per la scelta di un account Meta, di una campagna e di un set di annunci](./images/manage-platform-settings.png)

Ogni campo **[!UICONTROL ID tracciamento]** è precompilato con il nome dell&#39;esperienza: la piattaforma pubblicitaria utilizza questo valore come nome dell&#39;annuncio o della creatività per la generazione di rapporti e la risoluzione dei problemi. Modifica il valore nella stessa posizione se desideri utilizzare qualcos’altro.

![Modifica di un campo ID di tracciamento in linea nella tabella di attivazione](./images/tracking-id-edit.png)

Per spostarsi più rapidamente tra i campi **[!UICONTROL ID di tracciamento]**, utilizzare le seguenti scelte rapide da tastiera:

* Premi **Invio** per aprire il campo di modifica per il **[!UICONTROL ID di tracciamento]** selezionato.
* Premi il tasto freccia **Su** o **Giù** per passare al campo **[!UICONTROL ID di tracciamento]** precedente o successivo nella colonna.
* Premi di nuovo **Invio** per salvare le modifiche.

## Rivedi e pubblica le esperienze sulle loro piattaforme di annunci

Verificare che ogni riga mostri [!UICONTROL Pronto per l&#39;attivazione]. [!DNL Activate] flag mancanti o non validi, chiamate all&#39;azione non compatibili e ID di tracciamento duplicati come [!UICONTROL Richiede attenzione]. Quando ogni riga è pronta, fai clic su **[!UICONTROL Invia alle piattaforme]** e conferma nella finestra di dialogo di pubblicazione.

![Tabella di attivazione in cui ogni riga mostra Pronto per l&#39;attivazione, abilitazione dell&#39;invio alle piattaforme](./images/ready-to-activate.png)

[!DNL Activate] segnala lo stato di ogni annuncio quasi in tempo reale: In sospeso, quindi Inviato alle piattaforme o Non riuscito. Se un annuncio non riesce, passa il cursore del mouse sul relativo stato per visualizzare l’errore della piattaforma. È possibile riprovare contemporaneamente ogni annuncio non riuscito nella tabella facendo clic su **[!UICONTROL Riprova]**, anziché riprovare singolarmente. Le righe già inviate alle piattaforme non possono essere inviate nuovamente e includono un collegamento profondo all’annuncio nel gestore di annunci nativo della piattaforma di destinazione. La revisione finale pre-pubblicazione e l&#39;avvio degli annunci si verificano nel gestore degli annunci della piattaforma di destinazione: [!DNL Activate] distribuisce sempre gli annunci in uno stato inattivo.

![Tabella di attivazione che mostra una combinazione di stati In sospeso e Inviato alle piattaforme dopo la pubblicazione](./images/activation-status-pending.png)

Le tabelle di attivazione vengono visualizzate nella pagina di destinazione [!DNL Activate].

## Piattaforme supportate

Ogni piattaforma di annunci a pagamento dispone di campi di configurazione e prerequisiti specifici. Seleziona la piattaforma di annunci a pagamento per le linee guida sull’attivazione:

* [Meta](activate-meta-ad.md)
* [LinkedIn](activate-linkedin-ad.md)
* [Gestione campagne Google 360](activate-cm360-ad.md)
* [Amazon Ads](activate-amazon-ad.md)
* [Innovid](activate-innovid-ad.md)
* [TikTok](activate-tiktok-ad.md)
* [YouTube](activate-youtube-ad.md)
* [ChatGPT](activate-chatgpt-ad.md)
* [Il Trade Desk](activate-trade-desk-ad.md)
