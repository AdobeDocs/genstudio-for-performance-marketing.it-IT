---
title: Ruoli utente e autorizzazioni di Adobe GenStudio for Performance Marketing
description: Scopri i ruoli utente e le autorizzazioni di GenStudio for Performance Marketing.
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
source-git-commit: 3e9a2a4f42ba79389691705c571bf6bbd0b990c5
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 2%

---

# Ruoli utente e autorizzazioni

La creazione e l’implementazione di campagne di marketing moderne richiede la collaborazione tra le parti interessate con responsabilità e competenze diverse. _I ruoli utente_ controllano l&#39;accesso delle parti interessate alle numerose funzionalità di GenStudio for Performance Marketing. Il ruolo utente assegnato determina le attività che è possibile eseguire utilizzando questa piattaforma. Un amministratore di Adobe assegna un ruolo nel profilo di prodotto GenStudio in Adobe Admin Console. L&#39;e-mail di benvenuto identifica il ruolo assegnato.

>[!NOTE]
>
>Prima di assegnare questi ruoli a qualsiasi utente, è necessario designare un amministratore di Adobe in Adobe Admin Console per eseguire attività di configurazione una tantum. Questo Adobe di ruolo di amministratore funziona solo nel contesto di Adobe Admin Console. Non ha alcun ruolo nell’interfaccia della piattaforma GenStudio for Performance Marketing. Un amministratore di Adobe che necessita di diritti di gestore di sistema deve effettuare il provisioning come responsabile di sistema GenStudio in Adobe Admin Console. Vedere [Provisioning di GenStudio for Performance Marketing](product-provisioning.md).

## Diritti

_Diritti_ concedere l&#39;autorizzazione per eseguire attività specifiche e accedere a risorse protette. I diritti sono definiti nel ruolo utente all’interno del profilo di prodotto e gli utenti ricevono tali diritti quando vengono assegnati a tale ruolo.

## Ruoli utente

Tre tipi di ruoli utente di GenStudio for Performance Marketing supportano questa diversità di ruoli organizzativi. Le autorizzazioni sono personalizzate per ciascuno di questi tipi di utenti e supportano le responsabilità di ogni utente nell’organizzazione di marketing. I tre tipi di ruolo utente sono:

* **Gli editor di GenStudio** utilizzano le funzionalità di intelligenza artificiale generativa di GenStudio for Performance Marketing per creare risorse di campagne di marketing, richiedere la revisione e l&#39;approvazione del contenuto e pubblicare bozze approvate di questo contenuto. Tutti gli utenti di GenStudio for Performance Marketing possono accedere e utilizzare una risorsa una volta che il relativo editor l&#39;ha salvata in [!DNL Content].

* **I collaboratori GenStudio** sono la gamma più ampia di utenti GenStudio for Performance Marketing. I collaboratori possono visualizzare e approvare i contenuti e sono una parte essenziale del flusso di lavoro per garantire che i contenuti generati corrispondano alle esigenze e agli standard della tua organizzazione.

* I **manager di sistema di GenStudio** dispongono del set più ampio di autorizzazioni in GenStudio for Performance Marketing. I responsabili di sistema eseguono il compito essenziale di onboarding, ovvero stabilire i guardrail fondamentali per la creazione e la distribuzione delle risorse delle campagne. I responsabili di sistema implementano questi guardrail caricando informazioni specifiche per il marchio e l&#39;organizzazione come [linee guida per il marchio](./guidelines/overview.md). I responsabili di sistema dispongono dell&#39;autorizzazione per creare e pubblicare [!DNL Brands], ma non dispongono dei privilegi di amministrazione degli utenti.

### Editor GenStudio

_Gli editor_ o i creatori di contenuti dispongono delle autorizzazioni di base necessarie per creare risorse GenStudio for Performance Marketing [!DNL Brands], [!DNL Campaigns] e [!DNL Content]. Possono anche modificare ed eliminare le risorse create. GenStudio for Performance Marketing supporta la creazione rapida di centinaia di contenuti. Questi utenti possono generare frammenti di contenuto o intere esperienze che orchestrano parti discrete di contenuti approvati per soddisfare le esigenze di specifiche campagne di marketing.

