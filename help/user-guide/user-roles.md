---
title: Ruoli utente e autorizzazioni di Adobe GenStudio for Performance Marketing
description: Scopri i ruoli utente e le autorizzazioni di GenStudio for Performance Marketing.
level: Beginner
feature: Generative AI, Guidelines
role: Admin
exl-id: 33ebcf9c-e5f8-4011-b449-5f73d151f221
source-git-commit: 6ee58b22761be357bb9ff753cf9e5bd5b431c513
workflow-type: tm+mt
source-wordcount: '1133'
ht-degree: 1%

---

# Ruoli utente e autorizzazioni

La creazione e l’implementazione di campagne di marketing moderne richiede la collaborazione tra le parti interessate con responsabilità e competenze diverse. _I ruoli utente_ controllano l&#39;accesso delle parti interessate alle numerose funzionalità di GenStudio for Performance Marketing. Il ruolo utente assegnato determina le attività che è possibile eseguire utilizzando questa piattaforma. Un amministratore di sistema Adobe ti assegna un ruolo nel profilo di prodotto GenStudio in Adobe Admin Console. L&#39;e-mail di benvenuto identifica il ruolo assegnato.

>[!NOTE]
>
>Prima che a qualsiasi utente vengano assegnati questi ruoli, è necessario designare un amministratore di sistema Adobe in Adobe Admin Console per eseguire attività di configurazione una tantum. Questo ruolo di amministratore di Adobe funziona solo nel contesto di Adobe Admin Console. Non ha alcun ruolo nell’interfaccia della piattaforma GenStudio for Performance Marketing. Un amministratore di sistema di Adobe che necessita di diritti di gestore di sistema deve effettuare il provisioning come gestore di sistema di GenStudio in Adobe Admin Console. Vedere [Provisioning di GenStudio for Performance Marketing](product-provisioning.md).

## amministratore di sistema Adobe e manager di sistema GenStudio

Questi titoli dei ruoli utente possono sembrare simili, ma identificano ruoli univoci che forniscono diritti in ambienti diversi.

**Gli amministratori di sistema di Adobe** dispongono di privilegi per gli utenti avanzati in Adobe Admin Console ed eseguono tutte le attività di gestione degli utenti, ad esempio l&#39;aggiunta o l&#39;eliminazione di utenti. Questo ruolo di amministratore di sistema non fornisce privilegi nell’applicazione GenStudio for Performance Marketing, il che spiega perché gli amministratori di sistema di Adobe non richiedono una licenza per GenStudio. In genere, gli amministratori di sistema di Adobe utilizzano Admin Console per aggiungere ed eliminare account utente dalle distribuzioni di GenStudio e assegnare o rimuovere diritti, o autorizzazioni, da singoli utenti o gruppi di utenti.

**I manager di sistema di GenStudio** sono utenti avanzati in GenStudio for Performance Marketing, ma non dispongono dell&#39;autorizzazione per eseguire attività in Adobe Admin Console. Questo ruolo di manager di sistema richiede una licenza del prodotto GenStudio e corrisponde a un utente avanzato nella [descrizione del prodotto Adobe GenStudio for Performance Marketing](https://helpx.adobe.com/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html). I responsabili di sistema di GenStudio hanno diritto completo alle funzionalità di GenStudio for Performance Marketing, tra cui [!DNL Brands], [!DNL Persona] e [!DNL Product] creazione, eliminazione, aggiornamento e pubblicazione. [Descrizione del prodotto Adobe GenStudio for Performance Marketing](https://helpx.adobe.com/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html) spiega la correlazione tra i ruoli utente di GenStudio e le licenze del prodotto.

