---
title: Prise en main de la gouvernance et de la documentation des instances
description: Découvrez les stratégies essentielles et les bonnes pratiques pour commencer à utiliser la gouvernance et la documentation de votre Marketo Engage. Découvrez comment créer une documentation évolutive, simplifier la formation des utilisateurs et garantir la création avec une structure dans votre instance de Marketo Engage.
role: Admin
level: Beginner
doc-type: Article
solution: Marketo Engage
duration: 0
last-substantial-update: 2024-05-08T00:00:00Z
jira: KT-14815
thumbnail: KT-14815.jpeg
exl-id: b3dd05e1-c522-4631-a6b4-c0c6309f25d3
source-git-commit: 1205848b1985a99b91f9d4d25e1a79f0df379589
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 0%

---

# Prise en main de la gouvernance et de la documentation des instances

Une bonne documentation peut être presque aussi importante que l’implémentation de l’instance proprement dite. Un guide de gouvernance est une ressource essentielle qui décrit les détails de configuration de votre instance de Marketo Engage et couvre des sujets tels que les structures de programme/dossier, les limites de communication, etc. Ce document actif est une référence pour votre administrateur de Marketo Engage ou vos utilisateurs expérimentés, qui présente les bonnes pratiques spécifiques et les normes de gouvernance adaptées à votre instance et organisation de Marketo Engage.

Mais ça ne s&#39;arrête pas là. Votre équipe peut avoir besoin de documents d’activation ou de matériel de formation supplémentaires pour améliorer ses compétences avec Marketo Engage. Ces ressources peuvent inclure des exercices interactifs, des questionnaires d’accès ou des instructions sur les actions possibles dans Marketo Engage, ce qui bénéficie à tous les utilisateurs Marketo Engage de votre entreprise. Que vous créiez un guide de gouvernance complet ou que vous documentiez initialement les principaux aspects de configuration, l’enregistrement des décisions prises lors de l’intégration est essentiel pour garantir le succès de votre équipe actuelle et des futures générations d’embauches.

