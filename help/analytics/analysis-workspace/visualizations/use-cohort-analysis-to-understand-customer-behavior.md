---
title: Utilisation de l’analyse des cohortes pour comprendre le comportement des clients
description: Pour améliorer l’expérience client et les recettes, les entreprises doivent comprendre le comportement des clients. L’analyse des cohortes peut vous aider à comprendre l’engagement et la rétention, ce qui entraîne des actions telles que l’amélioration de la création de compte et la création de campagnes pour les mois à volume élevé.
feature-set: Analytics
feature: Cohort Analysis
role: User
level: Experienced
doc-type: Article
last-substantial-update: 2023-05-16T00:00:00Z
jira: KT-13213
thumbnail: KT-13213.jpeg
exl-id: 79392eea-a8b6-4ae2-98ef-6ebbd11d88a0
source-git-commit: 058d26bd99ab060df3633fb32f1232f534881ca4
workflow-type: tm+mt
source-wordcount: '1142'
ht-degree: 0%

---

# Utilisation de l’analyse des cohortes pour comprendre le comportement des clients

Pour améliorer l’expérience client et les recettes, les entreprises doivent comprendre le comportement des clients. L’analyse des cohortes peut vous aider à comprendre l’engagement et la rétention, ce qui entraîne des actions telles que l’amélioration de la création de compte et la création de campagnes pour les mois à volume élevé.

L’analyse des performances numériques est essentielle pour comprendre comment les clients interagissent avec une entreprise et quelles actions peuvent être entreprises pour améliorer leur expérience. Dans cet article de blog, nous allons explorer comment utiliser l’analyse des cohortes pour mieux comprendre le comportement des clients.

## Partie 1 : comparaison des performances numériques entre les premières visites et les visites récurrentes

### Définition de l’état

Un client cherche à comprendre les performances numériques au cours des deux dernières années et envisage de développer un programme de fidélité pour stimuler les performances numériques. Tout d’abord, nous pouvons examiner la combinaison actuelle du site entre les nouveaux utilisateurs et les utilisateurs réguliers afin de comprendre le comportement actuel des deux groupes de visiteurs.

Performances numériques actuelles

1. En 2022, 62 % des commandes provenaient de premières visites, contre 38 % des commandes de visites récurrentes (sujettes aux cookies, aux multiples appareils).
1. Le taux de conversion des nouvelles visites est légèrement plus élevé que celui des visites récurrentes pour les deux visites (11,6 % contre 11,4 %).
1. Par rapport à 2021, les taux de conversion ont diminué dans les deux segments.

![Table des visites](assets/cohort1.png)

## Partie 2 : Analyse des cohortes - Visites Renseignées Produit Global

Pour comprendre l’attractivité du canal numérique et l’opportunité de générer des acheteurs réguliers, la prochaine question à laquelle répondre est : quel est le volume de visiteurs qui reviennent sur le site chaque mois en 2022 ?

### Présentation de l’analyse des cohortes

L’analyse des cohortes est un outil utile pour comprendre comment les cohortes interagissent avec une marque au fil du temps. Pour commencer, nous avons déterminé les questions à répondre :

1. Dans une année donnée, quelle est la période moyenne de rétention par mois ?
1. Quel est le volume des visiteurs sur le site qui reviennent chaque mois au cours d’une année donnée ?
1. Quel est l’impact des connexions sur la rétention ?
1. Existe-t-il des produits spécifiques qui ont entraîné une plus grande rétention ?

Configuration du tableau de cohortes

1. Définir la période sur janvier à décembre 2022
1. **Critères d’inclusion :** visites
1. **Critères de retour :** visites
1. **Granularité :** mois
1. **Paramètres :** Calcul variable
\*\*Permet de calculer la rétention en fonction de la colonne précédente, et non de la colonne incluse. Ainsi, cela signifie qu’un utilisateur est inclus dans chaque mois\*\*
1. **Segments :** vous pouvez sélectionner des segments spécifiques pour approfondir cette analyse.
   1. Pages d’entrée spécifiques
   1. Type d’appareil
   1. Canaux marketing
   1. etc.

### Interprétation des résultats

**En 2022 :**

1) Les mois avec les taux de rétention les plus élevés +1 mois comprennent janvier, avril et novembre
1) Les mois avec le plus grand volume comprennent février et mai
1) ~1 000 visiteurs reviennent sur le site tous les mois

![2022 table de rétention](assets/cohort2.png)

**En 2021 :**

1) Les mois ayant les taux de rétention les plus élevés +1 mois comprennent avril, janvier et mars
1) Les mois avec le plus grand volume comprennent février et mai

![Table de rétention 2021](assets/cohort3.png)

**Éléments d’action :**

Créez un segment basé sur les ~1 000 visiteurs et en savoir plus à leur sujet :

- Où se trouvent-ils ?
- Quels produits achètent-ils tout au long de l&#39;année ?
- De quels magasins achètent-ils ?

Les mois clés mettent en évidence l’opportunité d’augmenter la rétention en fonction du volume :

- Existe-t-il des tactiques spécifiques qui peuvent générer des affinités supplémentaires en février et mai pour tirer parti du volume ?

