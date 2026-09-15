---
title: Creare un’esperienza di annunci Meta - Annunci carosello
description: Scopri come creare esperienze pubblicitarie con carosello Meta a più schede, gestire le schede e generare concetti on-brand in [!DNL GenStudio for Performance Marketing].
role: User
source-git-commit: 1b407c1c66a2426b21cbbf423774ebdff16a7dec
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 1%
---

# Creare un’esperienza di annuncio carosello Meta

Un annuncio carosello Meta è un formato di annuncio a pagamento che mostra da due a dieci schede wipeable, ciascuna con la propria immagine o video, titolo e collegamento.

Questa pagina descrive i passaggi specifici degli annunci carosello. Per i passaggi condivisi che non vengono ripetuti in questa pagina, ad esempio la scelta di un modello, l&#39;aggiunta di parametri, la revisione di varianti e la pubblicazione, vedere [Creare un&#39;esperienza di Meta Ad](/help/user-guide/create/create-meta-ad.md).

## Prerequisiti

Prima di creare un annuncio carosello, assicurati di disporre di un modello le cui pagine condividono tutte una proporzione, 1:1 o 4:5. Ogni pagina modello diventa una scheda. Per ulteriori informazioni, consulta [Linee guida per i modelli di annunci Meta](/help/user-guide/templates/meta-template.md).

## Scegli il formato del carosello

Dopo aver selezionato un modello e aver aperto l’area di lavoro, scegli il formato del carosello nel cassetto dei prompt.

1. Nel pannello _[!DNL Create your ads]_espandere_[!UICONTROL  Parametri ]_.
1. Dal menu a discesa **[!UICONTROL Formato]**, selezionare **[!UICONTROL Annuncio carosello]**.

   ![Crea il pannello degli annunci con il menu a discesa Formato impostato su Annuncio carosello e un elenco di schede](./carousel-format-cards.png){width="70%" zoomable="yes"}

Se inizi da un modello a pagina singola, [!DNL GenStudio for Performance Marketing] duplica la pagina per soddisfare il minimo di due schede. Se le pagine dei modelli non condividono tutte le stesse proporzioni, il parametro di formato viene bloccato finché non si utilizza un modello con proporzioni coerenti.

## Gestire le schede

Crea il set di schede nel cassetto delle richieste prima della generazione. Per aggiungere altre schede, duplica una scheda esistente.

* **Per duplicare una scheda**, seleziona **[!UICONTROL Duplica]** dalle opzioni della scheda.
* **Per riordinare le schede**, trascinare una scheda con il relativo handle in una nuova posizione.
* **Per eliminare una scheda**, selezionare **[!UICONTROL Elimina]** dalle opzioni della scheda. Le ultime due schede non possono essere eliminate, perché un carosello richiede almeno due schede.

Per ogni scheda, seleziona un’immagine e, se necessario, imposta un prodotto per scheda che sostituisce il prodotto principale. Puoi selezionare una sola immagine per scheda. Gli URL di destinazione per carta vengono impostati successivamente in [!DNL Activate]. Per ulteriori informazioni, vedere [Attivare un annuncio di Meta](/help/user-guide/activation/activate-meta-ad.md).

## Scrivi un prompt del carosello

Il prompt segnala l’intento del carosello, quindi descrivi la correlazione tra le schede. La copia carosello può seguire uno dei due approcci seguenti:

* **Modulare:** ogni scheda è un annuncio autonomo e nessuna copia scorre tra le schede. Utilizza questo approccio per una serie di messaggi correlati ma indipendenti, ad esempio diversi prodotti.
* **Sequenziale:** la copia si connette tra le schede per raccontare una storia, una sequenza dettagliata o una procedura. Utilizza questo approccio quando le schede si costruiscono l’una sull’altra.

Puoi anche descrivere se il carosello presenta uno o più prodotti, oltre a eventuali dettagli per scheda.

Ad esempio, questo prompt descrive un carosello modulare con più prodotti:

```properties
Create a multi-product carousel for our end-of-summer skincare sale. For each card, lead with the product's core benefit and emphasize the sale value.
```

Questo prompt descrive un carosello sequenziale che racconta una storia attraverso cinque schede:

```properties
Create a narrative carousel for our compliance alert-management platform. Start with shared intro text about the cost of alert fatigue. Across five cards, build the story: rising review costs, too many low-value alerts, false positives as the hidden cost driver, a solution that cuts false positives by more than 50%, and a closing learn-more call to action.
```

Per informazioni di base sui prompt, vedere [Scrivi prompt effettivi](/help/user-guide/effective-prompts.md).

## Generare e rivedere i concetti

Dopo aver impostato le schede e aver richiesto, genera il carosello e controlla i risultati.

1. Seleziona **[!UICONTROL Genera]**.

   [!DNL GenStudio for Performance Marketing] genera quattro concetti di carosello. Ogni concetto è un carosello multi-carta completo con il proprio marchio.

   ![Quattro concetti del carosello generati, ciascuno con un punteggio di marchio e un pulsante Modifica](./carousel-concepts.png){width="80%" zoomable="yes"}

1. Seleziona un concetto, quindi seleziona **[!UICONTROL Modifica]** per aprirlo per la modifica.
1. Utilizza le frecce per spostarti tra le schede, quindi modifica il testo o seleziona **[!UICONTROL Scambia]** per modificare l&#39;immagine di una scheda. Per ulteriori informazioni sulla modifica, vedere [Gestione varianti](/help/user-guide/create/manage-variants.md).

Se riordini le schede prima di generarle, l’area di lavoro viene aggiornata immediatamente. Se riordinate le schede nel cassetto delle richieste dopo la generazione, la modifica viene applicata solo dopo la nuova generazione e viene visualizzato un avviso di rigenerazione.

## Comprendere i campi condivisi e per scheda

Alcuni campi carosello si applicano a ogni scheda singolarmente, mentre altri si applicano all’intero annuncio. La tabella seguente descrive il comportamento di ciascun campo per gli annunci carosello Meta.

| Campo | Ambito |
|---|---|
| Titolo | Per scheda |
| Descrizione | Per scheda, facoltativo, impostato in [!DNL Activate] |
| Call to action | Condiviso nell’annuncio |
| Testo principale | Condiviso nell’annuncio |
| Media | Per scheda (immagine, video o mista) |
| Testo su immagine | Per scheda |
| URL di destinazione | Per scheda, impostato in [!DNL Activate] |

## Pubblicare, esportare e attivare

Quando il carosello è pronto, pubblicalo ed esportalo nello stesso modo che utilizzi per altri annunci Meta. Un carosello viene memorizzato come una singola esperienza che corrisponde a un concetto. Esportazione fornisce un file CSV e il supporto della scheda. Vedere [[!DNL Content]](/help/user-guide/content/overview.md) per informazioni sulla modalità di archiviazione delle esperienze pubblicate. Per attivare il carosello in Meta, vedi [Attivare un annuncio Meta](/help/user-guide/activation/activate-meta-ad.md).
