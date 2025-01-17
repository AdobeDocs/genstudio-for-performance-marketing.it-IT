---
title: Personalizzare un modello
description: Scopri come personalizzare e ottimizzare il modello per Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Templates, Content
exl-id: 292c1689-1b12-405d-951e-14ee6aebc75a
source-git-commit: 229d16019d71b8228acf16e651885ce8c6d325e5
workflow-type: tm+mt
source-wordcount: '1280'
ht-degree: 0%

---

# Personalizzare un modello

Puoi personalizzare un modello da utilizzare in GenStudio for Performance Marketing inserendo segnaposto di contenuto, o campi, utilizzati dall’IA generativa per inserire il contenuto.

Nelle sezioni successive viene illustrato come adattare i modelli di HTML per GenStudio for Performance Marketing utilizzando il linguaggio di modelli _[!DNL Handlebars]_. La sintassi [!DNL Handlebars] utilizza testo normale con doppie parentesi graffe come segnaposto di contenuto. Per informazioni su come preparare il modello, consulta [Informazioni [!DNL Handlebars]](https://handlebarsjs.com/guide/#what-is-handlebars) nella_ Guida lingua Handlebars _.


Quando il modello è pronto, puoi [caricarlo in GenStudio for Performance Marketing](use-templates.md#upload-a-template) e iniziare a generare e-mail personalizzate in base al modello personalizzato.

>[!TIP]
>
>Segui le [linee guida per l&#39;accessibilità](accessibility-for-templates.md) e le [best practice](/help/user-guide/content/best-practices-for-templates.md) in modo da poter raggiungere più destinatari e fornire un&#39;esperienza ottimale.

## Segnaposto di contenuto

GenStudio for Performance Marketing riconosce alcuni [elementi](use-templates.md#template-elements) all&#39;interno di un modello, ma solo se li identifichi con un nome di campo riconosciuto.

All&#39;interno dell&#39;intestazione o del corpo di un modello, è possibile utilizzare la sintassi [!DNL Handlebars] come segnaposto di contenuto in cui è necessario che GenStudio for Performance Marketing compili il modello con il contenuto effettivo. GenStudio for Performance Marketing riconosce e interpreta i segnaposto di contenuto in base al [nome _campo_ riconosciuto](#recognized-field-names).

Ad esempio, è possibile utilizzare `{{ headline }}` con la sintassi [!DNL Handlebars] per indicare dove deve essere posizionato il titolo dell&#39;e-mail:

```handlebars
<div>{{headline}}</div>
```

### Nomi di campi riconosciuti

Nella tabella seguente sono elencati i nomi dei campi riconosciuti da GenStudio for Performance Marketing per il popolamento in modelli. Aggiungere questi nomi di campo utilizzando la sintassi [!DNL Handlebars] al modello in cui è necessario GenStudio for Performance Marketing per generare il contenuto.

| Campo | Ruolo | Modello canale |
| ------------------ | ---------------------- | -------------------------------- |
| `{{pre_header}}` | Pre header | email |
| `{{headline}}` | Titolo | invia e-mail a <br>Meta ad <br>Visualizza annuncio |
| `{{body}}` | Corpo del testo | invia e-mail a <br>Meta ad <br>Visualizza annuncio |
| `{{cta}}` | Invito all’azione | invia e-mail a <br>Meta ad <br>Visualizza annuncio |
| `{{on_image_text}}` | Su testo immagine | Meta annuncio |
| `{{image}}` | Immagine: seleziona dal contenuto | invia e-mail a <br>Meta ad <br>Visualizza annuncio |
| `{{brand_logo}}` | Logo del marchio selezionato<br>Per informazioni sull&#39;utilizzo consigliato, vedere [Nome campo logo marchio](#brand-logo-field-name). | e-mail<br>Meta annuncio |

GenStudio for Performance Marketing compila automaticamente alcuni campi nei seguenti modelli:

- **Il modello di posta elettronica** non richiede l&#39;identificazione del campo `subject`
- **Il modello di annunci multimediali** non richiede l&#39;identificazione dei campi `headline`, `body` e `CTA`
- **Il modello Annunci visualizzati** non richiede l&#39;identificazione del campo `CTA`

>[!WARNING]
>
>Per gli annunci Instagram, il titolo generato non viene visualizzato nell’esperienza finale.

Il caricamento di un modello in GenStudio for Performance Marketing prevede un limite di 20 campi. Poiché il campo `subject` viene generato automaticamente in un messaggio e-mail, viene conteggiato come un campo. Ciò significa che sono consentiti 19 campi in un modello e-mail.

>[!TIP]
>
>Puoi verificare il tuo modello utilizzando [anteprima modello](#template-preview) in GenStudio for Performance Marketing.

#### Nome campo logo marchio

Al momento, non è possibile selezionare il logo del brand per il caricamento del modello. Gli esempi seguenti illustrano due metodi che eseguono il rendering del logo del brand in modo condizionale. Ogni metodo verifica l’origine, fornisce un’immagine predefinita o alternativa nel caso in cui il logo del brand non sia disponibile e applica uno stile:

**Esempio 1**: utilizzo della condizione Helper incorporati [!DNL Handlebars] direttamente nell&#39;attributo HTML `img src`:

```html
<img src="{{#if brand_logo}}{{brand_logo}}{{else}}<default-image>{{/if}}" alt="img alt text" style="max-width: 88px; margin: 10px auto; display: block;">
```

**Esempio 2**: utilizzo dell&#39;istruzione di condizione incorporata [!DNL Handlebars] per racchiudere il tag HTML `img`:

```handlebars
{{#if brand_logo}}
    <img src="{{brand_logo}}" alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
    {{else}}
    <img src="data:image/png;base64,iVBORw0KGgo..." alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
{{/if}}
```

#### Nomi di campi manuali

Tutti gli altri nomi di campo vengono trattati come campi popolati manualmente.

Per creare una sezione modificabile, aggiungere parentesi doppie attorno al nome della sezione:

```handlebars
{{customVariable}}
```

### Sezioni o gruppi

_Sezioni_ informano GenStudio for Performance Marketing che i campi in questa sezione richiedono un elevato grado di coerenza. Stabilire questa relazione aiuta l’intelligenza artificiale a generare contenuti che corrispondono agli elementi creativi della sezione.

Utilizzare un prefisso scelto nel nome del campo per indicare che un campo fa parte di una sezione o di un gruppo. Utilizzare un nome di campo (`headline`, `body`, `image` o `cta`) dopo il carattere di sottolineatura (`_`). Ad esempio, il titolo e il corpo seguenti appartengono alla sezione `pod1`:

- `pod1_headline`
- `pod1_body`

Ogni sezione può utilizzare solo uno di ogni tipo di campo. Nell&#39;esempio precedente, la sezione `pod1` può utilizzare un solo campo `pod1_headline`. A causa di questa regola, le sezioni non possono essere nidificate.

Ogni tipo di modello, ad esempio e-mail o annuncio Meta, ha vincoli specifici per il canale sull’utilizzo delle sezioni. Consulta [linee guida specifiche per il canale](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/content/templates/best-practices-for-templates#follow-channel-specific-template-guidelines) nell&#39;argomento _Best practice per l&#39;utilizzo dei modelli_.

Ad esempio, un modello e-mail può includere fino a tre sezioni; pertanto, puoi avere tre sezioni titolo e corpo:

- `pre-header`
- `pod1_headline`
- `pod1_body`
- `pod2_headline`
- `pod2_body`
- `pod3_headline`
- `pod3_body`
- `cta`

GenStudio for Performance Marketing è consapevole che `pod1_headline` è più strettamente correlato a `pod1_body` che a `pod2_body`.

Consulta [Richieste strutturate](/help/user-guide/effective-prompts.md#structured-prompts) per scoprire come creare un prompt che generi contenuti diversi per ogni sezione di un&#39;e-mail.

### Inviti all&#39;azione

Un invito all’azione (CTA) include una frase e un collegamento. Affinché le funzionalità _[!UICONTROL Riformula]_ e _[!UICONTROL Aggiungi collegamento]_ di CTA funzionino correttamente durante il processo di generazione delle varianti, è necessario includere segnaposto per il collegamento e la frase nel modello.

Per impostare i segnaposto di CTA, attenersi alle istruzioni riportate di seguito.

- È disponibile la riformulazione di CTA e il collegamento è modificabile

  ```html
  <a class="button" href="{{pod1_link}}" >{{cta}}</a>
  ```

- La rifrase CTA è disponibile, ma il collegamento è **non** modificabile perché il collegamento effettivo è fornito nel modello

  ```html
  <a align="center" href="https://link">{{cta}}</a>
  ```

- Il collegamento CTA è modificabile, ma la rifrase è **non** disponibile perché la frase è fornita nel modello

  ```html
  <a class="button" href="{{pod1_link}}" >Register now</a>
  ```

GenStudio for Performance Marketing può fornire anche frasi di invito all’azione varianti. Vedi [Rivedi invito all&#39;azione](/help/user-guide/create/manage-variants.md#revise-call-to-action).

## Anteprima modello

Quando [carichi un modello](use-templates.md#upload-a-template), GenStudio for Performance Marketing analizza il file HTML per individuare i campi riconosciuti. Utilizza l&#39;anteprima per rivedere i tuoi [elementi modello](use-templates.md#template-elements) e confermare di averli identificati correttamente con i [nomi di campo riconosciuti](#recognized-field-names).

Esempio di anteprima per un modello e-mail:

![Rilevati campi di anteprima](/help/assets/template-detected-fields.png){width="650"}

### Anteprima controllo

È possibile controllare la visibilità dei contenuti speciali utilizzando Helper incorporati (espressioni speciali nel linguaggio del modello [!DNL Handlebars] che eseguono determinate azioni). Ad esempio, puoi aggiungere un’istruzione condizionale che aggiunge parametri di tracciamento ai collegamenti nel modello esportato mantenendo puliti i collegamenti di anteprima.

Il valore `_genStudio.browser` viene impostato durante il rendering di un modello e il valore `genStudio.export` viene impostato durante l&#39;esportazione di un modello. Puoi decidere di includere un determinato contenuto nella parte superiore di un’e-mail utilizzando un wrapper condizionale, ad esempio, quando il modello viene utilizzato per l’esportazione:

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

Un altro esempio può essere quello di impedire l’utilizzo dei codici di tracciamento durante l’anteprima di un modello in GenStudio for Performance Marketing. L’esempio seguente mostra come aggiungere parametri di tracciamento ai collegamenti nel modello esportato, mantenendo allo stesso tempo puliti i collegamenti di anteprima:

```handlebars
<a class="button" {{#if _genStudio.browser }}
   href="{{ link }}"{{/if}}{{#if _genStudio.export }}
   href="{{ link }}?trackingid=<%=getTrackingId()%>&mv=email"{{/if}}
   target="_blank">{{ cta }}</a>
```

## Contenuto statico

I modelli e-mail e metadati spesso si collegano a immagini e file CSS ospitati al di fuori di GenStudio for Performance Marketing. Quando GenStudio for Performance Marketing genera le miniature per questi modelli o le esperienze da essi derivate, queste risorse esterne possono essere ignorate se non dispongono delle intestazioni CORS (Cross-Origin Resource Sharing) corrette.

Per garantire che queste risorse siano disponibili durante il processo di generazione delle miniature, considera due opzioni:

1. **Usa intestazioni CORS**: il server host deve inviare risposte con un&#39;intestazione `Access-Control-Allow-Origin` impostata sul valore `https://experience.adobe.com` per gli ambienti di produzione. Questo metodo consente a GenStudio for Performance Marketing di accedere alle risorse e di includerle.

1. **Usa URL dati**: incorpora le risorse esterne direttamente nel modello utilizzando URL dati. Questo metodo bypassa le restrizioni CORS e garantisce che le risorse siano disponibili durante la generazione delle miniature.

>[!TIP]
>
>Utilizza [aggiorna](/help/user-guide/content/use-templates.md#refresh-template) per aggiornare l&#39;anteprima del modello con il contenuto statico più recente.

## Esempi di modelli

+++Esempio: modello e-mail con una sezione

Di seguito è riportato un esempio di base di un modello HTML per un messaggio e-mail che contiene una sezione. L’intestazione contiene CSS semplice e in linea per lo stile. Il corpo contiene `pre-header`, `headline` e `image` [segnaposto](#content-placeholders) per l&#39;inserimento di contenuto da parte di GenStudio for Performance Marketing durante il processo di generazione dell&#39;e-mail.

```handlebars {line-numbers="true" highlight="13"}
<!DOCTYPE html>
<html>
<head>
    <title>Adobe</title>
    <style>
        .container {
            width: 100%;
            padding: 20px;
            font-family: Arial, sans-serif;
        }
    </style>
</head>
<body>{{ pre_header }}
    <div class="container">
        <h1>{{ headline }}</h1>
        <p><img alt="{{ headline }}"
                src="{{ image }}"
                width="600" height="600"
                border="0"/></p>
        <p>{{ body }}</p>
    </div>
</body>
</html>
```

+++

+++Esempio: modello e-mail con più sezioni

Di seguito è riportato lo stesso modello di HTML nell&#39;esempio precedente, ma con altre due sezioni. L’intestazione contiene CSS in linea per la formattazione di un gruppo. Il corpo utilizza due gruppi con [segnaposto contenuto](#content-placeholders) utilizzando un prefisso.

```handlebars {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
<head>
    <title>Adobe</title>
    <style>
        .container {
            width: 100%;
            padding: 20px;
            font-family: Arial, sans-serif;
        }
        .pod {
            background-color: #f8f8f8;
            margin: 10px;
            padding: 20px;
            border-radius: 5px;
        }
        .pod h2 {
            color: #333;
        }
        .pod p {
            color: #666;
        }
    </style>
</head>
<body>{{ pre_header }}
    <div class="container">
        <h1>{{ headline }}</h1>
        <p><img alt="{{ headline }}"
                src="{{ image }}"
                width="600" height="600"
                border="0"/></p>
        <p>{{ body }}</p>
    <!-- Pod1 -->
        <div class="pod">
            <h2>{{ pod1_header }}</h2>
            <p>{{ pod1_body }}</p>
        </div>
        <!-- End of Pod1 -->
    <!-- Pod2 -->
        <div class="pod">
            <h2>{{ pod2_header }}</h2>
            <p>{{ pod2_body }}</p>
        </div>
        <!-- End of Pod2 -->
    </div>
</body>
</html>
```

+++

+++Esempio: Meta ad template

Di seguito è riportato un esempio di base di un modello di annunci Meta. L’intestazione contiene CSS in linea per lo stile. Il corpo utilizza [segnaposto contenuto](#content-placeholders) utilizzando un prefisso.

```handlebars {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Adobe</title>
    <style>
        .ad-container {
            width: 300px;
            border: 1px solid #ddd;
            padding: 16px;
            font-family: Arial, sans-serif;
        }
        .ad-image {
            width: 100%;
            height: auto;
        }
        .ad-headline {
            font-size: 18px;
            font-weight: bold;
            margin: 12px 0;
        }
        .ad-body {
            font-size: 14px;
            margin: 12px 0;
        }
        .ad-cta {
            display: inline-block;
            padding: 10px 20px;
            background-color: #007bff;
            color: #fff;
            text-decoration: none;
            border-radius: 4px;
            text-align: center;
        }
    </style>
</head>
<body>
<div class="ad-container">
    <img src="{{ image }}" alt="Ad Image" class="ad-image">
    <div class="ad-headline">"{{ headline }}"</div>
    <div class="ad-body">"{{ body }}"</div>
    <a href="(https://example.com)" class="ad-cta">"{{ CTA }}"</a>
</div>
</body>
</html>
```

+++