Consulta [Ruoli amministrativi](https://helpx.adobe.com/enterprise/using/admin-roles.html#enterprise) nella _Guida all&#39;amministrazione di Enterprise e Teams_.

## Diritti

_Diritti_ concedere l&#39;autorizzazione per eseguire attività specifiche e accedere a risorse protette. I diritti, o autorizzazioni, sono definiti nel ruolo utente all’interno del profilo di prodotto e gli utenti ricevono tali diritti quando vengono assegnati a tale ruolo.

>[!IMPORTANT]
>
>Non aggiungere, modificare o eliminare profili di prodotto esistenti. La modifica dei profili di prodotto predefiniti può interrompere gravemente l’implementazione di GenStudio for Performance Marketing.

## Ruoli utente

Tre tipi di ruoli utente di GenStudio for Performance Marketing supportano questa diversità di ruoli organizzativi. I diritti sono personalizzati per ciascuno di questi tipi di utenti e supportano le responsabilità di ciascun utente nell’organizzazione di marketing. I tre tipi di ruolo utente sono:

* **Gli editor di GenStudio** utilizzano le funzionalità di intelligenza artificiale generativa di GenStudio for Performance Marketing per creare risorse di campagne di marketing, richiedere la revisione e l&#39;approvazione del contenuto e pubblicare bozze approvate di questo contenuto. Tutti gli utenti di GenStudio for Performance Marketing possono accedere e utilizzare una risorsa una volta che il relativo editor l&#39;ha salvata in [!DNL Content]. Gli editor di GenStudio sono utenti avanzati di GenStudio for Performance Marketing.

* **I collaboratori GenStudio** sono la gamma più ampia di utenti GenStudio for Performance Marketing. I collaboratori possono visualizzare e approvare i contenuti e sono una parte essenziale del flusso di lavoro per garantire che i contenuti generati corrispondano alle esigenze e agli standard della tua organizzazione. I collaboratori GenStudio sono _utenti collaboratori_ in GenStudio for Performance Marketing.

* I **manager di sistema di GenStudio** dispongono del set più ampio di autorizzazioni o diritti in GenStudio for Performance Marketing. I responsabili di sistema eseguono il compito essenziale di onboarding, ovvero stabilire i guardrail fondamentali per la creazione e la distribuzione delle risorse delle campagne. I responsabili di sistema implementano questi guardrail caricando informazioni specifiche per il marchio e l&#39;organizzazione come [linee guida per il marchio](./guidelines/overview.md). I responsabili di sistema dispongono dell&#39;autorizzazione per creare e pubblicare [!DNL Brands], ma non dispongono dei privilegi di amministrazione degli utenti. I responsabili di sistema di GenStudio sono utenti esperti di GenStudio for Performance Marketing.

### Editor GenStudio

_Gli editor_ o i creatori di contenuti dispongono delle autorizzazioni di base necessarie per creare risorse GenStudio for Performance Marketing [!DNL Brands], [!DNL Campaigns] e [!DNL Content]. Questi utenti avanzati possono anche modificare ed eliminare le risorse create. GenStudio for Performance Marketing supporta la creazione rapida di centinaia di contenuti. Questi utenti possono generare frammenti di contenuto o intere esperienze che orchestrano parti discrete di contenuti approvati per soddisfare le esigenze di specifiche campagne di marketing.

Gli editor interagiscono con le tecnologie di intelligenza artificiale generativa di GenStudio for Performance Marketing tramite _prompt_. Il cassetto dei prompt nell’area di lavoro fornisce gli strumenti per inserire i prompt nel contesto delle linee guida di una campagna specifica. Di conseguenza, la qualità e il successo dei contenuti generati dipendono in parte dalla qualità delle linee guida del brand caricate dalla tua organizzazione e dalla specificità del prompt. Vedere [Scrivi prompt effettivi](effective-prompts.md).

Nella tabella seguente vengono visualizzate le autorizzazioni dell’editor predefinito:

| Funzione | Creare | Aggiornare | Elimina | Visualizzazione |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | no | no | no | sì |
| [!DNL Campaigns] | sì | sì | sì | sì |
| [!DNL Content] | sì | sì | sì | sì |
| [!DNL Create] | sì | sì | sì | sì |
| [!DNL Insights] | può configurare solo i connettori |    |     | sì |
| [!DNL Personas] | sì | sì* | sì* | sì |
| [!DNL Products] | sì | sì* | sì* | sì |
| [!DNL Reviews and approvals] | sì | sì | sì | sì |
| [!DNL Templates] | no | no | no | sì |

Gli editor possono modificare ed eliminare [!DNL Personas] e [!DNL Products] creati.

I manager di sistema di GenStudio possono concedere agli editor l&#39;autorizzazione per modificare ed eliminare [!DNL Brand].

### Collaboratori GenStudio

_I collaboratori_ possono visualizzare le risorse in GenStudio for Performance Marketing ma non crearle, modificarle o eliminarle. I collaboratori visualizzano ad esempio il messaggio &quot;*Non hai accesso a questo contenuto*&quot; quando tentano di accedere a [[!DNL Create]](/help/user-guide/create/overview.md).

I collaboratori includono le parti interessate che sono essenziali per il successo del processo di revisione e approvazione dei contenuti, ma che non devono creare o modificare direttamente i contenuti. Esperti legali e manager dei creativi sono esempi di potenziali collaboratori. I collaboratori GenStudio for Performance Marketing possono disporre dell’autorizzazione per creare e visualizzare risorse in altri prodotti Creative Cloud.

Nella tabella seguente vengono visualizzate le autorizzazioni di collaborazione predefinite:

| Funzione | Creare | Aggiornare | Elimina | Visualizzazione |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | no | no | no | sì |
| [!DNL Campaigns] | no | no | no | sì |
| [!DNL Content] | no | no | no | sì |
| [!DNL Create] | no | no | no | sì |
| [!DNL Insights] | no | no | no | sì |
| [!DNL Personas] | no | no | no | sì |
| [!DNL Products] | no | no | no | sì |
| [!DNL Reviews and approvals] | no | no | no | sì |
| [!DNL Templates] | no | no | no | sì |

### Responsabili di sistema GenStudio

_I manager di sistema di GenStudio_ dispongono del set di autorizzazioni più potente in GenStudio for Performance Marketing. Questi utenti esperti eseguono il compito essenziale di onboarding, ovvero stabilire i guardrail fondamentali per la creazione e l’implementazione delle risorse delle campagne. I responsabili di sistema implementano questi guardrail caricando informazioni specifiche per il marchio e l&#39;organizzazione come [linee guida per il marchio](./guidelines/overview.md). I responsabili di sistema dispongono dell&#39;autorizzazione per creare e pubblicare [!DNL Brands], ma non dispongono dei privilegi di amministrazione degli utenti.

Nella tabella seguente vengono visualizzate le autorizzazioni predefinite di System Manager:

| Funzione | Creare | Aggiornare | Elimina | Visualizzazione |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | sì | sì | sì | sì |
| [!DNL Campaigns] | sì | sì | sì | sì |
| [!DNL Content] | sì | sì | sì | sì |
| [!DNL Insights] | sì | sì | sì | sì |
| [!DNL Personas] | sì | sì | sì | sì |
| [!DNL Products] | sì | sì | sì | sì |
| [!DNL Reviews and approvals] | sì | sì | sì | sì |
| [!DNL Templates] | sì | sì | sì | sì |

I manager di sistema possono anche caricare i modelli.

Consulta [Introduzione ad Adobe GenStudio for Performance Marketing](get-started.md) per una panoramica delle attività di configurazione preliminari.
