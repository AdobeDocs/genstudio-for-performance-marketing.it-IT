---
title: Guida di riferimento per gli strumenti dell’Assistente IA
description: Scopri gli strumenti Insights, Create, Plan, Activate e feedback che un assistente AI può utilizzare con [!DNL GenStudio for Performance Marketing].
role: User
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 244293cf4f83acbc252f1d5f3495db403ed4a9bb
workflow-type: tm+mt
source-wordcount: '2265'
ht-degree: 13%
---

# Riferimento per gli strumenti dell’assistente AI

Questo riferimento descrive gli strumenti che un assistente di IA connesso può utilizzare con [!DNL GenStudio for Performance Marketing]. L’elenco degli strumenti disponibili dipende dalla configurazione dell’organizzazione.

Chiedi all’assistente AI quali strumenti può accedere prima di avviare un flusso di lavoro.

## Aree di capacità

| Area | Scopo | Comportamento |
|---|---|---|
| Approfondimenti | Esegui query sulle prestazioni di e-mail e contenuti multimediali a pagamento e recupera i consigli creativi. | Sola lettura. |
| Crea | Trova le risorse, assembla le bozze dai modelli Express o dai consigli di Insights, quindi gestisci la revisione. | Leggi e scrivi. Crea documenti in Creative Cloud. |
| Piano | Estrarre i dettagli della campagna da una breve descrizione e salvarli in Workfront Planning. | Estrazione in sola lettura. Il salvataggio crea record in Workfront Planning e non può essere ripristinato automaticamente. |
| Attiva | Risolvi una destinazione di pubblicazione e invia un’esperienza approvata alla piattaforma. | Scrivi. Gli annunci vengono inviati alla piattaforma e pubblicati in stato off. Le accendi separatamente. Non reversibile tramite questi strumenti. |
| Feedback | Invia feedback sul prodotto al team [!DNL GenStudio for Performance Marketing]. | Scrivi. |

La maggior parte degli strumenti Approfondimenti riguarda `meta`, `linkedin` e `innovid`. Gli strumenti del valore della metrica coprono `meta` e `linkedin`. Il reporting delle campagne e-mail riguarda Adobe Journey Optimizer (`ajo`) e Adobe Campaign (`acc`).

La creazione supporta `meta`, `linkedin`, `display`, `tiktok` e `youtube`. Activate supporta `META`, `LINKEDIN` e `GOOGLECM360`.

## Strumenti Approfondimenti

### get_insights_capability

Restituisce i canali di Insights e le operazioni di reporting abilitati per la tua organizzazione. Utilizzare questo strumento quando la disponibilità non è chiara. I canali supportati sono `meta`, `linkedin`, `innovid`, `ajo` e `acc`.

Questo strumento restituisce i metadati della funzionalità, non i valori di campagna, annuncio o metrica. Per trovare le chiavi di metrica personalizzate della tua organizzazione, usa `list_connected_channels_and_metrics`.

### list_connected_channels_and_metrics

Restituisce le connessioni attive Meta, LinkedIn e Google Campaign Manager 360 della tua organizzazione, i canali e le operazioni supportati da Insights e le metriche di conversione personalizzate configurate. Utilizzarlo per trovare le chiavi di metrica prima di chiamare `get_insights_metric_values`.

Questo strumento restituisce chiavi di metrica, etichette e formati, non valori di metrica. Una connessione non garantisce la disponibilità dei dati storici di reporting.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `limit`, `offset` | No | Dimensioni della pagina e offset di paging. Ometti entrambi per restituire il catalogo completo. |

### get_insights_summary

Restituisce le metriche e le tendenze delle prestazioni del titolo per un canale su un intervallo di date selezionato.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `channel` | Sì | `meta`, `linkedin` o `innovid`. |
| `startDate` | No | Data di inizio nel formato `YYYY-MM-DD`. Il valore predefinito è 30 giorni fa. |
| `endDate` | No | Data di fine in formato `YYYY-MM-DD`. Il valore predefinito è oggi. |
| `metrics` | No | Metriche per il grafico: `spend`, `ctr`, `cpc`, `cpm`, `cpa`, `impressions`, `clicks`, `conversions`, `videoPlays`, `engagement`, `likes`, `comments` o `shares`. Il valore predefinito è `spend`, `ctr`, `cpc` e `cpm`. |

