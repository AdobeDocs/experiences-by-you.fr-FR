---
title: 'Balises : votre assistant personnel'
description: Découvrez comment
feature: Dimensions, Projects
role: User
level: Beginner, Intermediate, Experienced
doc-type: Article
duration: 36000
last-substantial-update: 2024-02-22T00:00:00Z
jira: KT-14963
thumbnail: KT-14963.jpeg
source-git-commit: e63d6cf68e70622ddcdbe92064d84ad72ca483c3
workflow-type: tm+mt
source-wordcount: '1427'
ht-degree: 0%

---


# #Tags - votre assistant personnel

_Découvrez comment #TAGS peut rationaliser vos analyses numériques, en tant qu’assistant personnel pour trouver efficacement ce dont vous avez besoin. Jeff Bloomer, champion d’Adobe Analytics, partage des idées d’experts sur la maximisation du potentiel de cet outil pour votre bénéfice._

Tout le monde se souvient d&#39;avoir joué à un bon jeu de tags, ou même de se cacher et chercher, quand nous étions enfants, n&#39;est-ce pas ?

![Enfants jouant](assets/kids-playing2.jpeg)

Le meilleur, c&#39;était quand nous étions ceux qui soit étaient revenus à la base (balise), soit restaient cachés le plus longtemps (cache-cache) jusqu&#39;à ce que nous entendions quelqu&#39;un crier : &quot;Olly Oxen free !&quot; (&quot;Vous tous sortez tous libres,&quot; dérivé de l&#39;allemand : &quot;alle auch sind frei !&quot;).  Ce qui signifie que tout le monde a réussi à se baser, à être trouvé, ou quelqu&#39;un a été marqué &quot;ça&quot;, et nous étions encore libres de jouer un autre tour !

L&#39;important est si le jeu était un tag ou un cache-cache, nous jouions à une activité amusante où tout le monde a été retrouvé encore et encore.

Quand nous nous tournons vers notre travail quotidien, la recherche de choses semble devenir beaucoup moins aventureuse et beaucoup plus ennuyeuse. Mais ce n&#39;est pas nécessaire si nous sommes prêts à mettre un peu de travail sur le front.  Une phrase bien connue de ma famille est : &quot;La plupart de la douleur est auto-infligée.&quot; Cependant, bien qu&#39;il puisse sembler un peu démodé de nos jours, il y a une phrase plus célèbre qui est aussi très pertinente dans cette situation : &quot;Un point dans le temps en sauve neuf.&quot; - Benjamin Franklin

Maintenant que j&#39;ai votre attention, je vais commencer par poser une question :


