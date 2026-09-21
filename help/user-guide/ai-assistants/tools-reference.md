---
title: Guida di riferimento per gli strumenti dell’Assistente IA
description: Scopri gli strumenti Insights, Create, Activate e feedback che un assistente AI può utilizzare con [!DNL GenStudio for Performance Marketing].
role: User
source-git-commit: 6fb7ddb7549ea6bcd66b6139fbde9ebe12ddaa22
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 15%
---

# Riferimento per gli strumenti dell’assistente AI

Questo riferimento descrive gli strumenti che un assistente di IA connesso può utilizzare con [!DNL GenStudio for Performance Marketing]. L’elenco degli strumenti disponibili dipende dalla configurazione dell’organizzazione.

Chiedi all’assistente AI quali strumenti può accedere prima di avviare un flusso di lavoro.

## Aree di capacità

| Area | Scopo | Comportamento |
|---|---|---|
| Approfondimenti | Esegui query sulle prestazioni dei contenuti multimediali a pagamento e recupera i consigli creativi. | Sola lettura. |
| Crea | Assembla le bozze dai modelli Express o dai consigli di Insights, quindi gestisci la revisione. | Leggi e scrivi. Crea documenti in Creative Cloud. |
| Attiva | Risolvi un target di pubblicazione e pubblica un’esperienza approvata. | Scrivi e distruggi. Può pubblicare un annuncio live e sostenere spese pubblicitarie. |
| Feedback | Invia feedback sul prodotto al team [!DNL GenStudio for Performance Marketing]. | Scrivi. |

La maggior parte degli strumenti Approfondimenti riguarda `meta`, `linkedin` e `innovid`. Gli strumenti per la metrica di conversione coprono `meta` e `linkedin`.

La creazione supporta `meta`, `linkedin`, `display`, `tiktok` e `youtube`. Activate supporta `META`, `LINKEDIN` e `GOOGLECM360`.

## Strumenti Approfondimenti

### get_insights_capability

Restituisce i canali, le operazioni e le metriche di conversione personalizzate di Insights abilitati per la tua organizzazione. Utilizzare questo strumento quando la disponibilità non è chiara.

Questo strumento restituisce i metadati della funzionalità, non i valori di campagna, annuncio o metrica.

### get_insights_summary

Restituisce le metriche e le tendenze delle prestazioni del titolo per un canale su un intervallo di date selezionato.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `channel` | Sì | `meta`, `linkedin` o `innovid`. |
| `startDate` | No | Data di inizio nel formato `YYYY-MM-DD`. Il valore predefinito è 30 giorni fa. |
| `endDate` | No | Data di fine in formato `YYYY-MM-DD`. Il valore predefinito è oggi. |
| `metrics` | No | Metriche per il grafico, ad esempio `spend`, `ctr`, `cpc`, `cpm`, `impressions`, `clicks` o `conversions`. |

### list_insights_campaigns

Restituisce una tabella ordinabile di metriche delle prestazioni della campagna e una riga dei totali.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `channel` | Sì | `meta`, `linkedin` o `innovid`. |
| `startDate`, `endDate` | No | Intervallo di date nel formato `YYYY-MM-DD`. Il valore predefinito è gli ultimi 30 giorni. |
| `search` | No | Filtro nome campagna. |
| `sortBy` | No | Campo di ordinamento, ad esempio `spend`, `impressions`, `clicks`, `ctr`, `cpc`, `cpm` o `name`. |
| `limit`, `offset` | No | Dimensioni della pagina e offset di paging. |

### list_insights_ads

Restituisce le prestazioni a livello di annuncio. Utilizza la modalità di navigazione predefinita per una tabella ordinabile o una modalità livello per annunci ad alte e basse prestazioni.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `channel` | Sì | `meta`, `linkedin` o `innovid`. |
| `tier` | No | `all`, `high` o `low`. Il valore predefinito è `all`. |
| `mainMetric` | Condizionale | Metrica di classificazione richiesta per la modalità livello `high` o `low`. |
| `campaigns` | No | Identificatori di campagna utilizzati per limitare il risultato. |
| `search` | No | Filtro nome annuncio. |
| `startDate`, `endDate` | No | Intervallo di date nel formato `YYYY-MM-DD`. |
| `limit`, `offset` | No | Dimensioni della pagina e offset di paging. |

La modalità livello restituisce gli identificatori pubblicitari necessari per `get_insights_ad_attributes`.

### get_insights_ad_details

Restituisce metadati creativi per un annuncio, inclusi copia, call to action, risorse e posizionamenti. Non restituisce le metriche delle prestazioni.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `channel` | Sì | `meta`, `linkedin` o `innovid`. |
| `accountId` | Sì | Identificatore account multimediale a pagamento. |
| `campaignId` | Sì | Identificatore della campagna. |
| `adId` | Sì | Identificatore annuncio. |
| `adgroupId` | No | Identificatore del gruppo di annunci quando il canale utilizza gruppi di annunci. |

