---
title: Guide complet pour la transition vers [!DNL Adobe Analytics] de Google [!DNL Analytics]
description: Découvrez l’emplacement d’une fonctionnalité équivalente et comment l’utiliser efficacement lors de la transition depuis Google [!DNL Analytics] to [!DNL Adobe Analytics]
solution: Analytics
feature: Third-party Integration
role: User
level: Beginner
kt: 9830
thumbnail: 34749.jpg
source-git-commit: c6c9e5b19c601592811151450aecd8dfdd084ff6
workflow-type: tm+mt
source-wordcount: '3323'
ht-degree: 72%

---

# Guide complet pour la transition vers [!DNL Adobe Analytics] de Google [!DNL Analytics]{#comprehensive-guide-for-transitioning-to-adobe-analytics}

## 1. Introduction

L’un des plus grands défis de la transition entre des outils est d’apprendre où trouver des fonctionnalités équivalentes et à les utiliser efficacement. Cette discussion fait partie d’un guide plus vaste pour aider les utilisateurs à passer à [!DNL Adobe Analytics] (soit en tant que nouvel utilisateur, soit en provenance de Google) [!DNL Analytics]) plus facile. Une comparaison approfondie avec Google Analytics, l’outil comparatif que la plupart des utilisateurs connaîtront, est fournie pour aider les utilisateurs à mettre en relation les connaissances existantes avec le nouvel ensemble d’outils. Comme rien ne remplace la pratique, cela vous aidera à démarrer et à réduire les frustrations que vous pourriez rencontrer pendant cette période.

Nous devons aussi effectuer une rapide comparaison terminologique :

| **Description** | **[!DNL Adobe Analytics]** | **Google[!DNL Analytics]** |
|--------------------------------------------------------------------------------------------------------------------------------|---------------------|----------------------|
| Mesure d’événement représentant une page (ou un écran sur une application) vue. | Page vue | Pageview |
| Mesure représentant un groupe d’interactions sur votre site web ou votre application qui ont lieu au cours de la même période. | Visite | Session |
| Mesure définissant un appareil identifié (en fonction de plusieurs critères, y compris des cookies et d’autres modèles de comportement, pour regrouper les informations sur l’utilisateur). | Visiteur unique | Utilisateur |

## 2. Les interfaces

Comparaison des personnes [!DNL Adobe Analytics] et Google [!DNL Analytics], ils commentent : [!DNL Adobe]L&#39;interface de est d&#39;abord intimidante. C’est vrai, mais c’est également une force, pas une faiblesse. [!DNL Adobe] offre un large éventail d’outils et de flexibilité dans votre visualisation de données, ce qui vous permet d’obtenir plus de liberté pour créer ce dont vous avez besoin.

Commençons par examiner le compte rendu des performances « sur site ».

### 2.1. Compte rendu des performances sur site

#### 2.1.1. Écran d’accueil

Les deux [!DNL Adobe Analytics] et Google [!DNL Analytics] fournir un moyen de personnaliser la première vue qu’un utilisateur voit lorsqu’il se connecte.

##### 2.1.1.1. Espace de travail / Écran d’accueil personnalisé ([!DNL Adobe Analytics])

[!DNL Adobe Analytics] ne présuppose pas la création d’un rapport prédéfini que tous les utilisateurs pourront afficher à la connexion. La page d’accueil par défaut permet à l’utilisateur d’accéder à l’écran de destination de Workspace qui affichera pour chaque utilisateur tous les rapports de l’espace de travail qu’il a créés ou qui ont été partagés avec lui. En outre, chaque utilisateur peut définir l’un de ces rapports comme écran d’accueil s’il le souhaite.

![workspace-create-project](assets/ga-to-aa_1.png)

Vous trouverez plus de détails concernant Workspace plus loin dans ce guide. Voir Section 2.1.2.1

>[!TIP]
>
>Créez et partagez des rapports standard pour votre entreprise afin que tout le monde dispose d’un point de départ pour afficher les informations sans avoir à créer immédiatement ses propres rapports.