![Combien d&#39;entre vous ?](assets/how-many-of-you.jpg)

Combien d&#39;entre vous ont fait ça ?  Vous avez commencé à rechercher une **dimension**, **période**, **segment**, ou **mesure calculée** et vous êtes inondés de cette liste géante (voir **Figure 1**) de tout ce que vous ne voulez PAS.  ***Analysis Workspace*** pense qu&#39;il essaie d&#39;être utile, mais en réalité, il n&#39;a réussi qu&#39;à ne pas être utile du tout.

![figure 1 recherche pour l’année](assets/tags-example-year.jpg)

*Figure 1 - Recherche de &quot;l’année&quot;*

Mieux encore, vous en avez créé. *new* **plages de dates** et **segments**, et parce qu’ils sont &quot;si nouveaux&quot;, vous pensez qu’au moins ces éléments devraient être rapides et faciles à trouver la prochaine fois que vous entrerez ***Adobe Workspace***. Ai-je raison ?

Eh bien, je déteste faire éclater votre bulle, mais essayez simplement de partir ***Adobe Analytics*** après avoir créé tous vos &quot;petits amis&quot; les plus récents, et quand vous revenez, la majorité d&#39;entre eux se sont simplement enfuis.  Si vous avez de la chance, *peut-être* l&#39;un d&#39;eux est resté pour vous attendre, mais les autres sont déjà partis et jouent à cache-cache.

## Réécriture du règlement

Donc, c&#39;est le jeu depuis le premier jour, mais si nous pouvions changer les règles ?

En fait, et si nous pouvions créer notre propre assistant personnel pour changer ces règles pour de bon ?

Sérieusement, ce dont nous parlons ici, ce sont les TAGS !  C&#39;est vrai!!  C&#39;est notre ami avec le hashtag, anciennement connu sous les noms de &quot;chiffre&quot; et de &quot;livre sterling&quot;, comme nous l&#39;avons vu sur nos téléphones.  Ceux d&#39;entre nous qui musiciens là-bas appellent même ça &quot;sharp&quot;.

Pour ceux qui ont *vraiment* Pour rappel, il se présente comme suit : **#**

Quoi qu&#39;il en soit, la raison pour laquelle nous parlons **#tags** parce qu&#39;ils sont entassés dans ce &quot;seau optionnel&quot; de &quot;trucs ennuyeux et ennuyeux, mignons et excentriques&quot; tout le monde a tendance à ignorer (comme les Descriptions), parce que nous sommes tous tellement pressés de créer les choses les plus importantes comme, oh je ne sais pas -

- Rapports Workspace
- Segments
- Mesures calculées 
- Périodes

Regardez, les gars !  Vous l&#39;appelez, nous avons vu et entendu toutes les excuses pour lesquelles ils sont ignorés :

&quot;Oh, hé, mais c&#39;est facile.  Je peux toujours revenir plus tard et juste mettre à jour ces choses lors de quelques pauses déjeuner, ou même pendant que je suis assis à une conférence et *tout rattraper*,&quot; dit tout le monde qui ne l&#39;a JAMAIS fait.

## Contenu de la boîte à outils

**Adobe** a même fait à WE THE PEOPLE le service de créer un ensemble sélectionné de #TAGS d&#39;usine, parce que, eh bien... ils ont dû nous démarrer quelque part.  Je vais vous faire part de quelques mises en garde supplémentaires dans quelques instants seulement, mais ce que je vous montre en premier lieu vous donnera le plus de chance pour votre argent !

Avant de créer l’un des vôtres, vous devez d’abord savoir comment rechercher des **tags**:

![Balises Gif](assets/tags-gif.gif)

Que vous soyez dans un projet nouveau ou existant, il vous suffit d’accéder à la barre de recherche des composants, de saisir un #hashtag, ainsi que l’un de ces termes principaux (il vous suffit de regarder la vidéo), et d’appuyer sur ENTRÉE ; ou, vous pouvez simplement commencer à faire défiler l’écran jusqu’à ce que vous trouviez un terme reconnaissable.

PREMIÈRE CAVETTE : Gardez à l’esprit que si vous respectez les conventions d’affectation de nom lorsque vous commencez à créer votre *own* balises, pratiquement toutes les *capitalisé* balise que vous voyez *should*, et je ferai attention avec ce mot &quot;devrait&quot;, être un **Adobe**, élément balisé d’usine.  Cela signifie que toutes les balises que vous créez se trouvent dans . **minuscule**.

## Créer votre propre assistant personnel

Maintenant, revenons à ce que j&#39;ai dit à propos d&#39;un &quot;assistant personnel&quot; plus tôt.  Et si je vous disais que vous pourriez commencer à sélectionner certains de vos composants existants préférés et ensuite en faire les SEULES que vous voyez ?

![3 balises screens](assets/3-screens-tags.jpg)


1. Si vous commencez à sélectionner plusieurs composants (Ctrl+GAUCHE, CLIC), certaines icônes s’affichent en haut.  L’une d’elles est l’icône BALISER.
1. Cliquez dessus, puis la boîte de dialogue BALISES s’ouvre. C’est là que vous pouvez afficher toutes les balises existantes associées à ces composants.
1. C’est à partir de cet écran que vous pouvez ensuite attribuer n’importe quel **additional/new** balises que vous pouvez souhaiter à ce stade.  (Exemple : **test\_v1**)
1. Pour ajouter une balise NEW à un composant, il vous suffit d’appuyer sur **ENTRER** sur votre clavier avant de cliquer sur le bouton ENREGISTRER .
1. Ensuite, lorsque vous avez attribué votre nouvelle balise, vous pouvez la rechercher en saisissant hashtag(#) et votre nouvelle balise.

Pardonnez le jeu de mots, mais &quot;#tag, vous y êtes !&quot;  Vous venez de vous épargner beaucoup moins de recherche dans le futur !  Maintenant vous voyez où votre diligence raisonnable et votre travail acharné vont enfin entrer en jeu.

## Mettre votre assistant personnel au travail

Disons que nous travaillons dans la **Industrie du tourisme** et nous préparons un rapport pour leur **heures ouvrables principales**.  Si nous devions lancer une recherche uniquement sur le terme &quot;VOYAGE&quot;, nous pourrions obtenir beaucoup plus de résultats que nécessaire.  En fait, si nous remontons une **Workspace** contenant même la moitié des résultats dont nous avions besoin, les composants ne seraient toujours pas facilement disponibles.

![Balises erronées](assets/tags-example-travel.jpg)

Cependant, si tout au long de notre quotidien nous travaillons, nous avons régulièrement marqué notre **segments**, **mesures**, etc. **components** au fur et à mesure, et peut-être en créer quelques nouveaux au moment où nous créons notre nouveau **workspace**, nous avons sérieusement démontré comment nous pouvons réécrire le règlement en notre faveur !

Dans ce cas, j&#39;ai créé un #tag simple pour tous ces éléments nommés : #core.

![cha-ching](assets/cha-ching.png)

Alors que vous continuez à prendre cette partie de vos habitudes de travail et à améliorer vos compétences pour le faire encore et encore, vous vous rendrez compte que l&#39;utilisation de #tags deviendra plus comme avoir votre propre assistant personnel.

Vous voulez d&#39;autres exemples du monde réel ? Tenez compte des points suivants :

1. Par exemple, que diriez-vous d’un moyen simple de trouver votre **segments** et votre **plages de dates** pour **tous les trimestres** in **2023**?

   ![Real world 1](assets/real-world-1.png)

   *Un conseil supplémentaire*: ce petit carré à droite vous permet même de modifier l’ordre de tri en *alphabétique*!


1. Bien sûr, tout le monde utilise **codes de suivi de campagne** dans une certaine mesure.  Si vous souhaitez avoir une vue claire de uniquement *your* jouets, pensez à ajouter **#tag** pour ne voir que les éléments principaux dont vous avez réellement besoin et filtrer tous les autres bruits :

![Real world 2](assets/real-world-2.png)

## Maintenant allez-y et jouez !

Bien sûr, se cacher et chercher était amusant quand on était enfant, mais maintenant nous sommes adultes.  Nous n&#39;avons pas le temps de chercher constamment les choses importantes, alors assurez-vous de vous rendre service et ne perdez plus de temps à combattre l&#39;outil.  Réécrivez les règles et faites en sorte que l’outil fonctionne pour vous.

### Balise, c&#39;est toi !


## Auteur

Ce document a été rédigé par :

![Jeff Bloomer](assets/jeff-bloomer.png)

**Jeff Bloomer**, gestionnaire, Analyses numériques chez Kroger Personal Finance

Adobe Analytics Champion