### get_insights_ad_attributes

Confronta le caratteristiche creative per gli annunci selezionati con la media dei canali. Utilizzala dopo che `list_insights_ads` identifica gli annunci con prestazioni elevate o basse.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `ads` | Sì | Annunci da spiegare, inclusi gli identificatori restituiti da `list_insights_ads`. |
| `mainMetric` | Sì | La metrica utilizzata per classificare gli annunci. |
| `campaigns` | No | Identificatori di campagna utilizzati per definire la popolazione di confronto. |
| `startDate`, `endDate` | No | Intervallo di date nel formato `YYYY-MM-DD`. |

### get_insights_tag_Categories

Restituisce le categorie di tag disponibili per l’organizzazione durante il periodo richiesto. Restituisce i nomi delle categorie, non le metriche delle prestazioni.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `channels` | Sì | Uno o più canali supportati. |
| `startDate`, `endDate` | No | Intervallo di date nel formato `YYYY-MM-DD`. |

### get_insights_ad_tags

Restituisce le prestazioni in base al valore di tag all’interno di una categoria, ad esempio prodotto, area geografica o tema creativo.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `channel` | Sì | `meta`, `linkedin` o `innovid`. |
| `tagCategory` | Sì | Categoria restituita da `get_insights_tag_categories`. |
| `tagSource` | No | `ad_tags` o `campaign_tags`. |
| `sortBy` | No | Metrica utilizzata per ordinare il risultato. |
| `search` | No | Filtro valore tag. |
| `startDate`, `endDate` | No | Intervallo di date nel formato `YYYY-MM-DD`. |

### get_insights_custom_metrics

Restituisce le metriche di conversione personalizzate configurate per la tua organizzazione. Utilizzarlo prima di `get_insights_conversion_metrics`.

Questo strumento restituisce identificatori di metrica, non valori di metrica.

### get_insights_conversion_metrics

Restituisce i valori e le tendenze della metrica di conversione configurata per Meta e LinkedIn.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `channels` | No | Canale di conversione supportato. Il valore predefinito è `meta`. |
| `metrics` | No | Identificatori di metrica restituiti da `get_insights_custom_metrics`. |
| `campaigns` | No | Identificatori di campagna utilizzati per limitare il risultato. |
| `startDate`, `endDate` | No | Intervallo di date nel formato `YYYY-MM-DD`. |

### get_insights_recommendations

Restituisce le modifiche creative proposte basate sui dati delle prestazioni dell’organizzazione. Una richiesta non può restituire consigli quando l’ambito selezionato non contiene annunci idonei.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `channels` | Sì | Uno o più canali supportati. |
| `campaigns` | No | Identificatori di campagna utilizzati per limitare il risultato. |
| `search` | No | Filtro nome campagna. |
| `recommendationId` | No | Identificatore utilizzato per recuperare in dettaglio un consiglio. |
| `limit`, `offset` | No | Dimensioni della pagina e offset di paging. |

## Creare gli strumenti

Crea strumenti per assemblare le bozze dai modelli Adobe Express e gestire la revisione prima che un’esperienza sia pronta per essere attivata.

### list_express_templates

Elenca i modelli Express disponibili con filtri e conteggi dei facet.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `channel` | No | `meta`, `display`, `linkedin`, `tiktok`, `youtube` o `__unspecified__`. |
| `query` | No | Termine di ricerca per modelli. |
| `aspectRatios`, `keywords`, `languages`, `mediaFormat`, `regions`, `timeframes` | No | Filtri facet modello. |
| `sortBy`, `order` | No | Ordinare campo e ordine. |
| `limit`, `offset` | No | Dimensioni della pagina e offset di paging. |

### description_express_template

Restituisce i campi di testo modificabili e i posizionamenti di immagini in un modello.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `templateId` | Sì | Identificatore del modello espresso. |

### list_cta_options

Restituisce i valori call-to-action consentiti per un canale.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `channel` | Sì | `linkedin`, `meta`, `display`, `tiktok` o `youtube`. |

### create_draft

Crea una bozza modificabile da un modello Express con una o più esperienze.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `templateId` | Sì | Identificatore del modello espresso. |
| `prompt` | Sì | Istruzioni di copia e descrizione di Creative memorizzate con la bozza. |
| `experiences` | Sì | Canale, campi di contenuto e sostituzioni facoltative dei campi di modello per ogni esperienza. |
| `name` | No | Nome documento. |

Utilizzare `list_cta_options` prima di creare una bozza per un canale con valori call-to-action fissi.

### create_draft_from_recommendations

Crea una bozza modificabile da un consiglio Approfondimenti specifico.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `channel` | Sì | `meta` o `linkedin`. |
| `adUid` | Sì | Identificatore di consigli restituito da `get_insights_recommendations`. |
| `prompt` | Sì | Descrizione di Creative basata sul consiglio. |
| `name` | No | Nome documento. |