##### 2.1.1.2. Informations sur l’écran d’accueil (Google [!DNL Analytics])

* Google [!DNL Analytics] L’écran d’accueil contient des visualisations préconfigurées. Elles couvrent des éléments tels que :
* Utilisateurs, sessions, taux de rebond et durée de session au cours des sept derniers jours.
* Utilisateurs par heure de la journée au cours des 30 derniers jours.
* Utilisateurs actuels en ce moment et principales pages actives.
* Canal de trafic, source/média et références au cours des 7 derniers jours
* Sessions par pays au cours des 7 derniers jours
* Pages les plus consultées au cours des 7 derniers jours
* Tendance des utilisateurs actifs au cours des 30 derniers jours
* etc.

Les utilisateurs de GA4 disposent de davantage d’options pour personnaliser et ajouter leurs propres rapports à l’écran d’accueil.

![google-analytics-interfaces](assets/ga-to-aa_2.png)

C&#39;est probablement la chose qui vous manque le plus dans [!DNL Adobe Analytics]. Il n’y a pas d’écran d’accueil préconfiguré pour vous. Cependant, vous pouvez facilement configurer un Workspace personnalisé pour répliquer vos besoins dans la liste ci-dessus et le définir comme écran d’entrée. Il y aura d’autres informations sur ce sujet ultérieurement (ou voir la section 2.1.2.1) [!DNL Adobe] Workspace).

#### 2.1.2. Report Builders sur site

En plus des rapports simples fournis par les outils d’analyse, chaque outil fournit également des outils plus puissants pour créer vos propres rapports personnalisés.

##### 2.1.2.1. [!DNL Adobe Analytics] Workspace

C&#39;est la puissance de [!DNL Adobe Analytics], depuis son introduction en 2017, il est devenu le lieu de prédilection pour [!DNL Analytics] et la principale raison pour laquelle la section Rapports sera bientôt supprimée.

Cet outil vous permet de créer des rapports avec une liberté presque totale.

Le rapport peut être divisé en panneaux, qui peuvent contenir un nombre illimité de visualisations. Les panneaux peuvent contenir des informations communes, telles quʼune période et des filtres de segments communs.

Les panneaux et les visualisations qu’ils contiennent peuvent être redimensionnés et déplacés pour afficher les éléments côte à côte ou empilés. Si vous souhaitez comparer deux suites de données différentes côte à côte, vous pouvez créer des panneaux divisés en deux parties égales, montrant les deux sites côte à côte pour faciliter la comparaison.

Les utilisateurs ont accès à un grand nombre de visualisations :

* Tableau à structure libre
* Tableau de cohortes
* Abandon
* Flux
* Graphiques
   * Aires (empilées et non empilées)
   * Ligne
   * Nuage de points
   * Barres (empilées et non empilées)
   * Puce
   * Anneau
   * Histogramme
   * Barres horizontales (empilées et non empilées)
* Carte
* Synthèse des blocs
   * Synthèse des modifications
   * Synthèse du texte
   * Texte (champ de texte libre permettant de saisir des informations supplémentaires pour fournir un contexte)
* Venn

Chaque panneau et visualisation peut recevoir un titre et une description, afin de fournir un contexte aux informations qui y sont répertoriées.
Dans [!DNL Adobe], les segments (essentiellement les filtres pour les données) s’appliquent rétroactivement et peuvent être extraits en colonnes de vos tableaux à structure libre pour comparer les données côte à côte. Par exemple, si un utilisateur souhaite comparer le trafic de deux catégories différentes sur son site, il peut créer un segment pour la « Catégorie A » et un autre pour la « Catégorie B ».

![analytics-page-views-report](assets/ga-to-aa_3.png)

Les tableaux à structure libre permettent de disposer de plusieurs colonnes et dʼeffectuer la segmentation nécessaire pour visualiser les données comme vous le souhaitez.

