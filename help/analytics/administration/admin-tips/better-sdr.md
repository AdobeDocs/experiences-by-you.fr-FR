---
title: Construire une culture des données et une meilleure référence pour la conception de solution
description: Modifiez votre stratégie de données et habilitez votre équipe à créer un document de référence de conception de solution (SDR) solide. Éliminez les écarts de mesure et favorisez une culture collaborative des données au moyen de méthodologies étape par étape.
feature: Implementation Basics
topic: Administration
role: User
level: Experienced
doc-type: Article
duration: 72000
last-substantial-update: 2024-04-25T00:00:00Z
jira: KT-15338
thumbnail: KT-15338.jpeg
exl-id: 99fcf68f-5698-4270-9055-ab224e6323a1
source-git-commit: b2e05ff39e065691dda530ed17762a55cf2e6778
workflow-type: tm+mt
source-wordcount: '1647'
ht-degree: 0%

---

# Construire une culture des données et une meilleure référence de conception de solution

_Modifiez votre stratégie de données et habilitez votre équipe à créer un document de référence de conception de solution (SDR) solide. Éliminer les écarts de mesure et favoriser une culture collaborative des données par des méthodologies pas à pas._

Il est enfin temps. Vous assemblez un solide DTS. Un SDR est le guide que vous utilisez pour implémenter vos mesures et dimensions. Vous avez défini comment on les appelle, quand ils se déclenchent, et vos développeurs adorent ça. Vous avez parcouru tout le processus de déploiement, écrit les critères d&#39;acceptation, parcouru vos empreintes, testé, et c&#39;est fait ! Votre instance de [!DNL Adobe Analytics] doit recevoir les célébrations des équipes marketing et produit lorsqu’elles analysent les données, obtiennent de nouvelles révélations sur vos clients et trouvent tous les domaines de succès et, enfin, les domaines de moindre succès. Mais vous n&#39;entendez pas les louanges que vous attendiez.

D’une équipe, vous entendez des plaintes comme :

&quot;Pourquoi ne puis-je pas déterminer le taux de conversion sur cet entonnoir ?&quot;

&quot;Pourquoi n’y a-t-il pas de mesure pour cela ?&quot;

&quot;J&#39;ai besoin de plus de détails ! Une mesure seule ne suffit pas. Il y a au moins trois dimensions différentes dont j&#39;ai besoin pour comprendre la performance. Pourquoi ne les avez-vous pas mis dedans ?&quot;

Mais c&#39;est l&#39;autre équipe qui est une cause d&#39;inquiétude encore plus grande. D&#39;eux, vous n&#39;entendez rien du tout. Pire encore, vous voyez des graphiques qui ont clairement été extraits de votre ancienne solution d&#39;analyse (celle qui n&#39;est plus entretenue, et qui chaque jour tombe plus loin dans un marécage de décrépitude et de données sales). Un sentiment de terreur vous remplit lorsque vous considérez les décisions qui pourraient être prises avec ce gâchis originel.

_Qu’est-ce qui s’est mal passé ?_

_Pourquoi y a-t-il des écarts dans la mesure ?_

_Pourquoi les membres de votre équipe n’acceptent-ils pas cela ?_

Je vais commencer en vous laissant sortir légèrement du crochet. _sera toujours_ une révision. Si votre site ou application est suffisamment complexe pour avoir besoin d’une solution d’analyse d’entreprise, il est garanti que vous manquerez quelque chose. Mais dans ce cas, vous n&#39;avez pas manqué d&#39;expliquer les écarts de mesure que je décris.

Ce qui s&#39;est mal passé est beaucoup plus difficile à mettre dans une feuille de calcul. Essentiellement, vous avez manqué votre première chance de créer une culture de données collaborative lors de la création de votre DTS.

Je veux vous guider à travers une méthode que mes collègues et moi-même avons développée pour à la fois créer un meilleur DTS avec moins d&#39;écarts, et pour que les utilisateurs finaux investissent (et même parfois enthousiastes) sur leur nouvelle instance de [!DNL Adobe Analytics]. Passons en revue comment et pourquoi vous devriez considérer cette méthode.

## Comment

_Découvrez la conférence sur les mesures. Utilisez une carte d’entonnoir pour visualiser chaque étape de votre plan. Créez des tableaux de bord fictifs à réviser en tant que groupe. Créez un dictionnaire de données pour les utilisateurs._

### Conférence sur les mesures

