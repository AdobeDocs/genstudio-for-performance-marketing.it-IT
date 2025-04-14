---
title: Connetti supporti a pagamento
description: Connect a channel account to activate and monitor your ads and media with Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Admin, Data Engineer
feature: Reporting and Insights
exl-id: e699041e-b462-45b3-8c4c-4de0d52cf0e6
source-git-commit: 2844914d25d9bc3a2be7f47d0cd7f26f7c921555
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---

# Connect paid media accounts

_[!DNL Data connectors]_enable seamless integration between GenStudio for Performance Marketing and your paid media network accounts. By connecting to third-party channel accounts, you can exchange critical data, such as campaign performance metrics in [[!DNL Insights]](/help/user-guide/insights/overview.md), and you can deliver fresh ad placements with [[!DNL Activate]](/help/user-guide/activation/overview.md). This integration allows GenStudio for Performance Marketing to manage your media and ads while receiving valuable insights, including impressions, clicks, and conversions, from your active campaigns.

**Per connettersi a un account multimediale a pagamento**:

1. Fare clic sui puntini di sospensione **[!UICONTROL ... Altro]** nella navigazione in basso a sinistra.

1. Seleziona **[!UICONTROL Impostazioni]** con l&#39;icona a forma di codice.

1. In _[!UICONTROL Impostazioni]_, scegli un tipo di connettore dalla sezione _[!UICONTROL Connettori dati]_ e fai clic su **[!UICONTROL Connetti]**.

   In alternativa, se sono presenti account connessi, è possibile fare clic su _account connessi_ per visualizzare un elenco di nomi, dettagli e stato degli account.

1. Vedere il [tipo di connettore](#connector-types) selezionato, esaminare i prerequisiti e continuare con i passaggi della connessione.

## Connessioni di supporti a pagamento

GenStudio for Performance Marketing supports various connector types to integrate with your preferred marketing platforms. Each connector type has specific prerequisites and set-up steps to complete for a successful connection.

### Meta ads connect

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

1. In the _[!UICONTROL Facebook Login for Business]_ pop-up (Meta to Adobe symbol), step through the following selections.

   - Verify the account information and click **[!UICONTROL Continue as]**
   - Grant access to select Pages and click **[!UICONTROL Continue]**
   - Concedi l&#39;accesso a determinate aziende e fai clic su **[!UICONTROL Continua]**
   - Accedi a uno o più account Instagram e fai clic su **[!UICONTROL Continua]**
   - Rivedi le selezioni e fai clic su **[!UICONTROL Salva]**

1. Nella visualizzazione _[!UICONTROL Meta Ads]_, seleziona uno o più account e fai clic su **[!UICONTROL Select]**.

Nella visualizzazione _[!UICONTROL Account Meta Ads]_ sono elencati `Account name`, `Added by`, `Date added` e `Status`. Utilizza **[!UICONTROL Aggiungi account]** per aggiungere altri account all&#39;elenco.

## Acquisizione dei dati

Inizialmente, GenStudio for Performance Marketing importa i dati storici relativi ai sei mesi più recenti. Questa procedura garantisce l’accesso immediato a informazioni rilevanti per l’analisi delle tendenze, la valutazione delle prestazioni e il processo decisionale informato. The ingestion process may take one to five days depending on the volume of data in your account.

>[!BEGINSHADEBOX]

**Data Ingestion and Retention Policy**

GenStudio for Performance Marketing conserva i dati del canale per 13 mesi. Questo criterio di conservazione include i 6 mesi di dati acquisiti durante la connessione iniziale, garantendo analisi e rapporti completi sui dati storici.

>[!ENDSHADEBOX]