Si vous ne souhaitez pas afficher de répartition par date, il vous suffit de glisser-déposer une autre dimension ou un autre segment pour afficher les données d’une autre manière. Par exemple, vous pouvez utiliser des segments pour le type d’appareil, puis ajouter une répartition par système d’exploitation pour vos utilisateurs d’appareils mobiles/tablette :

![analytics-compare-page-views-report](assets/ga-to-aa_4.png)

Grâce à Espace de travail, votre créativité nʼest plus bridée, car vous nʼêtes pas limité aux répartitions « standard ». Vous pouvez créer les visualisations dont vous avez besoin pour analyser avec moult détails les comparaisons.

>[!TIP]
>
>Jonglez sans crainte entre les différentes visualisations, donnez libre cours à votre créativité et montrez ce que vous savez faire ! En outre, valider ce que vous avez construit vous permettra de partager vos idées. Rien ne vaut l’expérience !

Vous pouvez créer des mesures ou des segments calculées à la volée qui ne figureront que dans le rapport, afin d’éviter de surcharger votre segment et votre référentiel de calculs. Vous pouvez ainsi créer des éléments ciblés nécessaires à des rapports spécifiques sans surcharger votre organisation d’éléments qui ne sont pas utilisables dans d’autres contextes.

Cette discussion n’est qu’une introduction à cet outil. Il existe d’autres guides complets pour vous aider à démarrer. Une fois que vous avez examiné ces guides, vous pouvez créer des rapports complets tels que les suivants :

![workspace-dashboard](assets/ga-to-aa_5.png)

Les espaces de travail ne s’enregistrent pas automatiquement. Il est donc plus facile d’effectuer un rapport ad hoc ponctuel sans boucher votre référentiel de rapports.

L’autre fonctionnalité puissante des espaces de travail est la possibilité d’appliquer des modificateurs interactifs à vos rapports sous la forme de listes déroulantes. Ces listes déroulantes ne fonctionnent pas sur les fichiers CSV ou PDF exportés de vos rapports. Toutefois, dans le rapport dynamique, ils vous permettent de mettre à jour toutes les visualisations d’un panneau afin d’afficher le même rapport sous différentes conditions. Plusieurs listes déroulantes peuvent être utilisées. Tant que les options ne s’excluent pas mutuellement, les éléments sélectionnés s’empileront pour permettre une présentation claire des informations.

>[!IMPORTANT]
>
>Pour en savoir plus sur l’utilisation des listes déroulantes et des répartitions à structure libre, voir <https://experienceleaguecommunities.adobe.com/t5/adobe-analytics-discussions/the-power-of-dropdown-filters-and-dimension-breakdowns-in-adobe/td-p/434680>.

##### 2.1.2.2. Google [!DNL Analytics]: tableaux de bord, rapports personnalisés et rapports enregistrés

Google dispose de quelques outils pour créer des rapports dans l’interface, mais ils suivent toujours l’affichage et les limites de la section des rapports.

Maintenant, pour ceux qui sont habitués à Google [!DNL Analytics] au moment où vous lisez ceci, vous pourriez dire, &quot;attendez une seconde, et Google Data Studio, n&#39;est-ce pas un meilleur équivalent à [!DNL Adobe]&quot;s Workspace ?&quot; Oui, mais Data Studio ne fait pas techniquement partie du [!DNL Analytics] et permet de se connecter à différentes sources de données. Cet outil est présenté plus loin dans la section « Accès aux rapports étendu », en particulier dans la section 2.2.3.

Les tableaux de bord Google et les rapports personnalisés vous permettent d’extraire plusieurs visualisations en un seul rapport. Cependant, contrairement à Workspace, vous n’avez accès qu’à des corrélations simples et ne décidez pas de quelles données placer dans quelles colonnes.

Dans les rapports personnalisés, l’un des plus grands défis se présente lorsque vous créez un filtre : celui-ci s’applique à tous les onglets du rapport. Il n’existe aucun moyen de comparer deux filtres différents dans le même rapport.

