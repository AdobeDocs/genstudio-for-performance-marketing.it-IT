---
title: Scrivi i Prompt Effettivi
description: Scopri come scrivere prompt efficaci per Adobe GenStudio for Performance Marketing.
role: User
level: Beginner
feature: Create Prompt, Generative AI
exl-id: 0cd4db4f-d031-4c1f-a4e7-adc220f947fc
source-git-commit: 72cd93d9d6fdd99d5a524d05cba923e9c0191960
workflow-type: tm+mt
source-wordcount: '752'
ht-degree: 2%

---

# Scrivi prompt effettivi

La comunicazione con l’intelligenza artificiale generativa è essenziale per lavorare in modo efficace in Adobe GenStudio for Performance Marketing.

GenStudio for Performance Marketing fornisce un prompt di IA generativo ogni volta che è possibile modificare una risorsa. I componenti di un prompt efficace devono includere un linguaggio descrittivo, esempi e informazioni non fornite dalle linee guida configurate.

Come best practice, fornisci a GenStudio for Performance Marketing le tue informazioni sul brand utilizzando [linee guida](/help/user-guide/guidelines/overview.md), quindi puoi sfruttare appieno l’intelligenza artificiale generativa per produrre esperienze di contenuti allineati al brand.

## Lingua descrittiva

Puoi usare il linguaggio naturale per articolare le tue idee e creare esperienze. Il prompt guida l’intelligenza artificiale nella generazione di contenuti di canale personalizzati e immagini complementari alla tua visione. Maggiore è il numero di dettagli forniti, maggiori sono le possibilità di produrre un&#39;immagine o un&#39;esperienza che soddisfi le tue esigenze. Utilizza un linguaggio chiaro e descrittivo per fornire il maggior numero di dettagli possibile:

- Per **immagini**, utilizza parole che descrivono atmosfera, umore, colore, composizione e stile.
- Per **copia**, utilizza parole che descrivono il pubblico, lo scopo, le descrizioni delle nuove funzionalità, gli esempi e le azioni.

Di seguito è riportato un prompt di esempio che articola le informazioni relative all’intento, al pubblico di destinazione e allo stile.

```bash
Write an email to motivate infrequent users of Photoshop to follow an in-app tutorial that teaches them to combine elements of two photos into a beautiful work of art. Highlight the generative AI capabilities of Photoshop and use references to natural imagery.
```

+++Vedi i risultati di esempio

![tre e-mail generate](/help/assets/sample-email.png)

+++

## Criteri di richiesta

In GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md), è possibile utilizzare **[!UICONTROL Criteri prompt]** ([_Parametri_](/help/user-guide/create/overview.md#parameters) e un prompt) nel cassetto dei prompt per aggiungere dettagli tramite la selezione per migliorare l&#39;interpretazione di IA.

Per [e-mail](/help/user-guide/create/email-experiences.md), i criteri di richiesta potrebbero includere l&#39;aggiunta di [linee guida](/help/user-guide/guidelines/overview.md) in _Parametri_, il caricamento di una risorsa da utilizzare nelle varianti di e-mail e un prompt descrittivo. Per un [annuncio Meta](/help/user-guide/create/create-meta-ad.md), i criteri di richiesta potrebbero includere una linea guida del brand in _Parametri_, la selezione o il caricamento di una risorsa esistente, impostazioni relative a immagini o risorse, ad esempio proporzioni, e un prompt. La potenza effettiva inizia con [le linee guida per la configurazione](/help/user-guide/guidelines/add-guidelines.md).

>[!NOTE]
>
>Se le linee guida vengono aggiunte in _Parametri_ nel cassetto dei prompt, non è necessario includervi un riferimento. GenStudio for Performance Marketing sfrutta questi elementi [!DNL Brands], [!DNL Products] e [!DNL Personas] nella generazione dei contenuti.

### Linee guida

Le linee guida di GenStudio for Performance Marketing aiutano l’intelligenza artificiale generativa a personalizzare la composizione delle risorse. Quando viene visualizzato un criterio di richiesta, è possibile scegliere [[!DNL Brand]](/help/user-guide/guidelines/brands.md), [[!DNL Persona]](/help/user-guide/guidelines/personas.md) e [[!DNL Product]](/help/user-guide/guidelines/products.md) dalle linee guida configurate.

>[!TIP]
>
>Puoi controllare come e quando GenStudio for Performance Marketing utilizza le linee guida di [!DNL Brand]. Consulta [Linee guida](/help/user-guide/guidelines/overview.md) per scoprire come configurare e gestire le linee guida per il brand.

### Richieste strutturate

Per le e-mail con più sezioni, puoi strutturare i prompt per fornire istruzioni specifiche per ogni sezione in modo da generare contenuti diversi per ogni sezione di un’e-mail. I prompt strutturati devono fare riferimento direttamente a [nomi di sezione nel modello e-mail](/help/user-guide/content/customize-template.md#sections-or-groups), in modo che il contenuto generato possa essere inserito nei segnaposto di contenuto corrispondenti.

Ad esempio, puoi dare istruzioni a GenStudio for Performance Marketing per generare contenuti per un’e-mail che promuove un nuovo prodotto nella prima sezione e che descrive i vantaggi di un risparmio sui costi nella seconda sezione.

Il prompt strutturato deve:

- Utilizza uno dei seguenti riferimenti al nome della sezione nel modello e-mail:
   - Pod
   - Gruppo
   - Sezione
   - Modulo

  Ad esempio, se il modello utilizza `moduleA` o `Group-3` come nome di sezione, è possibile fare riferimento a tali nomi di sezione nel prompt.

- Segui le regole/struttura consigliata. Se la struttura dei prompt non rispetta il formato specificato, il prompt si applica a *tutte* le sezioni e-mail e facilita comunque la generazione del contenuto.
- Utilizza i nomi delle sezioni definiti nel modello e-mail. I riferimenti dei prompt devono corrispondere ai nomi di sezione codificati nel modello e-mail.
- Non fare distinzione tra maiuscole e minuscole. Ad esempio, puoi utilizzare `Pod` o `pod` nel modello di e-mail e nel prompt strutturato.
- Fare riferimento prima al prompt utente generico e quindi alle direttive specifiche della sezione.
- Utilizzare due punti, un trattino, una virgola o un&#39;altra delimitazione (`,:;#$!~|@=-%&*^_`) come separazione tra il riferimento al nome della sezione e la direttiva. Ad esempio, è possibile utilizzare quanto segue come direttiva di richiesta specifica della sezione: `Pod1; Describe how to easily edit text and swap images.`

Di seguito è riportato un prompt di esempio che articola la struttura di prompt consigliata e sfrutta un modello di posta elettronica che utilizza il termine di identificazione `Pod` come in `Pod1`, `Pod2` e `Pod3`.

```properties
Create an exciting multi-pod email focusing on Creative Cloud and its powerful generative AI capabilities.

Encourage customers to convert to Photoshop or use a free Photoshop trial. We want to better educate them about app features.

Pod1: Focus on Adobe Photoshop and its new generative AI tools that enable creators to bring images to life in minutes.

Pod2: Focus on Adobe Illustrator and its new generative AI tools, such as Generative Shape Fill, which allows you to quickly fill your vector outline and explore a variety of options that match the look and feel of your own artwork.

Pod3: Focus on Adobe Acrobat Pro. Make users aware that with Acrobat Pro they can edit images and text inside a PDF.
```

Consulta [best practice per l&#39;utilizzo dei modelli](/help/user-guide/content/best-practices-for-templates.md).

## Riprova

La richiesta è un processo iterativo. Se i risultati non soddisfano le aspettative, rivedere la richiesta e apportare alcune modifiche o aggiungere ulteriori dettagli. In alternativa, puoi incollare le sezioni da una descrizione della campagna. Puoi anche richiedere che GenStudio for Performance Marketing eviti determinate parole, elementi o temi.

## Best practice

Alcune semplici best practice per creare prompt efficaci:

- Sii specifico e fornisci dettagli su cosa fare e non fare.
- Fornisci contesto utilizzando riferimenti esterni.
- Utilizzare le linee guida di GenStudio for Performance Marketing.
- Rivedi e adegua regolarmente le linee guida.
- Iterare e perfezionare.
- Imparare attraverso la sperimentazione.

{{in-academy}}
