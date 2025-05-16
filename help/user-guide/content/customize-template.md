---
title: Personalizzare un modello
description: Scopri come personalizzare il modello HTML utilizzando i segnaposto di contenuto riconosciuti da Adobe GenStudio for Performance Marketing generative AI.
level: Intermediate
role: Developer
feature: Media Templates, Content Generation, Generative AI
exl-id: 292c1689-1b12-405d-951e-14ee6aebc75a
source-git-commit: 04bb7adcc9ce7eaeca2ea1f3ef39882f8e43ff6d
workflow-type: tm+mt
source-wordcount: '1480'
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

GenStudio for Performance Marketing riconosce alcuni [elementi](use-templates.md#template-elements) all&#39;interno di un modello, ma solo se li identifichi con un [nome di campo riconosciuto](#recognized-field-names).

Nell&#39;intestazione o nel corpo di un modello di HTML è possibile utilizzare la sintassi [!DNL Handlebars] per inserire un segnaposto di contenuto in cui è necessario che GenStudio for Performance Marketing compili il modello con il contenuto effettivo. GenStudio for Performance Marketing riconosce e interpreta i segnaposto di contenuto in base al [nome _campo_ riconosciuto](#recognized-field-names).

Ad esempio, è possibile utilizzare `{{headline}}` con la sintassi [!DNL Handlebars] per indicare dove deve essere posizionato il titolo dell&#39;e-mail. GenStudio riconosce questo campo, genera un titolo pertinente in base alle linee guida e ai criteri di richiesta e inserisce il titolo in questa posizione:

```handlebars
<div>{{headline}}</div>
```

### Nomi di campi riconosciuti

Nella tabella seguente sono elencati i nomi di campo riconosciuti da GenStudio for Performance Marketing per l&#39;aggiunta di un segnaposto a un modello. Aggiungere questi nomi di campo utilizzando la sintassi [!DNL Handlebars] al modello in cui è necessario GenStudio for Performance Marketing per generare un determinato tipo di contenuto.

| Campo | Ruolo | Modello canale |
| ----------------------- | ------------------------- | ------------------------------------------------ |
| `{{pre_header}}` | Preheader | email |
| `{{headline}}` | Titolo | e-mail <br>Annuncio metadati <br>Banner e annuncio visualizzazione <br>Annuncio LinkedIn |
| `{{sub_headline}}` | Sottotitolo | e-mail<br>Banner e annuncio pubblicitario |
| `{{introductory_text}}` | Testo introduttivo | Annuncio LinkedIn |
| `{{body}}` | Corpo del testo | invia un messaggio e-mail a <br>Meta ad <br>Banner e display ad |
| `{{cta}}` | Invito all&#39;azione<br>Consulta [Inviti all&#39;azione](#calls-to-action) | e-mail <br>Annuncio metadati <br>Banner e annuncio visualizzazione <br>Annuncio LinkedIn |
| `{{image}}` | Immagine—seleziona da [!DNL Content] | e-mail <br>Annuncio metadati <br>Banner e annuncio visualizzazione <br>Annuncio LinkedIn |
| `{{on_image_text}}` | Nel testo dell&#39;immagine<br>Vedere [Nel testo dell&#39;immagine](#on-image-text). | Annuncio metadati <br>Annuncio LinkedIn |
| `{{link}}` | Call to action sull&#39;immagine<br>Vedi [Collegamento sull&#39;immagine](#link-on-image). | email |

<!-- | `{{brand_logo}}`        | Logo of selected brand<br>See [Brand logo field name](#brand-logo-field-name). | email<br>Meta ad <br>LinkedIn ad | -->

GenStudio for Performance Marketing genera automaticamente alcuni campi nei seguenti modelli:

- **Il modello di posta elettronica** non richiede l&#39;identificazione del campo `subject`
- **Meta Ad Template** non richiede l&#39;identificazione dei campi `headline`, `body` e `CTA`
- **Banner e modello di annuncio visualizzato** non richiedono l&#39;identificazione del campo `CTA`
- **LinkedIn ad template** non richiede l&#39;identificazione dei campi `headline`, `introductory_text` e `CTA`

>[!WARNING]
>
>Per gli annunci Instagram, il titolo generato non viene visualizzato nell’esperienza finale.

Il caricamento di un modello in GenStudio for Performance Marketing prevede un limite di 20 campi. Poiché il campo `subject` viene generato automaticamente in un messaggio e-mail, viene conteggiato come un campo. Ciò significa che sono consentiti 19 campi in un modello e-mail.

>[!TIP]
>
>Puoi verificare il tuo modello utilizzando [anteprima modello](#template-preview) in GenStudio for Performance Marketing.

### Inviti all&#39;azione

Un invito all’azione (CTA) include una frase e un collegamento. Affinché le funzionalità _[!UICONTROL Riformula]_ e _[!UICONTROL Aggiungi collegamento]_ funzionino correttamente durante il processo di generazione delle varianti, è necessario includere segnaposto per il collegamento e la frase nel modello.

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

### Collegamento nell&#39;immagine

Puoi personalizzare il modello di e-mail per consentire ai creativi di aggiungere un collegamento a un’immagine. Come per il collegamento CTA, attenersi alla seguente guida per applicare un segnaposto `link` a un tag immagine:

```html
<a href="{{link}}"><img src="image-source.jpg" alt="{{imageDescription}}"></a>
```

In questo esempio:

- `{{link}}` è un segnaposto per l&#39;URL effettivo.
- `src="image-source.jpg"` deve essere sostituito con l&#39;URL di origine effettivo dell&#39;immagine.
- `{{imageDescription}}` è un nome di campo definito dall&#39;utente che fornisce un segnaposto per il testo alternativo dell&#39;immagine, utile per l&#39;accessibilità e la SEO.

### Testo alternativo

Utilizzare un nome di campo definito dall&#39;utente come segnaposto per generare una descrizione di testo alternativo (attributo HTML `alt="text"`) per un&#39;immagine. Il segnaposto `{{imageDescription}}` seguente viene utilizzato con il campo `{{image}}` all&#39;interno dello stesso tag `<img>`, assicurando la persistenza della relazione tra l&#39;immagine e la relativa descrizione.

```html
<img src="{{image}}" alt="{{imageDescription}}">
```

In questo esempio:

- `{{image}}` è il segnaposto per l&#39;URL di origine dell&#39;immagine.
- `{{imageDescription}}` è il segnaposto per il testo alt, che fornisce una descrizione dell&#39;immagine a scopo di accessibilità e SEO (Search Engine Optimization).

### Su testo immagine

Il segnaposto `{{on_image_text}}` viene utilizzato per specificare una sovrapposizione di testo di brevi messaggi di impatto, posizionati direttamente sull&#39;immagine in un&#39;esperienza.

```html
<div class="image-text">{{on_image_text}}</div>
```

<!-- this field does not work in Create canvas 2025/03

### Brand logo field name

At this time, you cannot select the brand logo for the template upload. The following examples demonstrate two methods that conditionally render the brand logo. Each method verifies the source, provides a default or alternative image in case the brand logo is not available, and applies a style:

**Example 1**: Using [!DNL Handlebars] Built-in Helpers condition directly in the HTML `img src` attribute:

```html
<img src="{{#if brand_logo}}{{brand_logo}}{{else}}<default-image>{{/if}}" alt="img alt text" style="max-width: 88px; margin: 10px auto; display: block;">
```

**Example 2**: Using [!DNL Handlebars] Built-in condition statement to wrap the HTML `img` tag:

```html
{{#if brand_logo}}
    <img src="{{brand_logo}}" alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
    {{else}}
    <img src="data:image/png;base64,iVBORw0KGgo..." alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
{{/if}}
```

-->

### Nomi di campi manuali

Tutti gli altri nomi di campo sono definiti dall&#39;utente e vengono trattati come campi popolati manualmente. Ad esempio, è possibile riservare una sezione per il contenuto del piè di pagina.

Per creare una sezione modificabile, aggiungere parentesi doppie attorno al nome della sezione:

```html
<tbody>
    <tr>
        <td>
            <p><span class="footer-text">{{footerLegal}}</span></p>
        </td>
    </tr>
</tbody>
```

## Sezioni o gruppi

_Sezioni_ informano GenStudio for Performance Marketing che i campi in questa sezione richiedono un elevato grado di coerenza. Stabilire questa relazione aiuta l’intelligenza artificiale a generare contenuti che corrispondono agli elementi creativi della sezione.

Utilizzare un prefisso scelto nel nome del campo per indicare che un campo fa parte di una sezione o di un gruppo. Utilizza un nome di campo (ad esempio `headline`, `body`, `image` o `cta`) dopo il carattere di sottolineatura (`_`).

- _Corretto_ (👍): `pod1_body`
- _Errato_ (❌): `pod1body`

Ogni sezione può utilizzare solo uno di ogni tipo di campo. Ad esempio, i campi seguenti appartengono alla sezione `pod1`:

- `pod1_headline`
- `pod1_body`
- `pod1_image`
- `pod1_cta`

A causa di questa regola, le sezioni non possono essere nidificate.

Ogni tipo di modello, ad esempio e-mail o annuncio Meta, ha vincoli specifici per il canale sull’utilizzo delle sezioni. Consulta [linee guida specifiche per il canale](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/content/templates/best-practices-for-templates#follow-channel-specific-template-guidelines) nell&#39;argomento _Best practice per l&#39;utilizzo dei modelli_.

Ad esempio, un modello e-mail può includere fino a tre sezioni; pertanto, puoi avere tre sezioni titolo e corpo:


- `pre_header`
- `pod1_headline`
- `pod1_body`
- `pod2_headline`
- `pod2_body`
- `pod3_headline`
- `pod3_body`
- `cta`

GenStudio for Performance Marketing è consapevole che `pod1_headline` è più strettamente correlato a `pod1_body` che a `pod2_body`.

>[!TIP]
>
>Consulta [Richieste strutturate](/help/user-guide/effective-prompts.md#structured-prompts) per scoprire come creare un prompt che generi contenuti diversi per ogni sezione in un messaggio e-mail con più sezioni.

## Anteprima modello

Quando [carichi un modello](use-templates.md#upload-a-template), GenStudio for Performance Marketing analizza il file HTML per individuare i campi riconosciuti. Utilizza l&#39;anteprima per rivedere i tuoi [elementi modello](use-templates.md#template-elements) e confermare di averli identificati correttamente con i [nomi di campo riconosciuti](#recognized-field-names).

Esempio di anteprima per un modello e-mail:

![Campi di anteprima rilevati](/help/assets/template-detected-fields.png "Controllare i campi rilevati"){zoomable="yes"}

Consulta [Editor codice modello](/help/user-guide/content/code-editor.md).

### Anteprima controllo

È possibile controllare la visibilità dei contenuti speciali utilizzando Helper incorporati (espressioni speciali nel linguaggio del modello [!DNL Handlebars] che eseguono determinate azioni). Ad esempio, puoi aggiungere un’istruzione condizionale che aggiunge parametri di tracciamento ai collegamenti nel modello esportato mantenendo puliti i collegamenti di anteprima.

Il valore `_genStudio.browser` viene impostato durante il rendering di un modello e il valore `genStudio.export` viene impostato durante l&#39;esportazione di un modello. Puoi decidere di includere un determinato contenuto nella parte superiore di un’e-mail utilizzando un wrapper condizionale, ad esempio, quando il modello viene utilizzato per l’esportazione:

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

Un altro esempio può essere quello di impedire l’utilizzo dei codici di tracciamento durante l’anteprima di un modello in GenStudio for Performance Marketing. L’esempio seguente mostra come aggiungere parametri di tracciamento ai collegamenti nel modello esportato, mantenendo allo stesso tempo puliti i collegamenti di anteprima:

```html
<a class="button" {{#if _genStudio.browser }}
   href="{{link}}"{{/if}}{{#if _genStudio.export }}
   href="{{link}}?trackingid=<%=getTrackingId()%>&mv=email"{{/if}}
   target="_blank">{{cta}}</a>
```

## Contenuto statico

I modelli e-mail e metadati spesso si collegano a immagini e file CSS ospitati su altri domini. Quando GenStudio for Performance Marketing genera le miniature per le anteprime dei modelli o le esperienze da esse derivate, convalida l’origine di contenuto e incorpora una copia a scopo di anteprima.

I file esterni vengono temporaneamente incorporati solo allo scopo di creare l’anteprima del modello, che garantisce che l’anteprima rifletta accuratamente il contenuto così come viene visualizzato al momento della creazione. Questi file esterni sono **non** archiviati in modo permanente in GenStudio for Performance Marketing. Dopo la creazione dell’anteprima del modello, GenStudio for Performance Marketing continua a fare riferimento al collegamento di origine originale fornito nel modello.

### Aggiorna contenuto

Se l&#39;origine cambia dopo la creazione dell&#39;anteprima iniziale, utilizzare la funzione [aggiorna](/help/user-guide/content/use-templates.md#refresh-template) per aggiornare l&#39;anteprima del modello con la versione più recente del contenuto proveniente da origini esterne.

## Esempi di modelli

+++Esempio: modello e-mail con una sezione

Di seguito è riportato un esempio di base di un modello HTML per un messaggio e-mail che contiene una sezione. L’intestazione contiene CSS semplice e in linea per lo stile. Il corpo contiene `pre_header`, `headline` e `image` [segnaposto](#content-placeholders) per l&#39;inserimento di contenuto da parte di GenStudio for Performance Marketing durante il processo di generazione dell&#39;e-mail.

```html {line-numbers="true" highlight="13"}
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
    <body>{{pre_header}}
        <div class="container">
            <h1>{{headline}}</h1>
            <p><a href="{{link}}">
            <img alt="{{headline}}"
                    src="{{image}}"
                    width="600" height="600"
                    border="0"/></a></p>
            <p>{{body}}</p>
        </div>
    </body>
</html>
```

+++

+++Esempio: modello e-mail con più sezioni

Di seguito è riportato lo stesso modello di HTML nell’esempio precedente, ma con altre due sezioni. L’intestazione contiene CSS in linea per la formattazione di un gruppo. Il corpo utilizza due gruppi con [segnaposto contenuto](#content-placeholders) utilizzando un prefisso.

```html
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
    <body>{{pre_header}}
        <div class="container">
            <h1>{{headline}}</h1>
            <p>{{body}}</p>
            <!-- Pod1 -->
            <div class="pod">
                <h2>{{pod1_headline}}</h2>
                <p><img alt="{{ headline }}" src="{{pod1_image}}" width="200" height="200" border="0"></p>
                <p>{{pod1_body}}</p>
            </div>
            <!-- End of Pod1 -->
            <!-- Pod2 -->
            <div class="pod">
                <h2>{{pod2_headline}}</h2>
                <p><img alt="{{headline}}" src="{{pod2_image}}" width="200" height="200" border="0"></p>
                <p>{{pod2_body}}</p>
            </div>
            <!-- End of Pod2 -->
        </div>
    </body>
</html>
```

+++

+++Esempio: Meta ad template

Di seguito è riportato un esempio di base di un modello di annunci Meta. L’intestazione contiene CSS in linea per lo stile. Il corpo utilizza [segnaposto contenuto](#content-placeholders), ad esempio `image` e `on_image_text`, per indicare dove GenStudio for Performance Marketing può generare il contenuto.

```html {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title>Adobe</title>
        <style>
            .ad-container {
            font-family: Helvetica, sans-serif;
            position: relative;
            text-align: center;
            height: 100%;
            }
            .ad-image {
            width: 100%;
            height: 100%;
            object-fit: cover;
            }
            .ad-text {
            position: absolute;
            top: 0;
            left: 0;
            margin: 1em;
            background-color: rgba(0, 0, 0, 0.5);
            color: white;
            padding: 1em;
            font-size: 75px;
            }
        </style>
    </head>
    <body>
        <div class="ad-container">
            <img src="{{image}}" alt="Ad Image" class="ad-image" />
            <div class="ad-text">{{on_image_text}}</div>
        </div>
    </body>
</html>
```

+++