### list_insights_campaigns

Restituisce una tabella ordinabile di metriche delle prestazioni della campagna e una riga dei totali.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `channel` | Sì | `meta`, `linkedin` o `innovid`. |
| `startDate`, `endDate` | No | Intervallo di date nel formato `YYYY-MM-DD`. Il valore predefinito è gli ultimi 30 giorni. |
| `search` | No | Filtro nome campagna. |
| `sortBy` | No | Campo di ordinamento: `spend`, `impressions`, `clicks`, `ctr`, `cpc`, `cpm` o `name`. Il valore predefinito è `spend`. I risultati vengono sempre ordinati in ordine decrescente. |
| `limit`, `offset` | No | Dimensioni della pagina e offset di paging. Il valore predefinito è 20. |

### list_insights_email_campaigns

Restituisce una tabella ordinabile di campagne e-mail con metriche di consegna e coinvolgimento per Adobe Journey Optimizer e Adobe Campaign. Per le campagne pubblicitarie, utilizzare `list_insights_campaigns`.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `channel` | Sì | `ajo` o `acc`. |
| `startDate`, `endDate` | No | Intervallo di date nel formato `YYYY-MM-DD`. Il valore predefinito è l’ultimo giorno 30 prima della data di fine. |
| `search` | No | Filtro nome campagna. |
| `sortBy` | No | Campo di ordinamento: `campaignName`, `emailsNumber`, `emailsDelivered`, `totalClicks`, `openRate`, `ctr`, `ctor`, `bounceRate`, `unsubscribeRate` o `spamComplaintRate`. Il valore predefinito è `emailsDelivered`. I risultati vengono sempre ordinati in ordine decrescente. |
| `limit`, `offset` | No | Dimensioni della pagina e offset di paging. |

### list_insights_ads

Restituisce le prestazioni a livello di annuncio. Utilizza la modalità di navigazione predefinita per una tabella ordinabile o una modalità livello per annunci ad alte e basse prestazioni.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `channel` | Sì | `meta`, `linkedin` o `innovid`. |
| `tier` | No | `all`, `high` o `low`. Il valore predefinito è `all`. |
| `mainMetric` | No | Metrica di classificazione per la modalità livello `high` o `low`: `ctr`, `cpc`, `cpm`, `cpa`, `spend`, `impressions` o `clicks`. Ignorato in modalità Sfoglia. |
| `metrics` | No | Metriche aggiuntive da includere nei rapporti per ogni annuncio in modalità livello. |
| `campaigns` | No | Campagne utilizzate per limitare il risultato, fino a 50. Ogni campagna include `channel`, `accountId` e `campaignId`. |
| `search` | No | Filtro nome annuncio. |
| `sortBy` | No | Campo di ordinamento in modalità Sfoglia: `spend`, `impressions`, `clicks`, `ctr`, `cpc`, `cpm` o `name`. Il valore predefinito è `spend`. I risultati vengono sempre ordinati in ordine decrescente. |
| `spendMin`, `spendMax` | No | Limiti di spesa totali per ogni annuncio. Solo modalità livello. |
| `includeUnsupported` | No | Include gli annunci di cui non è possibile eseguire il rendering della creatività. Il valore predefinito è `false`. |
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
| `ads` | Sì | Da uno a 200 annunci per spiegare. Ogni annuncio include `channel`, `accountId`, `campaignId` e `adId` e facoltativamente `adGroupId` e `performanceTier` (`high` o `low`). Utilizzare gli identificatori restituiti da `list_insights_ads` in modalità livello. |
| `mainMetric` | Sì | La metrica utilizzata per classificare gli annunci: `ctr`, `cpc`, `cpm`, `cpa`, `spend`, `impressions` o `clicks`. |
| `campaigns` | No | Campagne utilizzate per definire la popolazione di confronto, fino a 50. Ogni campagna include `channel`, `accountId` e `campaignId`. |
| `spendMin`, `spendMax` | No | Limiti di spesa per la popolazione di confronto. |
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
| `tagSource` | No | `ad_tags` o `campaign_tags`. Il valore predefinito è `ad_tags`. |
| `sortBy` | No | Campo di ordinamento: `adsCount`, `spend`, `impressions`, `clicks`, `conversionCount`, `ctr`, `cpc`, `cpm` o `cpa`. Il valore predefinito è `adsCount`. |
| `search` | No | Filtro valore tag. |
| `startDate`, `endDate` | No | Intervallo di date nel formato `YYYY-MM-DD`. |
| `limit`, `offset` | No | Dimensioni della pagina e offset di paging. |

