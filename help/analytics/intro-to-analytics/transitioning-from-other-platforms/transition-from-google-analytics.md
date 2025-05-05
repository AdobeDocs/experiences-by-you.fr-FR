---
title: Guide complet pour la transition vers  [!DNL Adobe Analytics] à partir de Google [!DNL Analytics]
description: Découvrez l’emplacement d’une fonctionnalité équivalente et comment l’utiliser efficacement lors de la transition de Google [!DNL Analytics] vers [!DNL Adobe Analytics]
solution: Analytics
feature: Third-party Integration
role: User
level: Beginner
kt: 9830
thumbnail: 34749.jpg
exl-id: 646bdc8f-c95e-40be-b2f7-8e4ba5653d91
source-git-commit: 02e3a6dfa59df45113242bd8e874e18e9e1efd58
workflow-type: tm+mt
source-wordcount: '3323'
ht-degree: 0%

---

# Guide complet pour la transition vers [!DNL Adobe Analytics] à partir de Google [!DNL Analytics]{#comprehensive-guide-for-transitioning-to-adobe-analytics}

## 1. Introduction

L’un des plus grands défis de la transition entre les outils est d’apprendre où trouver des fonctionnalités équivalentes et d’apprendre à les utiliser efficacement. Cette discussion fait partie d’un guide plus large pour aider les utilisateurs à passer plus facilement à [!DNL Adobe Analytics] (soit en tant que nouvel utilisateur, soit en provenance de Google [!DNL Analytics]). Comparaison approfondie de la disponibilité générale, outil comparatif le plus susceptible d’être familiarisé avec la plupart des utilisateurs. Il est fourni pour aider les utilisateurs à mettre en relation les connaissances existantes avec le nouvel ensemble d’outils. Lorsqu&#39;il n&#39;y a pas de substitut à la pratique, cela vous aide à vous mettre en route et à réduire les frustrations que vous pouvez rencontrer pendant cette période.

Nous devrions avoir une comparaison terminologique rapide :

| **Description** | **[!DNL Adobe Analytics]** | **Google[!DNL Analytics]** |
|--------------------------------------------------------------------------------------------------------------------------------|---------------------|----------------------|
| Une mesure d’événement qui représente une page (ou un écran sur une application) a été affichée. | Page vue | Pageview |
| Mesure qui représente un groupe d’interactions sur votre site web ou votre application qui ont lieu pendant la même période. | Consultez votre | Session |
| Mesure qui définit un appareil identifié (en fonction de plusieurs critères, y compris des cookies et d’autres modèles de comportement, pour regrouper les informations sur l’utilisateur). | Visiteur unique | Utilisateur |

## 2. Les interfaces

Lorsque les gens comparent [!DNL Adobe Analytics] et Google [!DNL Analytics], ils commentent que l&#39;interface de [!DNL Adobe] est au début intimidante. C&#39;est vrai, mais c&#39;est aussi vrai ; croyez-le ou non ; une force, pas une faiblesse. [!DNL Adobe] offre un large éventail d’outils et de flexibilité dans votre visualisation de données, ce qui vous permet d’obtenir plus de liberté pour créer ce dont vous avez besoin.

Commençons par examiner les rapports &quot;sur site&quot;.

### 2.1. Création de rapports sur site

#### 2.1.1. Écran d’accueil

[!DNL Adobe Analytics] et Google [!DNL Analytics] offrent tous deux un moyen de personnaliser la première vue qu’un utilisateur voit lorsqu’il se connecte.

##### 2.1.1.1. Workspace / Écran d’accueil du jeu personnalisé ([!DNL Adobe Analytics])

[!DNL Adobe Analytics] ne présuppose pas la création d’un rapport prédéfini que tous les utilisateurs pourront afficher lors de leur connexion. La page d&#39;accueil par défaut permet à l&#39;utilisateur d&#39;accéder à l&#39;écran d&#39;entrée de Workspace, qui affiche à chaque utilisateur tous les rapports de l&#39;espace de travail qu&#39;il a créés ou partagés avec lui. En outre, chaque utilisateur peut définir l’un de ces rapports comme écran d’accueil s’il le souhaite.

