---
title: Enregistrer les erreurs de synchronisation CRM pour faciliter le dépannage
description: Découvrez comment utiliser un journal des erreurs de synchronisation CRM pour étudier les problèmes de synchronisation CRM et le maintenir en bon état.
feature-set: Marketo Engage
feature: Administration
role: Admin
level: Intermediate, Experienced
doc-type: Tutorial
last-substantial-update: 2023-10-16T00:00:00Z
jira: KT-13875
thumbnail: KT-13875.jpeg
hide: false
exl-id: 6a38f5dd-5d25-43d8-a1d3-e75ab396e555
source-git-commit: 058d26bd99ab060df3633fb32f1232f534881ca4
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 0%

---

# Enregistrer les erreurs de synchronisation CRM pour faciliter le dépannage

Comme [!DNL Marketo Engage] administrateur, vérifier si votre instance est synchronisée avec votre CRM doit être un élément clé de votre [routine quotidienne](https://nation.marketo.com/t5/champion-program-blogs/my-marketo-morning-routine-tips-for-driving-marketing-operation/ba-p/247508){target="_blank"}. While the [Notifications section](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/notification-types.html){target="_blank"} (le trouver dans le coin supérieur droit de votre [!DNL Marketo Engage] ) est l’emplacement où vous allez commencer à rechercher et à étudier les problèmes de synchronisation fréquents. Il existe une astuce pro qui peut vous aider à gérer l’intégrité de l’instance de manière organisée. [!DNL Adobe] Champion de Marketo (2019-2022), Amy Goldfine recommande aux utilisateurs administrateurs de conserver un journal des erreurs de synchronisation CRM afin de faciliter le dépannage.

![Capture d’écran de l’onglet Erreurs de synchronisation](/help/marketo-tutorial-inherited-instance/_assets/Marketo_Engage_Admin_Salesforce_Sync_Errors_Tab.png)

## Pourquoi conserver un enregistrement des erreurs de synchronisation CRM ?

En enregistrant les erreurs de synchronisation CRM, [!DNL Marketo Engage] Les administrateurs peuvent examiner les problèmes et tendances avec les administrateurs CRM pour résoudre la cause principale. Suivez les étapes ci-dessous pour documenter les problèmes de synchronisation CRM pour votre instance.

## Comment conserver un journal des erreurs de synchronisation CRM

Avant de commencer, téléchargez la [Modèle de journal des erreurs de synchronisation CRM](/help/marketo-tutorial-inherited-instance/_assets/downloads/Adobe-Marketo-Engage_CRM-Sync-Error-Log-Template.xlsx).

**Étape 1 :** Accédez au *[!UICONTROL Administration] section* in [!DNL Marketo Engage]. Sous *[!UICONTROL Intégration]*, cliquez sur *[!DNL Salesforce]*, *[!DNL Microsoft Dynamics]*, ou *[!DNL Veeva]*, selon le [!DNL CRM] vous utilisez , puis la fonction *[!UICONTROL Erreurs de synchronisation]* .

**Étape 2 :** Vous pouvez choisir de [exporter les enregistrements des erreurs en tant que [!DNL CSV] via le [!UICONTROL Filtrer] panel](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.html#filter-sync-errors){target="_blank"}. Si vous ne disposez que de quelques heures, effectuez directement une copie et un collage à partir de l’événement *[!UICONTROL Erreurs de synchronisation]* tab serait la voie à suivre.

**Étape 3 :** Notez la date à laquelle l’erreur s’est produite.

**Étape 4 :** Saisissez le nombre d&#39;enregistrements de personnes concernées par cette erreur. (Parfois, votre CRM ne génère une erreur que pour une seule personne. Parfois, il y aura beaucoup de gens avec la même erreur à la fois.)

**Étape 5 :** Notez l’adresse électronique d’une personne affectée par l’erreur. Cela facilite la référence et la discussion des erreurs avec l&#39;administrateur CRM.

**Étape 6 :** coller des liens vers l’enregistrement de la personne dans [!DNL [!DNL Marketo Engage]] et [!UICONTROL Prospère/contact CRM] enregistrement de cette personne.

**Étape 7 :** Dans la dernière colonne, collez le texte réel de l&#39;erreur.

## Et après ? 

**Identification des codes d’erreur :** Pour comprendre les codes d’erreur, consultez les descriptions de la documentation destinée aux développeurs. [Tableau Codes d’erreur de niveau réponse](https://developers.marketo.com/rest-api/error-codes/#response_level_error_codes){target="_blank"} et recherchez les étapes suivantes courantes pour résoudre les erreurs.

## Auteurs

**Amy Goldfine**\
[!DNL Adobe] Champion Marketo (2019-2022)
*Fondateur : MarketingOpsAdvice.com*

![Amy Goldfine](/help/marketo-tutorial-inherited-instance/_assets/authors/Customer_Author_Amy_Goldfine.png){width="25%"}

**Amy Chiu**
*Gestionnaire marketing de l’adoption et de la rétention à l’adresse[!DNL Adobe]*

![Amy Chiu](/help/marketo-tutorial-inherited-instance/_assets/authors/Adobe_Author_Amy_Chiu.png){width="25%"}