### get_insights_metric_values

Restituisce i valori e le tendenze per le metriche tracciate della tua organizzazione, ad esempio potenziali clienti, abbonamenti o ritorno sulla spesa pubblicitaria, per Meta e LinkedIn.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `channels` | No | `meta`, `linkedin` o entrambi. |
| `metrics` | No | Fino a 20 chiavi di metrica restituite da `list_connected_channels_and_metrics`. Il valore predefinito è il set visibile predefinito dell’organizzazione. |
| `campaigns` | No | Campagne utilizzate per limitare il risultato, fino a 50. Ogni campagna include `channel`, `accountId` e `campaignId`. |
| `startDate`, `endDate` | No | Intervallo di date nel formato `YYYY-MM-DD`. Il valore predefinito è gli ultimi 30 giorni. |

### get_insights_recommendations

Restituisce le modifiche creative proposte basate sui dati delle prestazioni dell’organizzazione. Una richiesta non può restituire consigli quando l’ambito selezionato non contiene annunci idonei.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `channels` | Sì | Uno o più di `meta`, `linkedin` o `innovid`. |
| `campaigns` | No | Campagne utilizzate per limitare il risultato, fino a 50. Ogni campagna include `channel`, `accountId` e `campaignId`. |
| `search` | No | Filtro nome campagna. |
| `recommendationId` | No | `adUid` di un consiglio, utilizzato per recuperarlo in dettaglio. |
| `onlyWithPreview` | No | Esclude i consigli privi di anteprima creativa di esempio. Il valore predefinito è `true`. |
| `limit`, `offset` | No | Dimensioni della pagina e offset di paging. |

## Creare gli strumenti

Gli strumenti di creazione consentono di trovare le risorse, assemblare le bozze dai modelli Adobe Express e gestire la revisione prima che un’esperienza sia pronta per essere attivata.

### list_express_templates

Elenca i modelli Express disponibili con filtri e conteggi dei facet.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `channel` | No | `meta`, `display`, `linkedin`, `tiktok`, `youtube` o `__unspecified__`. |
| `query` | No | Termine di ricerca per modelli. |
| `activatableMimeType`, `aspectRatios`, `externalTemplateSource`, `isHTML5Template`, `keywords`, `languages`, `mediaFormat`, `regions`, `timeframes` | No | Filtri facet modello. |
| `sortBy` | No | `modified` o `created`. Il valore predefinito è `modified`. |
| `order` | No | `asc` o `desc`. Il valore predefinito è `desc`. |
| `limit`, `offset` | No | Dimensioni della pagina e offset di paging. |

### description_express_template

Restituisce i campi di testo modificabili e i posizionamenti di immagini in un modello.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `templateId` | Sì | Identificatore del modello espresso. |

### list_cta_options

Restituisce i valori call-to-action consentiti per un canale. La visualizzazione restituisce un elenco vuoto perché accetta testo in formato libero.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `channel` | Sì | `linkedin`, `meta`, `display`, `tiktok` o `youtube`. |
| `limit`, `offset` | No | Dimensioni della pagina e offset di paging. Ometti entrambi per restituire ogni opzione. |

### search_assets

Esegue la ricerca nelle immagini e nei video del contenuto GenStudio. Utilizzatela per selezionare le risorse esistenti per una bozza. Sono escluse le risorse derivate, esterne e scadute. Questo strumento non carica, modifica, elimina o genera risorse e richiede l’adesione a GenStudio Content.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `query` | No | Ricerca per parola chiave o in linguaggio naturale nei metadati di una risorsa. |
| `mediaTypes` | No | `image`, `video` o entrambi. Il valore predefinito include entrambi. |
| `aspectRatios` | No | Proporzioni quali `1:1` o `16:9`. Se un rapporto non è disponibile, lo strumento restituisce le scelte disponibili. |
| `brands`, `campaigns`, `products`, `personas`, `channels` | No | Filtri per nome. |
| `customMetadata` | No | Fino a 5 campi di metadati, ciascuno con uno o più valori. |
| `uploadedBy` | No | `me` o un indirizzo e-mail del caricatore. |
| `createdAtFrom`, `createdAtTo` | No | Limiti di tempo per la creazione in formato ISO 8601. |
| `aiGenerated` | No | Filtra per stato di generazione IA. |
| `contentCredentials` | No | Filtra per stato Content Credentials. |
| `limit`, `offset` | No | Dimensioni della pagina e offset di paging. |

