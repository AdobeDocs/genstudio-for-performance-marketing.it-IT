---
title: Connetti supporti a pagamento
description: Collega un account di canale per attivare e monitorare annunci e contenuti multimediali con Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Admin, Data Engineer
feature: Reporting and Insights
exl-id: e699041e-b462-45b3-8c4c-4de0d52cf0e6
source-git-commit: af354448ef609db3c51026ee0e9991ac5cedeba5
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# Connettere account di media a pagamento

_[!DNL Data connectors]_consente l&#39;integrazione diretta tra GenStudio for Performance Marketing e gli account di rete per media a pagamento. Tramite la connessione agli account di canale di terze parti, è possibile scambiare dati critici, ad esempio le metriche delle prestazioni della campagna in [[!DNL Insights]](/help/user-guide/insights/overview.md), e distribuire nuovi posizionamenti di annunci con [[!DNL Activate]](/help/user-guide/activation/overview.md). Questa integrazione consente a GenStudio for Performance Marketing di gestire i contenuti multimediali e gli annunci e di ricevere informazioni importanti, tra cui impression, clic e conversioni, dalle campagne attive.

**Per connettersi a un account multimediale a pagamento**:

1. Fare clic sui puntini di sospensione **[!UICONTROL ... Altro]** nella navigazione in basso a sinistra.

1. Seleziona **[!UICONTROL Impostazioni]** con l&#39;icona a forma di codice.

1. In _[!UICONTROL Impostazioni]_, scegli un tipo di connettore dalla sezione _[!UICONTROL Connettori dati]_ e fai clic su **[!UICONTROL Connetti]**.

   In alternativa, se sono presenti account connessi, è possibile fare clic su _account connessi_ per visualizzare un elenco di nomi, dettagli e stato degli account.

1. Vedere il [tipo di connettore](#connector-types) selezionato, esaminare i prerequisiti e continuare con i passaggi della connessione.

## Connessioni di supporti a pagamento

GenStudio for Performance Marketing supporta vari tipi di connettori da integrare con le piattaforme di marketing preferite. Ogni tipo di connettore ha prerequisiti specifici e passaggi di configurazione da completare per una connessione di successo.

### Connessione a Google Campaign Manager 360

>[!BEGINSHADEBOX]

**Prerequisiti**:

- Account Google Campaign Manager 360
- Rimuovere eventuali blocchi popup nel browser

>[!ENDSHADEBOX]

**Per connettere un account Google Campaign Manager 360**:

1. Nella sezione _Data Connectors_, fai clic su **[!UICONTROL Connetti]** nella scheda _Google Campaign Manager 360_.

1. Accedi al tuo account Google Campaign Manager 360.

   Potrebbe essere necessario rimuovere i blocchi popup e quindi utilizzare **[!UICONTROL Aggiorna]** per riprovare.

1. Leggi i termini e le condizioni e fai clic su **[!UICONTROL Consenti]** per concedere l&#39;accesso.

1. Nella visualizzazione _[!UICONTROL Google Campaign Manager 360]_, selezionare uno o più inserzionisti e fare clic su **[!UICONTROL Seleziona]**.

Nella visualizzazione _[!UICONTROL Account Google Campaign Manager 360]_ sono elencati `Account name`, `Added by`, `Date added` e `Status`. Utilizza **[!UICONTROL Aggiungi account]** per aggiungere altri account all&#39;elenco.

### Connessione di meta-annunci

>[!BEGINSHADEBOX]

**Prerequisiti**:

- Account Facebook/Meta ads
- Accesso all&#39;account dei metadati con il livello di autorizzazione `View performance` per accedere ai report e visualizzare gli annunci
- Rimuovere eventuali blocchi popup nel browser

>[!ENDSHADEBOX]

**Per connettere un account di Meta Ads**:

1. Nella sezione _Data Connectors_, fai clic su **[!UICONTROL Connect]** nella scheda _Meta Ads_.

1. Accedi al tuo account Facebook.

   Potrebbe essere necessario rimuovere i blocchi popup e quindi utilizzare **[!UICONTROL Aggiorna]** per riprovare.

1. Segui le istruzioni di autenticazione di Facebook.

1. Nel pop-up _[!UICONTROL Accesso Facebook per le aziende]_ (simbolo da Meta ad Adobe), scorri le seguenti selezioni.

   - Verifica le informazioni sull&#39;account e fai clic su **[!UICONTROL Continua come]**
   - Concedi l&#39;accesso a pagine selezionate e fai clic su **[!UICONTROL Continua]**
   - Concedi l&#39;accesso a determinate aziende e fai clic su **[!UICONTROL Continua]**
   - Accedi a uno o più account Instagram e fai clic su **[!UICONTROL Continua]**
   - Rivedi le selezioni e fai clic su **[!UICONTROL Salva]**

1. Nella visualizzazione _[!UICONTROL Meta Ads]_, seleziona uno o più account e fai clic su **[!UICONTROL Select]**.

Nella visualizzazione _[!UICONTROL Account Meta Ads]_ sono elencati `Account name`, `Added by`, `Date added` e `Status`. Utilizza **[!UICONTROL Aggiungi account]** per aggiungere altri account all&#39;elenco.

## Acquisizione dei dati

Inizialmente, GenStudio for Performance Marketing importa i dati storici relativi ai sei mesi più recenti. Questa procedura garantisce l’accesso immediato a informazioni rilevanti per l’analisi delle tendenze, la valutazione delle prestazioni e il processo decisionale informato. Il processo di acquisizione può richiedere da uno a cinque giorni a seconda del volume di dati nel tuo account.

>[!BEGINSHADEBOX]

**Criteri di acquisizione e conservazione dei dati**

GenStudio for Performance Marketing conserva i dati del canale per 13 mesi. Questo criterio di conservazione include i 6 mesi di dati acquisiti durante la connessione iniziale, garantendo analisi e rapporti completi sui dati storici.

>[!ENDSHADEBOX]
