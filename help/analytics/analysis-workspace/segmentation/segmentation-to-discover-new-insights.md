---
title: Il vous suffit maintenant d’attendre un segment... En utilisant la segmentation pour découvrir de nouvelles informations dans Analysis Workspace
description: Découvrez comment utiliser les segments dans [!DNL Adobe Analytics] pour obtenir de nouvelles informations à partir de vos visualisations Analysis Workspace et de vos tableaux à structure libre.
feature-set: Analytics
feature: Segmentation
role: User
level: Beginner
doc-type: Article
last-substantial-update: 2023-05-16T00:00:00.000Z
jira: KT-13268
thumbnail: KT-13268.jpeg
exl-id: 3496b6ff-f8d6-48a1-92f4-442a792663e7
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
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
    internal-label: Personalization
subfeature_v2:
  - id: a1d50dda-6d94-4e16-8c30-5eb7181c4650
    internal-label: Segmentation
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
source-git-commit: 749b293ab38b8ea5a5f72517bd5c3455399137c2
workflow-type: tm+mt
source-wordcount: '866'
ht-degree: 2%
---
# Il vous suffit maintenant d’attendre un segment... en utilisant des segments pour découvrir de nouvelles informations dans Analysis Workspace

Que vous soyez un nouvel utilisateur [!DNL Adobe Analytics] ou un pro chevronné, vous exploiterez beaucoup les segments dans vos projets Analysis Workspace. Comme [[!DNL Adobe] ](https://experienceleague.adobe.com/docs/analytics/components/segmentation/seg-overview.html?lang=en) le décrit, « les segments vous permettent d’identifier des sous-ensembles de visiteurs en fonction de caractéristiques ou d’interactions de sites web ». Bien que le résultat de base de cette fonctionnalité implique l’isolation des groupes d’utilisateurs, des visites ou des accès à votre site, un analyste perspicace tel que vous peut faire preuve de créativité avec cet outil et trouver de nouvelles façons d’obtenir des informations sur l’activité de votre site. La liste des options possibles est longue. N’hésitez donc pas à créer la vôtre et à la partager avec d’autres personnes de votre entreprise ou en ligne dans des communautés telles que la [[!DNL Adobe Analytics] Communauté](https://experienceleaguecommunities.adobe.com/t5/adobe-analytics/ct-p/adobe-analytics-community?profile.language=fr) sur Experience League ou la communauté [#Measure Slack](https://www.measure.chat/).

Si vous avez besoin d’un bref rappel sur la création d’un segment, consultez la documentation d’Experience League sur l’utilisation du [créateur de segments](https://experienceleague.adobe.com/docs/analytics/components/segmentation/segmentation-workflow/seg-build.html?lang=en) dans Analysis Workspace.

## Comparaison et contraste des segments

Dans Analysis Workspace, vous pouvez comparer deux segments à l’aide de « [Comparaison des segments](https://experienceleague.adobe.com/docs/analytics/analyze/analysis-workspace/panels/segment-comparison/segment-comparison.html?lang=en) ». La comparaison des segments se trouve dans la section Panneaux de la barre de navigation de gauche :

![seg 01](assets/seg01.png)

Cependant, il arrive que vous n’ayez pas besoin d’un panneau de comparaison complet pour transmettre des informations clés à vos utilisateurs finaux. Heureusement, certaines fonctionnalités peuvent également être comparées dans un panneau standard.

La [visualisation en diagramme de Venn](https://experienceleague.adobe.com/docs/analytics/analyze/analysis-workspace/visualizations/venn.html?lang=en) peut vous aider à créer une comparaison rapide, ce qui vous permet de survoler et de voir les sessions, les commandes, les utilisateurs et utilisatrices, etc. qui se chevauchent entre 2 et 3 segments personnalisés. Vous pouvez également créer rapidement des segments en cliquant avec le bouton droit sur l’une des sections qui se chevauchent :

![Seg 02](assets/s02.png)

Parfois, les informations importantes ne se trouvent pas dans les données qui se chevauchent, mais dans les données qui ne se chevauchent pas. Un moyen rapide de l’afficher consiste à créer une copie d’un segment et à en faire un segment « Exclure » :

![Seg 03](assets/s03.png)

En empilant votre segment « exclure » avec l’autre segment de votre comparaison, vous pouvez désormais calculer rapidement le nombre de visites sur votre page de menu sans afficher également la page d’accueil dans la même session :

![Seg 04](assets/s04.png)

## Attaque par pile

De même, vous pouvez créer les données d’intersection d’un diagramme de Venn en empilant simplement tous les segments. Le nombre de segments ou de dimensions individuelles empilés est illimité. Par exemple, si je voulais rapidement savoir quels jours de la semaine le mois dernier mon site a eu une visite sur un téléphone portable, en particulier un Samsung Galaxy A52, qui a vu mon menu et mes pages nutritionnelles, mais n&#39;a PAS vu ma page d&#39;accueil, je peux le construire rapidement à la volée comme ceci :

![Seg 05](assets/s05.png)

Mais mieux encore, une fois que j’ai trouvé le sous-ensemble parfait de mon utilisateur ou de ma base de visites, je peux sélectionner toutes ces valeurs, effectuer un clic droit et créer un segment instantanément :

![Seg 06](assets/s06.png)

![Seg 07](assets/s07.png)

![Seg 08](assets/s08.png)

C&#39;est beaucoup de puissance dans un segment.

## Un segment de nombres pour un nombre de segments

De nombreux utilisateurs et utilisatrices prennent souvent en compte les valeurs nominales, ordinales ou d’intervalle lors de la création de segments, par exemple une page visitée, une tranche d’âge d’utilisateurs ou le nombre de visites qu’un utilisateur ou une utilisatrice a effectuées dans le passé. Cependant, vous pouvez également utiliser les données de ratio lors de la création d’un segment en regroupant ces valeurs, qu’il s’agisse de dimensions standard, de mesures standard ou de variables et mesures personnalisées pour votre organisation.

Par exemple, Temps passé sur la page ou Temps passé par visite dispose d’intervalles préconfigurés disponibles :

![seg 09](assets/s09.png)

Cependant, elles peuvent ne pas toujours correspondre aux besoins de votre entreprise. Il se peut que la plupart des visites du site durent moins de 10 minutes. Vous pouvez utiliser des mesures granulaires pour créer des intervalles de tailles différentes. En voici un créé pour examiner les visites qui durent entre 1 minute, 1 seconde et 1 minute, 30 secondes :

![Seg 10](assets/s10.png)

Une fois créée, je peux commencer à examiner mes visites, commandes et autres événements en fonction des différents groupes de temps regroupés que j’ai personnalisés :

![seg 11](assets/s11.png)

Vous pouvez même commencer à examiner la façon dont vos indicateurs de performance clés (IPC) changent en fonction du temps passé par un utilisateur, du nombre de pages visitées par celui-ci ou celle qu’il a visitées au cours des dernières visites, ou de toute autre valeur numérique, ce qui vous permet d’examiner une mesure en tant que facteur d’une autre mesure :

![Seg 12](assets/s12.png)

Les possibilités d’utilisation des segments pour trouver de nouvelles informations sont infinies ! Ce n&#39;est qu&#39;un point de départ. Essayez-en quelques-uns vous-même et informez la communauté de ce que vous découvrez : [[!DNL Adobe Analytics] Communauté](https://experienceleaguecommunities.adobe.com/t5/adobe-analytics/ct-p/adobe-analytics-community?profile.language=fr) sur Experience League ou la communauté [#Measure Slack](https://www.measure.chat/).

Bonne segmentation !

## Auteur

Ce document a été rédigé par :

![Dan Cummings ](assets/seg13.png)

**Dan Cummings**, directeur principal des [!DNL Analytics] d&#39;ingénierie des produits chez McDonald&#39;s Corporation

[!DNL Adobe Analytics] Champion
