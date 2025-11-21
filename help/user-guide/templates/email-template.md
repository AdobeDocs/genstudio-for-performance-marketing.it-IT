---
title: Linee guida per i modelli e-mail
description: Segui le best practice quando utilizzi modelli e-mail con Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 8b1e8d32-5a23-45ce-a2d4-ae6de3698c45
source-git-commit: 3251d81a6bfb0c1f7d2bf3c5bd319ad4e2237699
workflow-type: tm+mt
source-wordcount: '441'
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

Quando personalizzi il modello e-mail, utilizza segnaposto di contenuto per i seguenti campi obbligatori:

- `headline`
- `sub_headline`
- `body`
- `cta`
- `image` (selezionato da Content JPEG, PNG o GIF)

GenStudio for Performance Marketing genera automaticamente i campi seguenti. Rich text non abilitato. Non è necessario applicare segnaposto di contenuto per:

- `pre_header`
- `subject`

Il numero massimo di campi consentiti in un modello è 20. Consulta [Segnaposto di contenuto](/help/user-guide/templates/customize-template.md#content-placeholders) per ulteriori informazioni sull&#39;utilizzo dei nomi dei campi nei modelli.

## E-mail con più sezioni

_Sezioni_ ti consentono di organizzare il contenuto in gruppi distinti, supportando layout più complessi. In GenStudio for Performance Marketing, puoi definire ogni sezione utilizzando una convenzione di denominazione dei gruppi. Consulta [Personalizzare le sezioni del modello](/help/user-guide/templates/customize-template.md#sections-or-groups).

I modelli con più sezioni possono avere 0, 2 o 3 sezioni:

- Un modello di base (zero sezioni) può generare un singolo set di elementi modello, che non richiede la convenzione di denominazione del gruppo.
- Un modello complesso (più sezioni) può generare fino a tre set di elementi di modello, che richiedono di rispettare la convenzione di denominazione del gruppo: `<groupname_fieldname>`.
- Quando si utilizzano più sezioni, tutti gli elementi lasciati autonomi al di fuori di una sezione non vengono compilati.

Di seguito sono riportati alcuni esempi di nomi di campo, utilizzando la convenzione di denominazione dei gruppi, per due sezioni:

- Nella sezione 1:`pod1_headline`, `pod1_body`, `pod1_cta`
- Nella sezione 2:`pod2_headline`, `pod2_body`, `pod2_cta`

## Esempi di modelli

+++Esempio: modello e-mail con una sezione

Di seguito è riportato un esempio di base di un modello e-mail di HTML con una sezione. `<head>` include CSS in linea semplice per lo stile e `<body>` utilizza segnaposto di contenuto come `pre_header`, `headline`, `sub_headline`, `body`, `cta` e `image` con collegamento e. Questi segnaposto consentono a GenStudio for Performance Marketing di inserire contenuto dinamico durante la generazione dell’e-mail.

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Marketing Email</title>
        <style>
            .container {
                width: 100%;
                padding: 20px;
                font-family: Arial, sans-serif;
            }
            .cta-button {
                display: inline-block;
                background-color: #fff;
                color: #000;
                border: 2px solid #000;
                padding: 10px 20px;
                text-decoration: none;
                font-family: 'Source Sans Pro', Arial, sans-serif;
                font-weight: 600;
                font-size: 14px;
                margin-top: 20px;
                text-align: center;
            }
        </style>
    </head>
    <body>
        <div class="container">
            {{pre_header}}
            <h1>{{headline}}</h1>
            <p>
                <a href="{{link}}">
                    <img alt="banner headline" src="{{image}}" width="600" height="600">
                </a>
            </p>
            <h2>{{sub_headline}}</h2>
            <p>{{body}}</p>
            <a href="#" class="cta-button">{{cta}}</a>
        </div>
    </body>
</html>
```

+++

+++Esempio: modello e-mail con più sezioni

Questo è lo stesso modello di HTML nell’esempio precedente, ma con altre due sezioni. L’intestazione contiene CSS in linea per la formattazione di un gruppo. Il corpo utilizza due gruppi con [segnaposto contenuto](#content-placeholders) utilizzando un prefisso.

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
            .cta-button {
            display: inline-block;
            background-color: #fff; /* Background color to white */
            color: #000; /* Text color to black */
            border: 2px solid #000; /* Border color to black */
            padding: 10px 20px;
            text-decoration: none;            
            font-family: 'Source Sans Pro', Arial, sans-serif;
            font-weight: 600; /* Semibold */
            font-size: 14px;
            margin-top: 20px;
            text-align: center;
            }
        </style>
    </head>
    <body>{{pre_header}}
        <div class="container">
            <!-- Pod1 -->
            <div class="pod">
                <h2>{{pod1_headline}}</h2>
                <p><img alt="pic1" src="{{pod1_image}}" width="200" height="200" border="0"></p>
                <p>{{pod1_body}}</p>
            </div>
            <!-- End of Pod1 -->
            <!-- Pod2 -->
            <div class="pod">
                <h2>{{pod2_headline}}</h2>
                <p><img alt="pic2" src="{{pod2_image}}" width="200" height="200" border="0"></p>
                <p>{{pod2_body}}</p>
            </div>
            <!-- End of Pod2 -->
            <a href="#" class="cta-button">{{cta}}</a>
        </div>
    </body>
</html>
```

+++