Pour les comparaisons de surface, cela fonctionne. Ces variables sont toutes similaires aux variables [!DNL Adobe] Tableaux de bord, rapports personnalisés et signets hérités. Outils de base fournis pour répondre à vos besoins, qui se trouvent dans la suite de rapports.

#### 2.1.3. Rapports

Google et [!DNL Adobe] contiennent des rapports navigables qui sont des tableaux prédéfinis et des graphiques de chronologie de base basés sur une dimension.

##### 2.1.3.1. [!DNL Adobe Analytics] Rapports

[!DNL Adobe Analytics] comporte également une section Rapports , bien que celle-ci soit supprimée progressivement en faveur d’Analysis Workspace. En effet, cette interface va être abandonnée car Workspace s’avère être un outil plus puissant. La plupart de ces tableaux peuvent être créés et modifiés plus facilement. [!DNL Adobe]Les sections de la vidéo sont beaucoup plus décomposées, ce qui peut être décourageant :

![analytics-site-metrics](assets/ga-to-aa_6.png)

La plupart des éléments ci-dessus étant accessibles via les espaces de travail, je donne un bref aperçu de ces sections et de leur relation avec Google. [!DNL Analytics], et mettez en évidence ici les rapports qui sont toujours pertinents.

Les Mesures de site sont ce que leur nom indique : elles couvrent les mesures standard (pages vues, visiteurs uniques, visites, ainsi que les événements personnalisés que vous avez configurés). Cela est similaire à la disponibilité générale du rapport Comportement, mais inclut également certaines de ce que vous trouverez dans Audience (puisque [!DNL Adobe] ne fractionne pas les types de mesures).

Vous y trouverez des rapports de « robots ». Le trafic provenant des robots est exclu de tous vos rapports standard. Toutefois, deux rapports fournissent des informations sur ce qui se passe et sur les robots qui visitent votre site. Cela est particulièrement utile si vous configurez des règles de robots personnalisées pour exclure les robots spammeurs connus qui visitent fréquemment votre site. Vous pouvez obtenir des informations sur ce que ces robots font sans que vos principaux rapports ne soient inondés par ce trafic. Les rapports de robots sont actuellement indisponibles via l’espace de travail (mais de nouvelles fonctionnalités de création de rapports vont bientôt permettre aux utilisateurs d’obtenir ces informations).

Contenu du site est un groupe de [!DNL Adobe] dimensions standard : nom de page, sections du site, hiérarchies, serveurs, etc. Toutes cettes dimensions sont disponibles dans l’espace de travail.

Mobile est un regroupement de données spécifiques aux appareils mobiles, y compris les appareils, les types d’appareils, etc. Ces éléments sont disponibles dans l’espace de travail.

Les chemins ne sont pas disponibles dans l’espace de travail. L’espace de travail comporte un diagramme de flux dans lequel vous pouvez afficher les flux d’entrée et de sortie d’une seule page/valeur. En revanche, les chemins vous permettent d’afficher les chemins les plus couramment utilisés sur votre site web. Par défaut, Pages est le premier rapport de cheminement configuré pour vous. Cependant, vous pouvez l’activer pour les props personnalisées telles qu’une valeur « Type de page ». Vous pouvez examiner le cheminement dans les types de page. L’autre chose que j’aime à propos de Parcours est la façon simple dont les informations sont présentées. On peut vite être dépassé par le diagramme de flux dans l’espace de travail selon ce que l’on veut voir. Je vous recommande d’essayer les deux. Ils ont chacun un usage et une valeur spécifiques en fonction de ce que vous essayez de réaliser. N’importe quelle dimension peut être utilisée dans Flux, tandis que le cheminement doit être configuré sur une prop dans le panneau d’administration.