1. Rassemblez vos parties prenantes, en personne ou virtuellement, dans le but de découvrir ce qu’il faut mesurer. Cette réunion devrait inclure des cadres.
1. Vous trouverez des exemples évidents dans les post-it, tels que les recettes, les ventes ou les pistes, les indicateurs clés de produit (IPC) que vous connaissez seront mesurés. Répétez cette procédure avec des dimensions telles que l’état de connexion, les catégories de produits ou les termes de recherche.
1. Demandez à chacun d’ajouter ses propres post-it, en les regroupant selon les besoins.
1. Demandez aux gens de voter sur ceux qu&#39;ils trouvent importants. Ce sont des votes illimités car toutes ces mesures et dimensions ont probablement de l&#39;importance.
1. Pour toutes les mesures et dimensions qui ont des votes faibles, demandez aux parties prenantes qui les ont demandées d’expliquer pourquoi ces composants seraient utilisés. S&#39;il y a un bon cas d&#39;utilisation, conservez ces composants. S’il existe un meilleur moyen d’obtenir ces données, ou si personne ne peut expliquer comment ces données peuvent être exploitées, ou s’il existe une autre bonne raison de supprimer les mesures et dimensions, faites-le.
1. Ajoutez ces mesures et dimensions à votre DTS pour une révision initiale par les parties prenantes présentes.

### Cartographie de l’entonnoir