![workspace-create-project](assets/ga-to-aa_1.png)

Vous trouverez plus de détails ci-dessous concernant Workspace plus loin dans ce guide. Voir Section 2.1.2.1

>[!TIP]
>
>Créez/partagez des rapports standard pour votre organisation afin qu’ils disposent d’un point de départ pour afficher les informations sans avoir à créer immédiatement leurs propres rapports.



##### 2.1.1.2. Informations sur l’écran d’accueil (Google [!DNL Analytics])

* L’ écran d’accueil de Google [!DNL Analytics] contient des visualisations préconfigurées. Elles couvrent des éléments tels que :
* Utilisateurs, sessions, taux de rebond et durée de session au cours des sept derniers jours
* Utilisateurs par heure de la journée au cours des 30 derniers jours
* Utilisateurs actuels en ce moment et principales pages actives
* Canal de trafic, Source/Medium et Références au cours des sept derniers jours
* Sessions par pays au cours des sept derniers jours
* Pages principales des sept derniers jours
* Tendance des utilisateurs actifs au cours des 30 derniers jours
* et plus

Les utilisateurs de GA4 disposent d’autres options pour personnaliser et ajouter leurs propres rapports à l’écran d’accueil.

![google-analytics-interfaces](assets/ga-to-aa_2.png)

C&#39;est probablement la chose qui vous manque le plus dans [!DNL Adobe Analytics]. Il n&#39;y a pas d&#39;écran d&#39;accueil préconçu pour vous. Cependant, vous pouvez facilement configurer un Workspace personnalisé pour répliquer ce dont vous avez besoin dans la liste ci-dessus et le définir comme écran d’entrée. Il y aura d’autres informations sur cette rubrique ultérieurement (ou voir Section 2.1.2.1 [!DNL Adobe] Workspace).

#### 2.1.2. Reports Builder sur site

Outre les rapports simples fournis par les outils d’analyse, chaque outil fournit également des outils plus puissants pour créer vos propres rapports personnalisés.

##### 2.1.2.1. [!DNL Adobe Analytics] Workspace

Il s’agit de l’élément moteur de [!DNL Adobe Analytics]. Depuis son introduction en 2017, il est devenu le lieu de prédilection pour l’analyse [!DNL Analytics] et la principale raison pour laquelle la section Rapports est sur le point de disparaître.

Cet outil vous permet de créer des rapports avec une liberté presque totale.

Le rapport peut être divisé en panneaux et ces panneaux peuvent contenir un nombre illimité de visualisations. Les panneaux peuvent être définis sur des informations communes, telles que la période et les filtres de segments communs.

Les panneaux et les visualisations qu’ils contiennent peuvent être redimensionnés et déplacés pour afficher les éléments côte à côte ou empilés. Si vous souhaitez comparer deux suites de données différentes côte à côte, vous pouvez créer des panneaux qui divisent 50/50 le milieu affichant les deux sites côte à côte pour faciliter la comparaison.

Les utilisateurs ont accès à une multitude de visualisations :

* Tableau à structure libre
* Tableau de cohortes
* Abandon
* Flux
* Graphiques
   * Zone (empilée et non empilée)
   * Ligne
   * Diagramme
   * Barre (empilée et non empilée)
   * Puce
   * Anneau
   * Histogramme
   * Barre horizontale (empilée et non empilée)
* Carte
* Blocs récapitulatifs
   * Résumé des changements
   * Texte récapitulatif
   * Texte (champ de texte libre pour saisir des informations supplémentaires pour donner un contexte)
* Venn

Chaque panneau et visualisation peut être intitulé et faire l’objet d’une description afin de donner un contexte à ce que les informations présentent.
Dans [!DNL Adobe], les segments (essentiellement les filtres pour les données) s’appliquent rétroactivement. Ils peuvent être extraits dans les colonnes de vos tableaux à structure libre pour comparer les données côte à côte. Par exemple, si un utilisateur souhaite comparer deux catégories différentes sur son site pour le trafic, il peut créer un segment pour la &quot;catégorie A&quot; et un autre pour la &quot;catégorie B&quot;.

