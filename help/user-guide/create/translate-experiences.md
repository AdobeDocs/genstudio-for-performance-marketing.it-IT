---
title: Tradurre e localizzare le esperienze
description: Scopri come tradurre le esperienze e-mail e media a pagamento approvate in più lingue sull’area di lavoro di HTML in Adobe GenStudio for Performance Marketing.
feature: Create Canvas, Content Generation
role: User
level: Beginner
source-git-commit: bc59f6f5dce0c4f22228bcd06c2f5e60a4311e04
workflow-type: tm+mt
source-wordcount: '767'
ht-degree: 2%

---

# Tradurre e localizzare le esperienze

Adobe [!DNL GenStudio for Performance Marketing] offre la traduzione predefinita nell&#39;area di lavoro di HTML, in modo che gli addetti al marketing a livello globale e regionale possano ridimensionare le esperienze approvate in più lingue senza dover ricorrere a strumenti di traduzione esterni.

Per impostazione predefinita, la funzione utilizza Azure Open AI. La tua organizzazione può anche connettere un servizio di traduzione preferito tramite [estensioni di traduzione](/help/extensibility/deploy-app.md#find-translation-extensions).

La traduzione inizia da un&#39;esperienza approvata salvata in [!DNL Content]. L’esperienza sorgente può essere in qualsiasi lingua. Ogni variante tradotta viene aperta nell&#39;area di lavoro [!DNL Create] come bozza modificabile che è possibile esportare, inviare per la revisione e pubblicare come esperienza separata.

## Esperienze supportati

La traduzione predefinita nell’area di lavoro di HTML supporta:

* [Esperienze e-mail](/help/user-guide/create/email-experiences.md)
* Esperienze multimediali a pagamento, inclusi [Meta](/help/user-guide/create/meta-experiences.md), [LinkedIn](/help/user-guide/create/linkedin-experiences.md) e [Annunci Display](/help/user-guide/create/display-ad-experiences.md)

## Prima di iniziare

Conferma che l&#39;esperienza che desideri tradurre è **approvata** e disponibile nella [!DNL Content] _[!UICONTROL raccolta esperienze]_. Le bozze o le esperienze in revisione non sono origini di traduzione idonee.

Se la tua organizzazione registra un’estensione di traduzione personalizzata, GenStudio for Performance Marketing utilizza tale servizio invece della traduzione Azure Open AI predefinita. Consulta [Trova estensioni di traduzione](/help/extensibility/deploy-app.md#find-translation-extensions).

## Traduci da [!DNL Create] {#translate-from-create}

Avvia una traduzione dalla pagina di destinazione [!DNL Create] per localizzare un&#39;esperienza approvata.

![Traduci e localizza la copia nella pagina di destinazione Crea](./translate-create-workflow.png){width="600" zoomable="yes"}

**Per tradurre da[!DNL Create]**:

1. In [!DNL Create], scorrere fino alla sezione _Creazione contenuto_.
1. Fai clic su **[!UICONTROL Traduci e localizza copia]**.
1. Seleziona l’e-mail approvata o l’esperienza multimediale a pagamento che desideri tradurre. Fare clic sul pulsante **[!UICONTROL Usa]**.
1. Seleziona le lingue di destinazione dall’elenco delle lingue supportate. Fai clic su **[!UICONTROL Traduci]**.

Le varianti tradotte vengono visualizzate nell’area di lavoro.

## Traduci da [!DNL Content] {#translate-from-content}

Puoi anche avviare la traduzione da [!DNL Content] quando esplori le esperienze approvate.

### Dalla galleria di esperienze

![Traduci azione su un&#39;esperienza nella raccolta contenuti](./translate-content-gallery.png){width="500" zoomable="yes"}

**Per tradurre dalla raccolta esperienze**:

1. In [!DNL Content] aprire la scheda **[!UICONTROL Esperienze]**.
1. Individua l’esperienza approvata che desideri tradurre.
1. Fai clic sul menu delle opzioni (tre punti) nella scheda esperienza.
1. Fai clic su **[!UICONTROL Traduci]**.
1. Seleziona le lingue di destinazione dall’elenco delle lingue supportate. Fai clic su **[!UICONTROL Traduci]**.

## Utilizzare le traduzioni nell’area di lavoro

Nell’area di lavoro di HTML non è possibile modificare l’esperienza sorgente perché è già approvata. Le esperienze dell’origine e-mail sembrano bloccate. Puoi modificare il testo nelle varianti tradotte direttamente sull’area di lavoro. Consulta [Gestione varianti](/help/user-guide/create/manage-variants.md) per informazioni sulla modifica della copia delle varianti.

Le esperienze tradotte non eseguono la convalida del brand o visualizzano un punteggio di brand. L’esperienza sorgente è già stata creata con linee guida per il brand, rivista e approvata.

La rigenerazione dei frammenti non è supportata per le esperienze tradotte.

### Eliminare una lingua tradotta

**Per rimuovere una lingua tradotta dall&#39;area di lavoro**:

1. Nell&#39;area di lavoro [!DNL Create] fare clic sul menu delle opzioni (tre punti) nell&#39;intestazione della variante tradotta.
1. Fai clic su **[!UICONTROL Elimina]**.

![Elimina una lingua tradotta dall&#39;area di lavoro](./remove-translation-variant.png){width="500" zoomable="yes"}

La lingua tradotta viene rimossa dall’area di lavoro.

### Aggiornare una traduzione di contenuti multimediali a pagamento

Dopo aver modificato la copia multimediale a pagamento tradotta, puoi ricaricare l’output di traduzione originale.

**Per aggiornare una traduzione di file multimediali a pagamento**:

1. Nell&#39;area di lavoro [!DNL Create] aprire il menu delle opzioni nella variante tradotta modificata.
1. Fare clic su **[!UICONTROL Aggiorna traduzione]**.

>[!NOTE]
>
>Aggiorna traduzione è disponibile per le esperienze multimediali a pagamento. Al momento, la funzione di traduzione e-mail non supporta l’aggiornamento della traduzione.

## Esportazione, revisione e pubblicazione

Dopo il caricamento delle traduzioni nell&#39;area di lavoro, è possibile esportarle, inviarle per l&#39;approvazione e pubblicare le varianti approvate in [!DNL Content].

**Per esportare esperienze tradotte**:

1. Nell&#39;area di lavoro [!DNL Create], fare clic su **[!UICONTROL Esporta]** nella barra degli strumenti.
1. Seleziona un formato di esportazione.
   * E-mail: **CSV e immagini** o **Solo HTML**
   * File multimediali a pagamento: **CSV + JPG**, **CSV + PNG** o **HTML + immagini**
1. Fai clic su **[!UICONTROL Esporta]**.

Puoi anche [esportare esperienze da [!DNL Content]](/help/user-guide/content/manage-assets.md#export-experiences).

**Per richiedere revisione e approvazione**:

1. Nell&#39;area di lavoro [!DNL Create] fare clic su **[!UICONTROL Richiedi approvazione]**.
1. Assegnare almeno un approvatore e inviare la richiesta.

Consulta [Richiedi revisione e approvazione](/help/user-guide/approvals/request-review.md) per i dettagli sul flusso di lavoro di revisione.

**Per pubblicare traduzioni approvate**:

1. Dopo che gli approvatori hanno approvato le varianti tradotte, fai clic su **[!UICONTROL Pubblica]**.
1. Nella finestra di pubblicazione, conferma i metadati quali nome della campagna, intervalli di tempo, aree geografiche e parole chiave.

Consulta [Pubblicare contenuti approvati](/help/user-guide/approvals/publish-content.md).

Ogni traduzione pubblicata viene salvata in [!DNL Content] come esperienza separata.

## Metadati esperienza tradotti

Le traduzioni pubblicate includono metadati che collegano ogni variante alla sua origine, tra cui:

* **Titolo**: segue il pattern `Translation from "<source title>" <channel>`, ad esempio `Translation from "Summer campaign" Meta`
* **Creato da**, l&#39;utente che ha avviato la traduzione
* **Data creazione** — la data della traduzione
* **Origine tradotta**: un collegamento all&#39;esperienza di origine in [!DNL Content]
* **Tradotto da** — lingua di origine

## Limitazioni

Quando traduci esperienze sull’area di lavoro di HTML, tieni presenti i seguenti vincoli:

* L&#39;esperienza di origine deve essere già approvata e salvata in [!DNL Content].
* La convalida del brand non viene eseguita sulle varianti tradotte.
* La rigenerazione dei frammenti non è supportata nelle esperienze tradotte.
* Aggiorna traduzione è disponibile solo per i file multimediali a pagamento.

## Informazioni correlate

* [Esperienze e-mail](/help/user-guide/create/email-experiences.md)
* [Esperienze Meta](/help/user-guide/create/meta-experiences.md)
* [Visualizzare esperienze annuncio](/help/user-guide/create/display-ad-experiences.md)
* [Gestione risorse ed esperienze](/help/user-guide/content/manage-assets.md)
* [Trova estensioni di traduzione](/help/extensibility/deploy-app.md#find-translation-extensions)
