---
title: Construire une culture des données et une meilleure référence de conception de solution
description: Modifiez votre stratégie de données et habilitez votre équipe à créer un document de référence de conception de solution (SDR) solide. Éliminer les écarts de mesure et favoriser une culture collaborative des données au moyen de méthodologies étape par étape.
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
source-git-commit: b3b98aee5ee23e323a9bc762c673700b02366f4c
workflow-type: tm+mt
source-wordcount: '1640'
ht-degree: 0%

---

# Construire une culture des données et une meilleure référence de conception de solution

**Modifiez votre stratégie de données et habilitez votre équipe à créer un document de référence de conception de solution (SDR) solide. Éliminer les écarts de mesure et favoriser une culture collaborative des données au moyen de méthodologies étape par étape.**

Il est enfin temps. Vous avez créé une référence solide de conception de solution (DTS). Il s’agit du guide que vous utilisez pour implémenter vos mesures et dimensions, ce qu’elles sont appelées, quand elles se déclenchent, et que vos appareils l’ont adoré. Vous avez parcouru l&#39;ensemble du processus de déploiement, écrit les critères d&#39;acceptation, parcouru vos empreintes, QAing tout le processus, et c&#39;est fait ! C&#39;était beaucoup de travail, et maintenant c&#39;est fait. Votre instance d’Adobe Analytics doit faire passer le marketing et les produits de haut en bas au fur et à mesure qu’ils analysent les données, obtiennent de nouvelles révélations sur vos clients, et trouvent tous les domaines de succès et, enfin, les domaines de moindre succès. Mais vous n&#39;entendez pas les louanges que vous attendiez.

D&#39;un camp, vous entendez des plaintes.

&quot;Pourquoi ne puis-je pas déterminer le taux de conversion sur cet entonnoir ?&quot;

&quot;Pourquoi n’y a-t-il pas de mesure pour cela ?&quot;

&quot;J&#39;ai besoin de beaucoup plus de détails à ce sujet ! Une mesure seule ne suffit pas. Il y a au moins trois dimensions différentes dont j’ai besoin pour comprendre les performances. Pourquoi ne les avez-vous pas mis dedans ?&quot;

Mais c&#39;est l&#39;autre camp qui est une cause d&#39;inquiétude encore plus grande. D&#39;eux, vous n&#39;entendez rien du tout. Mais bien pire, vous voyez des graphiques qui ont été très clairement extraits de votre ancienne solution d&#39;analyse, vous savez, celle qui n&#39;est plus entretenue, et chaque jour tombe plus dans un marécage de décrépitude et de données sales. Un sentiment de terreur vous remplit quand vous pensez aux décisions qui pourraient être prises avec ce désordre.

Qu&#39;est-ce qui s&#39;est mal passé ? Pourquoi y a-t-il des écarts dans les mesures ? Pourquoi les membres de votre équipe n&#39;acceptent-ils pas cela ?

Je vais commencer en vous laissant sortir un peu du crochet. Il y a *always* ce sera une révision. Si votre site ou application est suffisamment complexe pour avoir besoin d’une solution d’analyse d’entreprise, il est pratiquement garanti que vous manquerez quelque chose. Mais pas assez pour expliquer les écarts de mesures dont je parle ici. Ce qui s&#39;est mal passé est beaucoup plus difficile à mettre dans une feuille de calcul. Vous avez manqué vos premières chances de créer une culture de données collaborative au moment même où vous avez créé votre DTS. Je veux vous guider à travers une méthode que mes collègues et moi-même avons développée pour à la fois construire un meilleur DTS avec moins d&#39;écarts, et pour que les utilisateurs finaux soient investis et même parfois enthousiasmés par leur nouvelle instance d&#39;Adobe Analytics. Passons en revue les hows et les pourquoi.

**Comment**

***La conférence sur la mesure :***

