---
title: Filtrare le visualizzazioni di Insights
description: Scopri come utilizzare le funzionalità di filtro avanzate con Insights.
level: Intermediate
feature: Reporting and Insights
exl-id: fbc53c2a-388c-4b51-94e2-626cd1e18e63
source-git-commit: 04bc6f911394d0f4c324abc347ce125203011960
workflow-type: tm+mt
source-wordcount: '868'
ht-degree: 0%

---

# Filtra per visualizzazioni Approfondimenti

Il dashboard [!DNL Insights] fornisce un set completo di filtri per un&#39;esperienza di esplorazione dati efficiente. Durante l’analisi di canali, annunci, contenuti multimediali o attributi specifici, le opzioni di filtro consentono di personalizzare la visualizzazione e semplificare il flusso di lavoro. Utilizza i filtri per parole chiave per un targeting preciso o esplora elenchi predefiniti per perfezionare la ricerca e concentrarti sui dati più importanti.

## Nozioni di base sui filtri

Ogni visualizzazione in [!DNL Insights] offre un elenco di opzioni filtro. Il filtro (funnel) a sinistra apre il menu **[!UICONTROL Filtro]**. Sia che si stia visualizzando la tabella o la raccolta, i filtri applicati vengono visualizzati nell&#39;elenco **[!UICONTROL Filtra per]** sopra la tabella o la raccolta. Per impostazione predefinita, sono selezionati un canale e un account.

![Filtra per](/help/assets/insights-filter-by.png "Filtra per"){width=600 zoomable="yes"}

I filtri applicati persistono in tutte le visualizzazioni. Seleziona **[!UICONTROL Cancella tutto]** sopra la tabella o la raccolta per rimuovere tutti i filtri selezionati.

### Campo di ricerca

Fare clic sull&#39;icona di ricerca (lente di ingrandimento) per digitare un termine di ricerca per individuare elementi specifici nella tabella o nella raccolta. Ad esempio, l&#39;immissione del termine `Gear` nella tabella [!UICONTROL Ads] filtra i risultati in modo da visualizzare solo gli annunci che utilizzano il termine `Gear` nel nome.

![Esempio di campo di ricerca](/help/assets/insights-search.png "Cerca annunci con Gear nel nome"){width=600 zoomable="yes"}

### Intervallo di date

Il selettore dell’intervallo di date è uno strumento utile per allineare i dati visualizzati agli obiettivi dell’analisi. Utilizza il selettore dell’intervallo di date per regolare l’intervallo di tempo per i dati visualizzati nella vista a tabella o a galleria. Per impostazione predefinita, l’intervallo di date è impostato sugli ultimi 30 giorni. Per includere più dati o concentrarsi su un periodo specifico, espandi l’intervallo di date.

![Selettore intervallo di date](/help/assets/insights-date-range.png "Seleziona un intervallo di date"){width=400}

Se nella vista a tabella o a galleria non viene visualizzato alcun elemento, la causa potrebbe essere l’intervallo di date selezionato, con l’esclusione dei dati rilevanti. In questi casi, aumenta l’intervallo di date per garantire che siano inclusi i dati desiderati.

### Pagine

Alcune tabelle possono occupare più pagine, come indicato di seguito nella tabella a destra. Utilizza le versatili opzioni di ricerca e filtro per perfezionare i risultati. Per spostarsi tra le pagine, utilizzare i controlli di impaginazione destra (avanti) e sinistra (indietro). Assicurati di applicare correttamente i filtri per includere tutti i dati rilevanti nelle pagine.

### Controllo diapositiva

Alcune opzioni di filtro includono un controllo diapositiva che consente di selezionare un valore all&#39;interno di un intervallo definito. Ad esempio, in _[!UICONTROL Attributi]_, il cursore **[!UICONTROL Conteggio file multimediali]** consente di filtrare gli attributi in base al numero di immagini o video associati. Trascinare il dispositivo di scorrimento per specificare un intervallo compreso tra un minimo di 0 e un massimo che può superare i 100.

## Filtro avanzato

Con i filtri _[!UICONTROL Campagne]_ e _[!UICONTROL Annunci]_, puoi sfruttare parole chiave precise per perfezionare l&#39;elenco. I filtri per parole chiave sono particolarmente utili per filtrare campagne o annunci che utilizzano una convenzione di denominazione complessa con più identificatori univoci. Ad esempio, il nome di una campagna può includere quanto segue:

- Nome o codice di regione specifico: `NA`, `EMEA`
- Acronimi del tipo di contenuto: `EB`, `CHT` o `DSP`
- Codici offerta o acronimi: `OFFER2023`, `PROMO`

Nel tempo, l’elenco di campagne e annunci potrebbe crescere in modo esponenziale. Considera lo scenario seguente per utilizzare il filtro _[!UICONTROL Campagne]_ per perfezionare la tabella [!UICONTROL Annunci].

**Per perfezionare la tabella Ads utilizzando il filtro Campaigns**:

1. In _[!DNL Insights]_, selezionare la visualizzazione **[!UICONTROL Annunci]**.

   ![Filtro annunci e tabella](/help/assets/insights-ads-filter.png "Visualizzazione annunci con menu filtro"){zoomable="yes"}

1. Fai clic sull&#39;interruttore del filtro (funnel) sopra il lato sinistro della tabella per aprire il menu **[!UICONTROL Filtro]**.

1. Verificare che il canale `Filter by` e l&#39;account selezionati siano corretti.

1. Espandi il filtro **[!UICONTROL Campagne]** e fai clic su **[!UICONTROL Seleziona]**.

   ![Filtra campagne](/help/assets/insights-filter-campaigns-expand.png "Espandi filtro campagne"){width=200}

1. Nel campo di ricerca _[!UICONTROL Seleziona campagne]_, immetti le parole chiave separate da virgole.

   Utilizza le parole chiave per perfezionare la ricerca con un filtro logico e preciso.

   - Per trovare i nomi delle campagne che contengono sia `adventure` **SIA** `ready`, immettere entrambe le parole chiave separate da una virgola:

     ![Cerca in tutte le parole chiave](/help/assets/insights-select-campaigns-and.png "Cerca nomi di campagne contenenti entrambe le parole chiave"){width=500}

   - Per trovare i nomi delle campagne che contengono `adventure` **OR** `ready`, immettere ogni parola chiave separatamente:

     ![Cerca parole chiave](/help/assets/insights-select-campaigns-or.png "Cerca nomi di campagne contenenti almeno una parola chiave"){width=500}

   - Per eseguire ricerche avanzate, combinare più set di parole chiave. Ad esempio, cerca i nomi delle campagne con `adventure` e `apparel` **OR** `sun` e `gear`:

     ![Cerca con più set di parole chiave](/help/assets/insights-advanced-or.png "Cerca i nomi delle campagne utilizzando più set di parole chiave"){width=500}

1. Seleziona una o più campagne dalla ricerca risultante e fai clic su **[!UICONTROL Applica]**.

   ![Elenco campagne](/help/assets/insights-select-campaigns-list.png "Seleziona campagne da includere")

Le campagne selezionate vengono ora visualizzate nell&#39;elenco _[!UICONTROL Filtra per]_ sopra la tabella o la raccolta di annunci. Puoi concentrarti esclusivamente sugli annunci collegati alle campagne selezionate. In questo esempio, i risultati filtrati includono 6 annunci, che forniscono una visualizzazione più mirata per l’analisi.

![Tabella filtrata per campagne](/help/assets/insights-filter-by-campaigns.png "Tabella con filtro campagne"){zoomable="yes"}

Puoi filtrare ulteriormente la tabella [!UICONTROL Media] in modo simile per i nomi di annunci. Espandi il filtro **[!UICONTROL Ads]** e fai clic su **[!UICONTROL Select]**. Puoi eseguire un filtro per parole chiave simile per perfezionare la tabella multimediale o la visualizzazione della galleria.

## Scarica risultati tabella

Puoi scaricare i risultati filtrati dalla vista tabella per ulteriori analisi o condivisioni. Fai clic sull’icona Scarica (freccia rivolta verso il basso) sopra il lato destro della tabella per scaricare un file CSV basato sulla tabella visualizzabile. Il download inizia automaticamente e inserisce il file CSV nel percorso di download predefinito.

Alcune tabelle possono avere più pagine, visibili nella parte destra della tabella. Il file CSV include i dati di _tutte_ pagine della tabella.