![analytics-page-views-report](assets/ga-to-aa_3.png)

Les tableaux à structure libre permettent plusieurs colonnes et une segmentation, selon les besoins, afin de visualiser les données comme vous le souhaitez.

Si vous ne souhaitez pas afficher de ventilation par date, faites simplement glisser une autre dimension ou un autre segment pour afficher les données d’une autre manière. Par exemple, utilisez des segments pour le type de périphérique, puis ajoutez une ventilation par système d’exploitation pour vos utilisateurs de périphériques mobiles/tablettes :

![analytics-compare-page-views-report](assets/ga-to-aa_4.png)

Workspace permet à votre créativité de voler, vous n&#39;êtes pas limité aux ventilations &quot;standard&quot;. Vous pouvez créer les visualisations dont vous avez besoin pour approfondir les comparaisons à exécuter.

>[!TIP]
>
>N&#39;ayez pas peur de jouer et d&#39;explorer. Il y a tellement de façons de penser en dehors de la boîte. De plus, validez ce que vous avez créé pour montrer ce que vous pensez. L&#39;expérience aide !

Vous pouvez créer des mesures calculées à la volée ou des segments qui ne résident que dans le rapport afin d’éviter d’inonder votre segment et votre référentiel de calculs. Vous pouvez ainsi créer des éléments ciblés nécessaires à des rapports spécifiques sans confondre votre organisation avec des éléments qui ne sont pas utilisables dans d’autres contextes.

Cette discussion n’est qu’une introduction à cet outil. Il existe d’autres guides complets pour vous aider à démarrer. Une fois que vous avez examiné ces guides, vous créez des rapports complets, tels que les suivants :

![workspace-dashboard](assets/ga-to-aa_5.png)

Les espaces de travail n’enregistrent pas automatiquement. Il est donc plus facile d’effectuer un rapport ad hoc ponctuel sans boucher votre référentiel de rapports.

L’autre fonctionnalité puissante des espaces de travail est la possibilité d’appliquer des modificateurs interactifs à vos rapports sous la forme de listes déroulantes. Ces menus déroulants ne fonctionnent pas sur les fichiers CSV exportés ou PDF de vos rapports. Toutefois, dans le rapport en direct, ils vous permettent de mettre à jour toutes les visualisations d’un panneau afin d’afficher le même rapport sous différentes conditions. Plusieurs listes déroulantes peuvent être utilisées. À condition que les options ne soient pas mutuellement exclusives, la pile d’éléments sélectionnée permet de présenter des informations de manière propre.

>[!IMPORTANT]
>
>Pour en savoir plus sur l’utilisation des listes déroulantes et des ventilations à structure libre, voir <https://experienceleaguecommunities.adobe.com/t5/adobe-analytics-discussions/the-power-of-dropdown-filters-and-dimension-breakdowns-in-adobe/td-p/434680?profile.language=fr>

##### 2.1.2.2 Google [!DNL Analytics] : tableaux de bord, rapports personnalisés et rapports enregistrés

Google dispose de quelques outils pour créer des rapports dans l’interface, mais ils suivent toujours l’affichage et les limites de la section des rapports.

Maintenant, pour ceux qui sont habitués à Google [!DNL Analytics] quand vous lisez ceci, vous pourriez dire, &quot;attendez une seconde, et Google Data Studio, n&#39;est-ce pas un meilleur équivalent à [!DNL Adobe]&#39;s Workspace ?&quot; Oui, mais Data Studio ne fait pas techniquement partie de l’outil [!DNL Analytics] et il permet des connexions à différentes sources de données. Cet outil est présenté plus loin dans la section &quot;Accès aux rapports étendu&quot;, en particulier dans la section 2.2.3.

Les tableaux de bord Google et les rapports personnalisés vous permettent d’extraire plusieurs visualisations en un seul rapport. Cependant, contrairement à Workspace, vous êtes toujours verrouillé dans des corrélations simples et quelles données peuvent être placées dans quelles colonnes.