1. Rassemblez vos parties prenantes, soit en personne, soit virtuellement dans le but de découvrir ce qu’il faut mesurer. Cela devrait inclure des exécutions.
1. Ayez déjà quelques exemples évidents sur le tableau des pense-bêtes, des éléments comme les recettes, les ventes ou les pistes, les indicateurs clés de performance que vous connaissez seront mesurés. Répétez cette procédure avec des dimensions, des éléments tels que l’état de connexion, les catégories de produits ou les termes de recherche.
1. Demandez à chacun d’ajouter ses propres post-it, en les regroupant selon les besoins.
1. Que les gens votent sur ceux qu&#39;ils pensent importants. Ce sont des votes illimités puisque peut-être toutes ces mesures et dimensions comptent.
1. Pour tous ceux qui ont des votes faibles, demandez aux parties prenantes d&#39;expliquer à quoi elles les utiliseront. S&#39;il y a un bon cas d&#39;utilisation, gardez-le dedans. S&#39;il y a un meilleur moyen d&#39;obtenir ces données, elles ne peuvent pas expliquer comment elles sont exploitables, ou il y a une autre bonne raison de les laisser de côté, de les frapper du tableau.
1. Ajoutez ces mesures et dimensions à votre DTS pour une révision initiale par les parties prenantes présentes.

***Cartographie des entonnoirs***

1. Obtenir une visualisation de tous les entonnoirs, étape par étape avec chaque état inclus
1. Avec les designers et les chefs de produits, passez en revue chaque étape et expliquez ce qu&#39;ils considèrent comme du succès dans cet entonnoir. S’agit-il d’un taux de conversion ? Choisit-il un chemin particulier ? Utilise-t-il certaines fonctionnalités ?
1. Posez des questions sur les mesures et dimensions nécessaires pour comprendre les performances de l’entonnoir à chaque étape de l’entonnoir et dans son ensemble.
1. Au-dessus de chaque étape de l’entonnoir, ajoutez les mesures et les dimensions qui seront mesurées à cette étape, y compris les mesures calculées.
1. Au début de chaque entonnoir, écrivez les rapports qui s’afficheront dans le tableau de bord que le chef de produit utilisera pour effectuer le suivi des performances, comme un rapport d’abandons, les taux de conversion du mois en cours et des tendances, et tout ce qui est plus spécifique à cet entonnoir.
1. Ajoutez les nouvelles mesures et dimensions que vous avez découvertes au SDR et envoyez-les aux parties prenantes pour une deuxième révision.

***Tableaux de bord d’aperçu***

1. À l’aide de la carte Entonnoir , créez des tableaux de bord de maquette.
1. Il doit y avoir une vue globale, telle qu’une [Tableau de bord du résumé exécutif](driving-success-with-executive-summary-dashboards.md)et les tableaux de bord pour chacun des entonnoirs.
1. Il y en aura également d’autres plus spécifiques à votre site ou application, comme les performances du produit ou les performances du contenu.
1. Distribuez-les aux parties prenantes concernées et obtenez des commentaires sur la conception.
1. Effectuez les mises à jour demandées et, si de nouvelles mesures ou dimensions sont nécessaires, ajoutez-les à votre SDR.
1. Envoyez les tableaux de bord et le SDR d’aperçu mis à jour pour une révision finale.

***Outils de démocratisation des données***

1. Créez un dictionnaire de données. Le DTS est destiné à vos appareils. Le dictionnaire de données est destiné aux utilisateurs finaux. Rendre ces données lisibles pour les utilisateurs finaux afin qu’ils puissent facilement rechercher les données disponibles et savoir les utiliser. Les utilisateurs finaux doivent en être les approbateurs finaux.
1. Annotations. Dans chaque organisation, il y a certaines dates qui comptent chaque année et d&#39;autres qui vont apparaître. Veillez à rassembler les informations pertinentes auprès de vos parties prenantes et à les ajouter en tant qu’annotations afin de mieux comprendre les données qu’elles affichent.
1. Traitement. Si votre DTS est grand, il pourrait être écrasant. La paralysie du choix ne s&#39;applique pas seulement à vos clients. Découvrez ce qui importe à chaque groupe d’utilisateurs et traitez les éléments qu’ils verront.

**Pourquoi**

***Obtention Des Exigences***