### list_Recent_draft

Elenca le recenti bozze di modelli Express con il relativo stato e i collegamenti.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `limit`, `offset` | No | Dimensioni della pagina e offset di paging. |

### get_draft_metadata

Restituisce il nome, i canali, lo stato di approvazione, i risultati del revisore e l’accesso del collaboratore di una bozza.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `draftId` | Sì | Identificatore risorsa bozza. |

### share_draft

Consente ai collaboratori di visualizzare o modificare l’accesso a una bozza senza richiedere l’approvazione.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `draftId` | Sì | Identificatore risorsa bozza. |
| `emails` | Sì | Uno o più indirizzi e-mail per collaboratori. |
| `role` | Sì | `editor` o `viewer`. |
| `message` | No | Messaggio di invito. |

### request_draft_approval

Invia una bozza a una o più persone per l&#39;approvazione.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `draftId` | Sì | Identificatore risorsa bozza. |
| `emails` | Sì | Uno o più indirizzi e-mail del revisore. |

### list_experience

Restituisce esperienze approvate e pubblicate, pronte per essere attivate. Le bozze non sono incluse.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `channel` | No | Filtro del canale esperienza. |
| `createdByMe` | No | Limita i risultati alle esperienze create dall’utente corrente. |
| `campaignNames` | No | Filtri esatti per il nome della campagna. |
| `creatorEmail` | No | Crea filtro e-mail. |
| `createdAtFrom`, `createdAtTo` | No | Limiti di data di creazione. |
| `language` | No | BCP 47. |
| `limit`, `cursor` | No | Dimensioni della pagina e cursore di impaginazione. |

## Attiva strumenti

Attiva gli strumenti per risolvere un target di media a pagamento e pubblicare un’esperienza approvata. La pubblicazione non è reversibile tramite questi strumenti e potrebbe comportare spese pubblicitarie.

### configure_activation_target

Risolve e convalida l’account multimediale a pagamento, la campagna, il set di annunci e la pagina Facebook quando necessario.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `platform` | Sì | `META`, `LINKEDIN` o `GOOGLECM360`. |
| `platformAccountId` | No | Identificatore account multimediale a pagamento. Ometti per scoprire gli account. |
| `campaignId` | No | Identificatore della campagna per Meta o LinkedIn. |
| `adsetId` | No | Set di annunci Meta o identificatore della campagna LinkedIn. |
| `pageId` | No | Identificatore della pagina Facebook per Meta. |

### create_activation

Pubblica un annuncio live di una singola immagine da un’esperienza approvata e da una destinazione convalidata.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `platform` | Sì | `META`, `LINKEDIN` o `GOOGLECM360`. |
| `targetId` | Sì | Target convalidato restituito da `configure_activation_target`. |
| `experienceId` | Sì | Identificatore esperienza approvato restituito da `list_experiences`. |
| `assetId` | No | Identificatore di variante per un’esperienza con più varianti idonee. |
| `name` | No | Nome visualizzato del posizionamento dell’annuncio. |

Se si chiama `create_activation` due volte, vengono creati due annunci separati invece di aggiornare il primo annuncio.

## Strumento Feedback

### submit_mcp_feedback

Invia al team [!DNL GenStudio for Performance Marketing] il feedback su uno strumento o un flusso di lavoro.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `category` | Sì | `bug`, `feature_request` o `workflow_friction`. |
| `comment` | Sì | Una descrizione concisa del feedback. |
| `tags` | No | Tag utilizzati per categorizzare il feedback. |
| `tool_name` | No | Lo strumento associato al feedback. |

## Flussi di lavoro comuni

Utilizzare queste sequenze quando uno strumento fornisce identificatori o configurazioni per un altro strumento:

- **Diagnosticare un annuncio:** Chiamare `list_insights_ads` in modalità livello `high` o `low`, quindi chiamare `get_insights_ad_attributes` con la stessa metrica di classificazione.
- **Analizza per tag:** Chiama `get_insights_tag_categories`, quindi chiama `get_insights_ad_tags` con una categoria restituita.
- **Rivedi le metriche di conversione:** Chiama `get_insights_custom_metrics`, quindi chiama `get_insights_conversion_metrics` con gli identificatori di metrica restituiti.
- **Trasforma un consiglio in bozza:** Chiama `get_insights_recommendations`, quindi chiama `create_draft_from_recommendation`.
- **Genera da un modello:** Chiama `list_express_templates`, `describe_express_template` e `list_cta_options`, quindi chiama `create_draft`.
- **Pubblica un&#39;esperienza approvata:** Chiama `list_experiences`, quindi chiama `configure_activation_target` e `create_activation`.

## Funzionalità correlate

- [Panoramica sugli assistenti AI](overview.md)
- [Connettere un assistente AI](connect-ai-assistants.md)
- [Utilizzare gli assistenti AI](use-ai-assistants.md)