En comprenant l’importance de la documentation et de la gouvernance, ce tutoriel décrit les bonnes pratiques provenant de pairs experts [Prise en main de la documentation sur la gouvernance et la formation de votre Marketo Engage](https://nation.marketo.com/t5/product-blogs/getting-started-on-your-marketo-governance-and-training/ba-p/242421){target="_blank} et [Comment documenter votre instance ?](https://nation.marketo.com/t5/product-discussions/how-do-you-document-your-instance/td-p/72877){target="_blank} pour vous aider à mettre en place un processus et à conserver la documentation pertinente pour vos utilisateurs internes.

## Pourquoi la documentation des modifications et des décisions pendant la mise en oeuvre de l’instance est essentielle

Approche de la documentation de votre Marketo Engage comme si vous guidiez un nouvel employé ne connaissant pas la technologie pour se connecter à l’instance. Il est facile d&#39;ignorer les connaissances fondamentales une fois que vous avez acquis de l&#39;expérience avec le Marketo Engage. En tant qu’administrateur, vous devez vous assurer que vos documents d’activation et de gouvernance s’adressent aux débutants. Pour faciliter l’apprentissage des nouveaux utilisateurs, une méthode pratique consiste à intégrer des définitions et des bonnes pratiques directement dans vos documents de formation.

La création de la documentation de l’instance lors de la configuration de l’instance offre plusieurs avantages :

* Rationalisez le processus de formation des nouveaux utilisateurs de manière évolutive.
* Faciliter l’élaboration de programmes à long terme en Marketo Engage en s’appuyant sur une solide base de documentation.
* Maintenez l’intégrité et l’organisation de votre instance au fil du temps.
* En cas de roulement de l’équipe, aplanissez la transition pour les nouveaux administrateurs de Marketo Engage.

En fin de compte, l’écriture des décisions que vous prenez pendant la mise en oeuvre vous aidera, ainsi que votre équipe, à réussir avec Marketo Engage sans dépendre d’une ou de quelques personnes pour appliquer les processus.

## Création de la documentation et de la gouvernance de votre instance de Marketo Engage

### Étape 1 - Décrire les rubriques clés de la documentation de votre instance

Définissez une configuration des normes de ce qui doit être documenté et de ce qui n’est pas nécessaire à la documentation. Cela permettra à l’organisation d’adopter le processus. À mesure que vous développez le document, il est important de documenter la raison d’être de la configuration. Cela aide les autres administrateurs autant que vous-même à éviter de perdre du temps sur des décisions qui n’ont pas produit de résultats.

Guide de votre plan de gouvernance et de documentation en commençant par l’exemple de composition ci-dessous :

1. L’objectif du Marketo Engage pour notre organisation
1. Objectif de cette documentation
1. Processus de maintenance/de modification du guide de gouvernance
1. Configuration administrative
   * Abonnements
   * Espaces de travail et partitions (le cas échéant)
   * Configuration technique (DKIM/SPF/Munchkin)
   * Rôles et responsabilités*
   * Utilisateurs*
   * Paramètres de campagne/d’email/de programme dynamiques
   * Limites de communication
   * Sécurité
   * Canaux*
   * Balises
1. Structure de données
   * Structure de champ
   * Objets personnalisés
1. Programmes opérationnels
   * Notation de personne
   * Cycle de vie des personnes
   * Gestion des données
1. Création Dans Une Instance Marketo Engage
   * [Centre d’excellence (COE)](https://business.adobe.com/blog/perspectives/center-of-excellence-top-10-questions-to-ask-yourself){target="_blank}
   * Structure de dossier
   * Conventions de dénomination
   * Organisation du programme
   * Modèles de programme*
   * Design Studio Assets (modèles d’email, modèles de landing page, fragments de code, formulaires)
   * Processus normalisés
   * Listes de contrôle
   * Segments
   * Stratégies d’archivage
   * Centre d’abonnements
1. Intégration CRM
   * Fonctionnement de la synchronisation
   * Synchronisation des campagnes
   * Dictionnaire de données
1. Autres intégrations
1. RGPD et conformité

\* Votre documentation doit au minimum inclure les détails des utilisateurs et des rôles, des modèles de programme et des canaux une fois la configuration terminée.

### Étape 2 - Création d’un fichier de modification

Un autre moyen essentiel de la gouvernance d’instance consiste à créer un fichier de modification et à l’appliquer à l’aide de ce fichier. Chaque fois que vous modifiez un paramètre de la section &quot;Admin&quot; ou d’un programme opérationnel, votre équipe doit le noter à un emplacement centralisé, tel qu’une feuille de calcul partagée. Cela peut vous aider à vous rappeler pourquoi vous avez fait un changement et à quoi ça ressemblait avant. Les champs que vous devez documenter dans la liste de modifications sont les suivants :

1. Date
1. Nom du programme
1. Lien du programme
1. Nom de la campagne dynamique
1. Lien de campagne dynamique
1. Changement effectué
1. Motif de la modification
1. Qui a apporté le changement

## Quelle est la suite ?

* Téléchargez l’ [exemple de documentation et de Changelog](/help/marketo-tutorial-implementing-new-instance/assets/template-adobe-marketo-engage-instance-documentation.xlsx) et adaptez-les en fonction des besoins de votre entreprise.
* Stockez la documentation sur une plateforme accessible sur laquelle votre entreprise préfère référencer et mettre à jour régulièrement. Par exemple, certains champions Marketo Engage utilisent Confluence (par Atlassian) ou Excel Spreadsheet.
* Assurez-vous que chaque règle que vous créez pour la gouvernance dispose d’un propriétaire pour l’appliquer et adapter la documentation, en la tenant à jour au fil du temps.

### Auteur

{{amy-chiu}}
