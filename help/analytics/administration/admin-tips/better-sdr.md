---
title: Créer une culture de données et une meilleure conception de solution Référence
description: Révolutionnez votre stratégie de données et permettez à votre équipe de créer un document de référence de conception de solution (SDR) solide. Éliminez les écarts de mesure et favorisez une culture collaborative des données au moyen de méthodologies étape par étape.
feature: Implementation Basics
topic: Administration
role: User
level: Experienced
doc-type: Article
duration: 72000
last-substantial-update: 2024-04-25T00:00:00.000Z
jira: KT-15338
thumbnail: KT-15338.jpeg
exl-id: 99fcf68f-5698-4270-9055-ab224e6323a1
product_v2:
  - id: fd1f54a9-f50c-467d-8956-cebbaf4f3eb8
    internal-label: Experience Manager
  - id: c68cd75e-5bca-4bc3-a60e-9e183f816441
    internal-label: Experience Manager Cloud Manager
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
source-git-commit: 749b293ab38b8ea5a5f72517bd5c3455399137c2
workflow-type: tm+mt
source-wordcount: '1692'
ht-degree: 0%
---
# Créer une culture de données et une meilleure référence en matière de conception de solutions

_Révolutionnez votre stratégie de données et permettez à votre équipe de créer un document de référence de conception de solution (SDR) solide. Éliminer les lacunes en matière de mesure et favoriser une culture de données collaborative au moyen de méthodologies étape par étape._

C&#39;est enfin l&#39;heure. Vous avez mis en place un solide RDS. Une SDR est le guide que vous utilisez pour implémenter vos mesures et dimensions. Vous avez défini leur nom, quand ils se déclenchent, et vos développeurs l&#39;adorent. Vous avez suivi tout le processus de déploiement, rédigé les critères d’acceptation, examiné vos sprints, les avez testés, et c’est fait ! Votre instance de [!DNL Adobe Analytics] doit faire en sorte que les équipes marketing et produit se réjouissent en explorant les données, obtiennent de nouvelles révélations sur vos clients et trouvent tous les domaines de succès et, enfin, les domaines de moins bon succès. Mais vous n&#39;entendez pas les éloges que vous attendiez.

Une équipe vous adresse des plaintes telles que :

« Pourquoi ne puis-je pas calculer le taux de conversion sur ce funnel ? »

« Pourquoi n’existe-t-il pas de mesure pour cela ? »

« J&#39;ai besoin de plus de détails ! Une mesure seule ne suffit pas. Il existe au moins trois dimensions différentes que je dois comprendre en termes de performances. Pourquoi ne les avez-vous pas mis dedans ? »

Mais c&#39;est l&#39;autre équipe qui est encore plus préoccupante. D&#39;eux, vous n&#39;entendez rien du tout. Pire encore, vous voyez des graphiques qui proviennent clairement de votre ancienne solution d’analyse (celle qui n’est plus gérée et qui, chaque jour, s’enfonce davantage dans un marais de décrépitude et de données corrompues). Un sentiment d&#39;appréhension vous emplit lorsque vous réfléchissez aux décisions qui pourraient être prises avec ce gâchis original.

_Que s’est-il passé ?_

_Pourquoi y a-t-il des lacunes dans la mesure ?_

_Pourquoi les membres de votre équipe n’adoptent-ils pas cela ?_

Je vais commencer par vous laisser un peu tranquille. Il y aura _toujours_ une certaine révision. Si votre site ou votre application est suffisamment complexe pour nécessiter une solution d’analyse d’entreprise, il est certain que vous allez passer à côté de quelque chose. Mais dans ce cas-ci, vous n&#39;avez pas manqué assez d&#39;explications pour expliquer les écarts de mesure que je décris.

Ce qui a mal tourné est beaucoup plus difficile à mettre dans une feuille de calcul. Essentiellement, vous avez manqué votre première chance de créer une culture de données collaborative pendant que vous élaboriez votre SDR.

Je souhaite vous présenter une méthode que mes collègues et moi avons développée pour créer un meilleur SDR avec moins d’écarts et pour inciter les utilisateurs finaux à investir (et même parfois à s’enthousiasmer) dans leur nouvelle instance de [!DNL Adobe Analytics]. Examinons comment et pourquoi vous devez envisager cette méthode.

## Le comment

_En savoir plus sur la conférence de mesure. Utilisez une carte funnel pour visualiser chaque étape de votre plan. Créez des tableaux de bord simulés à examiner en tant que groupe. Créez un dictionnaire de données pour les utilisateurs._

### La conférence sur la mesure

