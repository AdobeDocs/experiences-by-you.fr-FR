---
title: Création de modèles de notation des personnes pour les programmes de Marketo Engage
description: Adobe Marketo Engage vous permet de créer vos modèles de notation à partir de zéro. Avant de vous lancer directement dans Marketo Engage pour créer vos programmes de notation, vous devrez configurer les champs de score essentiels tels que Score démographique, Score comportemental et Score total de personne. Découvrez les stratégies utilisées par les champions Marketo Engage pour développer des modèles de notation qui répondent aux besoins de votre entreprise.
role: Admin
level: Beginner
doc-type: Article
solution: Marketo Engage
duration: 0
last-substantial-update: 2024-05-04T00:00:00Z
jira: KT-14810
thumbnail: KT-14810.jpeg
source-git-commit: 47ab8875bc4e41595cd40550330e43a88357b68d
workflow-type: tm+mt
source-wordcount: '2111'
ht-degree: 2%

---

# Création d’un modèle de notation des personnes

Le score de personne vous permet d’identifier les personnes qui sont les plus impliquées dans votre entreprise et qui sont votre profil client idéal afin que vous puissiez partager ces pistes avec votre équipe de vente et conclure des offres ! Avec les ventes, vous déterminez les pistes que vous souhaitez leur transmettre à l’aide d’un programme de notation prospect/personne dans Adobe Marketo Engage. Cela peut être déterminé par un minimum de notation comportementale, de notation démographique, ou les deux.

Dans ce tutoriel, nous vous proposons trois exercices suggérés par les champions Marketo Engage Christina Zuniga et Katja Keesom. Procédez comme suit pour déterminer quelles activités et caractéristiques sont des indicateurs importants qu’un prospect est intéressé par les achats (notation comportementale) et qui sont adaptés à vous (notation démographique), et tenez compte des nuances entre les marchés.

## Pourquoi développer et utiliser un modèle de notation de personne ?

Votre base de données peut contenir de nombreux prospects, mais comment savoir lesquels sont prêts à acheter vos produits et services ? À mesure que votre organisation marketing s’efforce d’optimiser la qualité des pistes et la préparation aux ventes, c’est là que le modèle de notation entre en jeu.

En évaluant les personnes dans votre base de données de Marketo Engage, vous pouvez mesurer la qualification de vos pistes générées et définir des critères pour le moment où elles sont prêtes pour les ventes. Cela permet à votre équipe commerciale de se concentrer sur les pistes les plus susceptibles de se fermer, tandis que l’équipe marketing continue à nourrir les autres personnes de la base de données via leurs programmes marketing.

## Exercice 1 - Détermination de l’intérêt des acheteurs avec les scores comportementaux

La notation comportementale donne une valeur numérique aux actions pouvant faire l’objet d’un suivi qu’un prospect entreprendre indiquant son intérêt pour vos produits et services et son intention d’acheter. Par exemple, la visite du site web présente un intérêt et la consultation de la page de tarification peut indiquer des intentions. En revanche, la consultation de la page des carrières peut indiquer que la personne n’achètera pas.

**Étape 1** - Faites la liste des activités de prospect qui ont de l’importance pour votre processus de vente ou qui sont importantes pour votre organisation. Il peut s’avérer utile de collaborer avec votre équipe de vente pour déterminer les activités qui indiquent qu’un prospect a l’intention d’acheter, ce qui vous aide à aligner les critères sur les ventes et à établir des priorités en fonction de leurs observations sur les contrats à durée limitée. Voici quelques questions que vous pouvez poser à votre équipe commerciale :

* Quelles activités indiquent une bonne ou une mauvaise piste pour vous ?
* Quel type de contenu consommé par un prospect a une intention d’achat plus forte ?

**Étape 2** - Liste des actions qui indiquent qu’un prospect n’est pas intéressé par votre produit. Veillez à répertorier les activités pouvant faire l’objet d’un suivi via Marketo Engage.

**Exemple 1a - Activités indiquant une intention d’achat**

| **Activités indiquant l’intention d’acheter** | **Activités indiquant AUCUNE intention d’acheter** |
| --- | --- |
| Page de tarification des visites | Aucune interaction dans les 90 derniers jours |
| Participer à un événement client annuel | Visite de la page carrières |
| Inscrivez-vous au webinaire | Désabonnements |
| Télécharger le livre blanc |     |
| Remplissage du formulaire de démonstration de demande |     |

**Étape 3** - Analysez et choisissez un score de seuil de remise des ventes.

