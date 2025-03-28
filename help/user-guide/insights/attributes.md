---
title: Panoramica sugli attributi
description: Scopri come valutare le prestazioni di attributi specifici in Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Reporting and Insights, Content Attributes, Content Performance
exl-id: 9d05c128-50d5-415a-ae60-7023c36c06ad
source-git-commit: 4afdde6fd08a9f33ff599f5f85b9c1b9d79870ec
workflow-type: tm+mt
source-wordcount: '840'
ht-degree: 0%

---

# Panoramica sugli attributi

La visualizzazione [!DNL Insights] _[!UICONTROL Attributi]_ mostra un elenco di attributi utilizzati nelle campagne pubblicitarie per l&#39;account canale selezionato.

{{connect-insights}}

La tabella _[!UICONTROL Attributes]_ è organizzata utilizzando il nome [!UICONTROL Attribute]. Puoi passare da un tipo di elenco all&#39;altro utilizzando il pulsante **[!UICONTROL Immagini]** e il pulsante **[!UICONTROL Video]**. Fai clic sull’icona delle impostazioni (cog) sopra il lato destro della tabella per attivare/disattivare le colonne visualizzabili.

L&#39;icona del filtro (funnel) sopra il lato sinistro della tabella apre il menu **[!UICONTROL Filtro]** in cui è possibile selezionare più elenchi. Seleziona **[!UICONTROL Cancella tutto]** sopra la tabella per rimuovere tutti i filtri.

![Filtro attributi e tabella](/help/assets/insights-attributes-filter.png){zoomable="yes"}

{{$include /help/_includes/download-insights.md}}

## Dettagli attributo

