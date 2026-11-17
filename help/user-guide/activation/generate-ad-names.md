---
title: Genera nomi annunci
description: Scopri come configurare modelli di denominazione, generare nomi di annunci coerenti e rivedere o personalizzare i nomi prima di inviare annunci alle piattaforme di attivazione supportate.
role: User
source-git-commit: 888a9509ed1c3705f67fbf541b38a49b7890ac7d
workflow-type: tm+mt
source-wordcount: '1746'
ht-degree: 1%
---

# Genera nomi di annunci

La denominazione automatica degli annunci in [!DNL GenStudio for Performance Marketing] ti consente di seguire le convenzioni di denominazione della tua organizzazione quando attivi gli annunci. I nomi coerenti supportano il reporting delle prestazioni, l’attribuzione e la riconciliazione della spesa.

Un modello di denominazione definisce le parti di un nome di annuncio e il loro ordine. Le parti di esempio includono il prodotto, la campagna e il mercato. Per creare un modello, carica un file Excel che descriva la convenzione di denominazione della tua organizzazione.

Utilizza il modello per generare nomi dalle informazioni su ogni esperienza, ad esempio il prodotto o la campagna. Rivedi e correggi i risultati prima di inviare i tuoi annunci. I nomi finali vengono inviati a ciascuna piattaforma di destinazione come nomi degli annunci.

## Prima di iniziare