Il risultato include riferimenti di risorse stabili per `create_draft` e URL firmati di breve durata.

### create_draft

Crea una bozza modificabile da un modello Express con una o più esperienze. Ogni chiamata crea una nuova bozza.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `templateId` | Sì | Identificatore del modello espresso. |
| `prompt` | Sì | Istruzioni di copia e descrizione di Creative memorizzate con la bozza. |
| `experiences` | Sì | Una o più esperienze. Vedi la tabella seguente. |
| `name` | No | Nome documento. |
| `allowAssetReuse` | No | Consente di riutilizzare una risorsa selezionata in più esperienze. Il valore predefinito è `false`. |

Ogni esperienza supporta i seguenti campi:

| Campo | Obbligatorio | Descrizione |
|---|---|---|
| `channel` | Sì | `linkedin`, `meta`, `display`, `tiktok` o `youtube`. |
| `title` | No | Titolo esperienza. Il valore predefinito è &quot;Concetto *n*&quot;. |
| `headline` | Meta e LinkedIn | Titolo principale. |
| `body` | Meta, LinkedIn e TikTok | Corpo del testo. Per LinkedIn, questo è il testo introduttivo. Per TikTok, questo è il testo principale. |
| `description` | YouTube | Descrizione annuncio. Facoltativo per Meta e LinkedIn. |
| `display_url` | Meta e LinkedIn | Visualizza l’URL visualizzato nell’annuncio. |
| `destination_url` | No | URL a cui l’annuncio si collega. |
| `cta` | No | Testo call-to-action da `list_cta_options`. |
| `templateFields` | No | Sostituzioni per gli elementi modello denominati da `describe_express_template`. Ogni sostituzione imposta il testo, un URL immagine con dimensioni o un URL video. |
| `assetTemplateFields` | No | Risorse di contenuto da `search_assets` per i campi immagine o video nel modello. |

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
| `emails` | Sì | Da uno a 20 indirizzi e-mail dei collaboratori. |
| `role` | Sì | `editor` o `viewer`. |
| `message` | No | Messaggio di invito. |

### request_draft_approval

Invia una bozza a una o più persone per l&#39;approvazione.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `draftId` | Sì | Identificatore risorsa bozza. |
| `emails` | Sì | Da uno a 20 indirizzi e-mail del revisore. |

### list_experience

Restituisce esperienze approvate e pubblicate, pronte per essere attivate. Le bozze non sono incluse.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `channel` | No | `email`, `meta`, `meta_organic`, `display`, `ctv`, `linkedin`, `linkedin_organic`, `tiktok`, `chatgpt` o `youtube`. |
| `createdByMe` | No | Limita i risultati alle esperienze create dall’utente corrente. |
| `campaignNames` | No | Fino a 5 filtri con il nome esatto della campagna. |
| `creatorEmail` | No | Crea filtro e-mail. |
| `createdAtFrom`, `createdAtTo` | No | Limiti di data di creazione. |
| `language` | No | BCP 47. |
| `limit`, `cursor` | No | Dimensioni della pagina (1-50, valore predefinito 20) e cursore di impaginazione. |

## Strumenti di pianificazione

Gli strumenti di pianificazione trasformano una bozza della campagna in una bozza revisionabile e la salvano in Workfront Planning.

### extract_campaign_from_brief

Estrae una bozza di campagna revisionabile da un documento di marketing incollato. Questo strumento non salva alcun record. Fatti e date mancanti non sono dedotti.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `briefText` | Sì | Testo normale completo di una descrizione della campagna, fino a 100.000 caratteri. File e collegamenti non supportati. |

Il risultato include una bozza della campagna, i risultati con virgolette di supporto, tipi di pubblico suggeriti e avvisi.

### create_workfront_campaign

