---
title: Ottimizzare l’attivazione
description: Scopri come ottimizzare le attivazioni per i canali di annunci a pagamento di terze parti.
feature: Ad Activation, Workflow
exl-id: 5bc624c2-d064-4190-8761-ed05d0629d1f
source-git-commit: 445b5c2fce07ee8bc67e96f95e670fecda356b22
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 0%

---

# Ottimizzare le attivazioni

L’attivazione di un’esperienza pubblicitaria per i canali di annunci a pagamento prevede due fasi principali:

* Preparazione dell’esperienza per l’attivazione

* Pubblicazione dell’esperienza ai relativi ad manager di canale a pagamento designati

Segui le best practice durante la creazione e l’attivazione dell’esperienza pubblicitaria per ridurre al minimo potenziali complicazioni o errori durante la consegna ai canali di destinazione.

## Best practice

Di seguito sono riportate alcune best practice comuni e gli errori che possono essere evitati.

* **Usa URL di destinazione validi e completi**

  Gli URL non validi possono generare errori. Errore di esempio: _L&#39;URL immesso non reindirizza a un sito Web. Immetti un URL valido e riprova. (100)_

* **Assicurati che l&#39;applicazione gestisca correttamente la scadenza del token**

  Le applicazioni devono richiedere nuovi token in base alle esigenze. Se necessario, ripeti l’autenticazione e ottieni un nuovo token di accesso effettuando di nuovo l’accesso o aggiornando la sessione. Errore di esempio: _Errore durante la convalida del token di accesso: la sessione è stata invalidata perché l&#39;utente ha cambiato la password o Facebook ha modificato la sessione per motivi di sicurezza. (190)_

* **Controlla il set di annunci e assicurati che sia attivo un solo annuncio alla volta**

  Se devi attivare più Meta Ads, crea un set di annunci Dynamic Creative separato per ciascuno di essi. Errore di esempio: _Dynamic Creative Ad Set consente al massimo un annuncio attivo. Gli utenti non possono creare più di un annuncio pubblicitario nello stesso Dynamic Creative Ad Set. (100)_

* **Abbina il numero di regole applicate con la quantità specificata dalla piattaforma**

  I canali a pagamento si aspettano che il numero di regole applicate corrisponda al formato specificato.  Se necessario, regola il numero di regole in modo che corrisponda al valore specificato dalla piattaforma. Errore di esempio: _L&#39;Ad AssetFeed ha X regole di destinazione per il formato: nome del formato, ma è prevista esattamente X regola di destinazione per questo formato. (100)_

* **Scegli un invito all&#39;azione (CTA) compatibile con l&#39;obiettivo del set di annunci**

  Gli inviti all’azione incompatibili con l’obiettivo in Set di annunci Dynamic Creative attivano un errore. Errore di esempio: _L&#39;invito all&#39;azione di tipo X non è supportato per l&#39;obiettivo Y in Dynamic Creative Ad Set. (100)_

* **Assicurarsi che il limite del set di annunci di destinazione supporti il numero di esperienze annuncio**

  Conferma che il limite di annunci del set di annunci di destinazione possa soddisfare le esperienze di annunci attivati. Se necessario, rimuovi eventuali annunci non necessari o inattivi dal set di annunci per rimanere entro questo limite. In alternativa, crea un nuovo set di annunci per attivare annunci aggiuntivi. Errore di esempio: _Hai raggiunto la campagna, il set di annunci o i limiti di annunci per account annuncio. Ogni set di annunci può contenere un massimo di 50 annunci. Sono inclusi gli annunci in pausa, inattivi e disattivati. (100)_

* **Assicurarsi che la piattaforma supporti il tipo di CTA selezionato**

  Verifica che la tua esperienza includa un tipo di CTA supportato. Errore di esempio: _(#100) Tipo di chiamata all&#39;azione non valido (100)_
