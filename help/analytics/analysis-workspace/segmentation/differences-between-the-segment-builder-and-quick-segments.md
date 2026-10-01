---
title: Différences entre le créateur de segments et les segments rapides dans Analysis Workspace
description: Les segments peuvent être l’un des outils les plus puissants de votre boîte à outils d’analyse des données. Découvrez les différences entre le créateur de segments et les segments rapides dans Analysis Workspace pour plus d’efficacité.
feature-set: Analytics
feature: Segmentation
role: User
level: Beginner
doc-type: article
kt: KT-13118
exl-id: baeaa90e-8cce-4ddd-b099-fecd266e410c
source-git-commit: 9589a00f530e3a2d2897c9e2bd4efc0baf0ff125
workflow-type: tm+mt
source-wordcount: '1269'
ht-degree: 0%
---
# Différences entre le créateur de segments et les segments rapides dans Analysis Workspace

Les segments peuvent être l’un des outils les plus puissants de votre boîte à outils d’analyse des données. Découvrez les différences entre le créateur de segments et les segments rapides dans Analysis Workspace pour plus d’efficacité.

>[!TIP]
>
> Cliquez sur l’image au bas de la page pour télécharger un rappel utile sur les moments où utiliser chaque outil dans Analysis Workspace.

Les segments peuvent être l’un des outils les plus puissants de votre boîte à outils d’analyse des données. Lorsque vous souhaitez examiner des groupes spécifiques de trafic, des sections de site ou des parcours de clients, les segments peuvent être un excellent moyen de concentrer votre analyse sur un sous-ensemble particulier de trafic sur votre site. Dans un environnement de vente au détail, les segments les plus utiles portent sur les différents types de groupes de clients, par exemple la nouvelle clientèle par rapport à la clientèle existante, la clientèle connectée à son compte ou les invités et invitées, etc. Mais vous pouvez également les créer pour différentes sections du site, les clients et clientes qui effectuent des actions spécifiques ou toute autre événement qui vous vient à l’esprit !

**Il existe deux méthodes principales pour créer des segments :**

* Utilisation du créateur de segments dans le menu de composants
* Utilisation des segments rapides en haut d’un panneau

Si vous créez votre segment à l’aide du créateur de segments, vous pouvez l’enregistrer pour le réutiliser dans d’autres projets. Il s’agit d’un excellent moyen de se concentrer sur des groupes spécifiques de clients et clientes, par exemple, les personnes qui visitent certaines sections du site, puis effectuent un achat. D’un autre côté, si vous effectuez une analyse exploratoire et souhaitez tester différents paramètres de segment, le créateur de segments rapides peut s’avérer très utile. Examinons quelques-uns des principaux avantages de chaque méthode.

## Segments rapides

En haut de chaque panneau, vous pouvez cliquer sur l’icône de segment rapide (un funnel avec le symbole +) pour ouvrir le créateur. Vous pouvez créer un segment à n’importe quel niveau (accès, visite ou visiteur) avec jusqu’à trois conditions. Tout comme le créateur de segments principal, le côté droit vous indique si le segment renvoie des données et le pourcentage de la population totale du trafic incluse dans le segment. Il s’agit toutefois d’une version simplifiée de la vue complète du volume de segment affichée dans le créateur de segments. Lors de l’ajout de plusieurs conditions, vous pouvez utiliser les opérateurs « and » et « or ». Il n’existe malheureusement pas d’option « Then » pour les segments rapides. Si vous avez besoin de segments séquentiels, vous devez donc utiliser le créateur de segments complet. Un segment rapide est également limité à un conteneur. Il est en fait destiné aux segments de base qui peuvent être créés et modifiés rapidement. Une fois qu’un segment rapide est appliqué à un panneau ou enregistré, il ne peut plus être modifié dans le panneau.

Lorsque vous effectuez une analyse exploratoire et que vous souhaitez tester différents types de segments pour voir comment différents groupes de clients ou clientes réagissent ou comment différentes catégories se comportent, utilisez les segments rapides, car leur création est beaucoup plus rapide que les segments complets. En outre, ces segments ne sont disponibles que dans le projet dans lequel ils ont été créés. Ainsi, s’il s’avère que ne fournit pas les résultats souhaités, vous n’avez pas à vous soucier de supprimer le segment enregistré de la liste principale. Si, après avoir testé les segments, vous réalisez qu’ils seront utiles dans d’autres projets, vous pouvez toujours cliquer sur le bouton « Ouvrir le créateur » pour ouvrir le segment dans le créateur de segments complet et l’enregistrer en tant que segment standard. Cependant, une fois cette opération effectuée, vous ne pourrez plus la modifier dans le créateur de segments rapides.