Gli attributi consentono di identificare [media](media.md#media-details) in base ai relativi dettagli, ad esempio colore, composizione, elementi visivi e altre proprietà.

Nella vista dei dettagli dell’attributo, puoi vedere quali annunci utilizzano l’attributo selezionato. I dettagli includono le prestazioni totali degli attributi e un raggruppamento delle metriche delle prestazioni relative a ciascun annuncio.

![Metriche delle prestazioni degli attributi](/help/assets/insights-attribute-details.png){zoomable="yes"}

GenStudio for Performance Marketing rileva determinate funzioni e applica l’attributo appropriato al contenuto multimediale o all’annuncio come tag. Consulta [Categorie](#categories) per esempi di questi tag. Per visualizzare tutti gli attributi associati a un annuncio, fai clic sull&#39;icona delle impostazioni (cog) sopra il lato destro della tabella per selezionare la colonna **[!UICONTROL Attributi]**.

## Categorie

Un attributo _categoria_ è un gruppo di classificazione che organizza attributi correlati che condividono una caratteristica comune. Queste categorie aiutano a semplificare l&#39;individuazione, l&#39;identificazione e la comprensione di attributi specifici fornendo un contesto più ampio e facilitandone l&#39;applicazione e l&#39;utilizzo.

GenStudio for Performance Marketing utilizza le funzionalità di intelligenza artificiale e machine learning di Adobe per studiare [immagini](image-features.md), [video](video-features.md) e [testo](text-features.md) e applicare [!UICONTROL attributi multimediali] in base alla probabilità di correttezza.

L’elenco degli attributi rilevati per il contenuto multimediale non è esaustivo. I file multimediali che contengono un set completo di funzioni possono essere limitati alle tre funzioni più dominanti identificate dall’intelligenza artificiale. Ad esempio, la figura seguente contiene diversi attributi dell&#39;immagine rilevati, tra cui più oggetti, colori di primo piano e di sfondo.

![attributi immagine](/help/assets/category/asset-attributes.png "L&#39;immagine di Toucan include più attributi rilevati"){width="300" zoomable="yes"}

>[!INFO]
>
>Non è possibile modificare i tag rilevati e applicati automaticamente.

## Prestazioni degli attributi

Le metriche di Insights possono aiutarti a valutare quali attributi ispirano più coinvolgimento dei clienti.

La tabella seguente fornisce definizioni e informazioni approfondite per le metriche chiave del marketing digitale nella vista tabella [!UICONTROL Attributi]. Ogni metrica include una breve definizione relativa agli attributi, al modo in cui viene calcolata e una o più informazioni per comprenderne il significato e l’impatto su una campagna pubblicitaria.

| Metrica | Definizione | Insight |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Attributo]** | Nome dell’attributo. | Ordina la tabella facendo clic sull’intestazione di colonna per una qualsiasi delle metriche chiave. |
| **[!UICONTROL Categoria]** | La [categoria](#categories) che rappresenta la qualità intrinseca di un attributo. |  |
| **[!UICONTROL # di immagini]** | Numero di immagini con questo attributo. | Il conteggio nella tabella Attributi può essere diverso da quello nella visualizzazione Dettagli attributo. Questa discrepanza può verificarsi se l’origine del canale, ad esempio Meta, e GenStudio utilizzano calcoli di riepilogo leggermente diversi. |
| **[!UICONTROL # di video]** | Il numero di video che hanno questo attributo. | Il conteggio nella tabella Attributi può essere diverso da quello nella visualizzazione Dettagli attributo. Questa discrepanza può verificarsi se l’origine del canale, ad esempio Meta, e GenStudio utilizzano calcoli di riepilogo leggermente diversi. |
| **[!UICONTROL Impression]** | Un conteggio di ogni volta che un’immagine o dei video con questo attributo vengono caricati nel canale, indipendentemente dall’interazione o dalla visualizzazione. | Un conteggio elevato delle impression può indicare un’ampia visibilità, ma per informazioni approfondite sulle prestazioni, consideralo in relazione ad altre metriche di coinvolgimento. |
| **[!UICONTROL Clic]** | Il numero di volte in cui gli utenti interagiscono con un’immagine o un video con questo attributo. | Un numero elevato di clic indica un forte interesse e coinvolgimento per il contenuto, che può essere efficace e raggiungere il pubblico giusto. |
| **[!UICONTROL CTR ]**<br>_Percentuale di click-through_ | Percentuale (%) di impression che hanno generato clic su immagini o video con questo attributo.<br>**Calcolo**: `clicks` diviso per `impressions` | Un elevato tasso di click-through indica che il contenuto è altamente pertinente e motivante per il pubblico nella messaggistica e nella progettazione, e sta mirando in modo efficace agli interessi del pubblico. |
| **[!UICONTROL CPM ]**<br>_Costo per mille_ | Costo per ogni mille impression pubblicitarie di un’immagine o di un video con questo attributo.<br>**Calcolo**: importo totale `spent` diviso per la portata, quindi moltiplicato per 1000 | Un valore basso può indicare una visibilità a costi contenuti, soprattutto se associata a un elevato tasso di click-through. |
| **[!UICONTROL CPA ]**<br>_Costo per azione_ | Costo medio speso per ottenere un’azione specifica del cliente, ad esempio un acquisto o un abbonamento.<br>**Calcolo**: importo totale `spent` diviso per il numero di azioni cliente completate | Consente di identificare gli attributi che determinano azioni utili per il cliente. |
| **[!UICONTROL CPC ]**<br>_Costo per clic_ | Costo medio associato a ogni clic su immagini o video con questo attributo.<br>**Calcolo**: importo totale `spent` diviso per `clicks` | Costi medi più bassi possono indicare una spesa pubblicitaria efficiente in termini di costi, soprattutto se confrontata con un aumento delle conversioni. |
| **[!UICONTROL Spesa]** | L&#39;importo speso dal bilancio in relazione agli attributi in un dato periodo di tempo. | Un importo di spesa elevato in un breve periodo può indicare un utilizzo rapido, che potrebbe portare a un precoce esaurimento delle risorse. Monitora l’importo speso rispetto alle metriche delle prestazioni chiave per monitorare il ritorno complessivo sull’investimento. |