Dans les rapports personnalisés, l’un des plus grands défis est que lorsque vous créez un filtre, il s’applique à tous les onglets du rapport. Il n’existe aucun moyen de comparer deux filtres différents dans le même rapport.

Pour les comparaisons de surface, c’est la tâche. Tous ces rapports sont similaires aux [!DNL Adobe] tableaux de bord, rapports personnalisés et signets hérités. Outils de base fournis pour répondre à vos besoins, qui se trouvent dans la suite de rapports.

#### 2.1.3. Rapports

Google et [!DNL Adobe] ont tous deux des rapports accessibles qui sont des tableaux prédéfinis et des graphiques de chronologie de base basés sur une dimension.

##### 2.1.3.1. [!DNL Adobe Analytics] Rapports

[!DNL Adobe Analytics] comporte également une section Rapports, bien que celle-ci soit supprimée progressivement en faveur d’Analysis Workspace. En fait, la fin de vie de cette interface a été annoncée, car Workspace est un outil plus puissant. La plupart de ces tables peuvent être créées et modifiées plus facilement. Les sections de [!DNL Adobe] sont beaucoup plus fragmentées, ce qui peut être décourageant :

![analytics-site-metrics](assets/ga-to-aa_6.png)

Comme la plupart des éléments ci-dessus sont accessibles via les espaces de travail, je donne un bref aperçu de ces sections et de leur relation avec Google [!DNL Analytics], et je mets en évidence les rapports qui restent pertinents ici.

Les mesures du site sont ce à quoi vous vous attendez ; elles couvrent les mesures standard (pages vues, visiteurs uniques, visites et événements personnalisés que vous avez configurés). Ceci est similaire à la disponibilité générale du rapport de comportement, mais inclut également certaines de ce que vous trouverez dans Audience (puisque [!DNL Adobe] ne divise pas les types de mesures).

Vous y trouverez des rapports &quot;Robots&quot;. Le trafic provenant des robots est exclu de tous vos rapports standard. Toutefois, deux rapports fournissent des informations sur ce qui se passe et les robots qui arrivent sur votre site. Cela est particulièrement utile si vous configurez des règles de robots personnalisées pour exclure les robots spammeurs connus qui visitent fréquemment votre site. Vous pouvez avoir un aperçu de ce que ces robots font sans que vos principaux rapports ne soient inondés, mais que le trafic en question. Les rapports sur les robots sont actuellement indisponibles via Workspace (mais de nouvelles fonctionnalités de création de rapports vont bientôt permettre aux utilisateurs d’y obtenir ces informations).

Le contenu du site est un groupe de [!DNL Adobe] dimensions standard : nom de page, sections du site, hiérarchies, serveurs, etc. Toutes ces dimensions sont disponibles dans Workspace.

Mobile est un groupe de données spécifiques aux appareils mobiles, y compris les appareils, les types d’appareils, etc. Elles sont disponibles dans Workspace.

Les chemins ne sont pas disponibles dans Workspace. Workspace comporte un diagramme Flux dans lequel vous pouvez afficher les flux d’entrée et de sortie pour une seule page/valeur. En revanche, les chemins vous permettent d’afficher les chemins les plus courants utilisés dans votre site web. Par défaut, Pages est le premier rapport de cheminement configuré pour vous. Cependant, vous pouvez l’activer pour les props personnalisées telles qu’une valeur &quot;Type de page&quot;. Vous pouvez examiner le cheminement dans les types de page. L&#39;autre chose que j&#39;aime personnellement à propos des Chemins est la façon simple dont les informations sont présentées... Le diagramme de flux dans l&#39;espace de travail (en fonction de ce que vous essayez de regarder) peut devenir accablant. Je vous recommande d&#39;essayer les deux... ils ont tous un usage et une valeur en fonction de ce que vous essayez de réaliser. N’importe quelle dimension peut être utilisée dans les flux, tandis que le cheminement doit être configuré sur une prop dans le panneau d’administration.