Gli editor interagiscono con le tecnologie di intelligenza artificiale generativa di GenStudio for Performance Marketing tramite _prompt_. Il cassetto dei prompt nell’area di lavoro fornisce gli strumenti per inserire i prompt nel contesto delle linee guida di una campagna specifica. Di conseguenza, la qualità e il successo dei contenuti generati dipendono in parte dalla qualità delle linee guida del brand caricate dalla tua organizzazione e dalla specificità del prompt. Vedere [Scrivi prompt effettivi](effective-prompts.md).

Nella tabella seguente vengono visualizzate le autorizzazioni dell’editor predefinito:

| Funzione obsoleta | Creare | Aggiornare | Elimina | Visualizzazione |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | no | no | no | sì |
| [!DNL Campaigns] | sì | sì | sì | sì |
| [!DNL Content] | sì | sì | sì | sì |
| [!DNL Create] | sì | sì | sì | sì |
| [!DNL Insights] | può configurare solo ad connectors |    |     | sì |
| [!DNL Personas] | sì | sì* | sì* | sì |
| [!DNL Products] | sì | sì* | sì* | sì |
| [!DNL Reviews and approvals] | sì | sì | sì | sì |

Gli editor possono modificare ed eliminare [!DNL Personas] e [!DNL Products] creati.

I manager di sistema di GenStudio possono concedere agli editor l&#39;autorizzazione per modificare ed eliminare [!DNL Brand].

### Collaboratori GenStudio

_I collaboratori_ possono visualizzare le risorse in GenStudio for Performance Marketing ma non crearle, modificarle o eliminarle. I collaboratori includono le parti interessate che sono essenziali per il successo del processo di revisione e approvazione dei contenuti, ma che non devono creare o modificare direttamente i contenuti. Esperti legali e manager dei creativi sono esempi di potenziali collaboratori. I collaboratori GenStudio for Performance Marketing potrebbero essere autorizzati a creare e visualizzare risorse in altri prodotti Creative Cloud.

Nella tabella seguente vengono visualizzate le autorizzazioni di collaborazione predefinite:

| Funzione obsoleta | Creare | Aggiornare | Elimina | Visualizzazione |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | no | no | no | sì |
| [!DNL Campaigns] | no | no | no | sì |
| [!DNL Content] | no | no | no | sì |
| [!DNL Create] | no | no | no | sì |
| [!DNL Insights] | no | no | no | sì |
| [!DNL Personas] | no | no | no | sì |
| [!DNL Products] | no | no | no | sì |
| [!DNL Reviews and approvals] | no | no | no | sì |

### Responsabili di sistema GenStudio

_I manager di sistema di GenStudio_ dispongono del set di autorizzazioni più potente in GenStudio for Performance Marketing. I responsabili di sistema eseguono il compito essenziale di onboarding, ovvero stabilire i guardrail fondamentali per la creazione e la distribuzione delle risorse delle campagne. I responsabili di sistema implementano questi guardrail caricando informazioni specifiche per il marchio e l&#39;organizzazione come [linee guida per il marchio](./guidelines/overview.md). I responsabili di sistema dispongono dell&#39;autorizzazione per creare e pubblicare [!DNL Brands], ma non dispongono dei privilegi di amministrazione degli utenti.

Nella tabella seguente vengono visualizzate le autorizzazioni predefinite di System Manager:

| Funzione obsoleta | Creare | Aggiornare | Elimina | Visualizzazione |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | sì | sì | sì | sì |
| [!DNL Campaigns] | sì | sì | sì | sì |
| [!DNL Content] | sì | sì | sì | sì |
| [!DNL Insights] | sì | sì | sì | sì |
| [!DNL Personas] | sì | sì | sì | sì |
| [!DNL Products] | sì | sì | sì | sì |
| [!DNL Reviews and approvals] | sì | sì | sì | sì |

Consulta [Introduzione ad Adobe GenStudio for Performance Marketing](get-started.md) per una panoramica delle attività di configurazione preliminari.
