---
title: Convalida del marchio in Adobe GenStudio for Performance Marketing
description: Scopri come funziona il sistema integrato di convalida del brand in GenStudio for Performance Marketing.
feature: Brand Personalization, Variant Generation, Compliance, Content Generation, Content Review, Generative AI
exl-id: 2e777186-3b7e-46a6-9d37-7c7b7c2aa7ae
source-git-commit: 29685c96353703705f3f742e88f3934644bc4282
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 0%

---

# Convalida del brand

In GenStudio for Performance Marketing, la convalida del brand è un componente essenziale che funziona in collaborazione con le funzionalità e le linee guida di IA generativa: [[!DNL Brands]](/help/user-guide/guidelines/brands.md), [[!DNL Products]](/help/user-guide/guidelines/products.md) e [[!DNL Personas]](/help/user-guide/guidelines/personas.md). In questo modo tutti i contenuti saranno allineati all’identità del brand, agli standard ADA e alle indicazioni sulla piattaforma dei singoli canali.

GenStudio for Performance Marketing esegue la convalida del brand e altri controlli dei contenuti su vari aspetti, tra cui:

* [!DNL Brand] linee guida definite o predefinite
* Linee guida per la piattaforma
<!-- * Ethical considerations related to gender, ethnicity, race, disability status, and age in AI-generated content -->
* Standard dell&#39;American with Disabilities Act (ADA)

## Riepilogo verifica contenuto

Un riepilogo della convalida del brand e altre informazioni di controllo del contenuto per ogni variante di contenuto generata è accessibile tramite l&#39;icona di riepilogo _Controllo contenuto_ per ogni variante nell&#39;area di lavoro.

Il riepilogo del _controllo contenuto_ visualizza:

* Percentuale di conformità con [[!DNL Brand]](brands.md) calcolata come il numero di [linee guida](overview.md) che hanno superato la convalida rispetto al numero di linee guida testate
* `Pass` o `Fail` risultato per le linee guida della piattaforma, ad esempio Meta o LinkedIn
* `Pass` o `Fail` risultato per gli standard di accessibilità ADA

![Riepilogo controllo contenuto](/help/assets/content-check-summary.png){width="400" zoomable="yes"}

Fai clic sulla percentuale per vedere quanto è conforme la variante. I punteggi vengono aggiornati automaticamente quando si apportano modifiche alle varianti. Puoi fare clic su _Visualizza e correggi i problemi_ per garantire un&#39;ulteriore conformità.

Consulta [Migliorare l&#39;allineamento del brand](#improve-brand-alignment).

## Pannello di controllo contenuto

Il pannello _Verifica contenuto_ si apre sul lato destro dell&#39;area di lavoro quando si fa clic sulla barra delle azioni di destra _o_ dall&#39;icona di riepilogo [_Verifica contenuto_](#content-check-summary) per una variante. Questo pannello fornisce una convalida dettagliata del brand. le linee guida per le piattaforme e le informazioni sugli standard di accessibilità, illustrando le opportunità di miglioramento per ogni sezione delle varianti.

![Pannello di controllo contenuto](/help/assets/content-check-panel.png){width="400" zoomable="yes"}

Il pannello _Verifica contenuto_ visualizza le informazioni di convalida e [conformità](/help/user-guide/guidelines/overview.md#compliance) per ogni sezione della variante:

* Rappresentazione delle informazioni di riepilogo del _controllo contenuto_ per [!DNL Brand], linee guida della piattaforma e standard di accessibilità
* _Sezione Necessità di revisione_ in cui viene visualizzato il numero di linee guida non riuscite e informazioni dettagliate su ciascuna linea guida da rivedere
* _Sezione passata_ che visualizza il numero di linee guida trasmesse e informazioni dettagliate su ciascuna linea guida passata

Consulta [Migliorare l&#39;allineamento del brand](#improve-brand-alignment) per scoprire come migliorare i punteggi del pannello _Verifica contenuto_.

### Tipo di contenuto

Nel pannello _Verifica contenuto_ è possibile attivare o disattivare i controlli degli standard di accessibilità e delle linee guida. Fai clic sull&#39;icona _Tipo di contenuto_ (icona livelli) nella parte superiore del pannello per attivare o disattivare:

* **[!DNL Brand]** - Esegue i controlli associati alle linee guida di [!DNL Brand]
* **Linee guida per Platform**: esegue i controlli associati alla piattaforma specifica per il canale, ad esempio Meta
* **Accessibilità** - Esegue i controlli associati agli standard di accessibilità ADA

Per **impostare il tipo di contenuto** per i controlli che si desidera eseguire, fare clic per disattivare o attivare i tipi disponibili e fare clic su **Applica**.

## Migliorare l’allineamento del brand

Per massimizzare l&#39;efficacia dei contenuti generati e mantenere un&#39;identità del brand coerente, utilizza il [_riepilogo del controllo dei contenuti_](#content-check-summary) e il [_pannello del controllo dei contenuti_](#content-check-panel). Puoi modificare manualmente sezioni specifiche per allinearle alle [[!DNL Brand] linee guida](brands.md), ai controlli delle linee guida della piattaforma e ai controlli degli standard di accessibilità.

**Per migliorare l&#39;allineamento del brand per le varianti generate**:

1. Fai clic sull&#39;icona del pannello _Verifica contenuto_ nella barra delle azioni a destra per visualizzare le informazioni di convalida e accessibilità per una singola variante.

   Puoi visualizzare un riepilogo delle _verifiche necessarie_ e _verifiche superate_ per vedere quali sezioni e linee guida necessitano di miglioramenti.

   >[!NOTE]
   >
   > La linea guida di _Brand voice_ indicata nel pannello _Verifica contenuto_ si applica all&#39;intera variante, non a una singola sezione. L’intera variante di contenuto è evidenziata per suggerire un miglioramento.

1. Fai clic su per correggere le linee guida attualmente non conformi.
1. Fai clic su per espandere ed esaminare ogni controllo che necessita di revisione nelle sezioni disponibili, ad esempio _Titolo_ e _Voce marchio_.

   Utilizza il ragionamento fornito per ogni controllo per guidarti nella revisione delle varianti.

1. Dopo aver apportato le revisioni necessarie, fai clic su **[!UICONTROL Ricontrolla il punteggio]** per ricontrollare e convalidare le modifiche per assicurarti che siano più allineate con l&#39;identità del tuo marchio, le linee guida della piattaforma e gli standard di accessibilità.

   Il processo di controllo del contenuto viene eseguito nuovamente. Se gli elementi rivisti superano la convalida, nella parte inferiore dell’area di lavoro viene visualizzato un banner verde per confermare che il punteggio è stato aggiornato. Se non ci sono state modifiche dopo un nuovo controllo, il banner conferma che non vi sono state modifiche al punteggio. Anche la percentuale nell&#39;icona di riepilogo del _controllo contenuto_ per la variante rivista mostra l&#39;avanzamento.

1. Continua a rivedere le sezioni per garantire che l’intera variante superi i controlli di convalida e accessibilità. Naviga tra le varianti utilizzando le frecce adiacenti a una singola variante nell’area di lavoro.