Les rapports Sources de trafic, [!DNL Campaign] et Canaux marketing sont tous similaires au rapport Acquisition du produit Google. Les sources de trafic se concentrent sur les référents réels, les [!DNL Campaign]s se concentrent sur vos codes [!DNL Campaign] et les canaux marketing se concentrent également sur les codes [!DNL Campaign], mais appliquent également une logique supplémentaire telle que déterminée par vous sur la manière de traiter les informations. [!DNL Adobe] offre plus de liberté sur la configuration de vos règles. En revanche, Google fait de nombreuses choses pour vous, et c&#39;est un changement de point de vue. Par défaut, l’attribution Google pour les [!DNL Campaign] codes est de six mois. L’attribution de [!DNL Adobe] est définie sur une semaine par défaut. Cela peut être modifié dans vos paramètres d’administration, mais dans Workspace, vous pouvez effectivement appliquer une attribution personnalisée en plus de n’importe quelle dimension, ce qui vous offre une flexibilité &quot;à la volée&quot; bien plus grande.

Les rapports Rétention des visiteurs et Profil du visiteur sont similaires aux rapports Audience dans Google [!DNL Analytics]. La rétention est davantage axée sur la fréquence des retours, tandis que le profil du visiteur est davantage axé sur la géographie et la technologie des utilisateurs.

Les rapports Conversion personnalisée et Trafic personnalisé sont tous deux des rapports de dimension personnalisés. Les conversions sont des eVars. Vous pouvez définir une expiration personnalisée sur la valeur de l’accès, de la visite, du mois et de l’année. Cette valeur reste en persistance pour un utilisateur pendant la période configurée, sauf si elle a été remplacée. Les variables de trafic sont des props. Vous pouvez également les configurer pour les rapports de cheminement ou sous forme d’éléments de liste qui divisent plusieurs valeurs en fonction d’un délimiteur de votre choix.

Le média est destiné aux fichiers vidéo ou audio dans lesquels vous avez configuré un suivi multimédia spécial.

Les rapports personnalisés sont une section dans laquelle un utilisateur peut personnaliser les colonnes et les ventilations qu’il a créées dans l’interface des rapports et les enregistrer en tant que rapport personnalisé. Cependant, comme nous l’avons mentionné ci-dessus, Workspace permet des ventilations et des corrélations beaucoup plus puissantes, tout ce qui doit être personnalisé doit être créé à cet endroit. C&#39;était une bonne solution avant l&#39;existence de Workspace.

La section Signets est similaire aux rapports personnalisés, où les rapports fréquemment utilisés peuvent être marqués dans l’interface des rapports afin de faciliter leur recherche.

Le tableau de bord est un produit hérité qui permet aux utilisateurs de combiner des mini-rapports de données en une seule visualisation. Toutefois, la fonctionnalité de Workspace (section 2.1.2.1) est tellement plus facile à utiliser que cela n’existe qu’en tant que point d’accès aux rapports hérités qui doivent être recréés avant l’expiration de cette fonctionnalité.

Les cibles permettent aux utilisateurs de créer un rapport basé sur une cible au cours d’une certaine période. Les équipes surveillent les campagnes pour voir si elles sont sur la bonne voie pour atteindre leurs cibles de trafic.

Tous les rapports disponibles ici sont autorisés pour plusieurs colonnes de mesures et ventilations de dimensions. Cependant, la simplicité des visualisations et une partie de la logique sous-jacente aux éléments pouvant être corrélés peuvent parfois être frustrantes.

##### 2.1.3.2. Rapports Google [!DNL Analytics]

Google [!DNL Analytics] divise ces rapports en sections suivantes : Temps réel, Audience, Acquisition, Comportement et Conversations (en GA3) et Cycle de vie (avec les sous-sections : Acquisition, Engagement, Monétisation, Rétention) et Utilisateur (avec les sous-sections : Données démographiques et technologie).

![google-analytics-interface-compare](assets/ga-to-aa_7.png)