È sufficiente impostare un modello una sola volta. Se alla tua piattaforma è già stato assegnato un modello nel progetto corrente, vai direttamente a [Genera nomi per un&#39;attivazione](#generate-names-for-an-activation).

In caso contrario, crea un modello e chiedi a un manager di sistema di [assegnarlo alle piattaforme](#assign-a-template-to-platforms). Ogni progetto può avere un modello predefinito diverso per la stessa piattaforma.

Per l&#39;impostazione dei modelli, preparare un file Excel di dimensioni non superiori a 3 MB con un solo foglio. I file CSV non sono supportati. Descrivi la convenzione di denominazione per singoli annunci, non campagne o gruppi di annunci.

Elencare i campi nell&#39;ordine richiesto. Per ogni campo, includi i valori consentiti, i codici corrispondenti e le istruzioni per la scelta di un valore. Ad esempio, l&#39;opzione `Image` per il campo `format` utilizza il codice `IMG` nel nome.

Per una struttura di esempio, scaricare l&#39;esempio di convenzione di denominazione di Meta [WKND (Excel)](assets/wknd-meta-naming-convention.xlsx). Il file definisce campi e valori di esempio per prodotto, campagna, mercato e altre parti di un nome di annuncio.

Sostituisci i valori e le regole di esempio con la convenzione della tua organizzazione prima di utilizzare il file per le tue attivazioni. I valori di piattaforma dell’esempio illustrano le scelte di denominazione, non un elenco di destinazioni di attivazione supportate.

## Creare un modello di denominazione

Crea un modello dal file delle convenzioni di denominazione esistente, quindi controlla la struttura estratta prima di utilizzarla.

1. Apri il progetto in cui desideri utilizzare il modello.
1. Vai a **[!UICONTROL Altro]** > **[!UICONTROL Impostazioni]**.
1. Seleziona **[!UICONTROL Configura]** accanto a **[!UICONTROL Modello nome annuncio]**.

   Se i modelli esistono già, apri **[!UICONTROL Modello nome annuncio]**, quindi seleziona **[!UICONTROL Crea modello]**.

1. Selezionare **[!UICONTROL Seleziona file]** nella finestra di dialogo **[!UICONTROL Carica file]**.
1. Scegliere il file di Excel.

   In alternativa, trascina il file nell’area di caricamento. Durante l&#39;analisi del foglio di calcolo **[!UICONTROL in corso...]**, i campi e i valori sono mappati al modello. Attendere alcuni minuti per il completamento dell&#39;analisi.

1. Rivedi i campi, i valori consentiti e **[!UICONTROL Anteprima nome annuncio]**.

   L’anteprima utilizza valori di esempio, non i dettagli di un annuncio specifico.

1. Seleziona **[!UICONTROL Salva]**.

I file di dimensioni superiori a 3 MB, i tipi di file non supportati e i file vuoti mostrano un errore senza modificare i modelli o le assegnazioni di piattaforma esistenti.

## Personalizzare un modello

Modifica un modello salvato per modificarne il nome, i campi, il separatore o le regole.

1. Vai a **[!UICONTROL Altro]** > **[!UICONTROL Impostazioni]** > **[!UICONTROL Modello nome annuncio]**.
1. Apri il menu a tre punti accanto al modello.
1. Seleziona **[!UICONTROL Modifica]**.
1. Per rinominare il modello, seleziona l’icona a forma di matita accanto al titolo.
1. Impostare il **[!UICONTROL Separatore di campo]** sul carattere che separa le parti del nome, ad esempio un carattere di sottolineatura (`_`).
1. Trascinare i campi nell&#39;ordine desiderato.

   Utilizza **[!UICONTROL Aggiungi campo]** o l&#39;icona del cestino di un campo per modificare i campi inclusi.

1. Per aprire le impostazioni di un campo, selezionare l&#39;icona della matita corrispondente.
1. Rivedi **[!UICONTROL Tipo]** e **[!UICONTROL Nome]** nella finestra di dialogo **[!UICONTROL Modifica campo]**.

   Utilizza **[!UICONTROL Elenco a discesa]** per un campo con scelte predefinite o **[!UICONTROL Testo libero]** per un valore immesso.

1. Per un campo a discesa, controlla **[!UICONTROL Opzioni]** e **[!UICONTROL Codice]**.

   **[!UICONTROL Opzioni]** contiene le scelte leggibili. **[!UICONTROL Il codice]** contiene i valori corrispondenti utilizzati nel nome dell&#39;annuncio. Ad esempio, l&#39;opzione `Image` utilizza il codice `IMG`.

   Per aggiungere una scelta, selezionare **[!UICONTROL Aggiungi opzione]**. Per rimuovere una scelta, selezionarne l&#39;icona meno. Non sono consentiti valori duplicati all’interno di un campo.

1. Immetti le **[!UICONTROL regole campo]** necessarie per scegliere o formattare il valore del campo.

   Per il campo a testo libero `creativeVersion`, immettere questa regola di esempio: `Use the experience name as a starting value, with spaces removed.`

1. Seleziona **[!UICONTROL Salva]** nella finestra di dialogo del campo.

   Ripeti la revisione del campo per tutti gli altri campi che richiedono modifiche.

1. Immettere le **[!UICONTROL regole modello]** applicabili al nome.

   Ad esempio, immettere `Remove spaces from Product and Campaign values.`

1. Seleziona **[!UICONTROL Salva]** nella parte superiore della pagina.

L’anteprima riflette l’ordine dei campi e il separatore aggiornati. Per verificare le modifiche salvate, riapri il modello.

L’editor di campi mostra la corrispondenza delle opzioni leggibili con i codici inclusi nei nomi generati:

![Modifica una finestra di dialogo di campo con le opzioni di formato Immagine, Video, Carosello e HTML5 e i codici corrispondenti.](images/ad-name-field-options-codes.png)

## Assegnare un modello alle piattaforme

I System Manager impostano il modello predefinito per ogni piattaforma all&#39;interno di un progetto. Se non sei un system manager, chiedi a uno di completare questa procedura.

1. Apri il progetto di cui desideri impostare la piattaforma predefinita.
1. Vai a **[!UICONTROL Altro]** > **[!UICONTROL Impostazioni]** > **[!UICONTROL Modello nome annuncio]**.
1. Apri il menu a tre punti accanto al modello.
1. Seleziona **[!UICONTROL Modifica]**.
1. Seleziona una o più piattaforme in **[!UICONTROL Piattaforme preferite]** nella parte inferiore dell&#39;editor.
1. Seleziona **[!UICONTROL Salva]**.

Ogni piattaforma ha un modello predefinito per progetto. Puoi assegnare lo stesso modello a diverse piattaforme.

I modelli sono disponibili per la visualizzazione e la modifica in più progetti. Tuttavia, puoi modificare le assegnazioni della piattaforma solo nel progetto corrente.

La sostituzione dell’impostazione predefinita di una piattaforma non elimina il modello precedente né modifica le assegnazioni di altri progetti.

L&#39;esempio seguente mostra l&#39;anteprima del modello, l&#39;ordine dei campi, le regole e le **[!UICONTROL piattaforme preferite]** con Meta Ads selezionato:

![Editor modelli WKND con un separatore di sottolineatura, 12 campi nome annuncio, regole modello e Meta Ads selezionati in Piattaforme preferite.](images/ad-name-template-editor.png)

## Generare nomi per un&#39;attivazione

Prepara l’attivazione prima di generare i nomi. I metadati di ogni esperienza contengono informazioni quali la campagna, il prodotto o l’utente tipo. Verifica che i metadati forniscano i valori necessari per il modello. Consulta [Flusso di lavoro di attivazione](create-activation.md) per assistenza nella preparazione di un&#39;attivazione.

Quando crei un’attivazione per la prima volta, il nome iniziale di ciascun annuncio dipende dall’assegnazione del modello della relativa piattaforma:

| Configurazione della piattaforma | Nome annuncio iniziale |
| --- | --- |
| Nel progetto corrente viene assegnato un modello di denominazione. | I campi modello vuoti vengono visualizzati come segnaposto, ad esempio `[market]_[year]`. I nomi vengono generati solo dopo aver selezionato **[!UICONTROL Genera nome annuncio]**. |
| Nessun modello di denominazione assegnato nel progetto corrente. | L’annuncio utilizza il nome della sua esperienza. La generazione dei nomi lascia invariato il nome. |

1. Apri **[!UICONTROL Attiva]** nel progetto previsto.
1. Aggiungi le tue esperienze a un’attivazione.
1. Completa la configurazione della piattaforma e tutte le informazioni richieste, tra cui copia, call-to-action (CTA) e l’URL del sito web.
1. Verifica che le esperienze dispongano dei metadati necessari per la convenzione di denominazione.
1. Selezionare **[!UICONTROL Genera nome annuncio]** sopra la tabella di attivazione.

   Attendere il completamento della **[!UICONTROL generazione dei nomi di annunci]** prima di rivedere i risultati.

1. Rivedi la colonna **[!UICONTROL Nome annuncio]**.

La generazione si applica a tutti gli annunci sulle piattaforme a cui è assegnato un modello, ad eccezione degli annunci con [sostituzioni di nomi personalizzate](#use-a-custom-ad-name). I nomi non vengono generati automaticamente all&#39;apertura della tabella.

Per le piattaforme a cui non è stato assegnato un modello, modifica manualmente i nomi degli annunci basati sull’esperienza in base alle esigenze.

Se non è stato assegnato alcun modello a nessuna piattaforma, non viene generato alcun nome.

## Correggere un singolo nome annuncio

Rivedi i nomi generati prima di inviare i tuoi annunci. Tutti i campi che rimangono vuoti dopo la generazione vengono visualizzati come segnaposto evidenziati, ad esempio `[market]`. Gli annunci interessati mostrano **[!UICONTROL Richiede attenzione]**.

Per trovare i nomi che richiedono correzioni, cercare i segnaposto evidenziati e gli stati **[!UICONTROL Richiede attenzione]** nella tabella di attivazione:

![Tabella di attivazione con un&#39;avvertenza per valori mancanti, segnaposto di mercato evidenziati nella colonna Nome annuncio e stati di attenzione necessari.](images/ad-names-missing-values.png)

1. Seleziona la riga dell’annuncio nella tabella di attivazione.
1. Seleziona **[!UICONTROL Modifica nome annuncio]**.
1. Aggiorna i menu a discesa o i campi di testo pertinenti.
1. Seleziona **[!UICONTROL Salva]**.

Ad esempio, se `market` non ha un valore, immettere o selezionare il mercato appropriato per sostituire `[market]` nel nome.

Verifica il nome aggiornato in base alla convenzione.

## Risolvi potenziali nomi duplicati

Nomi di annunci identici sulla stessa piattaforma sono contrassegnati come potenziali duplicati.

1. Seleziona uno degli annunci interessati.
1. Seleziona **[!UICONTROL Modifica nome annuncio]**.
1. Modificare il nome in modo che i due nomi siano diversi.
1. Seleziona **[!UICONTROL Salva]**.

L’avviso di potenziale duplicazione si cancella dopo che i nomi sono stati resi diversi.

## Modificare più nomi di annunci {#edit-several-ad-names-at-once}

Utilizza la modifica in serie per applicare una correzione condivisa mantenendo allo stesso tempo valori diversi tra gli annunci.

1. Seleziona gli annunci utilizzando le relative caselle di controllo di riga.
1. Seleziona **[!UICONTROL Modifica nome annuncio]** dalla barra degli strumenti di selezione.
1. Modifica solo i campi che richiedono lo stesso valore negli annunci selezionati.

   **[!UICONTROL I valori misti]** indicano che gli annunci selezionati hanno attualmente valori diversi per un campo. Lascia questo campo intatto per mantenere il valore di ogni annuncio.

1. Seleziona **[!UICONTROL Salva]**.
1. Esamina i nomi aggiornati per verificare la precisione e i potenziali duplicati.

Solo gli annunci selezionati vengono aggiornati. Gli annunci non selezionati rimangono invariati.

L&#39;editor bulk visualizza **[!UICONTROL valori misti]** per campi che differiscono tra gli annunci selezionati:

![Dettagli della finestra di dialogo Modifica 4 nomi di annunci che mostra valori misti per prodotto, campagna, creativeVersion e persona.](images/ad-names-bulk-edit.png)

Ad esempio, se si modifica solo l&#39;utente tipo da `OutdoorBeginners` a `Adventurers`, i diversi prodotti verranno mantenuti. I seguenti nomi abbreviati illustrano la modifica:

| Prima | Dopo |
| --- | --- |
| `WKND_TrailBag_OutdoorBeginners` | `WKND_TrailBag_Adventurers` |
| `WKND_RiosShirt_OutdoorBeginners` | `WKND_RiosShirt_Adventurers` |

## Utilizza un nome annuncio personalizzato

Invece di modificare singoli campi modello, utilizza una sostituzione per sostituire l’intero nome generato con un nome personalizzato.

1. Seleziona la riga dell’annuncio.
1. Seleziona **[!UICONTROL Modifica nome annuncio]**.
1. Attiva **[!UICONTROL Sostituisci nomi annunci]**.
1. Immetti il nome personalizzato.
1. Seleziona **[!UICONTROL Salva]**.

Il nome personalizzato rimane invariato quando si generano di nuovo i nomi.

Con la sostituzione abilitata, modifica il nome completo anziché i singoli campi modello:

![Finestra di dialogo Modifica nome annuncio con l&#39;opzione Ignora nomi annuncio abilitata e il nome completo dell&#39;annuncio WKND disponibile per la modifica.](images/ad-name-override.png)

Per tornare alla denominazione basata su modello, effettuare le seguenti operazioni:

1. Apri **[!UICONTROL Modifica nome annuncio]** per l&#39;annuncio.
1. Disattiva **[!UICONTROL Sostituisci nomi annunci]**.
1. Seleziona **[!UICONTROL Salva]**.
1. Selezionare **[!UICONTROL Genera nome annuncio]** sopra la tabella di attivazione.

Questa azione rigenera anche i nomi per altri annunci nella tabella a cui è stato assegnato un modello e a cui non è stata assegnata alcuna sostituzione del nome personalizzato.

## Rispondi alle modifiche al modello

Quando si modifica una tabella di attivazione, viene visualizzato un avviso se un modello utilizzato è stato modificato o eliminato.

Se il modello è stato modificato, esaminare il modello aggiornato prima di rigenerare i nomi. Seleziona **[!UICONTROL Genera nome annuncio]** per applicarlo.

Se il modello è stato eliminato o è necessario sostituirlo, effettua le seguenti operazioni:

1. Chiedere a un responsabile di sistema di assegnare un modello sostitutivo alla piattaforma interessata nello stesso progetto.
1. Torna alla tabella di attivazione.
1. Selezionare **[!UICONTROL Genera nome annuncio]**.
1. Rivedi i nomi aggiornati.

I nomi con sostituzioni attivate rimangono invariati durante la rigenerazione.

## Inviare annunci alle piattaforme

Rivedi i nomi finali e i campi non risolti dell&#39;indirizzo, i potenziali duplicati e altri **[!UICONTROL Richiedi attenzione]** prima di inviare annunci.

Quando l&#39;attivazione è pronta, selezionare **[!UICONTROL Invia a piattaforme]**.

[!DNL GenStudio for Performance Marketing] invia il nome finale di ogni annuncio alla piattaforma di destinazione come nome dell&#39;annuncio. Il nome inviato include eventuali modifiche ai campi modello o alle sostituzioni di nomi personalizzati. I nomi degli annunci sulla piattaforma corrispondono esattamente ai nomi finali rivisti.

Per le destinazioni di visualizzazione come Innovid, i nomi vengono visualizzati come nomi creativi.