Sources de trafic [!DNL Campaign]Les rapports sur les canaux marketing et sur les canaux marketing sont tous similaires au rapport Acquisition du produit Google. Les sources de trafic se concentrent sur les référents réels, [!DNL Campaign]s Se concentre sur vos [!DNL Campaign] Codes et canaux marketing sont également axés sur [!DNL Campaign] Codes, mais applique également une logique supplémentaire telle que déterminée par vous sur la manière de traiter les informations. [!DNL Adobe] offre plus de liberté sur la configuration de vos règles. Par contraste, Google effectue de nombreuses tâches à votre place. Cela constitue un changement de réflexion. Par défaut, l’attribution Google est  pour [!DNL Campaign] Les codes sont de six mois. [!DNL Adobe]Par défaut, l’attribution de est définie sur une semaine. Cette mesure peut être modifiée dans vos paramètres d’administration, mais dans Espace de travail, vous pouvez appliquer une attribution personnalisée en plus de n’importe quelle dimension, ce qui vous offre une flexibilité à la volée bien plus grande.

Les rapports Rétention des visiteurs et Profil du visiteur sont similaires aux rapports Audience dans Google [!DNL Analytics]. Le rapport Rétention est davantage axé sur la fréquence des retours, tandis que le rapport Profil des visiteurs est davantage axé sur la géographie et la technologie des utilisateurs.

Les rapports Conversion personnalisée et Trafic personnalisé sont tous deux des rapports de dimension personnalisés. Les conversions sont des eVars. Vous pouvez définir une date d’expiration personnalisée pour la valeur, telle que le nombre d’accès, de visites, de mois ou d’années. Cette valeur est maintenue pour un utilisateur pendant la période configurée, sauf si elle a été remplacée. Les variables de trafic sont des props. Vous pouvez également les configurer pour les rapports de cheminement ou sous la forme d’éléments de liste qui divisent plusieurs valeurs en fonction d’un délimiteur de votre choix.

Le rapport Médias est destiné aux fichiers vidéo ou audio dans lesquels vous avez configuré un suivi spécial des médias.

Rapports personnalisés est une section dans laquelle un utilisateur peut personnaliser les colonnes et les répartitions qu’il a créées dans l’interface des rapports et les enregistrer en tant que rapport personnalisé. Cependant, comme nous l’avons mentionné ci-dessus, l’espace de travail permet des répartitions et des corrélations beaucoup plus puissantes. Toute personnalisation doit être effectuée dans cet espace. C’était une bonne solution avant l’existence de Workspace.

La section Signets est similaire aux rapports personnalisés, où les rapports fréquemment utilisés pouvaient être marqués d’un signet dans l’interface des rapports afin de faciliter leur recherche.

Le tableau de bord était un produit hérité qui permettait aux utilisateurs de combiner des petits rapports de données en une seule visualisation. Toutefois, la fonctionnalité de l’espace de travail (section 2.1.2.1) est bien plus facile à utiliser, si bien que cela n’existe qu’en tant que point d’accès aux rapports hérités qui doivent être recréés avant l’expiration de cette fonctionnalité.

Les cibles permettent aux utilisateurs de créer un rapport basé sur une cible au cours d’une certaine période. Les équipes surveillent les campagnes pour déterminer si elles sont sur la bonne voie pour atteindre leurs cibles de trafic.

Tous les rapports disponibles ici pouvaient avoir plusieurs colonnes de mesures et répartitions de dimensions. Toutefois, la simplicité des visualisations et une partie de la logique qui sous-tend les éléments pouvant être corrélés pouvaient s’avérer frustrantes.

##### 2.1.3.2. Google [!DNL Analytics] Rapports

Google [!DNL Analytics] divise ces rapports en sections suivantes : Temps réel, Audience, Acquisition, Comportement et Conversations (en GA3) et Cycle de vie (avec les sous-sections Acquisition, Engagement, Monétisation, Rétention) et Utilisateur (avec les sous-sections : Données démographiques et Technologie).

![google-analytics-interface-compare](assets/ga-to-aa_7.png)

Vous pouvez apporter des ajustements mineurs à ces visualisations, ajouter une répartition de dimension secondaire, modifier la visualisation, créer un filtre sur les données, etc. Vous pouvez enregistrer vos personnalisations en tant que rapport enregistré.

