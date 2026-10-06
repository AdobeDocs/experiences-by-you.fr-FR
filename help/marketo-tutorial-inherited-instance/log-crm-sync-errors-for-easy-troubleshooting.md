---
title: Consigner les erreurs de synchronisation CRM pour faciliter le dépannage
description: Découvrez comment utiliser un journal des erreurs de synchronisation CRM pour examiner les problèmes de synchronisation CRM et assurer son bon fonctionnement.
feature-set: Marketo Engage
feature: Administration
role: Admin
level: Intermediate, Experienced
doc-type: Tutorial
last-substantial-update: 2023-10-16T00:00:00.000Z
jira: KT-13875
thumbnail: KT-13875.jpeg
exl-id: 6a38f5dd-5d25-43d8-a1d3-e75ab396e555
product_v2:
  - id: fd1f54a9-f50c-467d-8956-cebbaf4f3eb8
    internal-label: Experience Manager
  - id: c68cd75e-5bca-4bc3-a60e-9e183f816441
    internal-label: Experience Manager Cloud Manager
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
source-git-commit: 749b293ab38b8ea5a5f72517bd5c3455399137c2
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%
---
# Consigner les erreurs de synchronisation CRM pour le dépannage

En tant qu’administrateur [!DNL Marketo Engage], la vérification de la synchronisation de votre instance avec votre CRM doit être un élément clé de votre [routine quotidienne](https://nation.marketo.com/t5/champion-program-blogs/my-marketo-morning-routine-tips-for-driving-marketing-operation/ba-p/247508){target="_blank"}. Bien que la [section Notifications](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/notification-types.html){target="_blank"} (localisez-la dans le coin supérieur droit de votre interface [!DNL Marketo Engage]) soit l’endroit où vous commencerez à trouver et à étudier les problèmes de synchronisation fréquents, il existe une astuce pro qui pourrait vous aider à gérer l’intégrité de l’instance de manière organisée. [!DNL Adobe] Championne Marketo (2019-2022), Amy Goldfine recommande aux utilisateurs administrateurs de tenir un journal des erreurs de synchronisation CRM pour faciliter la résolution des problèmes.

![Capture d’écran de l’onglet Erreurs de synchronisation](/help/marketo-tutorial-inherited-instance/_assets/Marketo_Engage_Admin_Salesforce_Sync_Errors_Tab.png)

## Pourquoi conserver un enregistrement des erreurs de synchronisation CRM ?

En consignant les erreurs de synchronisation CRM, les administrateurs [!DNL Marketo Engage] peuvent examiner les problèmes et les tendances avec les administrateurs CRM pour résoudre la cause première. Suivez les étapes ci-dessous pour documenter vos problèmes de synchronisation CRM pour votre instance.

## Comment conserver un journal des erreurs de synchronisation CRM

Avant de commencer, téléchargez le modèle de journal [Erreurs de synchronisation CRM](/help/marketo-tutorial-inherited-instance/_assets/downloads/Adobe-Marketo-Engage_CRM-Sync-Error-Log-Template.xlsx).

**Étape 1 :** accédez à la section *[!UICONTROL Admin]* dans [!DNL Marketo Engage]. Sous *[!UICONTROL Intégration]*, cliquez sur *[!DNL Salesforce]*, *[!DNL Microsoft Dynamics]* ou *[!DNL Veeva]*, selon le [!DNL CRM] utilisé, puis sur l’onglet *[!UICONTROL Erreurs de synchronisation]*.

**Étape 2 :** vous pouvez choisir d’[exporter les enregistrements d’erreurs sous forme  [!DNL CSV]  fichier via le panneau [!UICONTROL Filtrer]](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.html#filter-sync-errors){target="_blank"}. Si vous ne disposez que de quelques heures, il est recommandé de copier et coller directement à partir de l’onglet *[!UICONTROL Erreurs de synchronisation]*.

**Étape 3 :** Notez la date à laquelle l’erreur s’est produite.

**Étape 4 :** saisissez le nombre d’enregistrements de personne affectés par cette erreur. (Parfois, votre CRM ne renvoie une erreur que pour une seule personne. Parfois, il y aura plusieurs personnes avec la même erreur à la fois.)

**Étape 5 :** notez l’adresse e-mail d’une personne affectée par l’erreur. Vous pouvez ainsi facilement référencer les erreurs et en discuter avec l’administrateur CRM.

**Étape 6 :** coller des liens vers l’enregistrement de personne dans [!DNL Marketo Engage] et [!UICONTROL Lead/Contact CRM] l’enregistrement de cette personne.

**Étape 7 :** dans la dernière colonne, collez le texte réel de l’erreur.

## Quelle est la prochaine étape ?

**Identifier les codes d’erreur :** pour comprendre les codes d’erreur, consultez les descriptions de la documentation destinée aux développeurs [tableau Codes d’erreur au niveau de la réponse](https://developers.marketo.com/rest-api/error-codes/#response_level_error_codes){target="_blank"} et recherchez les étapes suivantes standard pour résoudre les erreurs.

## Auteurs

**Amy Goldfine**\
[!DNL Adobe] Champion Marketo(2019-2022)
*fondateur, MarketingOpsAdvice.com*

![ Amy Goldfine ](/help/marketo-tutorial-inherited-instance/_assets/authors/Customer_Author_Amy_Goldfine.png){width="25%"}

**Amy Chiu**
*Responsable marketing Adoption &amp; Rétention chez[!DNL Adobe]*

![ Amy Chiu ](/help/marketo-tutorial-inherited-instance/_assets/authors/Adobe_Author_Amy_Chiu.png){width="25%"}
