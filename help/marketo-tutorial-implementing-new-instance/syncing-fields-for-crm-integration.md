---
title: Synchronisation des champs pour les connecteurs CRM natifs
description: Découvrez comment rationaliser votre intégration CRM initiale en sélectionnant de manière stratégique les champs CRM essentiels à utiliser par le Marketo Engage. Effectuez l’exercice du dictionnaire de données pour identifier les champs dont vous avez besoin pour une synchronisation CRM fluide qui aide les équipes de vente et de marketing à rester alignées.
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
source-wordcount: '1567'
ht-degree: 0%

---

# Champs de synchronisation pour les connecteurs CRM natifs

Utilisez-vous Salesforce ou Microsoft Dynamics au sein de votre organisation ? Si c’est le cas, avec les connecteurs CRM natifs du Marketo Engage (c’est-à-dire Salesforce, Microsoft Dynamics et Veeva), vous pouvez coordonner les activités de marketing et de vente en partageant facilement des informations pertinentes entre Marketo Engage et CRM. Avant de configurer la synchronisation CRM initiale, veillez à identifier les champs que vous souhaitez synchroniser entre les deux systèmes afin de préserver la propreté de la base de données de votre Marketo Engage.

Découvrez comment réaliser cet exercice avec les bonnes pratiques suggérées par Adobe Professional Services. Suivez cette procédure pour comprendre les champs standard et personnalisés et documenter leurs relations entre Marketo Engage et votre gestion de la relation client.

## Identifier les champs à synchroniser avant l&#39;intégration de votre CRM à Marketo Engage

Lors de l&#39;intégration de votre CRM à Marketo Engage, vous n&#39;aurez probablement pas besoin de synchroniser tous vos champs CRM avec Marketo Engage. En étant stratégique par rapport aux champs dont vous avez besoin, vous pouvez aider votre instance de Marketo Engage à traiter le flux de données plus efficacement.