Vous pouvez apporter des ajustements mineurs à ces visualisations, ajouter une ventilation de dimension secondaire, modifier la visualisation, créer un filtre sur les données, etc. Vous pouvez enregistrer vos personnalisations en tant que rapport enregistré.

Ces informations fournissent des informations rapides et faciles sur vos données. Cependant, vous ne pouvez pas comparer des éléments tels que Utilisateurs aux pages vues pour une page dans le même tableau, et vous ne pouvez pas ajouter plusieurs dimensions supplémentaires pour afficher des données supplémentaires.

Ils sont bons pour des données analytiques rapides, mais si vous devez vraiment creuser profondément, ils souffrent des limitations.

### 2.2. Accès aux rapports étendu

Outre la création de rapports sur site, la plupart des outils offrent des fonctionnalités étendues qui vous permettent de passer votre analyse en dehors des outils et de créer quelque chose d’un peu plus personnalisé.

#### 2.2.1. Report Builder [!DNL Adobe Analytics] (extension Microsoft® Excel)

Workspace est un excellent outil, mais il est parfois nécessaire de regrouper les données dans une feuille de calcul personnalisée, éventuellement pour regrouper plusieurs sources de données. C&#39;est là que le Report Builder entre en jeu.

Report Builder est un plug-in pour Microsoft® Excel qui vous permet de créer des connexions à vos données [!DNL Adobe Analytics] afin d’extraire des données tabulaires que vous pouvez manipuler dans Excel. En règle générale, pour utiliser cette fonctionnalité efficacement, vous devez extraire les données dans certains onglets de données brutes, puis utiliser les références de cellule Excel pour extraire les données de ces onglets dans un seul rapport consolidé, puis créer des graphiques et des visualisations.

>[!NOTE]
>
>Report Builder dispose d’une autorisation spéciale qui doit être appliquée à vos utilisateurs pour accéder à ce module externe. Cela doit être accordé aux utilisateurs qui ont appris à utiliser l’outil correctement.

#### 2.2.2. [!DNL Adobe Analytics] Connexion de l’API

Si vous avez besoin de [!DNL Adobe Analytics] données pour être digérées par autre chose qu’Excel et que vous souhaitez que les données traitées, y compris les exclusions de règles de robots, utilisez l’API de [!DNL Adobe] pour extraire directement les données. Ensuite, traitez les données à l&#39;aide d&#39;un script ou ajoutez-les à une base de données pour les utiliser avec un autre système.

Notez que l’API extrait toujours les données de corrélation en appliquant les ventilations et les segments comme indiqué dans la requête de tirage.

Le Workspace de [!DNL Adobe] (Section 2.1.2.1) utilise l’API pour créer les rapports. Si vous activez le mode de débogage dans Workspace, il vous montre les appels d’API exacts utilisés. Il s’agit d’une méthode rapide pour créer vos appels d’API. En utilisant Workspace pour créer et valider les données que vous souhaitez extraire, vous utilisez ensuite ces appels d’API pour extraire les données vers votre propre traitement.


#### 2.2.3. Google [!DNL Analytics] Data Studio

Si vous lisez depuis le début, vous savez déjà d’en haut que j’ai mentionné Data Studio comme étant équivalent à Workspace de [!DNL Adobe]. Data Studio vous permet d’extraire des données Google [!DNL Analytics], mais aussi des données provenant d’autres sources. C’est très utile si vous souhaitez consolider vos données d’analyse avec d’autres données collectées. Toutefois, avec Google [!DNL Analytics], le même type de limitations de visualisation est présent. La façon dont les lignes et les colonnes sont formées est encore limitée.

C&#39;est encore un outil puissant, et je ne dissuaderais pas les gens de l&#39;utiliser de quelque manière que ce soit. Mon expérience personnelle est que je trouve le comportement rigide assez limité.


#### 2.2.4. Extension de feuille de calcul Google

Pour mon propre usage, lorsque je dois extraire des données de manière étendue à partir de Google [!DNL Analytics], mon outil de choix personnel est l’extension de feuille de calcul Google. Même si je dois établir plusieurs connexions avec mes tableaux GA, je peux référencer les cellules des données brutes et créer les rapports dont j’ai besoin. Ensuite, je les visualise à l’aide des fonctionnalités graphiques de la feuille de calcul Google.