Crea una campagna di Workfront Planning con prodotti e utenti tipo collegati da una bozza rivista e approvata dall&#39;utente. Questo strumento non è idempotente e non è possibile eseguire il rollback automatico dei record. Controllare Workfront prima di riprovare una scrittura che potrebbe essere riuscita.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `campaignDraft` | Sì | Il progetto approvato. Richiede `name`. I campi facoltativi sono `description`, `objective`, `keyMessaging`, `startDate`, `endDate` (`YYYY-MM-DD`), `status`, `channels`, `products` e `personas`. |
| `channelSelections` | No | Scelte approvate per nomi di canale ambigui. |
| `entitySelections` | No | Record persona e prodotto esistenti approvati. Utilizza `null` per richiedere un nuovo record. |
| `createMissingEntities` | No | Crea i prodotti e gli utenti tipo selezionati come nuovi. Il valore predefinito è `false`. |

Se un prodotto, un utente tipo o un canale è ambiguo, lo strumento restituisce le scelte da confermare e non apporta modifiche.

## Attiva strumenti

Attivare gli strumenti per risolvere una destinazione di media a pagamento e inviare un’esperienza approvata alla piattaforma. Gli annunci vengono pubblicati in stato disattivato (Meta in pausa, LinkedIn draft, Campaign Manager 360 inattivo), pertanto devi attivarli separatamente prima della consegna. L’invio di annunci alla piattaforma non è reversibile tramite questi strumenti.

### configure_activation_target

Risolve e convalida l’account multimediale a pagamento, la campagna, il set di annunci e la pagina Facebook quando necessario.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `platform` | Sì | `META`, `LINKEDIN` o `GOOGLECM360`. |
| `platformAccountId` | No | Identificatore account multimediale a pagamento. Ometti per scoprire gli account. |
| `campaignId` | No | Identificatore della campagna per Meta o LinkedIn. Non utilizzato per Campaign Manager 360. |
| `adsetId` | No | Set di annunci Meta o identificatore della campagna LinkedIn. Non utilizzato per Campaign Manager 360. |
| `pageId` | No | Identificatore della pagina Facebook per Meta. |

Per Campaign Manager 360, è necessario solo l’account dell’annuncio.

### create_activation

Invia un’esperienza approvata alla piattaforma come annunci, utilizzando un target convalidato. Gli annunci vengono pubblicati in stato off. Meta crea un annuncio con la prima immagine per ogni proporzioni. LinkedIn e Campaign Manager 360 creano un annuncio per ogni immagine risolta.

| Parametro | Obbligatorio | Descrizione |
|---|---|---|
| `platform` | Sì | `META`, `LINKEDIN` o `GOOGLECM360`. |
| `targetId` | Sì | Target convalidato restituito da `configure_activation_target`. |
| `experienceId` | Sì | Identificatore esperienza approvato restituito da `list_experiences`. |
| `name` | No | Nome visualizzato del posizionamento dell’annuncio. L&#39;impostazione predefinita è il titolo dell&#39;annuncio dell&#39;esperienza. |

Il risultato elenca il numero di annunci creati, messi in coda e saltati, con lo stato iniziale di ogni annuncio e un collegamento in [!DNL GenStudio for Performance Marketing]. Lo stato `PENDING` indica che il processo è in coda, non che l&#39;annuncio è in consegna.

Chiamando `create_activation` due volte si creano annunci aggiuntivi invece di aggiornare i primi annunci.

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
- **Rivedi le metriche tracciate:** Chiama `list_connected_channels_and_metrics`, quindi chiama `get_insights_metric_values` con le chiavi di metrica restituite.
- **Trasforma un consiglio in bozza:** Chiama `get_insights_recommendations`, quindi chiama `create_draft_from_recommendation`.
- **Genera da un modello:** Chiama `list_express_templates`, `describe_express_template` e `list_cta_options`, quindi chiama `create_draft`.
- **Genera da risorse esistenti:** Chiama `search_assets`, quindi passa i riferimenti della risorsa restituiti a `create_draft` in `assetTemplateFields`.
- **Salva una descrizione della campagna in Workfront:** Chiama `extract_campaign_from_brief`, controlla la bozza, quindi chiama `create_workfront_campaign`.
- **Invia un&#39;esperienza approvata a una piattaforma:** Chiama `list_experiences`, quindi chiama `configure_activation_target` e `create_activation`.

## Funzionalità correlate

- [Panoramica sugli assistenti AI](overview.md)
- [Connettere un assistente AI](connect-ai-assistants.md)
- [Utilizzare gli assistenti AI](use-ai-assistants.md)
