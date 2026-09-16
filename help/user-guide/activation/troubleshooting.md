---
title: Ottimizzare l'attivazione
description: Scopri come ottimizzare le attivazioni per i canali di annunci a pagamento di terze parti.
level: Intermediate
feature: Ad Activation
exl-id: 5bc624c2-d064-4190-8761-ed05d0629d1f
TQID: https://experienceleague.adobe.com/-D3DGxTpZ-0J-grE5-jKPrptf4C1Z-OE1t0DCoqhRLQ
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 1%
---
# Ottimizzare le attivazioni

L’attivazione di un’esperienza pubblicitaria per i canali di annunci a pagamento prevede due fasi principali:

* Configurazione dei dettagli di installazione di annunci e piattaforme per ogni riga nella tabella di attivazione

* Pubblicazione dell’attivazione ai gestori di annunci dei canali di annunci a pagamento designati

Segui le best practice durante la configurazione e l’attivazione delle esperienze pubblicitarie per ridurre al minimo potenziali complicazioni o errori durante la consegna ai canali di destinazione.

## Best practice

Di seguito sono riportate alcune best practice comuni e gli errori che possono essere evitati.

* **Utilizza un ID di tracciamento univoco per ogni riga**

  [!DNL Activate] contrassegna gli ID di tracciamento duplicati come [!UICONTROL Richiede attenzione] e non ti consente di pubblicare finché ogni riga nel formato e nella tabella della piattaforma interessati non avrà un ID di tracciamento univoco. Se modifichi in blocco un ID di tracciamento su più righe, conferma di voler applicare lo stesso valore a ogni riga selezionata.

* **Usa URL di destinazione validi e completi**

  Gli URL non validi possono generare errori. Errore di esempio: _L&#39;URL immesso non reindirizza a un sito Web. Immetti un URL valido e riprova. (100)_

* **Assicurati che l&#39;applicazione gestisca correttamente la scadenza del token**

  Le applicazioni devono richiedere nuovi token in base alle esigenze. Esegui nuovamente l’autenticazione e ottieni un nuovo token di accesso effettuando di nuovo l’accesso o aggiornando la sessione. Errore di esempio: _Errore durante la convalida del token di accesso: la sessione è stata invalidata perché l&#39;utente ha cambiato la password o Facebook ha modificato la sessione per motivi di sicurezza. (190)_

* **Controlla il set di annunci e assicurati che sia attivo un solo annuncio alla volta**

  Se devi attivare più annunci Meta Ads, crea un set di annunci Dynamic Creative separato per ciascuno di essi. Errore di esempio: _Dynamic Creative Ad Set consente al massimo un annuncio attivo. Gli utenti non possono creare più di un annuncio pubblicitario nello stesso Dynamic Creative Ad Set. (100)_

* **Abbina il numero di regole applicate con la quantità specificata dalla piattaforma**

  I canali a pagamento si aspettano che il numero di regole applicate corrisponda al formato specificato.  Se necessario, regola il numero di regole in modo che corrisponda al valore specificato dalla piattaforma. Errore di esempio: _L&#39;Ad AssetFeed ha X regole di destinazione per il formato: nome del formato, ma è prevista esattamente X regola di destinazione per questo formato. (100)_

* **Scegli un call-to-action (CTA) compatibile con l&#39;obiettivo del set di annunci**

  Gli inviti all’azione incompatibili con l’obiettivo in Set di annunci Dynamic Creative attivano un errore. Errore di esempio: _Il tipo di call to action X non è supportato per l&#39;obiettivo Y in Dynamic Creative Ad Set. (100)_

* **Assicurarsi che il limite del set di annunci di destinazione supporti il numero di esperienze annuncio**

  Conferma che il limite di annunci del set di annunci di destinazione possa soddisfare le esperienze di annunci attivati. Se necessario, rimuovi eventuali annunci non necessari o inattivi dal set di annunci per rimanere entro questo limite. In alternativa, crea un nuovo set di annunci per attivare annunci aggiuntivi. Errore di esempio: _Hai raggiunto la campagna, il set di annunci o i limiti di annunci per account annuncio. Ogni set di annunci può contenere un massimo di 50 annunci. Sono inclusi gli annunci in pausa, inattivi e disattivati. (100)_

* **Assicurarsi che la piattaforma supporti il tipo di CTA selezionato**

  Verifica che la tua esperienza includa un tipo di CTA supportato. Errore di esempio: _(#100) Tipo di call to action (100)_ non valido