1. Réunissez vos parties prenantes, en personne ou virtuellement, dans le but de découvrir ce qu&#39;il faut mesurer. Cette réunion devrait inclure quelques cadres.
1. Disposez déjà d’exemples évidents sur le tableau concernant les pense-bêtes, tels que les recettes, les ventes ou les prospects, les indicateurs clés de produit (IPC) que vous savez être mesurés. Répétez l’opération avec des dimensions telles que le statut de connexion, les catégories de produits ou les termes de recherche.
1. Demandez à chacun d’ajouter ses propres notes autocollantes, en les regroupant si nécessaire.
1. Demandez aux gens de voter sur ceux qu&#39;ils jugent importants. Il s’agit de votes illimités, car toutes ces mesures et dimensions ont probablement de l’importance.
1. Pour les mesures et dimensions qui ont des votes faibles, demandez aux parties prenantes qui les ont demandées d’expliquer pourquoi ces composants seraient utilisés. S’il existe un bon cas d’utilisation, conservez ces composants. S’il existe un meilleur moyen d’obtenir ces données, ou si personne ne peut expliquer comment ces données sont exploitables, ou s’il existe une autre bonne raison de supprimer les mesures et les dimensions, faites-le.
1. Ajoutez ces mesures et dimensions à votre SDR en vue d’une révision initiale par les parties prenantes présentes.

### La carte funnel