* Une fois qu’une piste indique un intérêt suffisant en effectuant certaines des activités que vous avez définies à l’étape 1 et que le score total dépasse ce seuil, vous les remettrez aux ventes. Ce seuil sera simplement un nombre qui permet de définir une référence pour les scores que vous affectez à des comportements individuels.
* Votre nombre seuil doit être suffisamment grand pour qu’une personne ait besoin d’effectuer plusieurs interactions avec votre marque pour y répondre. Par exemple, il est peu probable qu’une ouverture d’email soit un qualificateur suffisant. Si vous venez de commencer, essayez d’utiliser un seuil de 100 et d’élaborer la notation de votre personne à partir de là.
* La définition d’un seuil élevé ou faible dépend de l’équipe commerciale qui souhaite le plus bénéficier des opportunités commerciales et les développer. Si vous disposez de données sur vos offres récentes, analysez-les et découvrez les actions entreprises par les clients dans le cadre d’offres concluantes. Cela peut vous aider à déterminer le nombre de points de contact associés à une piste de vente qualifiée et à extrapoler à partir de là le nombre seuil à atteindre.

**Exemple 1b - Seuil de remise des ventes :**

| Nombre moyen de points de contact pour une piste qualifiée | 4 |
| --- | --- |
| Seuil de remise des ventes | 50 |

**Étape 4** - Attribuez un score à chaque activité répertoriée dans &quot;Exemple 1a - Activités indiquant une intention d’achat&quot;.

* Utilisez un score de comportement positif pour les activités qui indiquent un intérêt pour augmenter le score de prospect global d’un prospect et un score négatif pour indiquer un désintérêt.
* En utilisant votre seuil de &quot;Exemple 1b - Seuil de remise des ventes&quot; comme référence, déterminez vos scores de comportement par rapport à l’importance de leurs actions. Par exemple, les prospects qui demandent une démonstration doivent passer directement aux ventes. Il est logique d’attribuer à cette action une valeur de point égale à votre seuil de remise des prospects. En attendant, télécharger un livre blanc n&#39;est pas un indicateur aussi solide de l&#39;achat d&#39;intérêt et devrait donc valoir moins de points.

**Exemple 1c - Activités de notation indiquant l’intention d’acheter :**

| Seuil de remise des ventes = 50 points |     |
| --- | --- |
| Activité | Score |
| Remplissage de &quot;demande d’un formulaire de démonstration&quot; | +50 |
| Aucune interaction dans les 90 derniers jours | \-10 |
| Téléchargement d’un livre blanc | +5 |
| Visitez-nous à un salon | +15 |

**Étape 5** - Rappelez-vous, la notation est un processus itératif ! Examinez et ajustez continuellement les scores et les seuils lorsque vous collectez plus de données pour l’analyse.

## Exercice 2 - Identification de la bonne adéquation avec les scores démographiques

Maintenant que vous avez défini les activités indiquant l’intention d’achat, vous devez compléter le modèle de notation avec vos profils de prospects idéaux. Pour déterminer si un prospect est adapté à d’autres conversations de vente, il est important d’attribuer des scores démographiques en plus des scores comportementaux afin que le modèle détermine les meilleures pistes en termes d’ajustement et d’intention.

**Étape 1** - Faites la liste des caractéristiques de vos prospects idéaux.

* Envisagez de répertorier les attributs tels que leur secteur d’activité, leur société, leur département et leur rôle. Assurez-vous que ces caractéristiques correspondent aux champs démographiques disponibles dans votre instance de Marketo Engage.
* Collaborez avec votre équipe de vente afin de déterminer les prospects qui répondent le plus aux questions de vente et qui sont des contacts clés lors des opportunités de vente.
   * Il peut s’avérer utile d’analyser les opportunités récemment clôturées afin de déterminer les caractéristiques de vos meilleurs clients. Par exemple,
      * Parcourir les opportunités perdues et fermées de motifs peut vous conduire à trouver des données démographiques que vous souhaitez éviter.
      * Identifiez les décideurs et les champions internes qui vos efforts de vente. Explorez en détail les données et amenez vos résultats à un atelier avec une partie de votre équipe de vente afin de valider ou d’affiner vos conclusions.
   * Vous pouvez également interroger votre équipe commerciale avec les exemples de questions suivants :
      * Avec quel département sont-ils habituellement en contact ?
      * Quels sont les titres des postes des personnes impliquées dans les démonstrations de produits et qui sont les personnes devant valider l’achat ?

**Exemple 2a - Caractéristiques idéales des prospects**

| **Catégorie** | **Caractéristiques Idéales Du Prospect** |
| --- | --- |
| Secteur industriel | Aérospatiale, fabrication |
| Taille de l’entreprise | 100 - 999, 1 000 - 9 999 |
| Intitulé du poste | Director, vice-président, niveau C |
| Service | HR |

**Étape 2** - Attribuez un score à chaque caractéristique en fonction de sa pertinence dans votre profil de prospect idéal. Utilisez des scores positifs pour les caractéristiques souhaitables et des scores négatifs pour les caractéristiques qui rendent le prospect moins adapté à votre produit.

