---
title: Editor di codice modello
description: Scopri come utilizzare l’editor di codice modello in GenStudio for Performance Marketing.
level: Intermediate
feature: Media Templates, Content Generation
exl-id: b46fc7a9-88c1-474a-9d7b-1df7740d8f5a
source-git-commit: 19d0b8b929e293179a091cc7b5a6a1268b0abbbd
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 0%

---

# Editor di codice modello

L’editor di codice modello è progettato per aiutarti a verificare e perfezionare il modello per un utilizzo ottimale durante la generazione di nuove esperienze con GenStudio for Performance Marketing. L’editor supporta la sintassi Handlebars, che utilizza segnaposto all’interno del modello per indicare dove GenStudio for Performance Marketing deve generare il contenuto per te.

>[!TIP]
>
>Prima di caricare il codice HTML del modello nella visualizzazione [!DNL Content] _Modelli_, prepara il modello inserendo i segnaposto di contenuto definiti nella guida [Personalizza modelli](customize-template.md).

## Controlla i campi rilevati

Nel riquadro _[!UICONTROL Controlla campi rilevati]_ è visualizzato un elenco di campi riconosciuti da GenStudio for Performance Marketing nel modello. Rivedi l’elenco e puoi scorrere il codice HTML per esaminare la formazione del modello.

![Visualizzazione editor di codice](/help/assets/template-detected-fields.png "Controlla i campi rilevati"){width="600" zoomable="yes"}

Se noti che manca un campo nell’elenco, cerca nel codice del modello e individua la posizione del campo mancante. Inserire il segnaposto corretto utilizzando la sintassi Handlebars e un [nome di campo riconosciuto](/help/user-guide/content/customize-template.md#recognized-field-names). Utilizza il modulo Trova e sostituisci, che viene visualizzato nella parte inferiore dell’editor di codice, per cercare stringhe specifiche nel codice. (Windows `CTRL`+`F` o macOS `CMD`+`F`)

### Effettua una correzione

Se nel modello sono presenti errori, è possibile che venga visualizzato un messaggio di `Template is invalid` che include una breve spiegazione del problema. Nell&#39;esempio seguente, il messaggio indica che il campo `_image` non è conforme alla convenzione di denominazione dei campi stabilita nel modello a più pod. Il messaggio informa inoltre che è necessario aggiornare il nome del campo con il prefisso corretto. Trova il campo `_image` nell&#39;editor di codice del modello e aggiorna il nome come consigliato.

![Correggere un modello non valido](/help/assets/animation/template-code-editor.gif){width="600" zoomable="yes"}

Il riquadro _[!UICONTROL Controlla i campi rilevati]_ si aggiorna per riflettere le modifiche apportate. Dopo aver verificato che i campi sono corretti e completi, fai clic su **[!UICONTROL Avanti]** per continuare a [caricare il modello](/help/user-guide/content/use-templates.md#add-a-template).
