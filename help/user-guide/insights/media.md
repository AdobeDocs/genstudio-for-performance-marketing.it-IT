---
title: Panoramica dei contenuti multimediali
description: Scopri come valutare le prestazioni multimediali in Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Reporting and Insights, Media Performance, Content Attributes
exl-id: 1e93422b-2645-4e29-a216-fc1008afbfc7
source-git-commit: 8a5d15df7a347c4ee7767610fc9bb23fc7b71db4
workflow-type: tm+mt
source-wordcount: '664'
ht-degree: 0%

---

# Panoramica dei contenuti multimediali

La visualizzazione [!DNL Insights] _[!UICONTROL File multimediali]_ mostra un elenco di file multimediali utilizzati negli annunci e nelle campagne pubblicitarie per l&#39;account selezionato. _Media_ rappresenta un&#39;immagine, un video, un testo o altro contenuto creativo approvato per l&#39;utilizzo nelle iniziative di marketing.

{{connect-insights}}

La tabella _[!UICONTROL Media]_ è organizzata con **[!UICONTROL ID file multimediale]**. È possibile passare da una visualizzazione all&#39;altra utilizzando l&#39;icona dell&#39;elenco delle visualizzazioni (tabella) e l&#39;icona della visualizzazione della raccolta (griglia). Fai clic sull’icona delle impostazioni (cog) sopra il lato destro della tabella per attivare/disattivare le colonne visualizzabili. L&#39;icona del filtro (funnel) sopra il lato sinistro della tabella apre il menu **[!UICONTROL Filtro]** in cui è possibile selezionare più elenchi. Seleziona **[!UICONTROL Cancella tutto]** sopra la tabella per rimuovere tutti i filtri.

![Filtro supporti e tabella](/help/assets/insights-media-filter.png){zoomable="yes"}

{{$include /help/_includes/download-insights.md}}

La visualizzazione della galleria _[!UICONTROL File multimediali]_ mostra un collage di anteprime multimediali e una metrica, ad esempio il tasso di click-through. Fai clic sull&#39;icona delle impostazioni (cog) sopra il lato destro della galleria per aprire **[!UICONTROL Impostazioni scheda]** e attivare/disattivare una delle tre metriche visualizzabili:

- CPA (Costo per azione)
- CTR (tasso di click-through)
- CPC (costo per clic)
- Spesa

## Dettagli contenuti multimediali

Nella visualizzazione _Dettagli file multimediali_, puoi vedere quali annunci utilizzano i file multimediali selezionati. I dettagli includono prestazioni multimediali totali, annunci tramite l’elemento multimediale, attributi definiti dall’utente e funzioni rilevate da IA associate all’elemento multimediale.

![Dettagli file multimediali](/help/assets/insights-media-details.png){zoomable="yes"}

## Prestazioni multimediali

Le metriche di Insights possono aiutarti a valutare quali elementi multimediali contribuiscono al successo di una campagna e quali attributi multimediali sono più efficaci.

La tabella seguente fornisce definizioni e informazioni approfondite per le metriche di marketing digitale chiave nella vista tabella [!UICONTROL Media]. Ogni metrica include una breve definizione relativa ai contenuti multimediali, del modo in cui viene calcolata e una o più informazioni per comprenderne il significato e l’impatto.

| Metrica | Definizione | Insight |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL ID supporto]** | Il nome associato a un’immagine, un video, un testo o un altro contenuto creativo. | Ordina la tabella facendo clic sull’intestazione di colonna per una qualsiasi delle metriche chiave. |
| **[!UICONTROL Impression]** | Un conteggio di ogni volta che il contenuto multimediale viene caricato nel canale, indipendentemente dall’interazione o dalla visualizzazione. | Un conteggio elevato delle impression può indicare un’ampia visibilità, ma per informazioni approfondite sulle prestazioni, consideralo in relazione ad altre metriche di coinvolgimento. |
| **[!UICONTROL Clic]** | Il numero di volte in cui gli utenti interagiscono con un elemento cliccabile, come un collegamento, sul supporto. | Un numero elevato di clic indica un forte interesse e coinvolgimento per il contenuto, che può essere efficace e raggiungere il pubblico giusto. |
| **[!UICONTROL CTR ]**<br>_Percentuale di click-through_ | Percentuale (%) di impression che hanno generato clic sui contenuti multimediali all’interno di un annuncio.<br>**Calcolo**: `clicks` diviso per `impressions` | Un elevato tasso di click-through indica che i contenuti multimediali sono altamente pertinenti e coinvolgenti per il pubblico. Suggerisce che i messaggi e la progettazione catturino efficacemente l’interesse del pubblico e gli spingano ad agire. Inoltre, un CTR elevato può implicare che i media siano ben mirati e risuonino con il pubblico previsto, portando a migliori prestazioni complessive della campagna. |
| **[!UICONTROL CPM ]**<br>_Costo per mille_ | Costo per ogni mille impression multimediali.<br>**Calcolo**: importo totale `spent` diviso per il numero di impression, quindi moltiplicato per 1000 | Un valore CPM basso può indicare prestazioni multimediali convenienti, soprattutto se associato a un tasso di click-through elevato. |
| **[!UICONTROL CPA ]**<br>_Costo per azione_ | Costo medio speso per ottenere un’azione specifica del cliente, ad esempio un acquisto o un abbonamento.<br>**Calcolo**: importo totale `spent` diviso per il numero di azioni cliente completate | Consente di identificare i contenuti multimediali che si traducono in azioni utili per i clienti. |
| **[!UICONTROL CPC ]**<br>_Costo per clic_ | Costo medio associato a ogni clic sul supporto.<br>**Calcolo**: importo totale `spent` diviso per `clicks` | Costi medi più bassi possono indicare una spesa pubblicitaria efficiente in termini di costi, soprattutto se confrontata con un aumento delle conversioni. |
| **[!UICONTROL Spesa]** | L&#39;importo speso dal bilancio in relazione ai singoli media in un determinato periodo di tempo. | Un importo di spesa elevato in un breve periodo può indicare un utilizzo rapido, che potrebbe portare a un precoce esaurimento delle risorse. Monitora l’importo speso rispetto alle metriche delle prestazioni chiave per monitorare il ritorno complessivo sull’investimento. |
| **[!UICONTROL Utilizzato in questi annunci]** | Il numero di annunci che utilizzano questo supporto. | |
| **[!UICONTROL Attributi]** | Elenco di attributi rilevati e applicati al supporto. | |