**Exemple 2b - Attribution de scores aux caractéristiques de perspective idéales et indésirables**

| **Caractéristique** | **Score** |
| --- | --- |
| Industrie - Aérospatiale | +10 |
| Secteur - Secteur manufacturier | +5 |
| Taille de l’entreprise - 100 à 999 | +5 |
| Taille de l’entreprise - 1 000 à 9 999 | +10 |
| Taille de l’entreprise - &lt;10 | \-10 |

## Exercice 3 - Inclure une flexibilité locale dans votre modèle de notation

Avec les modèles de notation comportementaux et démographiques de base que vous avez remplis, vous pouvez l’amener au niveau suivant en offrant une flexibilité locale. Les valeurs commerciales peuvent varier selon les marchés lorsqu’une organisation opère à l’échelle mondiale. Dans l’exercice suivant, vous apprendrez à appliquer des scores pour refléter la valeur réelle de l’entreprise des activités ou caractéristiques de prospect dans différentes situations.

Préférez-vous une présentation vidéo pour cet exercice ? Tune in as Marketo Engage Champion Katja Keesom démontre la flexibilité locale dans le modèle de notation.

>[!VIDEO](https://video.tv.adobe.com/v/3426914/?learn=on)

**Étape 1** - Prenez les activités et les caractéristiques des exercices 1 et 2 et déterminez pour chaque élément s’ils varient selon l’emplacement ou la ligne de produit.

**Exemple 3a - Signaux sur les marchés mondiaux et locaux :**

| **Signal** | **Global** | **Local** |
| --- | --- | --- |
| Activités | <ul><li>Formulaire &quot;Demander une démonstration&quot; rempli</li><li>Aucune interaction dans les 90 derniers jours (environ 3 mois)</li></ul> | <ul><li>Visitez-nous à l’atelier</li><li>Téléchargement d’un livre blanc</li></ul> |
| Caractéristiques | <ul><li>Service</li><li>Intitulé du poste</li></ul> | <ul><li>Secteur industriel</li><li>Taille de l’entreprise</li></ul> |

**Étape 2** - Définissez votre matrice de notation pour les marchés locaux :

* Configurez une matrice différente pour les éléments démographiques et comportementaux.
* Déterminez les thèmes sur lesquels vous devez demander l’avis de l’équipe locale.
* Définissez le nombre de valeurs utilisées pour évaluer dans vos rubriques.
* Attribuez des valeurs individuelles en alignant la valeur relative sur les scores globaux.
* Envisagez de définir des scénarios courants lorsque des prospects interagissent avec votre marque et de tester votre notation globale pour eux.
   * Par exemple, un parcours de prospect courant s’affiche lorsqu’une personne accède à votre site web sur une page de contenu, puis clique sur la page d’un produit et télécharge une brochure. Vous leur envoyez une invitation à un webinaire, à laquelle ils répondent en s&#39;inscrivant, mais sans participer. Déterminez si vos ventes souhaitent déjà parler à cette personne ou non et évaluez si votre modèle de notation permet à ces prospects d’obtenir le bon score global pour refléter ce niveau d’intérêt.

**Exemple 3b - Matrice de notation démographique :**

| **Matrice démographique** | **Priorité 1** | **Priorité 2** | **Priorité 3** |
| --- | --- | --- | --- |
| Valeurs élevées | 20 points | 10 points | 7 points |
| Valeurs moyennes | 10 points | 7 points | 3 points |
| Faibles valeurs | 5 points | 3 points | 1 point |

**Étape 3** - Collectez les commentaires de vos équipes commerciales locales ou régionales pour développer une vision globale. Vous remarquerez qu’aucun score individuel n’est inclus dans l’exemple 3c. Cela permet à l’équipe commerciale de se concentrer sur la valeur relative des différentes rubriques au cours du processus de révision. Cependant, votre modèle complet doit être documenté en tant que documents d’arrière-plan pour d’autres administrateurs de Marketo Engage.

* Verrouillez les éléments qui ne peuvent pas être ajustés pour la cohérence globale (ici dans la colonne &quot;Mise en oeuvre de la rubrique&quot;).
* Marquez (ici dans les colonnes &quot;Priorité&quot; et &quot;Score&quot;) ce qui peut être ajusté aux influences locales.

**Exemple 3c - Valeur relative des rubriques de notation :**

<table>
 <tr>
    <th>#</th>
    <th>Mise en oeuvre de la rubrique</th>
    <th>Démographique/Comportement</th>
    <th>Rubrique</th>
    <th>Priorité</th>
    <th>Valeurs</th>
    <th>Scores</th>
 </tr>
 <tr>
    <td rowspan="6">1</td>
    <td rowspan="6"><b>OBLIGATOIRE</b></td>
    <td rowspan="6">Démographique</td>
    <td rowspan="6">Secteur industriel</td>
    <td rowspan="6"><b>2</b></td>
    <td>Technologie</td>
    <td><b>Élevé</b></td>
  </tr>
  <tr>
    <td>Mode</td>
    <td><b>Élevé</b></td>
  </tr>
  <tr>
    <td>Vente au détail</td>
    <td><b>Méthode</b></td>
  </tr>  
  <tr>
    <td>Fabrication</td>
    <td><b>Méthode</b></td>
  </tr>
  <tr>
    <td>Soins de santé</td>
    <td><b>Faible</b></td>
  </tr>
  <tr>
    <td>…</td>
    <td><b>Faible</b></td>
  </tr>
<tr>
    <td rowspan="3">2</td>
    <td rowspan="3"><b>Oui</td>
    <td rowspan="3">Démographique</td>
    <td rowspan="3">Taille de l’entreprise (employés)</td>
    <td rowspan="3"><b>3</td>
    <td>&gt;1 000 employés</td>
    <td><b>Élevé</td>
  </tr>
  <tr>
    <td>250 à 999 employés</td>
    <td><b>Méthode</td>
  </tr>
  <tr>
    <td>1 à 249 employés</td>
    <td><b>Faible</td>
  </tr>  
<tr>
    <td rowspan="3">3</td>
    <td rowspan="3"><b>Non</b></td>
    <td rowspan="3">Comportement</td>
    <td rowspan="3">Visites de page sur votre site web</td>
    <td rowspan="3"><b>2</b></td>
    <td>&gt;Pages d’informations sur les produits</td>
    <td><b>Faible</b></td>
  </tr>
  <tr>
    <td>Pages de tarifs</td>
    <td><b>Méthode</b></td>
  </tr>
  <tr>
    <td>Page de demande de démonstration</td>
    <td><b>Élevé</b></td>
  </tr>
</table>

## Et après ?

* Téléchargez la [feuille d’exercice de notation des personnes](./assets/build-person-scoring-model-and-local-flexibility-in-adobe-marketo-engage.docx){target="_blank} pour développer votre modèle de notation hors ligne.
* Créez la notation de votre personne en Marketo Engage. Vérifier [tutoriel](https://experienceleague.adobe.com/en/docs/marketo-learn/tutorials/lead-and-data-management/lead-scoring-watch){target="_blank} et [demo](https://experienceleague.adobe.com/en/docs/events/marketo-and-mochas-recordings/2023/lead-scoring){target="_blank} pour commencer. Vous pouvez importer un programme de notation prospect/personne [modèle](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program){target="_blank} à partir de la bibliothèque de référence du Marketo Engage pour accélérer la création du programme.
* Créez deux versions du programme de notation :
   * Un programme central qui exécute toute notation qui ne peut pas être mise à jour localement.
   * Une copie locale avec les éléments de notation configurables.
* Configurez vos valeurs de notation en tant que jetons dans votre programme de notation. Cela garantit la cohérence même lorsque vous ajustez les scores au fil du temps.
   * Un exemple courant de scores segmentés en jetons consiste à disposer d’un jeton pour les activités de grande valeur qui correspondent automatiquement à votre seuil, comme la demande d’une démonstration ou la réservation d’une réunion avec votre équipe de vente. Même si vous modifiez le score minimum requis pour atteindre votre seuil, vous pouvez facilement mettre à jour toutes les activités à forte valeur simultanément en mettant à jour un jeton.
* Ajustez votre campagne dynamique locale pour chaque emplacement :
   * Déterminez les données démographiques et les activités comportementales qui ne doivent noter qu’une seule fois (c’est-à-dire l’industrie) et qui doivent noter chaque fois qu’un prospect est admissible (c’est-à-dire qu’il a participé à un webinaire). Cela garantit que les contacts potentiels déclenchés par le changement de valeur de données sont pertinents pour les ventes.
   * Vérifiez que vos choix s’excluent mutuellement.
   * Effectuez vos mises à jour dans les deux étapes de flux afin que le score de personne soit mis à jour de la même manière que le score démographique. Ainsi, le score de personne reste en ligne avec la combinaison du score de comportement et du score démographique.
* Testez la campagne dynamique une fois la création de votre programme terminée. Par exemple, accédez à votre formulaire de démonstration, renseignez-le avec un e-mail de test et vérifiez le score de votre personne de test dans [Base de données Marketo Engage](https://experienceleague.adobe.com/en/docs/marketo/using/getting-started-with-marketo/quick-wins/simple-scoring#step-view-the-person-info){target="_blank}.
* Après avoir créé votre modèle, envisagez de configurer une alerte pour augmenter les ventes une fois que le score de la personne a atteint le seuil de remise des ventes. En savoir plus sur la configuration d’une alerte avec cette [tutoriel](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert){target="_blank}.

### Auteurs

{{christina-zuniga}}

{{katja-keesom}}

{{amy-chiu}}