![Segment rapide](assets/quick-segement.png)

## Créateur de segments

Pour accéder au créateur de segments, cliquez sur le symbole + situé au-dessus de la liste des segments dans le menu Composants, situé à gauche, ou cliquez sur la liste déroulante Composants et sélectionnez « Créer un segment... ». Contrairement aux segments rapides, toutes les options sont disponibles. Pour ajouter plusieurs conditions, vous pouvez créer des segments séquentiels à l’aide de l’opérateur « then ». Les segments séquentiels vous permettent également d’utiliser le « groupe logique » comme niveau (au lieu de l’accès, de la visite ou du visiteur ou de la visiteuse). Le créateur de segments vous permet également d’ajouter une description aux segments, afin de renseigner sur la personne qui a créé le segment ou le type de données qu’il a été conçu pour filtrer. Vous pouvez aussi ajouter des « balises » au segment à des fins d’organisation. Ces deux opérations ne sont pas possibles dans le créateur de segments rapides.

L’utilisation du créateur de segments est essentielle lorsque votre segment comportera plus de 3 conditions, si vous devez utiliser des conteneurs ou si vous souhaitez des segments séquentiels. Le créateur de segments complet dispose de beaucoup plus d’options pour créer des segments plus complexes, ce qui peut vous aider à ventiler différents types de clients, catégories, parcours de clients, etc. Une fois ces segments créés et enregistrés, ils sont ajoutés à la liste principale des segments. Ils peuvent alors être balisés, approuvés, partagés, utilisés dans plusieurs rapports et publiés sur Experience Cloud. La publication dans Experience Cloud vous permet d’utiliser le segment dans d’autres produits [!DNL Adobe], tels que dans [!DNL Adobe] Target pour le ciblage de personnalisation. Les segments créés dans le créateur de segments ne peuvent pas être modifiés dans le panneau des segments rapides. Vous devez ouvrir le créateur de segments pour y apporter des modifications. Heureusement, la prévisualisation à droite fournit une analyse plus détaillée du trafic généré par le segment au cours des 90 derniers jours. Il est donc plus facile de s’assurer que le segment contient ce que vous souhaitez avant de l’enregistrer.

![Créateur de segments](assets/segment-builder-quick.png)

## Cas d’utilisation

Selon le secteur d’activité, la finalité des segments personnalisés peut être différente. Travaillant pour la division e-commerce d’un grand retailer, nous effectuons souvent des analyses exploratoires pour déterminer les chemins empruntés par les clients et clientes avant d’acheter. Lorsque des pics ou des baisses d’actions sont recensés, comme l’ajout de produits à un panier ou le passage d’une commande, c’est là que l’utilisation des segments rapides peut s’avérer utile. Au cours d’une analyse, je peux rapidement créer un segment pour un type spécifique de client ou cliente ou pour une action/un lien spécifique sur lequel il ou elle clique. Comme il n’est pas nécessaire d’ouvrir le créateur de segments et d’enregistrer chaque segment, je peux ajouter rapidement les conditions et les supprimer tout aussi rapidement. Cela permet de gagner beaucoup de temps lorsque vous essayez d’expliquer pourquoi un changement est constaté sur notre site.

Sinon, il y a des fois où le créateur de segments a été mon objectif. Tous les clients et clientes ne se ressemblent pas comme deux gouttes d’eau. Bien souvent, il s’avère utile d’examiner des types spécifiques de clients et clientes identifiés par les actions ou les chemins empruntés. Grâce au créateur de segments, nous pouvons ajouter plusieurs conditions pour identifier les différents types de clients et clientes et enregistrer les segments afin qu’ils puissent être partagés et utilisés par plusieurs analystes. Il est important que ces types de segments soient cohérents entre les rapports. Il est donc préférable de créer un segment que tout le monde peut utiliser plutôt que de laisser chaque personne créer sa propre version, car les résultats peuvent différer.

Dans l’ensemble, les segments rapides et le créateur de segments sont tous deux d’excellents outils à utiliser dans votre analyse. Ils ont chacun leurs objectifs, leurs avantages et leurs inconvénients. Consultez notre fiche pratique téléchargeable de conseils et astuces ci-dessous pour obtenir un guide de référence rapide.

## Auteur

Ce document a été rédigé par :

![ Mandy George ](assets/mandy-george-2.png)

**Mandy George**, analyste numérique III à Best Buy Canada

Adobe Analytics Champion

## Téléchargement

[![Téléchargement De Segments Rapides](assets/quick-segments-download-small.jpg)](Assets/ Adobe_Analytics_Segments_Vs_Segment_Builder_Reference_Guide.pdf)