Analyse répétée des commandes pour comprendre les acheteurs réguliers

- Les taux de rétention des +1 mois sont-ils les plus élevés pour les mêmes mois ?
- Les mois de visites les plus élevés sont-ils les mêmes pour les commandes ?

## Partie 3 : ajout de deux mesures à des critères d’inclusion

### Comprendre l’impact de la connexion

Puisque ce client cherche à comprendre la valeur d’un programme de fidélité, l’étape suivante de l’analyse consiste à ajouter dans l’événement de succès de connexion en tant que mesure d’inclusion à la cohorte.

Avertissement : l’analyse des cohortes ne peut pas être utilisée pour les mesures calculées (telles que le taux de conversion) ou les mesures non entières (telles que les recettes). Seules les mesures pouvant être utilisées dans les segments peuvent être utilisées dans l’analyse des cohortes. Elles ne peuvent être incrémentées que de plus de 1 à la fois.

Le site est-il plus susceptible de retenir les utilisateurs qui se connectent ?

Quel serait l’impact si nous pouvions amener plus d’utilisateurs à se connecter ? Est-ce une expérience plus attrayante ?

### Configuration du tableau de cohortes

1. **Définir la plage de dates :** de janvier à décembre 2022
1. **Critères d’inclusion :** Visites + événement de succès de connexion
1. **Critères de retour :** visites
1. **Granularité :** mois
1. **Paramètres :** Calcul variable
\*\*Permet de calculer la rétention en fonction de la colonne précédente, et non de la colonne incluse. Ainsi, cela signifie qu’un utilisateur est inclus dans chaque mois\*\*

### Interprétation des résultats

**En 2022 :**

1) Les mois ayant les taux de rétention les plus élevés +1 mois comprennent janvier, avril et novembre (les mêmes mois que le premier tableau de cohortes)
1) Les mois avec le plus grand volume comprennent février, mai et décembre
1) ~2 500 visiteurs reviennent chaque mois \*\*plus que le double\*\*

**Éléments d’action :**

Exploration de l’expérience utilisateur du site pour demander aux utilisateurs de créer un compte lors de l’extraction

![Tableau de cohortes 4](assets/cohort4.png)

## Partie 4 : cohorte de Dimension personnalisée

Cohorte de Dimension personnalisée : créez des cohortes en fonction de la dimension sélectionnée, plutôt que des cohortes en fonction du temps (par défaut). De nombreux clients souhaitent analyser leurs cohortes en fonction d’autres éléments que le temps. La nouvelle fonctionnalité Cohorte de Dimension personnalisée vous offre la possibilité de créer des cohortes en fonction des dimensions de leur choix. Utilisez des dimensions telles que le canal marketing, la campagne, le produit, la page, la région ou toute autre dimension dans [!DNL Adobe Analytics] pour afficher l’évolution de la rétention en fonction des différentes valeurs de ces dimensions. La variable

La définition de segment de cohorte de Dimension personnalisée applique l’élément de dimension uniquement dans le cadre de la période d’inclusion, et non dans le cadre de la définition du renvoi.

Après avoir choisi l’option Cohorte de Dimension personnalisée , vous pouvez faire glisser et déposer n’importe quelle dimension dans la zone de dépôt. Vous pouvez ainsi comparer des éléments de dimension similaires sur la même période. Par exemple, vous pouvez comparer les performances des villes côte à côte.

côté, produits, campagnes, etc. Elle renverra vos 14 principaux éléments de dimension. Vous pouvez toutefois utiliser un filtre (accessible en pointant sur la droite de la dimension qui a été glissée dessus) pour afficher uniquement les éléments de dimension de votre choix. Une cohorte de Dimension personnalisée ne peut pas être utilisée avec la fonction Tableau de latence .

### Quels produits sont les moteurs de l’attractivité du site ?

Le tableau Cohorte de Dimension personnalisée met en évidence les produits qui génèrent des taux de rétention supérieurs à la moyenne.  Ce tableau permet d’identifier vos principaux produits afin de piloter des campagnes marketing internes et externes à l’aide de produits dignes d’attention.

**En février :** 3 produits se démarquent avec des taux de rétention plus élevés

1) Produit 1
1) Product 2
1) Product 3

**En mars :**

1) Produit 1
1) Product 2
1) Produit 3 : souvent plus performant avec un taux de rétention plus élevé que la rétention moyenne.

![&#x200B; Table de cohortes 5](assets/cohort5.png)

## Conclusion

L’analyse des cohortes et la cohorte de Dimension personnalisée sont de puissants outils pour comprendre le comportement des clients et améliorer les performances numériques. En analysant les taux de rétention, les taux de connexion et l’impact de produits spécifiques, les entreprises peuvent prendre des décisions basées sur les données afin d’améliorer l’expérience client et de stimuler la croissance.

## Auteur

Ce document a été rédigé par :

![Jennifer Yacenda](assets/jennifer-yacenda.png)

**Jennifer Yacenda&lbrace;1, Senior Director at Marriott**

[!DNL Adobe Analytics] Champion