Vous obtenez ainsi des informations rapides et faciles sur vos données. Cependant, vous ne pouvez pas comparer des éléments comme Utilisateurs aux Pages vues pour une page dans le même tableau. Vous ne pouvez pas non plus ajouter plusieurs dimensions supplémentaires pour afficher des données supplémentaires.

Elles sont utiles pour des données analytiques rapides, mais si vous devez vraiment creuser profondément, il y a des limitations.

### 2.2. Accès aux rapports étendu

Outre le « compte rendu des performances sur site », la plupart des outils offrent des fonctionnalités étendues qui vous permettent de sortir votre analyse des outils et de créer quelque chose d’un peu plus personnalisé.

#### 2.2.1. [!DNL Adobe Analytics] Report Builder (extension Microsoft® Excel)

L’espace de travail est un excellent outil, mais il est parfois nécessaire d’intégrer vos données dans une feuille de calcul personnalisée, éventuellement pour pouvoir assembler plusieurs sources de données. C’est là que Report Builder entre en jeu.

Report Builder est un plug-in pour Microsoft® Excel qui vous permet de créer des connexions à vos [!DNL Adobe Analytics] données pour extraire des données tabulaires que vous pouvez manipuler dans Excel. En règle générale, pour utiliser cette fonctionnalité efficacement, vous devez extraire les données dans certains onglets de données brutes, puis utiliser les références de cellule Excel pour extraire les données de ces onglets dans un seul rapport consolidé, et enfin créer des graphiques et des visualisations.

>[!NOTE]
>
>Report Builder dispose d’une autorisation spéciale qui doit être appliquée à vos utilisateurs pour qu’ils puissent accéder à ce plug-in. Cela ne devrait être accordé qu’aux utilisateurs qui ont appris à utiliser l’outil correctement.

#### 2.2.2. [!DNL Adobe Analytics] Connexion API

Si vous avez besoin de [!DNL Adobe Analytics] Les données doivent être digérées par autre chose qu’Excel. Vous souhaitez que les données traitées, y compris les exclusions de règles de robots, utilisent [!DNL Adobe]API de pour extraire directement les données. Ensuite, traitez les données à l’aide d’un script ou ajoutez-les à une base de données en vue de les utiliser avec un autre système.

Notez que l’API extrait toujours les données de corrélation en appliquant les répartitions et les segments comme indiqué dans la requête d’extraction.

[!DNL Adobe]L’espace de travail de , (section 2.1.2.1) utilise l’API pour créer les rapports. Si vous activez le mode de débogage dans Workspace, il vous montre les appels d’API exacts utilisés. Il s’agit d’une méthode rapide pour créer vos appels d’API. En utilisant l’espace de travail pour créer et valider les données que vous souhaitez extraire, vous utilisez ensuite ces appels d’API pour extraire les données vers votre propre traitement.


#### 2.2.3. Google [!DNL Analytics] Data Studio

Si vous lisez depuis le début, vous savez déjà d’en haut que j’ai mentionné Data Studio comme étant un équivalent [!DNL Adobe]Espace de travail de . Data Studio vous permet d’extraire dans Google [!DNL Analytics] mais aussi des données provenant d’autres sources. C’est très utile si vous souhaitez consolider vos données d’analyse avec d’autres données collectées. Toutefois, avec Google [!DNL Analytics], le même type de limitations de visualisation est présent. La façon de former des lignes et des colonnes est encore limitée.

Cela n’en reste pas moins un outil puissant, et je n’essaie pas du tout de vous dissuader de l’utiliser. Pour ma part, je trouve le comportement rigide assez contraignant.


#### 2.2.4. Extension Google Sheets

Pour mes propres utilisations, lorsque j’ai besoin d’extraire des données de manière étendue à partir de Google [!DNL Analytics], mon outil de choix personnel est l’extension de feuille de calcul Google. Même si je dois établir plusieurs connexions avec mes tableaux GA, je peux référencer les cellules des données brutes et créer les rapports dont j’ai besoin. Ensuite, je les visualise à l’aide des fonctionnalités graphiques de Google Sheets.


