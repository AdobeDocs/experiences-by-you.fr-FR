---
title: Synchronisation des champs pour les connecteurs CRM natifs
description: Découvrez comment rationaliser votre intégration CRM initiale en sélectionnant de manière stratégique les champs CRM essentiels à l’utilisation de Marketo Engage. Effectuez l’exercice du dictionnaire de données pour identifier les champs dont vous avez besoin pour une synchronisation CRM fluide qui aide les équipes commerciales et marketing à rester alignées.
role: Admin
level: Beginner
doc-type: Article
solution: Marketo Engage
duration: 0
last-substantial-update: 2024-05-04T00:00:00Z
jira: KT-14811
thumbnail: KT-14811.jpeg
exl-id: 42b7ca3d-e445-4c11-ad3d-d4e70c101c8e
source-git-commit: 1205848b1985a99b91f9d4d25e1a79f0df379589
workflow-type: tm+mt
source-wordcount: '2235'
ht-degree: 0%

---

# Champs de synchronisation pour les connecteurs CRM natifs

Utilisez-vous Salesforce ou Microsoft Dynamics au sein de votre entreprise ? Si tel est le cas, avec les connecteurs CRM natifs de Marketo Engage (c’est-à-dire Salesforce, Microsoft Dynamics et Veeva), vous pouvez coordonner les activités de marketing et de vente en partageant de manière transparente les informations pertinentes entre Marketo Engage et CRM. Avant de configurer la synchronisation CRM initiale, veillez à identifier les champs que vous souhaitez synchroniser entre les deux systèmes pour que votre base de données Marketo Engage reste propre.

Découvrez comment réaliser cet exercice à l’aide des bonnes pratiques suggérées par Adobe Professional Services. Suivez afin de comprendre les champs standard et les champs personnalisés et de documenter leurs relations entre Marketo Engage et votre CRM.

## Identifier les champs à synchroniser avant d’intégrer votre CRM à Marketo Engage

Lors de l’intégration de votre CRM à Marketo Engage, vous n’aurez probablement pas besoin de synchroniser tous vos champs CRM avec Marketo Engage. Adopter une approche stratégique concernant les champs dont vous avez besoin peut aider votre instance Marketo Engage à traiter le flux de données plus efficacement.

La synchronisation initiale entre votre Marketo Engage et votre système CRM crée automatiquement des associations pour la plupart des champs standard existants (par exemple e-mail, prénom/nom, société, etc.). En outre, le connecteur synchronise également les [champs personnalisés](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/custom-field-type-glossary){target="_blank"} pour vos leads, contacts, comptes et opportunités en créant de nouveaux champs dans Marketo Engage qui sont automatiquement mappés à ces champs à partir de votre CRM.

L’identification et l’organisation des champs que vous souhaitez synchroniser à partir de votre CRM avant d’effectuer la synchronisation initiale sont des étapes essentielles du processus de configuration du connecteur natif. Il s’agit d’un exercice de dictionnaire de données qui vous permet de réduire le nombre de champs en double créés et de faciliter le plus possible les étapes de remappage suivantes. Cet exercice implique généralement l’intervention des équipes marketing et commerciales ainsi que de votre administrateur CRM pour s’assurer que seuls les champs pertinents sont synchronisés avec votre instance Marketo Engage.

## Créer votre dictionnaire de données

En règle générale, la bonne pratique consiste à synchroniser uniquement les champs CRM qui seront nécessaires à des fins marketing. Commencez par cet exercice pour organiser les champs de votre CRM qui devront être mappés à Marketo Engage et exécuter correctement la synchronisation CRM initiale la première fois.

