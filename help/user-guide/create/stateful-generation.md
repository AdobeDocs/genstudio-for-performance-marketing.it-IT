---
title: Generare e perfezionare i contenuti con la generazione con conservazione dello stato
description: Scopri come generare contenuti nel brand e perfezionarli a turno in una conversazione con la stampa vocale e suggerimenti visivi in [!DNL GenStudio for Performance Marketing].
feature: Create Prompt, Generative AI, Content Generation
role: User
level: Beginner
source-git-commit: 22db02c07a9f33cb1c70df9286ad6eb143dafd38
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%
---
# Generare e perfezionare i contenuti con la generazione con conservazione dello stato

[!DNL GenStudio for Performance Marketing] utilizza la generazione con stato per facilitare la creazione di contenuti nel brand e quindi perfezionarli di volta in volta in una conversazione, invece di ricominciare ogni volta con un nuovo prompt. Mentre si perfeziona, la generazione ricorda le istruzioni precedenti e le varianti che si mantengono, quindi applica solo la modifica richiesta.

La generazione con conservazione dello stato aggiunge tre tipi di contesto alle generazioni: la stampa vocale mantiene la copia nella voce del marchio, i segnali visivi vengono copiati in un&#39;immagine o in un video e l&#39;URL di una pagina Web aggiunge il contesto di riferimento da una pagina scelta.

## Generare e perfezionare i contenuti

1. In [!DNL GenStudio for Performance Marketing], avvia una generazione per il canale e il formato. Consulta la [[!DNL Create] panoramica](/help/user-guide/create/overview.md) per iniziare una generazione per ogni canale.
1. _Facoltativo_: per mettere a terra la copia nella tua creatività, seleziona **[!UICONTROL Seleziona dal contenuto]**, quindi scegli un&#39;immagine o un video da utilizzare come [segnale visivo](#ground-content-in-an-image-or-video).
1. Seleziona **[!UICONTROL Genera]**. [!DNL GenStudio for Performance Marketing] crea un set di varianti e applica la tua [voce marchio](#keep-copy-in-your-brand-voice) automaticamente sui canali supportati.
1. Perfezionate i risultati nel cassetto dei prompt. Digitare la modifica desiderata, ad esempio `shorten the headline`, `make variant 2 punchier` o `change the headline`. La generazione applica solo tale modifica e mantiene le istruzioni precedenti.
1. Per mantenere una variante mentre si continua a perfezionare, digitare un&#39;istruzione nel cassetto dei prompt, ad esempio `keep variant 2`.
1. Quando il contenuto è pronto, esportalo o invialo per la revisione.

## Mettere a terra il contenuto di un&#39;immagine o di un video

I segnali visivi consentono alla generazione di leggere un&#39;immagine o un video allegato, quindi di scrivere una copia che rifletta tale contenuto creativo. L&#39;opzione **[!UICONTROL Opzioni Creative]** controlla i segnali visivi ed è attivata per impostazione predefinita.

Per utilizzare un segnale visivo, selezionare **[!UICONTROL Seleziona dal contenuto]** e scegliere un&#39;immagine o un video prima della generazione. Per generare senza un segnale visivo, disattivare **[!UICONTROL Opzioni Creative]**.

>[!NOTE]
>I suggerimenti visivi non sono disponibili per gli annunci display multi-frame o per gli annunci carosello.

## Mantieni la copia nella tua voce del marchio

La stampa vocale applica la voce appresa del tuo marchio alla copia generata, in modo che suoni sul marchio senza ulteriori prompt. È attivata per impostazione predefinita per i canali con [Informazioni](/help/user-guide/insights/overview.md), ad esempio LinkedIn e Meta.

## Utilizzare una pagina web come contesto

Puoi puntare la generazione a una pagina web e utilizzarne il contenuto come contesto. Nel cassetto dei prompt, digitare un&#39;istruzione che includa l&#39;URL, ad esempio `Use this URL to generate an ad for this channel: https://www.example.com`.

>[!NOTE]
>Immetti l’URL nella richiesta. Non aggiungerlo tramite _Parametri_.

## Funzionalità correlate

- [Gestisci varianti](/help/user-guide/create/manage-variants.md): modifica e perfeziona le varianti generate direttamente sull&#39;area di lavoro.
- [Scrivi prompt effettivi](/help/user-guide/effective-prompts.md): i prompt di creazione producono risultati migliori.
