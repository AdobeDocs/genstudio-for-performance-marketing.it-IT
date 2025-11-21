---
title: Editor codice modello
description: Scopri come utilizzare l’editor di codice modello in GenStudio for Performance Marketing.
level: Intermediate
role: Developer
feature: Media Templates, Content Generation
exl-id: b46fc7a9-88c1-474a-9d7b-1df7740d8f5a
source-git-commit: 9e51e853542d20f0b90b10071f4f26aaae1d6aad
workflow-type: tm+mt
source-wordcount: '783'
ht-degree: 0%

---

# Editor di codice modello

L’editor di codice modello è progettato per aiutarti a verificare e perfezionare il modello per un utilizzo ottimale durante la generazione di nuove esperienze con GenStudio for Performance Marketing. L’editor supporta la sintassi Handlebars, che utilizza segnaposto all’interno del modello per indicare dove GenStudio for Performance Marketing deve generare il contenuto per te.

>[!TIP]
>
>Prima di caricare il codice HTML del modello nella visualizzazione [!DNL Content] _Modelli_, prepara il modello inserendo i segnaposto di contenuto definiti nella guida [Personalizza modelli](customize-template.md).

## Controlla i campi rilevati

Nel riquadro _[!UICONTROL Controlla campi rilevati]_ è visualizzato un elenco di campi riconosciuti da GenStudio for Performance Marketing nel modello. Rivedi l’elenco e puoi scorrere il codice HTML per esaminare la formazione del modello.

![Visualizzazione editor di codice](/help/assets/template-detected-fields.png "Controlla i campi rilevati"){width="600"}

Se noti che manca un campo nell’elenco, cerca nel codice del modello e individua la posizione del campo mancante. Inserire il segnaposto corretto utilizzando la sintassi Handlebars e un [nome di campo riconosciuto](/help/user-guide/templates/customize-template.md#recognized-field-names). Utilizza il modulo Trova e sostituisci, che viene visualizzato nella parte inferiore dell’editor di codice, per cercare stringhe specifiche nel codice. (Windows `CTRL`+`F` o macOS `CMD`+`F`)

## Regolare i ruoli per una variabile

È possibile selezionare e modificare i ruoli di campo per i ruoli di campo basati su testo (ad esempio, `headline`, `sub_headline`, `body`, `cta`, `on_image_text`, `custom`) con un elenco a discesa durante la verifica della struttura del modello. Le selezioni del ruolo del campo persistono durante le modifiche del modello, in modo da non perdere le personalizzazioni e migliorare l’efficienza del flusso di lavoro.

>[!NOTE]
>
>I ruoli delle variabili immagine non possono essere regolati.

![Selezione di campi con più ruoli](/help/assets/multirole-dropdown-field.png "Selezione di campi con più ruoli"){width="600"}

Per assegnare un ruolo a una variabile:

1. Trova la variabile nel riquadro _[!UICONTROL Controlla campi rilevati]_. Queste variabili vengono individuate automaticamente.
2. Esamina i ruoli assegnati a ciascuna variabile. I ruoli vengono assegnati automaticamente, ma possono essere regolati utilizzando il menu a discesa per qualsiasi variabile nel modello.
3. Regola un ruolo selezionando un nuovo ruolo dal menu a discesa.
4. Fai clic su **[!UICONTROL Avanti]** per continuare.

## Effettua una correzione

Se nel modello sono presenti errori, è possibile che venga visualizzato un messaggio di `Template is invalid` che include una breve spiegazione del problema. Nell&#39;esempio seguente, il messaggio indica che il campo `_image` non è conforme alla convenzione di denominazione dei campi stabilita nel modello a più pod. Il messaggio informa inoltre che è necessario aggiornare il nome del campo con il prefisso corretto. Trova il campo `_image` nell&#39;editor di codice del modello e aggiorna il nome come consigliato.

![Correggere un modello non valido](/help/assets/animation/template-code-editor.gif){width="600"}

Il riquadro _[!UICONTROL Controlla i campi rilevati]_ si aggiorna per riflettere le modifiche apportate. Dopo aver verificato che i campi sono corretti e completi, fai clic su **[!UICONTROL Avanti]** per continuare a [caricare il modello](/help/user-guide/templates/use-templates.md#add-a-template).

## Problemi e soluzioni comuni dei modelli

| **Errore** | **Descrizione** | **Soluzione** |
|-----------------------------|---------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------|
| Impossibile analizzare | Impossibile analizzare il contenuto del modello come Handlebars valido. | Verifica la presenza di errori di sintassi HTML e Handlebars nel modello e correggili per garantire una formattazione valida per [segnaposto di contenuto](/help/user-guide/templates/customize-template.md#content-placeholders). |
| Gruppo non assegnato | Un campo immagine in un modello e-mail a più gruppi non è assegnato ad alcun gruppo. | Verificare l&#39;uso coerente dei prefissi di sezione. Ogni [sezione](/help/user-guide/templates/customize-template.md#sections-or-groups) può utilizzare solo un tipo di campo (`headline`, `body`, `image` `cta`). Assegna il campo `image` a un gruppo valido nel modello. |
| Immagine mancante | Manca un campo immagine richiesto. | Per alcuni tipi di modelli, ad esempio Meta, display o banner pubblicitario, è necessario un solo campo `image`. Aggiungi il campo `image` richiesto al tuo modello. |
| Gruppo singolo non valido | Il modello e-mail contiene esattamente un gruppo, che non è valido. | Un modello e-mail di base contiene un singolo set di elementi modello che non richiedono la convenzione di denominazione dei gruppi definita in [Sezioni o gruppi](/help/user-guide/templates/customize-template.md#sections-or-groups). Regola il modello in modo che non contenga sezioni rimuovendo qualsiasi sintassi di denominazione dei gruppi. |
| Nessun campo | Il modello non contiene campi. | Aggiungi [nomi di campo riconosciuti](/help/user-guide/templates/customize-template.md#recognized-field-names) utilizzando la sintassi Handlebars al modello in cui è necessario GenStudio for Performance Marketing per generare un determinato tipo di contenuto. |
| Proprietà richieste mancanti | Mancano alcune proprietà di metadati richieste. | Ogni tipo di modello ha requisiti e vincoli basati sulle linee guida del canale. Ad esempio, Meta richiede proporzioni e gli annunci display richiedono dimensioni. [Segui le linee guida per modelli specifici per il canale](/help/user-guide/templates/best-practices-for-templates.md#follow-channel-specific-template-guidelines). |
| Nome riservato utilizzato | È in uso un nome di campo non consentito o riservato. | Alcuni [nomi di campo](/help/user-guide/templates/customize-template.md#recognized-field-names), ad esempio `subject` o `introductory_text`, sono riservati. Rinominare i campi che utilizzano nomi riservati o non consentiti. |
| Troppi campi | Il numero di campi supera il limite globale di 20. | Rimuovi i campi non necessari per garantire che il totale non superi i 20. |
| Troppi gruppi | Il numero di gruppi supera il massimo consentito per il canale. | I modelli Meta, display e LinkedIn non consentono più sezioni. L’e-mail richiede la denominazione dei gruppi quando si definiscono due o tre sezioni. Riduci il numero di gruppi nel modello per soddisfare i requisiti del [canale](/help/user-guide/templates/best-practices-for-templates.md#follow-channel-specific-template-guidelines). |
| Campo non supportato | Il modello utilizza un campo non supportato dal canale. | Sostituisci o rimuovi i campi non supportati in base ai [nomi di campo riconosciuti](/help/user-guide/templates/customize-template.md#recognized-field-names). |