## 3. Exportations de données brutes

Lorsque vous avez vraiment besoin de données brutes, les deux [!DNL Adobe] et Google offrent la possibilité d’extraire des informations de cette manière.

### 3.1. [!DNL Adobe] Flux de données

Dans la section 2.2.2, j&#39;ai mentionné que la [!DNL Adobe Analytics] API extraite de &quot;données traitées&quot;. Le flux de données brutes extrait les données traitées par les « règles de traitement » définies dans le panneau d’administration, mais ces données brutes incluent toutes les données qui sont exclues partout ailleurs.

Cela signifie que toutes vos exclusions de robots, vos données internes filtrées par IP, etc. sont incluses dans les flux de données brutes. Il existe des indicateurs pour identifier ces données. Ainsi, si vous créez un lac de données, l’équipe d’ingénieurs peut créer une logique pour traiter ces données en conséquence.

Les flux de données brutes peuvent être personnalisés pour envoyer toutes les colonnes de données ou uniquement des colonnes spécifiques si vous avez besoin d’un flux plus ciblé.

Les flux peuvent être envoyés directement vers FTP, SFTP ou S3.


### 3.2. Google Big Query

Malheureusement, il s’agit d’un outil Google que je n’ai jamais utilisé. En théorie, il devrait être semblable à [!DNL Adobe]Flux de données d’ , permettant à votre équipe d’ingénieurs d’accéder aux données brutes de votre Google [!DNL Analytics] compte .

Cependant, plutôt que de fournir un vidage complet des données brutes, il permet à vos ingénieurs d’accéder aux données via des requêtes SQL pour extraire les données brutes ciblées ou toutes les colonnes de données brutes.

## 4. Conclusion

Comme avec tout système, la pratique est nécessaire pour se familiariser avec l’outil. Heureusement, ce guide vous aide à prendre en main ou fournit des conseils pour améliorer votre utilisation de [!DNL Adobe Analytics].

Toutefois, je vous recommande vivement d’utiliser les deux [!DNL Adobe Analytics] et Google [!DNL Analytics] dans votre stratégie de mise en oeuvre (même si Google [!DNL Analytics] est uniquement la version gratuite). Cela vous permet d’avoir un système de sauvegarde pour vous assurer que vous avez des données, car aucun système n’est infaillible.

Au-delà de ce guide, vous disposez de nombreuses ressources qui peuvent vous aider à améliorer votre stratégie :

* [[!DNL Adobe] Experience League](https://experienceleague.adobe.com/#home) - Contient des tutoriels, des vidéos, de la documentation et des forums de la communauté.
* [[!DNL Adobe] Groupes d’utilisateurs](https://analytics-augs.adobe.com/) - Un hub d’événements gérés par la communauté pour aider les utilisateurs à se connecter les uns aux autres et améliorer leurs implémentations.
* [[!DNL Adobe Analytics] Canal YouTube des groupes d’utilisateurs](https://www.youtube.com/channel/UCQOHnCs7KZgsuFHVzwboQuA) - Ne pouvait pas faire une [!DNL Adobe Analytics] session de groupe d’utilisateurs ? Regardez à nouveau les sessions précédentes des groupes dʼutilisateurs à travers le monde pour en savoir plus sur la façon dont vos pairs utilisent lʼoutil.
* [Mesurer le canal du Slack de conversation](https://www.measure.chat/) - Se connecter avec [!DNL Adobe Analytics] des utilisateurs du monde entier partagent des informations sur l’industrie, posent des questions à leurs pairs et rejoignent des groupes d’intérêt axés sur les mesures.
* Et bien plus encore !

## Auteur

Ce document a été rédigé par :

![Jennifer Dungan](assets/Jennifer_Dungan_Headshot150.png)

Jennifer Dungan, responsable de l’optimisation [!DNL Analytics] at Torstar

[!DNL Adobe Analytics] Champion

