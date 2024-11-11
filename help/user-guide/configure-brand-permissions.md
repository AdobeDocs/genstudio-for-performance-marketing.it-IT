---
title: Assegna  [!DNL Brand]  autorizzazioni
description: Informazioni sull'assegnazione di diritti per i creatori e gli editor di GenStudio for Performance Marketing [!DNL Brand] .
level: Intermediate
feature: Brands Service, Generative AI
source-git-commit: 3c391753ebd0d19ad7dcb17870915eeccc55cc05
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 1%

---

# Assegna autorizzazioni [!DNL Brand]

Per impostazione predefinita, i responsabili di sistema di GenStudio possono creare e modificare [!DNL Brands]. I ruoli editor contenuti e collaboratore dispongono delle autorizzazioni di modifica e creazione, ma non possono richiedere alcun diritto di gestione del sistema. Per concedere agli editor di contenuti e ai collaboratori questi diritti relativi a [!DNL Brand], un amministratore di Adobe deve eseguire alcune attività di configurazione aggiuntive in Adobe Admin Console. Consulta [Adobe Admin Console](https://helpx.adobe.com/enterprise/using/admin-console.html#Overview) nella _guida all&#39;amministrazione di Enterprise e Teams_.

L’aggiunta di utenti e gruppi di utenti sono attività di base comuni a tutti i prodotti Adobe con diritti gestiti tramite l’Admin Console. Per una panoramica sulla gestione degli utenti e sulle procedure per l&#39;aggiunta di utenti e gruppi di utenti, vedere [Utenti Adobe Admin Console](https://helpx.adobe.com/it/enterprise/using/users.html) nella _guida per l&#39;amministrazione di Enterprise e Team_.

## Passaggio 1: creare un gruppo di utenti

**Per creare un gruppo di utenti**:

1. Accedi all&#39;Admin Console e passa a **[!UICONTROL Utenti]** > **[!UICONTROL Utenti Gruppi]**.

1. Fare clic su **[!UICONTROL Nuovo gruppo utenti]**. Viene aperto il popup _Crea un nuovo gruppo utenti_.

1. Aggiungere un nome di gruppo utenti informativo al campo **[!UICONTROL Nome gruppo utenti]** per identificare lo scopo del nuovo gruppo. Ad esempio, &quot;Brand manager&quot;.

1. Se necessario, aggiungere una descrizione del gruppo e del relativo scopo.

1. Fai clic su **[!UICONTROL Salva]**. Nell&#39;Admin Console viene aperto il popup _Nuovo gruppo_ con il nome del gruppo appena creato.

Consulta [Gestione dei gruppi di utenti](https://helpx.adobe.com/it/enterprise/using/user-groups.html) nella _Guida all&#39;amministrazione di Enterprise e Teams_.

## Passaggio 2: assegnare un profilo di GenStudio System Manager a un gruppo di utenti

Dopo aver creato un nuovo gruppo di utenti e aver aggiunto gli utenti, puoi assegnare il profilo **Adobe GenStudio system manager** a questo gruppo. I diritti associati al profilo assegnato concedono a tutti gli utenti del gruppo le autorizzazioni di GenStudio [!DNL Brands] (creazione, aggiornamento ed eliminazione di marchi).

**Per assegnare un profilo al gruppo di utenti**:

1. Passa al gruppo di utenti appena creato e fai clic sulla scheda _Profili di prodotto assegnati_.

1. Dalla scheda _Profili di prodotto assegnati_, fai clic su **[!UICONTROL Assegna profilo]**. Viene aperto il popup _Assegna prodotti e profili_.

1. Selezionare `Adobe GenStudio` dall&#39;elenco _Seleziona prodotti_.

1. Fare clic su **[!UICONTROL Applica]**. Viene aperto il popup _Seleziona profili di prodotto_, in cui sono visualizzati i profili di prodotto associati all&#39;Adobe GenStudio.

1. Selezionare `Adobe GenStudio system manager`.

1. Fare clic su **[!UICONTROL Applica]**. Viene aperto il popup _Assegna prodotti e profili_, in cui viene visualizzato il profilo di prodotto per il gruppo di utenti appena creato.

1. Fai clic su **[!UICONTROL Salva]**.

Consulta [Assegnare profili di prodotto a gruppi di utenti](https://helpx.adobe.com/it/enterprise/using/user-groups.html) nella _guida per l&#39;amministrazione di Enterprise e Teams_.

## Passaggio 3: creare un progetto [!DNL Brands]

Un _progetto_ fornisce un percorso di archiviazione in cui alcuni utenti possono salvare le risorse, in questo caso [!DNL Brands] risorse.

**Per creare un progetto [!DNL Brands] dalla scheda _Archiviazione_**:

1. Passa alla scheda _Archiviazione_ nell&#39;Admin Console.

1. Fai clic su **[!UICONTROL Progetti]** nella navigazione laterale. Viene visualizzata la scheda _Progetti_.

1. Fare clic su **[!UICONTROL Crea progetto]**. Viene aperto il popup _Nuovo progetto_.

1. Immetti `Adobe GenStudio Brands` nel campo del nome del progetto. Inserisci il nome del progetto esattamente come mostrato qui. Non includere spazi aggiuntivi o modificare la lettera maiuscola.

1. Fai clic su **[!UICONTROL Crea]**. Viene aperto il popup _Invita al progetto_.

Consulta [Gestione dei progetti](https://helpx.adobe.com/enterprise/using/projects-in-business-storage.html) nella _Guida all&#39;amministrazione di Enterprise e Team_.

## Passaggio 4: invitare un gruppo di utenti al progetto

È ora possibile aggiungere il gruppo utenti appena creato al progetto `Adobe GenStudio [!DNL Brands]`.

**Per invitare il gruppo di utenti al progetto appena creato**:

1. Dal popup _Invita al progetto_, aggiungi al progetto il gruppo di utenti appena creato.

1. Scegliere l&#39;opzione di autorizzazione **Può modificare**.

1. Fai clic su **[!UICONTROL Invita]**.

## Passaggio 5: Aggiungere utenti al gruppo di utenti

Per assegnare agli utenti l&#39;autorizzazione per creare, modificare e pubblicare [!DNL Brands], aggiungerli al gruppo di utenti appena creato.

**Per aggiungere utenti al gruppo di utenti**:

1. Dall&#39;_Admin Console_, passa a **[!UICONTROL Utenti]** > **[!UICONTROL Gruppi di utenti]**.

1. Seleziona il nome del gruppo di utenti creato in precedenza. Viene aperto il popup _Aggiungi utenti a questo gruppo di utenti_.

1. Aggiungi un utente nuovo o esistente tramite nome utente o indirizzo e-mail. Scopri come gestire i gruppi di utenti in [Gestire i gruppi di utenti](https://helpx.adobe.com/it/enterprise/using/user-groups.html) nella _Guida all&#39;amministrazione di Enterprise e Teams_.

Agli utenti vengono concesse le autorizzazioni di creazione, modifica e pubblicazione di [!DNL Brand] di Adobe GenStudio System Manager quando vengono aggiunti al gruppo. Gli utenti ricevono inoltre un invito e-mail automatico per modificare il progetto Adobe GenStudio for Performance Marketing [!DNL Brands].
