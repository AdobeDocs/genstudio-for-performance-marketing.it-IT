---
title: Connettere un Assistente AI
description: Scopri come collegare un assistente di intelligenza artificiale supportato a [!DNL GenStudio for Performance Marketing] e verificare l'accesso agli strumenti disponibili.
role: User
source-git-commit: 6fb7ddb7549ea6bcd66b6139fbde9ebe12ddaa22
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 0%
---

# Connettere un assistente AI

Connetti un assistente di IA supportato a [!DNL GenStudio for Performance Marketing] prima di eseguire query sui dati delle prestazioni, assemblare le bozze o pubblicare annunci approvati. Le opzioni di connessione variano in base all’assistente di intelligenza artificiale e all’organizzazione.

## Prerequisiti

Prima di connetterti, verifica di disporre di:

- Un account Adobe attivo con accesso a [!DNL GenStudio for Performance Marketing].
- Piano supportato che consente connessioni MCP remote quando si utilizza Claude, ChatGPT o Microsoft Copilot. Per istruzioni specifiche sulla configurazione manuale delle connessioni MCP, consulta la documentazione dell’assistente AI.

## Connettere Adobe CX Enterprise Coworker

Gli strumenti [!DNL GenStudio for Performance Marketing] vengono gestiti come una connessione nativa in Adobe CX Enterprise Coworker. La tua organizzazione controlla la disponibilità, pertanto non inserisci l’URL diretto del server MCP.

Avvia una nuova conversazione e [verifica la connessione](#verify-the-connection). Se gli strumenti non vengono visualizzati, contatta l’amministratore della tua organizzazione o il rappresentante Adobe.

## Connect Claude

Claude richiede un piano Pro, Max, Team o Enterprise. Lo stesso connettore remoto funziona in Claude sul web e nell&#39;applicazione desktop.

1. In Claude, seleziona **[!UICONTROL Personalizza]** nella barra laterale a sinistra.
1. Seleziona **[!UICONTROL Connettori]**, quindi l&#39;icona Aggiungi.
1. Selezionare **[!UICONTROL Aggiungi connettore personalizzato]**.
1. Immettere `https://genstudio-services.adobe.io/mcp` come URL del server MCP.
1. Accedi con il tuo Adobe ID.
1. Selezionare l&#39;organizzazione IMS che ha accesso a [!DNL GenStudio for Performance Marketing].

&#x200B;> [!NOTE]
&#x200B;> In un piano Team o Enterprise, il proprietario di un&#39;organizzazione potrebbe dover aggiungere prima il connettore. Se il connettore è già disponibile, selezionare **[!UICONTROL Connetti]**.

## Connetti ChatGPT

ChatGPT richiede un account Plus, Pro, Business, Enterprise o Education. Le connessioni MCP personalizzate sono disponibili sul web in modalità sviluppatore.

1. Accedi a [ChatGPT](https://chatgpt.com) in un browser Web.
1. Apri **[!UICONTROL Impostazioni]**, quindi abilita **[!UICONTROL Modalità sviluppatore]**.
1. In **[!UICONTROL Impostazioni]**, apri l&#39;area per app o connettori.
1. Aggiungere una connessione MCP personalizzata denominata `GenStudio`.
1. Immettere `https://genstudio-services.adobe.io/mcp` come URL del server MCP.
1. Usa **[!UICONTROL OAuth]** come metodo di autenticazione.
1. Accedi con il tuo Adobe ID.
1. Selezionare l&#39;organizzazione IMS che ha accesso a [!DNL GenStudio for Performance Marketing].

&#x200B;> [!NOTE]
> ChatGPT può modificare la posizione delle impostazioni dello sviluppatore e del connettore. Se queste etichette differiscono nel tuo account, segui le istruzioni OpenAI correnti per l’aggiunta di un connettore MCP remoto.

## Connetti codice

Codex richiede l&#39;interfaccia della riga di comando Codex e un account Codex autenticato.

1. Apri `~/.codex/config.toml` per tutti i progetti o `.codex/config.toml` per un progetto.
1. Aggiungi questa configurazione:

   ```toml
   [mcp_servers.genstudio]
   url = "https://genstudio-services.adobe.io/mcp"
   auth = "oauth"
   ```

1. Esegui `codex mcp login genstudio`.
1. Accedi con il tuo Adobe ID nella finestra del browser che si apre.
1. Selezionare l&#39;organizzazione IMS che ha accesso a [!DNL GenStudio for Performance Marketing].

## Connect Writer

Writer richiede l&#39;accesso ad AI Studio.

1. In Writer, aprire **[!UICONTROL AI Studio]**.
1. Seleziona **[!UICONTROL Connettori e strumenti]**.
1. Selezionare **[!UICONTROL Crea connettore personalizzato]**.
1. Selezionare **[!UICONTROL Server MCP]** come tipo di connettore.
1. Immettere un nome e una descrizione per il connettore.
1. Immettere `https://genstudio-services.adobe.io/mcp` come URL del server MCP.
1. Imposta l&#39;accesso del team del connettore.
1. Selezionare **[!UICONTROL OAuth 2.0 (livello utente)]** come metodo di autenticazione.
1. Accedi con il tuo Adobe ID.
1. Seleziona **[!UICONTROL Salva]**.

Gli strumenti [!DNL GenStudio for Performance Marketing] vengono visualizzati nella libreria di strumenti di AI Studio. Ogni utente di Writer accede con un singolo Adobe ID.

## Connetti Copilota Microsoft

Microsoft controlla il flusso di configurazione per le connessioni MCP personalizzate in Copilot. Segui la [documentazione Microsoft Copilot](https://learn.microsoft.com/en-us/copilot/) corrente per aggiungere un server MCP remoto, quindi utilizza `https://genstudio-services.adobe.io/mcp` come URL del server.

Quando richiesto, accedi con il tuo Adobe ID e seleziona l&#39;organizzazione IMS che ha accesso a [!DNL GenStudio for Performance Marketing].

## Verificare la connessione

Dopo l&#39;installazione, verificare che gli strumenti siano disponibili.

1. Avvia una nuova conversazione nell’assistente AI.
1. Chiedi all&#39;assistente quali strumenti [!DNL GenStudio for Performance Marketing] può accedere.
1. Conferma che nella risposta siano elencati gli strumenti per Approfondimenti, Crea e Attiva.
1. Richiedi un riepilogo delle prestazioni per un canale multimediale a pagamento connesso.

L’assistente restituisce i dati sulle prestazioni disponibili o spiega perché nessun dato corrisponde alla richiesta.

&#x200B;> [!TIP]
&#x200B;> Se l’autenticazione non riesce, riconnettiti e conferma di aver selezionato l’organizzazione IMS corretta. Se non vengono visualizzati strumenti, verificare che l&#39;account disponga dell&#39;accesso a [!DNL GenStudio for Performance Marketing].

## Funzionalità correlate

- [Panoramica sugli assistenti AI](overview.md)
- [Utilizzare gli assistenti AI](use-ai-assistants.md)
- [Riferimento per gli strumenti dell’assistente AI](tools-reference.md)
