---
title: Panoramica delle campagne
description: Guarda una panoramica del coinvolgimento dei clienti, delle prestazioni, del budget e delle spese per le campagne di marketing in Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Reporting and Insights, Ad Performance
exl-id: 99059c81-0fef-4759-b52b-d6f7f9f82a52
source-git-commit: 494afe3f823c78eecd10ccc321cd83d69336077b
workflow-type: tm+mt
source-wordcount: '713'
ht-degree: 0%

---

# Panoramica delle campagne

La visualizzazione [!DNL Insights] _[!UICONTROL Campagne]_ mostra un elenco di campagne per l&#39;account annuncio del canale connesso.

{{connect-insights}}

La tabella _[!UICONTROL Campagne]_ è organizzata utilizzando la campagna pubblicitaria basata su canale. Fai clic sull’icona delle impostazioni (cog) sopra il lato destro della tabella per attivare/disattivare le colonne visualizzabili.

![Filtro campagne e tabella](/help/assets/insights-campaigns-filter.png){zoomable="yes"}

Quando selezioni una campagna, la scheda [[!UICONTROL Annunci]](ads.md) si apre in un elenco di nomi di annunci associati alla campagna, che ti consente di identificare quali annunci hanno contribuito al suo successo complessivo.

{{filter-table}}

## Obiettivi

Al momento della creazione di una campagna con Meta ads, potresti aver selezionato un obiettivo in linea con i tuoi obiettivi aziendali. In GenStudio for Performance Marketing sono visibili sei obiettivi degli annunci Meta:

1. **Consapevolezza**: raggiungi il pubblico più vasto e sensibilizza la tua azienda.
1. **Traffico**: aumenta il traffico verso il sito o l&#39;applicazione.
1. **Coinvolgimento**: interagire con clienti esistenti e potenziali.
1. **Lead**: crea connessioni per espandere il pubblico.
1. **Promozione app**: promuovi la tua applicazione.
1. **Vendite**: concentrati su come raggiungere le persone che probabilmente useranno il tuo prodotto.

## Prestazioni del canale

A seconda degli obiettivi prestazionali, le metriche [!DNL Insights] possono essere utili per valutare se si sta raggiungendo l&#39;obiettivo.

Ad esempio, se l&#39;obiettivo è la consapevolezza, un aumento del tasso di `impressions` potrebbe indicare l&#39;espansione della portata. Per capire se questo sta raggiungendo il tuo obiettivo, puoi guardare le metriche che indicano che il tuo contenuto è coinvolgente, come `clicks` o `video plays`. In che modo il pubblico interagisce efficacemente con i contenuti?

La tabella seguente fornisce definizioni e informazioni approfondite per le metriche chiave del marketing digitale nella vista Canali. Ogni metrica include una breve definizione relativa ai canali, del modo in cui viene calcolata e una o più informazioni per comprenderne il significato e l’impatto sulle campagne di marketing.

| Metrica | Definizione | Insight |
| ----------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Nome campagna Meta]** | Elenco di nomi di campagne per l’account del canale connesso. Lo stato della campagna può essere `Active`, `Paused`, `Deleted` o `Archived`. Filtra le campagne per stato e obiettivo. | Ordina la tabella facendo clic sull’intestazione di colonna per una qualsiasi delle metriche chiave. |
| **[!UICONTROL Lancio]** | La data in cui la campagna è stata rilasciata o pubblicata sul mercato. | Un conteggio elevato delle impression può indicare che l’annuncio sta raggiungendo il pubblico previsto. |
| **[!UICONTROL Impression]** | Un conteggio di ogni caricamento di contenuto nel canale, indipendentemente dall’interazione o dalla visualizzazione. | Un conteggio elevato delle impression può indicare un’ampia visibilità, ma per insight con prestazioni reali, consideralo insieme ad altre metriche di coinvolgimento. |
| **[!UICONTROL Clic]** | Il numero di volte in cui gli utenti interagiscono con un elemento cliccabile, ad esempio un collegamento o un pulsante call-to-action, all’interno della campagna pubblicitaria. | Un numero elevato di clic indica un forte interesse e coinvolgimento per il contenuto, che può essere efficace e raggiungere il pubblico giusto. |
| **[!UICONTROL CTR ]**<br>_Percentuale di click-through_ | Percentuale (%) di impression che hanno generato clic sulla campagna all’interno di un canale.<br>**Calcolo**: (`clicks` diviso per `impressions`) x 100 = % | Un elevato tasso di click-through indica che il contenuto è altamente pertinente e motivante per il pubblico nella messaggistica e nella progettazione, e sta mirando in modo efficace agli interessi del pubblico. |
| **[!UICONTROL CPM ]**<br>_Costo per mille_ | Costo per ogni mille impression pubblicitarie per la campagna pubblicitaria. <br>**Calcolo**: (importo totale `spent` diviso per `impressions`) x 1000 | Un valore basso può indicare una visibilità a costi contenuti, soprattutto se associata a un elevato tasso di click-through. |
| **[!UICONTROL CPC ]**<br>_Costo per clic_ | Costo medio associato a ogni clic in una campagna pubblicitaria.<br>**Calcolo**: importo totale `spent` diviso per `clicks` = $ | Costi medi più bassi possono indicare una spesa pubblicitaria efficiente in termini di costi, soprattutto se confrontata con un aumento delle conversioni. |
| **[!UICONTROL Riproduzioni video]** | Il numero di volte in cui un video inizia a essere riprodotto in una campagna pubblicitaria, escluse le riproduzioni. La riproduzione di un video viene avviata quando l’utente fa clic su di essa o quando il video viene riprodotto automaticamente. | Un numero elevato di riproduzioni video può indicare che il video sta catturando l’attenzione e può indicare che la miniatura, il titolo o il posizionamento stanno effettivamente disegnando negli spettatori. |
| **[!UICONTROL Budget]** | Totale dei fondi stanziati per una campagna pubblicitaria per raggiungere gli obiettivi della campagna. | Un bilancio elevato implica maggiori risorse per una portata più ampia e un impatto potenzialmente maggiore. |
| **[!UICONTROL Spesa]** | L’importo speso dal budget in un dato periodo di tempo per inserire annunci tra diverse piattaforme. | Un importo di spesa elevato in un breve periodo può indicare un utilizzo rapido, che potrebbe portare a un precoce esaurimento delle risorse. Monitora l’importo speso rispetto alle metriche delle prestazioni chiave per monitorare il ritorno complessivo sull’investimento. |
