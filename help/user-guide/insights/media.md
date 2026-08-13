---
title: Panoramica contenuti multimediali
description: Scopri come valutare le prestazioni multimediali in Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Reporting and Insights, Media Performance, Content Attributes
exl-id: 1e93422b-2645-4e29-a216-fc1008afbfc7
TQID: https://experienceleague.adobe.com/fSBgN1uvr39dd7AV3Kvr3D5UnSDY2-dE1aX1g2Q7fTc
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: f321b88b-6bb7-49cc-a16a-ae2b665ebd32
subfeature_v2:
  - id: a29f532b-105a-4aec-8a5d-e7e725214866
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
  - id: dd48f9df-f2e2-49fe-a918-332a8e240ffe
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 647
ht-degree: 0%

---

# Panoramica dei contenuti multimediali

La visualizzazione [!DNL Insights] _[!UICONTROL File multimediali]_ mostra un elenco di file multimediali utilizzati negli annunci e nelle campagne pubblicitarie per l&#39;account selezionato. _Media_ rappresenta un&#39;immagine, un video, un testo o altro contenuto creativo approvato per l&#39;utilizzo nelle iniziative di marketing.

{{connect-insights}}

La tabella _[!UICONTROL Media]_ è organizzata con **[!UICONTROL ID file multimediale]**. È possibile passare da una visualizzazione all&#39;altra utilizzando l&#39;icona dell&#39;elenco delle visualizzazioni (tabella) e l&#39;icona della visualizzazione della raccolta (griglia). Fai clic sull’icona delle impostazioni (cog) sopra il lato destro della tabella per attivare/disattivare le colonne visualizzabili.

![Filtro supporti e tabella](/help/assets/insights-media-filter.png){zoomable="yes"}

La visualizzazione della galleria _[!UICONTROL File multimediali]_ mostra un collage di anteprime multimediali e una metrica, ad esempio il tasso di click-through. Fai clic sull&#39;icona delle impostazioni (cog) sopra il lato destro della galleria per aprire **[!UICONTROL Impostazioni scheda]** e attivare/disattivare una delle tre metriche visualizzabili:

- CPA (Costo per azione)
- CTR (tasso di click-through)
- CPC (costo per clic)
- Spesa

{{filter-table}}

## Dettagli contenuti multimediali

Nella visualizzazione _Dettagli file multimediali_, puoi vedere quali annunci utilizzano i file multimediali selezionati. I dettagli includono prestazioni multimediali totali, annunci tramite l’elemento multimediale, attributi definiti dall’utente e funzioni rilevate da IA associate all’elemento multimediale.

![Dettagli file multimediali](/help/assets/insights-media-details.png){zoomable="yes"}

### Attributi multimediali

{{$include /help/_includes/generated-attributes.md}}

## Prestazioni multimediali

Le metriche di Insights possono aiutarti a valutare quali elementi multimediali contribuiscono al successo di una campagna e quali attributi multimediali sono più efficaci.

La tabella seguente fornisce definizioni e informazioni approfondite per le metriche di marketing digitale chiave nella vista tabella [!UICONTROL Media]. Ogni metrica include una breve definizione relativa ai contenuti multimediali, del modo in cui viene calcolata e una o più informazioni per comprenderne il significato e l’impatto.

| Metrica | Definizione | Insight |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL ID supporto]** | Il nome associato a un’immagine, un video, un testo o un altro contenuto creativo. | Ordina la tabella facendo clic sull’intestazione di colonna per una qualsiasi delle metriche chiave. |
| **[!UICONTROL Impression]** | Un conteggio di ogni volta che il contenuto multimediale viene caricato nel canale, indipendentemente dall’interazione o dalla visualizzazione. | Un conteggio elevato delle impression può indicare un’ampia visibilità, ma per insight con prestazioni reali, consideralo in relazione ad altre metriche di coinvolgimento. |
| **[!UICONTROL Clic]** | Il numero di volte in cui gli utenti interagiscono con un elemento cliccabile, come un collegamento, sul supporto. | Un numero elevato di clic indica un forte interesse e coinvolgimento per il contenuto, che può essere efficace e raggiungere il pubblico giusto. |
| **[!UICONTROL CTR &#x200B;]**<br>_Percentuale di click-through_ | Percentuale (%) di impression che hanno generato clic sui contenuti multimediali all&#39;interno di un annuncio.<br>**Calcolo**: `clicks` diviso per `impressions` | Un elevato tasso di click-through indica che i contenuti multimediali sono altamente pertinenti e coinvolgenti per il pubblico. Suggerisce che i messaggi e la progettazione catturino efficacemente l’interesse del pubblico e gli spingano ad agire. Inoltre, un CTR elevato può implicare che i media siano ben mirati e risuonino con il pubblico previsto, portando a migliori prestazioni complessive della campagna. |
| **[!UICONTROL CPM &#x200B;]**<br>_Costo per mille_ | Il costo medio per ogni mille impression multimediali.<br>**Calcolo**: importo totale `spent` diviso per il numero di impression, quindi moltiplicato per 1000 | Un valore CPM basso può indicare prestazioni multimediali convenienti, soprattutto se associato a un tasso di click-through elevato. |
| **[!UICONTROL CPA &#x200B;]**<br>_Costo per azione_ | Costo medio speso per ottenere un&#39;azione specifica del cliente, ad esempio un acquisto o un abbonamento.<br>**Calcolo**: importo totale `spent` diviso per il numero di azioni del cliente completate | Consente di identificare i contenuti multimediali che si traducono in azioni utili per i clienti. |
| **[!UICONTROL CPC &#x200B;]**<br>_Costo per clic_ | Costo medio associato a ogni clic sul supporto.<br>**Calcolo**: importo totale `spent` diviso per `clicks` | Costi medi più bassi possono indicare una spesa pubblicitaria efficiente in termini di costi, soprattutto se confrontata con un aumento delle conversioni. |
| **[!UICONTROL Spesa]** | L&#39;importo speso dal bilancio in relazione ai singoli media in un determinato periodo di tempo. | Un importo di spesa elevato in un breve periodo può indicare un utilizzo rapido, che potrebbe portare a un precoce esaurimento delle risorse. Monitora l’importo speso rispetto alle metriche delle prestazioni chiave per monitorare il ritorno complessivo sull’investimento. |
| **[!UICONTROL Utilizzato in questi annunci]** | Il numero di annunci che utilizzano questo supporto. | |
| **Attributi** | Elenco delle funzioni intrinseche presenti in questo supporto. | Gli attributi aiutano a identificare gli elementi creativi che risuonano di più con il tuo pubblico. |
