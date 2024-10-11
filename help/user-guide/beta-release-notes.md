---
title: Note sulla versione di Adobe GenStudio for Performance Marketing Beta
description: Scopri le funzioni e i miglioramenti più recenti di Adobe GenStudio for Performance Marketing.
hidefromtoc: true
exl-id: 2ae60dcb-ac95-4ed4-bceb-84b396f7fa4e
source-git-commit: 9b5e8b37ba988c3dd4a1e5a828487997375474ac
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 0%

---

# Note sulla versione di Adobe GenStudio for Performance Marketing Beta

Queste note evidenziano correzioni e miglioramenti significativi apportati ad Adobe GenStudio for Performance Marketing nella settimana che termina il 4 ottobre.

## Nuove funzioni e miglioramenti

* È stata migliorata la funzionalità di filtro in tutto il prodotto. Sono stati risolti i problemi relativi al filtro per età e genere in [!DNL Insights].  <!-- GS-1198 -->

* Puoi modificare le risorse immagine (JPG o PNG) direttamente da Adobe Express. Gli editor di contenuti possono utilizzare l&#39;area di lavoro _[!UICONTROL Powered by Adobe Express]_ per rimuovere gli sfondi, applicare riempimenti generativi, regolare effetti e ritagliare immagini senza uscire da GenStudio for Performance Marketing. <!-- GS-4615 -->

* È stata migliorata l’esperienza di caricamento progressivo per le varianti generate, e-mail generate e messaggistica contestuale. <!-- GS-4651 3062-->

* Gli editor di contenuti possono ora utilizzare la funzione di regolazione del ritaglio per ritagliare le immagini sottoposte a rendering in varianti. <!-- GS-2342 -->

* Sono stati risolti i problemi relativi al ridimensionamento e alla duplicazione dei modelli. <!-- GS-4895 -->

* La convalida del brand ora spiega la causa degli errori che si verificano durante la convalida.

* Le anteprime dei modelli ora visualizzano il testo sull&#39;immagine come previsto. <!-- GS-5917 -->

## Ulteriori miglioramenti e problemi risolti

* L&#39;area di lavoro [!DNL Create] ora esegue il rendering dei tipi di carattere personalizzati dai modelli come previsto. <!-- GS-3415 -->

* Il font corretto viene ora applicato durante l’esportazione di annunci Meta. <!-- GS-5875 -->

* Sono stati risolti i problemi relativi al caricamento dei modelli che hanno portato al caricamento corretto, ma che non hanno mostrato visibilità nell’interfaccia del prodotto. <!-- GS-4815 5650-->

* Gli utenti possono ora ritagliare manualmente i metadati dopo averli ridimensionati. <!-- GS-5871 -->

* Gli utenti non dovranno più accedere due volte a un account di canale Meta ads quando accedono anche a Facebook. <!-- GS-3009 -->

* La visualizzazione Area di lavoro delle risorse e delle esperienze ora rimane coerente nel processo di creazione, revisione e approvazione dei contenuti. <!-- GS-5877 -->

* L’area di lavoro ora visualizza solo quattro varianti durante la rigenerazione dopo un’operazione di ridimensionamento. <!-- GS-5869 -->

* Il controllo ortografico basato su browser ora funziona come previsto nell&#39;area di lavoro [!DNL Create]. <!-- GS-5760 -->

* Gli annunci visualizzati ora vengono esportati come file PNG quando si seleziona **[!UICONTROL Esporta come PNG]**. In precedenza, gli annunci visualizzati venivano esportati come JPEG quando era selezionato il formato PNG. <!-- GS-5545 -->

* La spaziatura è stata aumentata tra il pulsante **[!UICONTROL Ritaglio manuale]** e il pulsante **[!UICONTROL Genera]**. In precedenza, il pulsante **[!UICONTROL Ritaglio manuale]** era parzialmente oscurato. <!-- GS-6084 -->

* Nelle anteprime dei modelli ora vengono visualizzati i font di Google come previsto. <!-- GS-5946 -->

* I font TypeKit e Google importati vengono ora caricati come previsto durante l&#39;esportazione. <!-- GS-5948 -->

* Sono stati risolti dei problemi relativi alla generazione di contenuti con modelli personalizzati. In precedenza, quando un editor di contenuti tentava di generare una risorsa utilizzando un modello personalizzato, la finestra a comparsa di generazione non veniva visualizzata e nella console venivano visualizzati degli errori. <!-- GS-5262 -->

* L&#39;area di lavoro 2D di DisplayAds ora mantiene la propria posizione quando un utente fa clic con il pulsante destro del mouse sull&#39;area di lavoro prima di fare clic con il pulsante sinistro del mouse fuori dal menu di scelta rapida. In precedenza, l’area di lavoro si spostava quando l’utente faceva clic con il pulsante sinistro del mouse, rendendo parzialmente inaccessibile il contenuto della bozza.  <!-- GS-5687 -->

* Il caricamento degli effetti shimmer persiste fino al completamento della rigenerazione dell&#39;immagine.  <!-- GS-5811 -->

* I punteggi di convalida del brand non vengono più invalidati dopo che un utente ha apportato modifiche alle e-mail, ai metadati o agli annunci di visualizzazione generati. In precedenza, questo punteggio era nascosto. <!-- GS-5379 -->

* I modelli con stili CSS associati al relativo elemento `body` ora vengono utilizzati come previsto durante l&#39;esportazione delle esperienze. <!-- GS-5947 -->

* Sono stati risolti i problemi relativi al ritaglio manuale di immagini di grandi dimensioni. <!-- GS-6039 -->

* Ora quando un utente aggiunge una nuova risorsa in [!DNL Content] viene visualizzato un solo messaggio popup. <!-- GS-5020 -->

* Sono state migliorate le prestazioni di Canvas durante la modifica del testo.  <!-- GS-5118 -->

* Sono stati aggiunti spazi mancanti tra le stringhe nell&#39;area di lavoro dell&#39;e-mail o del meta annuncio di [!DNL Create]. <!-- GS-5019 -->

* Dopo aver apportato le modifiche in Express, gli editor possono ora salvare un file con nomi che contengono caratteri speciali. <!-- GS-6131 -->

### Localizzazione

Questa versione include miglioramenti alla localizzazione in tutta l’interfaccia del prodotto, incluse le seguenti aree dell’interfaccia:

* L&#39;URL per la destinazione dell&#39;opzione **[!UICONTROL Ulteriori informazioni]** nel menu del prompt [!DNL Create]. <!-- GS-5029 -->

* Formati numerici adiacenti ai campi di input per la ricerca [!DNL Insights] > [!DNL Experience]. <!-- GS-4494 -->

## Problema noto

* I frammenti e-mail rigenerati non vengono visualizzati nella variante dopo la selezione. Dopo la riapertura della bozza vengono tuttavia visualizzate alcune varianti. <!-- GS-5913 -->