1. Obtenez une visualisation de tous les entonnoirs, étape par étape avec chaque état inclus.
1. Avec les concepteurs et les chefs de produit, passez en revue chaque étape et discutez de ce que chacun considère comme le succès dans ce funnel. Est-ce le taux de conversion ? Choisit-elle une voie en particulier ? Utilise-t-il certaines fonctionnalités ?
1. Posez des questions sur les mesures et dimensions nécessaires pour comprendre les performances de funnel à chaque étape du funnel et de manière globale.
1. Au-dessus de chaque étape du funnel, ajoutez les mesures et dimensions qui sont mesurées à cette étape, y compris les mesures calculées.
1. Au début de chaque funnel, écrivez les rapports qui se trouvent dans le tableau de bord que le chef de produit peut utiliser pour effectuer le suivi des performances. Ces rapports incluent un [rapport sur les abandons](https://experienceleague.adobe.com/fr/docs/analytics/analyze/analysis-workspace/visualizations/fallout/fallout-flow), [mois en cours](https://experienceleague.adobe.com/fr/docs/analytics/analyze/analysis-workspace/components/calendar-date-ranges/custom-date-ranges), [taux de conversion en tendance](https://experienceleague.adobe.com/fr/docs/analytics/analyze/analysis-workspace/visualizations/line) et tout élément plus spécifique à ce funnel.
1. Ajoutez les nouvelles mesures et dimensions que vous avez découvertes à la SDR et envoyez-les aux parties prenantes pour une deuxième révision.

### Les tableaux de bord de prévisualisation

1. À l’aide de la carte funnel comme guide, créez des tableaux de bord de maquette.
1. Il doit y avoir une vue d’ensemble, telle qu’un [&#x200B; Tableau de bord du résumé exécutif](driving-success-with-executive-summary-dashboards.md) et des tableaux de bord pour chacun des entonnoirs.
1. Il y aura également des options plus spécifiques à votre site ou application, telles que les performances du produit ou les performances du contenu.
1. Distribuez-les aux parties prenantes concernées et obtenez des commentaires sur la conception.
1. Effectuez les mises à jour demandées et, si de nouvelles mesures ou dimensions sont nécessaires, ajoutez-les à votre SDR.
1. Envoyez les tableaux de bord de prévisualisation mis à jour et la SDR pour une révision finale.

### Outils de démocratisation des données

1. Créez un dictionnaire de données. La SDR est destinée à vos développeurs, mais le dictionnaire de données est destiné à vos utilisateurs finaux. Rendez-le lisible afin que tout le monde puisse facilement rechercher les données disponibles et savoir comment les utiliser. Vos utilisateurs finaux doivent en être les approbateurs finaux.
1. Annoter. Dans chaque organisation, il y a des dates qui comptent chaque année et d&#39;autres qui vont se présenter. Veillez à collecter les dates pertinentes auprès de vos parties prenantes et à les ajouter en tant qu’annotations pour améliorer la compréhension des données qu’elles voient.
1. Organisez. Si votre SDR est volumineux, il peut être écrasant. La paralysie de choix ne s&#39;applique pas seulement à vos clients. Découvrez ce qui importe à chaque groupe d’utilisateurs et d’utilisatrices, ainsi que les éléments qu’ils verront.

## Le pourquoi

_Découvrez les exigences de la collecte de données, la création d’une culture de données, l’éveil d’une réflexion approfondie sur les données, la création d’un sentiment d’appartenance à l’égard des données et la simplification des données._

### Rassembler les exigences

La collecte des exigences est évidente, mais il existe plusieurs façons efficaces de le faire. J&#39;ai eu recours à des entrevues individuelles, à des questionnaires et à des examens de rapports existants. Ces stratégies fonctionnent, mais pas aussi bien que les méthodes que je viens de décrire. Cependant, je ne pense pas que la différence entre les méthodes de collecte des exigences soit importante. La méthode que j&#39;ai décrite vous conduit à 95 % du chemin, et ces autres méthodes vous conduisent à 90 % du chemin.

Alors, quel est le _pourquoi_ ?

### Créer une culture de données

Dans ce processus, vous :

* Suscitez une réflexion approfondie sur la manière de mesurer le succès
* Créez un sentiment d’appropriation chez vos parties prenantes.
* Faciliter la compréhension des données pour les parties prenantes

### Susciter une réflexion approfondie sur les données

Pour de nombreuses personnes au sein de votre entreprise, les données sont une chose qu’elles consomment. Ils l&#39;utilisent. Ils l&#39;analysent. Ils n&#39;y pensent pas sérieusement. Certaines personnes ont hérité de rapports et de processus de leurs prédécesseurs, mais ne les ont pas modifiés par souci de continuité. Peut-être que ces gens n&#39;ont jamais eu besoin de penser au _pourquoi_ des données.

Ce processus leur donne l&#39;occasion de vraiment _comprendre_ les données. Poser des questions comme : Qu’est-ce que le succès ? Comment le sauriez-vous si vous réussissiez ? Comment sauriez-vous quoi changer si vous n&#39;aviez pas réussi ? Ces questions doivent être résolues au début de la création de chaque site, application et produit, mais bien trop souvent, elles ne le sont pas. En posant ces questions, vous aidez une personne à mieux comprendre non seulement les données, mais également leur produit.

### Créer un sentiment d’appropriation des données

Un sentiment d&#39;appartenance n&#39;est pas quelque chose qu&#39;une personne acquiert facilement. On ne le trouve pas dans la réunion de trente minutes à laquelle les participants ont assisté il y a trois mois. Cela ne crée pas un questionnaire ennuyeux auquel ils répondent trop rapidement en raison d&#39;autres problèmes de travail urgents tels que les démonstrations et les dates de publication du sprint.

L&#39;appropriation est le produit de la réflexion profonde d&#39;une personne et de son travail avec vous et vos collègues. C&#39;est ce qu&#39;ils ont examiné à plusieurs reprises, pour lequel ils ont fourni une rétroaction continue, et ce qu&#39;ils ont approuvé après que cette rétroaction a été intégrée. C&#39;est à eux ! C&#39;est grâce à eux que c&#39;est utile. Ce sont _leurs données_ et c&#39;est ce processus qui les a rendues les leurs.

### Simplifier les données

Vous leur avez également montré comment ils utiliseront le processus et à quoi il ressemblera dans les [tableaux de bord de prévisualisation](#the-preview-dashboards). Toute nouvelle solution est _difficile_. Il y a tant à apprendre, et étant donné l&#39;énorme personnalisation de [!DNL Adobe Analytics], la courbe d&#39;apprentissage peut être abrupte. Vous en avez retiré 80 %. Avant même que la première ligne de code ait été écrite, vos parties prenantes savent à quoi ressembleront leurs tableaux de bord. Ils sauront les lire et en tirer un sens. Ils sauront à quoi ressemble littéralement le succès, car ils vous ont dit quels indicateurs et dimensions définissent le succès. Et vous leur avez dit comment ce succès sera visualisé pour eux. La diffusion des tableaux de bord réels est un rafraîchissement, pas une nouvelle tâche d&#39;apprentissage effrayante.

Ce n&#39;est pas nécessairement la façon la plus rapide de rassembler un document SDR. C&#39;est beaucoup de travail et cela exige beaucoup de coordination des horaires, d&#39;autant plus qu&#39;il est vital que vous ayez des cadres dans la combinaison. En fin de compte, une solution d’analyse d’entreprise représente un investissement considérable en temps et en argent. Vous devez donc vous assurer que l’adoption et la satisfaction sont élevées. Cette méthode fait beaucoup pour que cela se produise.

**Auteur**

Ce document a été rédigé par :

![gitai-headshot](assets/gitai-headshot-150.jpg)

Gitai Ben-Ammi, directeur associé, Architecture d’entreprise chez Accenture

[!DNL Adobe Analytics] Champion