1. Obtenez une visualisation de tous les entonnoirs, étape par étape avec chaque état inclus.
1. Avec les concepteurs et les responsables de produits, passez en revue chaque étape et discutez de ce que tout le monde considère comme un succès dans cet entonnoir. S’agit-il du taux de conversion ? Choisit-il un chemin particulier ? Utilise-t-il certaines fonctionnalités ?
1. Posez des questions sur les mesures et dimensions nécessaires pour comprendre les performances de l’entonnoir à chaque étape de l’entonnoir et dans son ensemble.
1. Au-dessus de chaque étape de l’entonnoir, ajoutez les mesures et les dimensions qui sont mesurées à cette étape, y compris les mesures calculées.
1. Au début de chaque entonnoir, écrivez les rapports qui s’affichent dans le tableau de bord que le chef de produit peut utiliser pour effectuer le suivi des performances. Ces rapports incluent un [ rapport d’abandons ](https://experienceleague.adobe.com/en/docs/analytics/analyze/analysis-workspace/visualizations/fallout/fallout-flow), un [ mois en cours ](https://experienceleague.adobe.com/en/docs/analytics/analyze/analysis-workspace/components/calendar-date-ranges/custom-date-ranges), des [ taux de conversion de tendance ](https://experienceleague.adobe.com/en/docs/analytics/analyze/analysis-workspace/visualizations/line) et tout ce qui est plus spécifique à cet entonnoir.
1. Ajoutez les nouvelles mesures et dimensions que vous avez découvertes au SDR et envoyez-les aux parties prenantes pour une deuxième révision.

### Tableaux de bord d’aperçu

1. À l’aide de la carte d’entonnoir comme guide, créez des tableaux de bord de simulation.
1. Il doit y avoir une vue globale, telle qu’un [tableau de bord du résumé de l’exécution](driving-success-with-executive-summary-dashboards.md) et des tableaux de bord pour chacun des entonnoirs.
1. Il y en aura également d’autres plus spécifiques à votre site ou application, comme les performances du produit ou les performances du contenu.
1. Distribuez-les aux parties prenantes concernées et obtenez des commentaires sur la conception.
1. Effectuez les mises à jour demandées et, si de nouvelles mesures ou dimensions sont nécessaires, ajoutez-les à votre SDR.
1. Envoyez les tableaux de bord et le SDR d’aperçu mis à jour pour une révision finale.

### Outils de démocratisation des données

1. Créez un dictionnaire de données. Le SDR est destiné aux développeurs, mais le dictionnaire de données est destiné aux utilisateurs finaux. Rendez-le lisible afin que chacun puisse facilement rechercher les données disponibles et savoir les utiliser. Les utilisateurs finaux doivent en être les approbateurs finaux.
1. Annotez. Dans chaque organisation, il y a certaines dates qui comptent chaque année et d&#39;autres qui vont apparaître. Veillez à collecter les dates appropriées auprès des parties prenantes et ajoutez-les en tant qu’annotations afin de mieux comprendre les données qu’elles affichent.
1. Traitez. Si votre DTS est grand, il pourrait être écrasant. La paralysie du choix ne s&#39;applique pas seulement à vos clients. Découvrez ce qui importe à chaque groupe d’utilisateurs et traitez les éléments qu’ils verront.

## La raison

_Découvrez les exigences en matière de collecte, de création d’une culture des données, d’amorçage de données approfondies, de création d’un sentiment de propriété sur les données et de simplification des données._

### Collecte des exigences

Rassembler les exigences est une méthode évidente, mais il existe plusieurs façons efficaces de le faire. J&#39;ai utilisé des interviews individuelles, des questionnaires et des révisions de rapports existants. Ces stratégies fonctionnent, mais pas aussi bien que les méthodes que je viens de décrire. cependant, je ne pense pas que la différence entre les méthodes de collecte des exigences soit significative. La méthode que j&#39;ai décrite vous donne 95% du chemin, et ces autres méthodes vous donnent 90% du chemin.

Alors, qu&#39;est-ce que le _pourquoi_ ?

### Créer une culture des données

Dans ce processus, vous :

* Spark réfléchit en détail à la manière de mesurer le succès
* Créer un sentiment de propriété dans vos parties prenantes
* Faciliter la compréhension des données par les parties prenantes

### Spark profonde réflexion sur les données

Pour la plupart des personnes de votre entreprise, les données sont quelque chose qu&#39;elles consomment. Ils l&#39;utilisent. Ils l&#39;analysent. Ils n&#39;y réfléchissent pas profondément. Certaines personnes ont hérité des rapports et processus de leurs prédécesseurs, mais ne les ont pas modifiés pour assurer la continuité. Peut-être que ces personnes n&#39;ont jamais eu besoin de penser au _pourquoi_ des données.

Ce processus leur donne la possibilité de vraiment _comprendre_ les données. Poser des questions comme Qu&#39;est-ce que le succès ? Comment sauriez-vous si vous réussissiez ? Comment sauriez-vous quoi changer si vous n&#39;aviez pas réussi ? Il faut répondre à ces questions au début de la création de chaque site, application et produit, mais bien trop souvent, ce n&#39;est pas le cas. En posant ces questions, vous aidez à approfondir la compréhension qu&#39;une personne a non seulement des données, mais aussi de leur produit.

### Créer un sentiment de propriété sur les données

Un sentiment de propriété n&#39;est pas quelque chose qu&#39;une personne acquiert facilement. On ne le trouve pas dans cette réunion de trente minutes à laquelle on a assisté il y a trois mois. Il n’est pas créé par le fait qu’un questionnaire embêtant auquel ils ont répondu trop rapidement soit dû à d’autres problèmes de travail urgents tels que les démonstrations et les dates de publication du sprint.

La propriété est le produit d&#39;une profonde réflexion et de leur travail avec vous et vos collègues. C&#39;est ce qu&#39;ils ont cherché à plusieurs reprises, pour lequel ils ont fourni des commentaires constants, et ce qu&#39;ils ont approuvé après que ces commentaires ont été incorporés. C&#39;est la leur ! Le fait que c&#39;est utile est dû à eux. Ce sont leurs _données_ et c&#39;est ce processus qui en a fait les leurs.

### Simplification des données

Vous leur avez également expliqué comment ils utiliseront le processus et à quoi il ressemblera dans les [tableaux de bord de prévisualisation](#the-preview-dashboards). Toute nouvelle solution est _hard_. Il y a tant à apprendre, et compte tenu de l’énorme personnalisation de [!DNL Adobe Analytics], la courbe d’apprentissage peut être raide. Vous en avez pourtant supprimé 80%. Même avant la rédaction de la première ligne de code, les parties prenantes savent à quoi ressemblera leur tableau de bord. Ils sauront les lire et leur donner du sens. Ils sauront à quoi ressemble littéralement le succès parce qu’ils vous ont dit quelles mesures et dimensions définissent le succès. Et vous leur avez dit comment ce succès sera visualisé pour eux. La diffusion des tableaux de bord réels est une actualisation, et non une nouvelle tâche d’apprentissage effrayante.

Ce n&#39;est pas nécessairement le moyen le plus rapide de rassembler un DTS. C&#39;est beaucoup de travail et ça nécessite beaucoup de coordination des horaires, surtout qu&#39;il est vital que vous ayez des cadres dans le mélange. En fin de compte, cependant, une solution d’analyse d’entreprise est un énorme investissement de temps et d’argent, et vous voulez vous assurer que l’adoption et la satisfaction sont élevées. Cette méthode fait beaucoup pour que cela arrive.

**Auteur**

Ce document a été rédigé par :

![gitai-headshot](assets/gitai-headshot-150.jpg)

Gitai Ben-Ammi, directeur associé de l&#39;architecture commerciale chez Accenture

[!DNL Adobe Analytics] Champion