>[!NOTE]
>Si des champs personnalisés de votre CRM disposent déjà d’un champ personnalisé équivalent dans Marketo Engage avant de commencer la synchronisation initiale, un nouveau champ « en double » est créé dans Marketo Engage pour le champ CRM. Vous pouvez remapper le champ CRM au champ Marketo Engage d’origine et masquer le champ en double une fois la synchronisation initiale terminée. Pour ce faire, contactez le [service clientèle d’Adobe](https://experienceleague.adobe.com/en/docs/customer-one/using/home#create-a-support-ticket-with-admin-console){target="_blank"}. Voir l’étape 7 pour plus de détails.

**Étape 1 :** une liste approximative des champs actuellement disponibles dans votre CRM et indiquez si vous souhaitez qu’ils apparaissent dans Marketo Engage.

* Intégrez les commentaires de votre administrateur CRM, de vos équipes de marketing et de ventes dans le processus de prise de décision.
* Documentez les noms d’API et les types de champs pour chaque champ
* Déterminez le niveau d’accès que Marketo Engage doit avoir pour ces champs (c’est-à-dire en lecture seule ou en lecture-écriture)


**Étape 2 :** consultez la section [Admin > Gestion des champs](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/view-field-mappings-between-marketo-and-salesforce){target="_blank"} de votre instance Marketo Engage pour identifier les champs personnalisés créés précédemment directement dans le système que vous souhaitez inclure dans la synchronisation.

* Documentez les noms d’API et les types de champs pour chaque champ.
* Indiquez les champs qui ont déjà un champ équivalent dans votre CRM.
* Indiquez les champs qui n’ont pas encore de champ équivalent dans votre CRM.


**Étape 3 :** commencer à créer le dictionnaire de données avec les champs de mappage par défaut

* Étant donné que Marketo Engage utilise une base de données plate, il est recommandé de formater votre dictionnaire de données comme suit :

   * Première colonne : noms des champs Marketo Engage
   * Deuxième colonne : noms des API Marketo Engage
   * Troisième colonne : [Type de champ ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/custom-field-type-glossary){target="_blank"} (à savoir booléen, devise, date, etc.)
   * Dans les colonnes suivantes, répétez l’opération pour les types d’objets CRM (Lead, Contact, Compte, Opportunité) avec une colonne supplémentaire pour le niveau d’accès que vous souhaitez accorder à Marketo Engage (c’est-à-dire Lecture, Écriture, Modification)
  <br>

  Voici un exemple de ce à quoi il pourrait ressembler :
  ![Tableau du dictionnaire de données](/help/marketo-tutorial-implementing-new-instance/assets/data_dictionary.png){width="100%" zoomable="yes"}


* Commencez par ajouter les champs par défaut qui seront automatiquement mappés pour votre CRM :

   * [Salesforce](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/default-salesforce-field-mapping){target="_blank"}
   * [Microsoft Dynamics](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/microsoft-dynamics-sync-details/default-dynamics-field-mapping){target="_blank"}
   * [Veeva](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/veeva-crm-sync/sync-details/default-veeva-field-mapping){target="_blank"}

* Vérifiez que chaque champ par défaut dans Marketo Engage correspond au champ de votre CRM avec lequel vous souhaitez effectuer la synchronisation. Par exemple, le champ « Désabonné » dans Marketo Engage peut être le champ « Désabonnement de l’e-mail » dans votre CRM.
* Ajustez le nom, les privilèges et le [type de données](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/custom-field-type-glossary){target="_blank"} de l’API CRM, si nécessaire.

**Étape 4 :** ajouter des champs supplémentaires au dictionnaire de données

* Incluez le Nom d’affichage, les privilèges CRM souhaités et le type de données pour chaque champ.
* Si un champ existe dans le CRM, mais pas dans Marketo Engage, renseignez l’affichage Marketo Engage et les noms d’API avec les mêmes valeurs dans le champ CRM .
* Si un champ existe dans Marketo Engage mais pas dans le CRM, renseignez le nom d’affichage du CRM avec la valeur souhaitée, mais laissez le nom de l’API CRM vide jusqu’à ce que le champ soit créé.
* Si des champs équivalents existent dans les deux systèmes, incluez-les sur la même ligne et indiquez qu’ils doivent être remis en correspondance dans la section « Notes » à l’extrémité droite de votre feuille de dictionnaire de données.

>[!NOTE]
>Si vous envisagez de créer un champ de filtre de synchronisation ([](https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758){target="_blank"} | [Microsoft Dynamics](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/custom-dynamics-sync-filter-details/create-a-custom-dynamics-sync-filter){target="_blank"}), veillez à l’inclure dans cette étape, mais laissez les noms d’API vides jusqu’à ce que le champ soit créé dans votre CRM.

**Étape 5 :** consulter le dictionnaire de données avec votre administrateur CRM

* Créez des champs dans CRM pour ceux qui existent déjà dans Marketo Engage et mettez à jour le dictionnaire de données avec les noms d’affichage et d’API pour le nouveau champ CRM.
* Effectuer le mappage des champs entre les objets Lead et Contact dans votre CRM ([](https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758){target="_blank"} | [Microsoft Dynamics](https://community.dynamics.com/blogs/post/?postid=8a91d93e-2181-45dd-a8fb-1092010bc8f1){target="_blank"}). Lorsqu’un prospect est converti en contact, cela permet de s’assurer que les champs peuvent être consolidés en un seul champ dans Marketo Engage.
* Assurez-vous que le profil de synchronisation Marketo dispose des privilèges appropriés pour chaque champ, comme indiqué dans le dictionnaire de données :
   * [Définition des autorisations de profil dans Salesforce](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited#set-profile-permissions){target="_blank"}
   * [Définition des autorisations de profil dans Microsoft Dynamics](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up#create-application-user-in-microsoft){target="_blank"}
   * [Définition des autorisations de profil dans Veeva](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/veeva-crm-sync/setup/step-2-of-3-create-a-veeva-crm-user-for-marketo-engage#set-profile-permissions){target="_blank"}

**Étape 6 :** effectuer la synchronisation initiale

* Assurez-vous que tous les champs que vous souhaitez synchroniser avec Marketo Engage disposent des privilèges appropriés dans votre CRM, tel que défini par le dictionnaire de données.
* Assurez-vous que tous les champs que vous **pas** souhaitez synchroniser avec Marketo Engage sont [masqués du profil de synchronisation Marketo](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync){target="_blank"}. Il est beaucoup plus facile d’ajouter de nouveaux champs à la synchronisation ultérieurement que de supprimer les champs qui ont été synchronisés involontairement.
* Connectez-vous votre CRM à l’aide du champ Filtre de synchronisation ? Si vous effectuez une synchronisation avec Salesforce, contactez le service clientèle d’Adobe pour vous assurer que la fonctionnalité de filtrage est activée avant de démarrer votre synchronisation initiale.


**Étape 7 :** consultez la section Gestion des champs dans Marketo Engage

* Confirmez/mettez à jour les noms d’affichage et d’API pour les nouveaux champs synchronisés.
* Identifiez les champs dupliqués qui peuvent nécessiter un remappage. Les champs en double se produisent dans quelques scénarios :
   * Les champs personnalisés du CRM créent un champ (potentiellement en double) dans Marketo Engage la première fois qu’ils se synchronisent, si un champ équivalent existait déjà dans Marketo Engage.
   * Champs personnalisés Marketo-Engage-Only (c’est-à-dire un champ créé directement dans Marketo Engage) et vous pouvez avoir un champ équivalent synchronisé à partir du CRM.



**Étape 8 :** contactez le service clientèle d’Adobe pour effectuer un remappage si des champs dupliqués apparaissent

* Contactez l’assistance avec les informations suivantes pour les champs qui doivent être remis en correspondance :
   * Afficher les noms des API et pour les nouveaux champs en double créés par le CRM.
   * Nom d’affichage du champ Marketo Engage auquel vous souhaitez mapper le champ CRM.
   * Reportez-vous à cet exemple [ICI](https://nation.marketo.com/t5/knowledgebase/re-mapping-sfdc-marketo-fields/ta-p/299284){target="_blank"}.
* Une fois le remappage terminé, passez en revue les noms d’API pour les champs remappés dans Marketo Engage et mettez à jour les valeurs dans la colonne « Nom de l’API » de votre dictionnaire de données pour vous assurer qu’elle contient les informations les plus précises possible.

## Quelle est la prochaine étape ?

* Créez votre dictionnaire de données pour organiser vos champs en vue de l’intégration CRM.
* Familiarisez-vous avec le processus de synchronisation initial pour votre CRM

>[!BEGINTABS]

>[!TAB ]

Découvrez comment Marketo Engage et Salesforce vont de pair pour synchroniser vos données de vente et de marketing.

>[!VIDEO](https://video.tv.adobe.com/v/3424719/?learn=on)

+++**Liens utilisés dans la vidéo :**

* [Comprendre la synchronisation Salesforce](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync){target="_blank"}

* [Ajouter des champs Marketo à Salesforce (Entreprise/Illimité)](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited){target="_blank"}

* [Création d’un utilisateur Marketo dans Salesforce (Enterprise/Unlimited)](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited){target="_blank"}

* [Connecter Marketo et Salesforce (Enterprise/Unlimited)](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited){target="_blank"}

* [Les utilisateurs doivent configurer l’application connectée côté Salesforce avant de passer à Marketo et à la synchronisation Salesforce.](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0){target="_blank"}

* [Statut de synchronisation de Salesforce](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/salesforce-sync-status){target="_blank"}

* [Masquer et afficher un champ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/hide-and-unhide-a-field){target="_blank"}

* [Tutoriel : en savoir plus sur la synchronisation de Marketo avec votre CRM](https://experienceleague.adobe.com/en/docs/marketo-learn/tutorials/lead-and-data-management/crm-sync-learn){target="_blank"}

+++

>[!TAB ]

Découvrez comment fonctionne la synchronisation Microsoft Dynamics 365 et configurez correctement la configuration pour permettre aux deux systèmes de communiquer entre eux.

>[!VIDEO](https://video.tv.adobe.com/v/3424737/?learn=on)

+++**Liens utilisés dans la vidéo :**

* [Comprendre la synchronisation Microsoft Dynamics](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/understanding-the-microsoft-dynamics-sync){target="_blank"}

* [Téléchargement de la solution de gestion des prospects Marketo](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/download-the-marketo-lead-management-solution){target="_blank"}

* [Mise à jour de la solution Marketo pour Microsoft Dynamics](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/update-the-marketo-solution-for-microsoft-dynamics){target="_blank"}

* [Accorder le consentement pour l’ID client et l’enregistrement de l’application](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/grant-consent-for-client-id-and-app-registration)

* [Valider la synchronisation Microsoft Dynamics](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/validate-microsoft-dynamics-sync){target="_blank"}

* [Statut de synchronisation](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/microsoft-dynamics-sync-details/sync-status){target="_blank"}

* [Correction des problèmes de synchronisation de la validation de Dynamics](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/fix-dynamics-validation-sync-issues){target="_blank"}

* [Créer un filtre de synchronisation Dynamics personnalisé](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/custom-dynamics-sync-filter-details/create-a-custom-dynamics-sync-filter.html){target="_blank"}

* [Afficher l’URL du service d’organisation](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/view-the-organization-service-url){target="_blank"}

* [Modifier les champs à synchroniser avant de les supprimer dans Dynamics](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/microsoft-dynamics-sync-details/editing-fields-to-sync-before-deleting-them-in-dynamics){target="_blank"}

* [Tutoriel : en savoir plus sur la synchronisation de Marketo avec votre CRM](https://experienceleague.adobe.com/en/docs/marketo-learn/tutorials/lead-and-data-management/crm-sync-learn){target="_blank"}

+++

>[!ENDTABS]

### Auteurs

{{peter-livadas}}

{{amy-chiu}}