La synchronisation initiale entre votre Marketo Engage et votre système CRM crée automatiquement des associations pour la plupart des champs standard existants (c’est-à-dire email, prénom/nom, entreprise, etc.). De plus, le connecteur synchronise également [&#x200B; Champs personnalisés](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/administration/field-management/custom-field-type-glossary){target="_blank"} pour vos Leads, contacts, comptes et opportunités en créant dans Marketo Engage de nouveaux champs automatiquement mappés à ces champs à partir de votre CRM.

L’identification et l’organisation des champs que vous souhaitez synchroniser à partir de votre CRM avant d’effectuer la synchronisation initiale est une étape essentielle du processus de configuration du connecteur natif. Nous appelons cela un exercice de dictionnaire de données, qui vous aide à minimiser le nombre de champs en double qui sont créés et à faire en sorte que toutes les étapes de recodification suivantes se déroulent aussi facilement que possible. Cet exercice implique généralement l’entrée des équipes marketing et de vente et de votre administrateur CRM pour vous assurer que seuls les champs pertinents sont synchronisés avec votre instance de Marketo Engage.

## Création de votre dictionnaire de données

En règle générale, la bonne pratique consiste à synchroniser uniquement les champs de gestion de la relation client nécessaires à des fins marketing. Commencez par cet exercice pour organiser les champs de votre CRM qui devront être mappés à Marketo Engage et exécuter correctement la première synchronisation CRM initiale.

>[!NOTE]
>Si des champs personnalisés de votre CRM possèdent déjà un champ personnalisé équivalent en Marketo Engage avant le début de la synchronisation initiale, un nouveau champ &quot;duplicata&quot; est créé dans Marketo Engage pour le champ CRM. Vous pouvez réassocier le champ CRM au champ de Marketo Engage d’origine et masquer le champ dupliqué une fois la synchronisation initiale terminée, mais vous devez contacter le [service clientèle d’Adobe](https://experienceleague.adobe.com/fr/docs/customer-one/using/home#create-a-support-ticket-with-admin-console){target="_blank"} pour ce faire. Voir l’étape 7 pour plus de détails.

**Étape 1 :** Créez une liste approximative de champs actuellement disponibles dans votre CRM et indiquez si vous souhaitez qu’ils apparaissent dans Marketo Engage.

* Incluez les commentaires de votre administrateur CRM, de vos équipes marketing et de vente dans le processus de prise de décision.
* documenter les noms et les types de champ de l’API pour chaque champ ;
* Déterminer le niveau d’accès que le Marketo Engage doit avoir pour ces champs (lecture seule ou lecture-écriture)


**Étape 2 :** Passez en revue la [section Admin > Gestion des champs](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/administration/field-management/view-field-mappings-between-marketo-and-salesforce){target="_blank"} de votre instance de Marketo Engage pour Identifier tous les champs personnalisés précédemment créés directement dans le système que vous souhaitez inclure dans la synchronisation.

* Documentez les noms et les types de champs de l’API pour chaque champ.
* Indique les champs qui ont déjà un champ équivalent dans votre CRM.
* Indique les champs qui n’ont pas déjà un champ équivalent dans votre CRM.


**Étape 3 :** Commencez à créer le dictionnaire de données avec les champs de mappage par défaut.

* Comme Marketo Engage utilise une base de données plate, il est recommandé de mettre en forme votre dictionnaire de données comme suit :

   * Première colonne : noms des champs du Marketo Engage
   * Deuxième colonne : Noms des API du Marketo Engage
   * Troisième colonne : [Type de champ de Marketo Engage](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/administration/field-management/custom-field-type-glossary){target="_blank"} (booléen, devise, date, etc.)
   * Dans les colonnes suivantes, répétez l’opération pour les types d’objets CRM (prospect, contact, compte, opportunité) avec une colonne supplémentaire pour le niveau d’accès que vous souhaitez que le Marketo Engage ait (c.-à-d. Lecture, Écriture, Modification).

  <br>

  Voici un exemple de ce à quoi il ressemblerait :
  ![&#x200B; Table du dictionnaire de données &#x200B;](/help/marketo-tutorial-implementing-new-instance/assets/data_dictionary.png){width="100%" zoomable="yes"}


* Ajoutez tout d&#39;abord les champs par défaut qui seront automatiquement mappés pour votre CRM :

   * [Salesforce](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/default-salesforce-field-mapping){target="_blank"}
   * [Microsoft Dynamics](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/microsoft-dynamics-sync-details/default-dynamics-field-mapping){target="_blank"}
   * [Veeva](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/crm-sync/veeva-crm-sync/sync-details/default-veeva-field-mapping){target="_blank"}

* Confirmez que chaque champ par défaut dans Marketo Engage correspond au champ de votre CRM avec lequel vous souhaitez effectuer la synchronisation. Par exemple, le champ &quot;Désabonné&quot; dans Marketo Engage peut être le champ &quot;Désabonnement par e-mail&quot; dans votre CRM.
* Ajustez le nom, les privilèges et le [type de données](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/administration/field-management/custom-field-type-glossary){target="_blank"} de l’API CRM si nécessaire.

**Étape 4 :** Ajouter des champs supplémentaires au dictionnaire de données

* Incluez le nom d’affichage, les privilèges CRM souhaités et le type de données pour chaque champ.
* Si un champ existe dans le CRM, mais pas dans le Marketo Engage, renseignez les noms des API et de l&#39;affichage du Marketo Engage avec les mêmes valeurs dans le champ CRM.
* Si un champ existe dans Marketo Engage, mais pas dans le CRM, renseignez le nom d&#39;affichage du CRM avec la valeur souhaitée, mais laissez le nom de l&#39;API CRM vide jusqu&#39;à la création du champ.
* S’il existe des champs équivalents dans les deux systèmes, incluez-les sur la même ligne et indiquez qu’ils doivent être mappés dans la section &quot;Notes&quot; à l’extrémité droite de votre feuille de dictionnaire de données.

>[!NOTE]
>Si vous envisagez de créer un champ Filtre de synchronisation ([Salesforce](https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758){target="_blank"}) | [Microsoft Dynamics](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/custom-dynamics-sync-filter-details/create-a-custom-dynamics-sync-filter){target="_blank"}), veillez à l’inclure dans cette étape, mais laissez les noms d’API vides jusqu’à ce que le champ soit créé dans votre CRM.

**Étape 5 :** Consultez le dictionnaire de données avec votre administrateur CRM

* Créez des champs dans le CRM pour ceux qui existent déjà dans Marketo Engage et mettez à jour le dictionnaire de données avec les noms Display et API du nouveau champ CRM.
* Effectuez le mappage des champs entre les objets Lead et Contact dans votre CRM ([Salesforce](https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758){target="_blank"}) | [Microsoft Dynamics](https://community.dynamics.com/blogs/post/?postid=8a91d93e-2181-45dd-a8fb-1092010bc8f1){target="_blank"}). Lorsqu&#39;une piste est convertie en contact, les champs peuvent être consolidés dans un seul champ de Marketo Engage.
* Assurez-vous que le profil de synchronisation Marketo dispose des privilèges appropriés sur chaque champ, comme indiqué dans le dictionnaire de données :
   * [&#x200B; Définition des autorisations de profil dans Salesforce](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited#set-profile-permissions){target="_blank"}
   * [Définition des autorisations de profil dans Microsoft Dynamics](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up#create-application-user-in-microsoft){target="_blank"}
   * [Définition des autorisations de profil dans Veeva](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/crm-sync/veeva-crm-sync/setup/step-2-of-3-create-a-veeva-crm-user-for-marketo-engage#set-profile-permissions){target="_blank"}

**Étape 6 :** Effectuez la synchronisation initiale

* Assurez-vous que tous les champs que vous souhaitez synchroniser avec Marketo Engage disposent des privilèges appropriés dans votre CRM tels que définis par le dictionnaire de données.
* Assurez-vous que tous les champs que vous souhaitez **et non** synchroniser avec Marketo Engage sont [masqués du profil de synchronisation Marketo](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync){target="_blank"}. Il est beaucoup plus facile d’ajouter de nouveaux champs à la synchronisation plus tard que de supprimer des champs qui ont été synchronisés involontairement.
* Connectez-vous votre CRM au champ Filtre de synchronisation ? Si vous effectuez une synchronisation avec Salesforce, contactez le service clientèle d’Adobe pour vous assurer que la fonctionnalité de filtrage est activée avant de démarrer votre synchronisation initiale.


**Étape 7 :** Consultez la section Gestion des champs dans Marketo Engage

* Confirmez/mettez à jour les noms d’affichage et d’API pour les nouveaux champs synchronisés.
* Identifiez les champs dupliqués qui peuvent nécessiter un remapping. Les champs dupliqués se produisent dans certains cas :
   * Les champs personnalisés dans le CRM créent un nouveau champ (potentiellement dupliqué) en Marketo Engage la première fois qu’ils se synchronisent si un champ équivalent existe déjà dans Marketo Engage.
   * Champs personnalisés Marketo-Engage-Only (c’est-à-dire un champ créé directement dans Marketo Engage) et vous pouvez avoir un champ équivalent synchronisé à partir du CRM.



**Étape 8 :** Contactez le service clientèle d’Adobe pour effectuer un mappage en cas de doublons de champs.

* Contactez l’assistance avec les informations suivantes pour les champs qui doivent être mappés :
   * Afficher les noms des API et pour les nouveaux champs en double créés par le CRM.
   * Nom d’affichage du champ du Marketo Engage auquel vous souhaitez mapper le champ CRM.
   * Reportez-vous à cet exemple [HERE](https://nation.marketo.com/t5/knowledgebase/re-mapping-sfdc-marketo-fields/ta-p/299284){target="_blank"}.
* Une fois le mappage terminé, passez en revue les noms d’API des champs mappés dans Marketo Engage et mettez à jour les valeurs de la colonne &quot;Nom d’API&quot; de votre dictionnaire de données pour vous assurer qu’il contient les informations les plus précises.

## Quelle est la suite ?

* Créez votre dictionnaire de données pour organiser vos champs pour l’intégration CRM.
* Familiarisez-vous avec le processus de synchronisation initial pour votre CRM

>[!BEGINTABS]

>[!TAB Salesforce]

Découvrez comment Marketo Engage et Salesforce se combinent pour maintenir la synchronisation de vos données marketing et de ventes.

>[!VIDEO](https://video.tv.adobe.com/v/3453798/?learn=on&captions=fre_fr)

+++**Liens utilisés dans la vidéo :**

* [Comprendre la synchronisation Salesforce](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync){target="_blank"}

* [Ajouter des champs Marketo à Salesforce (Enterprise/Unlimited)](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited){target="_blank"}

* [Créer un utilisateur Marketo dans Salesforce (Enterprise/Unlimited)](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited){target="_blank"}

* [Connecter Marketo et Salesforce(Enterprise/Unlimited)](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited){target="_blank"}

* [Les utilisateurs doivent configurer l’application connectée du côté Salesforce avant de passer à Marketo et à la synchronisation Salesforce.](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0){target="_blank"}

* [État de synchronisation Salesforce](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/crm-sync/salesforce-sync/salesforce-sync-status){target="_blank"}

* [Masquer et afficher un champ](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/administration/field-management/hide-and-unhide-a-field){target="_blank"}

* [Tutoriel : En savoir plus sur la synchronisation de Marketo avec votre CRM](https://experienceleague.adobe.com/fr/docs/marketo-learn/tutorials/lead-and-data-management/crm-sync-learn){target="_blank"}

+++

>[!TAB Microsoft Dynamics]

Découvrez le fonctionnement de la synchronisation Microsoft Dynamics 365 et configurez correctement la configuration pour permettre aux deux systèmes de communiquer entre eux.

>[!VIDEO](https://video.tv.adobe.com/v/3430213/?learn=on&captions=fre_fr)

+++**Liens utilisés dans la vidéo :**

* [Présentation de la synchronisation Microsoft Dynamics](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/understanding-the-microsoft-dynamics-sync){target="_blank"}

* [Télécharger la solution Marketo Lead Management](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/download-the-marketo-lead-management-solution){target="_blank"}

* [Mise à jour de la solution Marketo pour Microsoft Dynamics](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/update-the-marketo-solution-for-microsoft-dynamics){target="_blank"}

* [Accorder le consentement pour l’ID de client et l’enregistrement d’application](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/grant-consent-for-client-id-and-app-registration)

* [Valider la synchronisation Microsoft Dynamics](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/validate-microsoft-dynamics-sync){target="_blank"}

* [État de synchronisation](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/microsoft-dynamics-sync-details/sync-status){target="_blank"}

* [Correction des problèmes de synchronisation de la validation Dynamics](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/fix-dynamics-validation-sync-issues){target="_blank"}

* [Créer un filtre de synchronisation Dynamics personnalisé](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/custom-dynamics-sync-filter-details/create-a-custom-dynamics-sync-filter.html?lang=fr){target="_blank"}

* [Afficher l’URL du service d’organisation](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/view-the-organization-service-url){target="_blank"}

* [Modification de champs à synchroniser avant de les supprimer dans Dynamics](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/microsoft-dynamics-sync-details/editing-fields-to-sync-before-deleting-them-in-dynamics){target="_blank"}

* [Tutoriel : En savoir plus sur la synchronisation de Marketo avec votre CRM](https://experienceleague.adobe.com/fr/docs/marketo-learn/tutorials/lead-and-data-management/crm-sync-learn){target="_blank"}

+++

>[!ENDTABS]

### Auteurs

{{peter-livadas}}

{{amy-chiu}}