C&#39;est évident, mais il y a d&#39;autres moyens efficaces d&#39;obtenir les besoins. J&#39;en ai personnellement utilisé un sur un seul entretien, questionnaires et révisions de rapports existants. Ça marchera, même si je ne pense pas aussi bien que les méthodes que je viens de décrire. Je ne pense vraiment pas que l&#39;écart dans la collecte des exigences soit aussi important. La méthode que j&#39;ai décrite vous permettra d&#39;y parvenir à 95 %, et ces autres méthodes vous donneront 90 % du chemin. Alors, quelle est la grande raison ?

***Pour créer une culture des données***

Grâce à ce processus, vous :

- Spark réfléchit en détail à la manière de mesurer le succès
- Créer un sentiment de propriété dans vos parties prenantes
- Faciliter la compréhension des données par les parties prenantes

***Lancer une réflexion approfondie sur les données***

Pour la plupart des personnes de votre entreprise, les données sont quelque chose qu&#39;elles consomment. Ils l&#39;utilisent. Ils l&#39;analysent. Ils n&#39;y réfléchissent pas profondément. Certains d’entre eux ont hérité des rapports et processus de leurs prédécesseurs, mais ils n’ont pas changé en raison de la nécessité de continuité. Ils n&#39;ont jamais eu besoin de penser à la raison des données.

Ce processus leur donne l&#39;opportunité de vraiment *comprendre* data. En posant les questions, qu&#39;est-ce que le succès ? Comment sauriez-vous si vous réussissiez ? Comment sauriez-vous quoi changer si vous n&#39;aviez pas réussi ? Il s’agit d’un exercice qui doit être effectué au début de la création de chaque site, application et produit, mais qui bien trop souvent ne l’est pas. En posant ces questions, vous aidez à approfondir leur compréhension non seulement des données, mais aussi de leur propre produit.

***Création d’un sentiment de propriété sur les données***

Ce n&#39;est pas quelque chose qui a été distribué haut. Ce n&#39;est pas une réunion de trente minutes il y a trois mois. Ce n&#39;est pas un questionnaire si ennuyeux qu&#39;ils ont été traqués pendant une semaine pour y répondre et qu&#39;ils l&#39;ont fait pressé parce qu&#39;ils avaient une démonstration pour arriver à afin qu&#39;ils puissent faire la date de publication du sprint. C&#39;est le produit de leur profonde réflexion et de leur travail avec vous et leurs collègues, ce qu&#39;ils ont cherché plusieurs fois, qui a fourni des commentaires constants, et qu&#39;ils ont approuvé après que ce retour a été intégré. C&#39;est la leur ! Le fait que c&#39;est utile est dû à eux. C&#39;est *leur* et c&#39;est le processus qui en a fait la leur.

***Faciliter la compréhension des données***

Vous leur avez également montré comment ils l’utiliseront et à quoi il ressemblera dans les tableaux de bord de prévisualisation. Toute nouvelle solution *hard*. Il y a tellement de choses à apprendre et compte tenu de l’énorme personnalisation d’Adobe Analytics, la courbe d’apprentissage peut être assez raide. Vous en avez pourtant supprimé 80%. Même avant la rédaction de la première ligne de code, les parties prenantes savent à quoi ressemblera leur tableau de bord. Ils sauront les lire et leur donner du sens. Ils sauront à quoi ressemble littéralement le succès parce qu&#39;ils vous ont dit quelles mesures et dimensions définissent le succès, et vous leur avez dit comment cela sera visualisé pour eux. La diffusion des tableaux de bord réels est une actualisation, et non une nouvelle tâche d’apprentissage effrayante.

Ce n&#39;est pas le moyen le plus rapide de rassembler un DTS. C&#39;est beaucoup de travail et ça nécessite beaucoup de coordination des horaires, surtout qu&#39;il est vital que vous ayez des cadres dans le mélange. En fin de compte, une solution d’analyse d’entreprise est un investissement énorme en temps et en argent, et vous voulez vous assurer que l’adoption et la satisfaction sont élevées. Cette méthode fait beaucoup pour que cela arrive.

**Auteur**

Ce document a été rédigé par :

![capture d’écran de Gitai](assets/gitai-headshot-150.jpg)

Gitai Ben-Ammi, directeur associé de l&#39;architecture commerciale chez Accenture

Adobe Analytics Champion
