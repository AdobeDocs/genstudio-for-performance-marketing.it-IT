---
title: Linee guida per i modelli e-mail
description: Segui le best practice quando utilizzi modelli e-mail con Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 8b1e8d32-5a23-45ce-a2d4-ae6de3698c45
source-git-commit: d9d774f727b69b18af6114965fdb8ffb450f797b
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Linee guida per i modelli e-mail

Un modello e-mail di marketing funge da base per campagne e-mail visivamente coinvolgenti e reattive. In generale, i modelli di HTML consentono di controllare il layout, la composizione tipografica, i colori e le immagini in modo da allinearli alle linee guida del marchio. Durante la preparazione del modello per l’utilizzo in GenStudio for Performance Marketing, utilizza HTML semantico e CSS in linea per lo stile ed evita script o dipendenze esterne. Modelli HTML ben strutturati possono migliorare l’esperienza del destinatario e i tassi di consegna e coinvolgimento.

Segui queste best practice per la progettazione quando personalizzi i modelli e-mail per l’utilizzo con GenStudio for Performance Marketing:

- Utilizzare i caratteri Adobe o Google
- Utilizzare HTML e CSS in linea puliti e reattivi
- **non** utilizza JavaScript
- **not** utilizza la larghezza fissa nel corpo o nel contenitore
- **not** utilizza la codifica base64 per le immagini perché può aumentare notevolmente le dimensioni del modello
- La dimensione massima del file HTML è 102 KB

## Nomi di campi riconosciuti

GenStudio for Performance Marketing genera automaticamente il campo `subject` per le e-mail. Quando personalizzi il modello, utilizza segnaposto di contenuto per i seguenti campi obbligatori:

- `pre_header` (Rich Text non abilitato)
- `headline`
- `sub_headline`
- `body`
- `cta`
- `image` (selezionato da Content JPEG, PNG o GIF)

Il numero massimo di campi consentiti in un modello è 20. Consulta [Segnaposto di contenuto](/help/user-guide/content/customize-template.md#content-placeholders) per ulteriori informazioni sull&#39;utilizzo dei nomi dei campi nei modelli.

## E-mail con più sezioni

_Le sezioni_ consentono di organizzare il contenuto in gruppi distinti, che supportano layout più complessi. In Genstudio per Performance Marketing, puoi definire ogni sezione utilizzando una convenzione di denominazione del gruppo. Consulta [Personalizzare le sezioni del modello](/help/user-guide/content/customize-template.md#sections-or-groups).

I modelli con più sezioni possono avere 0, 2 o 3 sezioni:

- Un modello di base (zero sezioni) può generare un singolo set di elementi modello, che non richiede la convenzione di denominazione del gruppo.
- Un modello complesso (più sezioni) può generare fino a tre set di elementi modello, che richiedono l&#39;adesione alla convenzione di denominazione del gruppo: (`groupname_fieldname`)

Esempi di nomi dei campi per due sezioni:

- `pod1_headline`, `pod1_body`, `pod1_cta`
- `pod2_headline`, `pod2_body`, `pod2_cta`

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