## 3. Exports de données brutes

Lorsque vous avez vraiment besoin de données brutes, [!DNL Adobe] et Google vous offrent la possibilité d’extraire des informations de cette manière.

### 3.1. [!DNL Adobe] Flux de données

Dans la section 2.2.2, j’ai mentionné que l’API [!DNL Adobe Analytics] provient des &quot;données traitées&quot;. Le flux de données brutes extrait les données traitées par les &quot;règles de traitement&quot; configurées dans le panneau d’administration, mais ces données brutes incluent toutes les données qui sont exclues partout ailleurs.

Cela signifie que toutes vos exclusions de robots, vos données internes filtrées par IP et d’autres données exclues se trouvent dans les flux de données brutes. Il existe des indicateurs pour identifier ces données. Par conséquent, si vous créez un lac de données, l’équipe d’ingénierie peut créer une logique pour traiter ces données en conséquence.

Les flux de données brutes peuvent être personnalisés pour envoyer toutes les colonnes de données ou uniquement des colonnes spécifiques si vous avez besoin d’un flux plus ciblé.

Les flux peuvent être envoyés directement vers FTP, SFTP ou S3.


### 3.2. Google Big Query

Malheureusement, il s’agit d’un outil Google que je n’ai jamais utilisé. En théorie, il doit être similaire au flux de données de [!DNL Adobe], ce qui permet à votre équipe d’ingénieurs d’accéder aux données brutes de votre compte Google [!DNL Analytics].

Cependant, plutôt que de fournir un vidage complet des données brutes, il permet à vos ingénieurs d’accéder aux données via des requêtes SQL pour extraire les données brutes ciblées ou toutes les colonnes de données brutes.

## 4. Conclusion

Comme tout système, il faut s&#39;entraîner pour se familiariser avec l&#39;outil. Heureusement, ce guide vous aide à démarrer ou fournit des conseils pour améliorer votre utilisation de [!DNL Adobe Analytics].

Cependant, je vous recommande vivement d’utiliser [!DNL Adobe Analytics] et Google [!DNL Analytics] dans votre stratégie de mise en oeuvre (même si Google [!DNL Analytics] n’est que la version gratuite). Vous pouvez ainsi disposer d’un système de sauvegarde pour vous assurer que vous disposez de données, car aucun système n’est infaillible.

De nombreuses ressources sont disponibles au-delà de ce guide pour vous aider à améliorer votre stratégie :

* [[!DNL Adobe] Experience League](https://experienceleague.adobe.com/fr#home) - Contient des tutoriels, des vidéos, de la documentation et des forums de la communauté
* [[!DNL Adobe] Groupes d’utilisateurs](https://analytics-augs.adobe.com/) - Un hub d’événements gérés par la communauté pour aider les utilisateurs à se connecter les uns aux autres et améliorer leurs mises en oeuvre.
* [[!DNL Adobe Analytics] Canal YouTube des groupes d’utilisateurs](https://www.youtube.com/channel/UCQOHnCs7KZgsuFHVzwboQuA) - Impossible d’effectuer une session de groupe d’utilisateurs [!DNL Adobe Analytics] ? Regardez les sessions précédentes de groupes d’utilisateurs à travers le monde pour en savoir plus sur l’utilisation de l’outil par vos pairs.
* [Mesurez le canal du Slack de conversation](https://www.measure.chat/) - Connectez-vous à [!DNL Adobe Analytics] utilisateurs à travers le monde et partagez les leçons du secteur, posez des questions à vos pairs et rejoignez des groupes d’intérêt axés sur les mesures.
* et plus encore !

## Auteur

Ce document a été rédigé par :

![Jennifer Dungan](assets/Jennifer_Dungan_Headshot150.png)

Jennifer Dungan, responsable de l’optimisation [!DNL Analytics] chez Torstar

[!DNL Adobe Analytics] Champion
