---
title: Prise en main de la gouvernance et de la documentation des instances
description: Découvrez les principales stratégies et bonnes pratiques pour commencer à utiliser la gouvernance et la documentation de Marketo Engage. Découvrez comment créer une documentation évolutive, rationaliser la formation des utilisateurs et garantir une création avec une structure dans votre instance Marketo Engage.
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
source-wordcount: '862'
ht-degree: 0%

---

# Prise en main de la gouvernance et de la documentation des instances

Une documentation de qualité peut être presque aussi importante que l’implémentation de l’instance elle-même. Un guide de gouvernance est une ressource essentielle qui décrit les détails de configuration de votre instance Marketo Engage, en couvrant des sujets tels que les structures de programme/dossiers, les limites de communication, etc. Ce document dynamique est une référence destinée à l’administration ou aux utilisateurs expérimentés de Marketo Engage. Il présente les bonnes pratiques spécifiques et les normes de gouvernance adaptées à votre instance et organisation Marketo Engage.

Mais ça ne s&#39;arrête pas là. Votre équipe peut avoir besoin de documents d’activation ou de supports de formation supplémentaires pour améliorer sa maîtrise de Marketo Engage. Ces ressources peuvent inclure des exercices interactifs, des quiz d’accès ou des instructions sur les actions autorisées dans Marketo Engage, pour le bénéfice de tous les utilisateurs et utilisatrices de Marketo Engage au sein de votre entreprise. Qu’il s’agisse de créer un guide de gouvernance complet ou de documenter les principaux aspects de configuration au départ, l’enregistrement des décisions prises lors de l’intégration est essentiel pour assurer la réussite de votre équipe actuelle et des futures générations de nouvelles recrues avec Marketo Engage.

En comprenant l’importance de la documentation et de la gouvernance, ce tutoriel explore les bonnes pratiques provenant de l’expertise de vos pairs [Prise en main de votre documentation sur la gouvernance et la formation Marketo Engage](https://nation.marketo.com/t5/product-blogs/getting-started-on-your-marketo-governance-and-training/ba-p/242421){target=« _blank} et [Comment documentez-vous votre instance ?](https://nation.marketo.com/t5/product-discussions/how-do-you-document-your-instance/td-p/72877){target=« _blank} pour vous aider à mettre en place un processus et à conserver la documentation pertinente pour vos utilisateurs internes.

## Pourquoi il est essentiel de documenter les modifications et les décisions lors de la mise en œuvre de l’instance

Abordez votre documentation Marketo Engage comme si vous guidiez un nouvel employé peu familier avec la technologie à intégrer à l’instance. Il est facile d’ignorer les connaissances fondamentales une fois que vous avez acquis de l’expérience avec Marketo Engage. En tant qu’administrateur, vous devez vous assurer que vos documents d’activation et de gouvernance s’adressent aux débutants. Pour faciliter l&#39;apprentissage des nouveaux utilisateurs, une méthode pratique consiste à incorporer des définitions et des bonnes pratiques directement dans vos supports de formation.

La création de la documentation d’instance lors de la configuration de l’instance offre plusieurs avantages :

* Rationalisez le processus de formation pour les nouveaux utilisateurs de manière évolutive.
* Faciliter le développement de programmes à long terme dans Marketo Engage en s’appuyant sur une base de documentation solide.
* Conservez l’intégrité et l’organisation de votre instance au fil du temps.
* Facilitez la transition pour les nouveaux administrateurs Marketo Engage en cas de rotation de l’équipe.

En fin de compte, la prise de décisions prise lors de l’implémentation vous aidera, vous et votre équipe, à utiliser Marketo Engage avec succès, sans dépendre d’une ou de quelques personnes pour appliquer les processus.

## Comment créer la gouvernance et la documentation de votre instance Marketo Engage

### Étape 1 : définition des rubriques clés dans la documentation de votre instance.

Définissez un ensemble de normes sur ce qui doit être documenté et ce qui n’est pas nécessaire à documenter. Cela permettra à l&#39;organisation d&#39;adopter le processus. Lorsque vous développez le document, il est important de documenter la raison de la configuration. Cela permet aux autres administrateurs autant qu’à vous-même d’éviter de perdre du temps sur des décisions qui n’ont pas donné de résultats.

Guidez votre plan de gouvernance et de documentation en commençant par l’exemple de plan ci-dessous :

1. L’objectif de Marketo Engage pour notre organisation
1. Objectif de cette documentation
1. Processus de mise à jour/modification du guide de gouvernance
1. Configuration administrative
   * Abonnement(s)
   * Espaces de travail et partitions (le cas échéant)
   * Configuration technique (DKIM/SPF/Munchkin)
   * Rôles et responsabilités*
   * Utilisateurs*
   * Campagne intelligente/Paramètres d’e-mail/de programme
   * Limites de communication
   * Sécurité
   * Canaux*
   * Balises
1. Structure des données
   * Structure de champ
   * Objets personnalisés
1. Programmes Opérationnels
   * Score de la personne
   * Cycle de vie d&#39;une personne
   * Data Management
1. Création Dans L’Instance Marketo Engage
   * [Centre d’excellence (COE)](https://business.adobe.com/blog/perspectives/center-of-excellence-top-10-questions-to-ask-yourself){target=« _blank}
   * Structure de dossiers
   * Conventions de dénomination
   * Organisation du programme
   * Modèles de programme*
   * Design Studio Assets (modèles d’e-mail, modèles de page de destination, fragments de code, formulaires)
   * Processus normalisés
   * Checklists
   * Segmentations
   * Stratégies d’archivage
   * Centre d’abonnements
1. Intégration CRM
   * Fonctionnement de la synchronisation
   * Synchronisation de la campagne
   * Dictionnaire de données
1. Autres intégrations
1. RGPD et conformité

\* Au minimum, votre documentation doit inclure les détails des utilisateurs et des rôles, les modèles de programme et les canaux une fois la configuration terminée.

### Étape 2 - Créer un journal des modifications

Un autre moyen essentiel de gouvernance des instances consiste à créer un journal des modifications et à l’appliquer. Chaque fois que vous modifiez un paramètre dans la section « Admin » d’un programme opérationnel, votre équipe doit le noter dans un emplacement centralisé, tel qu’une feuille de calcul partagée. Cela peut vous aider à vous rappeler pourquoi vous avez apporté un changement et comment c’était avant. Les champs à documenter dans le journal des modifications sont les suivants :

1. Date
1. Nom du programme
1. Lien du programme
1. Nom de la campagne intelligente
1. Lien de campagne intelligente
1. Modification apportée
1. Motif de la modification
1. Qui a apporté le changement

## Quelle est la prochaine étape ?

* Téléchargez les [exemples de documentation et de journal des modifications](/help/marketo-tutorial-implementing-new-instance/assets/template-adobe-marketo-engage-instance-documentation.xlsx) et adaptez-les en fonction des besoins de votre entreprise.
* Stockez la documentation sur une plateforme accessible, où votre entreprise préfère la consulter et la mettre à jour régulièrement. Par exemple, certains champions de Marketo Engage utilisent Confluence (par Atlassian) ou Excel Sheets.
* Assurez-vous que chaque règle que vous créez pour la gouvernance dispose d’un propriétaire pour l’appliquer et adapter la documentation, en la tenant à jour au fil du temps.

### Auteur

{{amy-chiu}}
