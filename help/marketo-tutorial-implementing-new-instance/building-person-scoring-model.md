---
title: Créer des modèles de notation de personne pour les programmes Marketo Engage
description: Découvrez comment créer vos modèles de notation à partir de zéro.
role: Admin
level: Beginner
doc-type: Article
solution: Marketo Engage
duration: 0
last-substantial-update: 2024-05-04T00:00:00Z
jira: KT-14810
thumbnail: KT-14810.jpeg
exl-id: 73976144-f02b-4423-9b4b-410330117ba9
source-git-commit: 1205848b1985a99b91f9d4d25e1a79f0df379589
workflow-type: tm+mt
source-wordcount: '2148'
ht-degree: 2%

---

# Créer un modèle de notation de personne

La notation des personnes vous permet d’identifier les personnes les plus impliquées dans votre entreprise et qui constituent votre profil client idéal, afin que vous puissiez partager ces prospects avec votre équipe de vente et conclure des affaires ! En collaboration avec les ventes, vous déterminez les prospects que vous souhaitez leur transmettre à l’aide d’un programme de notation des prospects/personnes dans Adobe Marketo Engage. Cela peut être déterminé par un score comportemental minimal, un score démographique ou les deux.

Dans ce tutoriel, nous vous proposons trois exercices proposés par Christina Zuniga et Katja Keesom, championnes de Marketo Engage. Suivez afin de déterminer quelles activités et caractéristiques sont des indicateurs importants qu’un prospect souhaite acheter (score comportemental) et qui vous conviennent (score démographique), et tenez compte des nuances entre les marchés.

## Pourquoi développer et utiliser un modèle de notation de personne ?

Votre base de données contient peut-être de nombreux prospects, mais comment savoir lesquels sont prêts à acheter vos produits et services ? Lorsque votre organisation marketing cherche à optimiser la qualité des prospects et la préparation des ventes, c’est là que le modèle de notation entre en jeu.

En notant les personnes dans votre base de données Marketo Engage, vous pouvez évaluer le degré de qualification des prospects générés et définir des critères pour le moment où ils sont prêts à être vendus. Cela permet à votre équipe de vente de se concentrer sur les prospects les plus susceptibles de fermer pendant que l’équipe marketing continue à soutenir les autres personnes dans la base de données via leurs programmes marketing.

## Exercice 1 - Déterminer l&#39;intérêt de l&#39;acheteur avec les scores comportementaux

La notation comportementale donne une valeur numérique aux actions qu’un prospect peut suivre et qui indiquent son intérêt pour vos produits et services, ainsi que son intention d’achat. Par exemple, une visite du site web indique un intérêt, et une visite de la page de tarification peut indiquer l’intention. En revanche, la consultation de la page Carrières peut indiquer que la personne ne compte pas acheter.

**Étape 1** - Établissez une liste des activités des prospects qui comptent pour votre processus de vente ou qui sont importantes pour votre entreprise. Il peut s’avérer utile de travailler avec votre équipe des ventes pour déterminer quelles activités indiquent qu’un prospect a l’intention d’acheter, ce qui vous aide à aligner les critères sur les ventes et à établir des priorités en fonction de leurs observations des affaires conclues. Voici quelques questions suggérées que vous pouvez poser à votre équipe des ventes :

* Quelles sont les activités qui indiquent une bonne ou une mauvaise piste ?
* Quel type de contenu consommé par un prospect a une intention d’achat plus forte ?

**Étape 2** - Répertoriez les actions qui indiquent qu’un prospect n’est pas intéressé par votre produit. Veillez à répertorier les activités pouvant être suivies via Marketo Engage.

**Exemple 1a - Activités indiquant l’intention d’acheter**

| **Activités indiquant l’intention d’acheter** | **Activités indiquant AUCUNE intention d’achat** |
| --- | --- |
| Page de tarification de la visite | Aucune interaction au cours des 90 derniers jours |
| Assister à l’événement client annuel | Page Visiter les carrières |
| S’inscrire au webinaire | Désabonnements |
| Télécharger l’article technique |     |
| Remplir le formulaire de démonstration de la demande |     |

**Étape 3** - Analysez et choisissez un score de seuil de remise des ventes.

* Une fois qu’un prospect fait preuve d’un intérêt suffisant en exécutant certaines des activités que vous avez définies à l’étape 1 et que le score total dépasse ce seuil, vous le remettrez aux ventes. Ce seuil sera simplement un nombre qui aidera à établir un point de référence pour les scores que vous attribuez à des comportements individuels.
* Votre nombre seuil doit être suffisamment élevé pour qu’une personne ait à effectuer plusieurs interactions avec votre marque pour l’atteindre. Par exemple, il est peu probable qu’une ouverture d’e-mail soit un qualificateur suffisant. Si vous venez de commencer, essayez de travailler avec un seuil de 100 et de créer votre score de personne à partir de là.
* Définir un seuil élevé ou faible dépend des prospects que votre équipe de vente souhaite le plus recevoir et développer en opportunités commerciales. Si vous disposez de données existantes sur vos ventes récentes, analysez-les et voyez quelles mesures les clients ont prises dans les affaires réussies. Cela peut vous aider à déterminer le nombre de points de contact inclus dans un prospect commercial qualifié et à extrapoler à partir de là votre nombre seuil.

**Exemple 1b - Seuil pour la remise des ventes :**

| Nombre moyen de points de contact pour le prospect qualifié | 4 |
| --- | --- |
| Seuil de remise des ventes | 50 |

**Étape 4** - Attribuez un score à chaque activité répertoriée dans &#39;Exemple 1a - Activités indiquant l&#39;intention d&#39;acheter&#39;.

* Utilisez un score de comportement positif pour les activités qui indiquent un intérêt afin d’augmenter le score global des prospects et un score négatif pour indiquer un désintérêt.
* À l’aide du seuil de « Exemple 1b - Seuil de remise des ventes » comme référence, déterminez vos scores de comportement par rapport à l’importance de leurs actions. Par exemple, les prospects qui demandent une démonstration doivent accéder directement aux ventes. Le plus logique consiste à attribuer à cette action une valeur de point égale à votre seuil de remise de prospect. En attendant, télécharger un livre blanc n&#39;est pas un indicateur aussi fort de l&#39;intérêt d&#39;achat et devrait donc valoir moins de points.

**Exemple 1c - Notation des activités indiquant l’intention d’achat :**

| Seuil de remise des ventes = 50 points |     |
| --- | --- |
| Activité | Score |
| A rempli « demander un formulaire de démonstration » | +50 |
| Aucune interaction au cours des 90 derniers jours | \-10 |
| Télécharger un livre blanc | +5 |
| Rendez-vous sur un salon professionnel | +15 |

**Étape 5** - Souvenez-vous que la notation est un processus itératif ! Examinez et ajustez en permanence les scores et les seuils à mesure que vous collectez davantage de données à analyser.

## Exercice 2 - Déterminer la bonne adéquation avec les scores démographiques

Maintenant que vous avez défini les activités indiquant l’intention d’achat, vous devez compléter le modèle de notation avec vos profils de prospects idéaux. Pour déterminer si un prospect convient à une conversation commerciale ultérieure, il est important d’attribuer des scores démographiques en plus des scores comportementaux afin que le modèle puisse déterminer les meilleurs prospects en termes d’adéquation et d’intention.

**Étape 1** - Faites une liste des caractéristiques pour vos prospects idéaux.

* Pensez à répertorier les attributs tels que le secteur, la société, le service et le rôle. Assurez-vous que ces caractéristiques correspondent aux champs démographiques disponibles dans votre instance Marketo Engage.
* Collaborez avec votre équipe des ventes pour déterminer quels prospects répondent le plus aux demandes de renseignements sur les ventes et constituent des contacts clés lors des occasions de vente.
   * Il peut s’avérer utile d’analyser les opportunités récemment closes et confirmées pour déterminer les caractéristiques de vos meilleurs clients. Par exemple,
      * Explorez les opportunités perdues et clôturées pour identifier des modèles afin de trouver les données démographiques à éviter.
      * Identifiez les décideurs et les champions internes qui pilotent vos efforts de vente. Plongez-vous dans les données et présentez vos conclusions à un atelier avec une partie de votre équipe de vente afin de les valider ou de les affiner.
   * Vous pouvez également interroger votre équipe des ventes avec les exemples de questions suivants :
      * Avec quel ministère travaillent-ils habituellement?
      * Quels sont les titres des postes des personnes impliquées dans les démonstrations de produits et qui sont les personnes qui doivent approuver l’achat ?

**Exemple 2a - Caractéristiques idéales du prospect**

| **Catégorie** | **Caractéristiques de perspective idéales** |
| --- | --- |
| Secteur industriel | Aérospatiale, fabrication |
| Taille de l&#39;entreprise | 100 - 999, 1 000 - 9 999 |
| Intitulé du poste | Directeur, Vice-Président, Niveau C |
| Service | H |

**Étape 2** - Attribuez un score à chaque caractéristique en fonction de sa pertinence dans votre profil de prospect idéal. Utilisez des scores positifs pour les caractéristiques souhaitables et des scores négatifs pour les caractéristiques qui rendent le prospect moins adapté à votre produit.

**Exemple 2b - Attribution de scores aux caractéristiques idéales et indésirables du prospect**

| **Caractéristique** | **Score** |
| --- | --- |
| Industrie - Aérospatiale | +10 |
| Industrie - Fabrication | +5 |
| Taille de l&#39;entreprise - 100 - 999 | +5 |
| Taille de l&#39;entreprise - 1 000 - 9 999 | +10 |
| Taille de l&#39;entreprise - &lt;10 | \-10 |

## Exercice 3 - Incorporer la flexibilité locale dans votre modèle de notation

Avec les modèles de notation comportementale et démographique de base que vous avez complétés, vous pouvez passer au niveau supérieur en permettant une flexibilité locale. Les valeurs d’entreprise peuvent varier selon les marchés lorsqu’une organisation opère à l’échelle mondiale. Dans l’exercice suivant, vous apprendrez à appliquer des scores pour refléter la valeur commerciale réelle des activités ou caractéristiques du prospect dans différentes situations.

Préférez-vous une présentation vidéo pour cet exercice ? Katja Keesom, championne de Marketo Engage, démontre l’importance de la flexibilité locale dans le modèle de notation.

>[!VIDEO](https://video.tv.adobe.com/v/3457441/?captions=fre_fr&learn=on)

**Étape 1** - Prenez les activités et les caractéristiques des exercices 1 et 2 et déterminez pour chaque article si elles varient selon l&#39;emplacement ou la gamme de produits.

**Exemple 3a - Signaux sur les marchés mondiaux et locaux :**

| **Signal** | **Global** | **Local** |
| --- | --- | --- |
| Activities | <ul><li>Rempli le formulaire « Demander une démonstration »</li><li>Aucune interaction au cours des 90 derniers jours (environ 3 mois)</li></ul> | <ul><li>Visitez-nous au salon professionnel</li><li>Télécharger un livre blanc</li></ul> |
| Caractéristiques | <ul><li>Service</li><li>Fonction</li></ul> | <ul><li>Secteur</li><li>Taille de l&#39;entreprise</li></ul> |

**Étape 2** - Définissez votre matrice de notation pour les marchés locaux :

* Configurez une matrice différente pour les éléments démographiques et comportementaux.
* Déterminez les sujets prioritaires sur lesquels vous pourrez demander l&#39;avis de l&#39;équipe locale.
* Définissez le nombre de valeurs utilisées pour évaluer dans vos rubriques.
* Attribuez des valeurs individuelles en alignant la valeur relative sur les scores globaux.
* Pensez à définir des scénarios courants lorsque les prospects interagissent avec votre marque et testez votre score global pour ces scénarios.
   * Par exemple, un parcours de prospects courant que vous voyez est qu’une personne accède à votre site web sur une page de contenu, puis clique sur une page de produit et télécharge une brochure. Vous pouvez les cibler avec une invitation à un webinaire, et ils y répondent en s’enregistrant, mais sans y assister. Déterminez si vos ventes souhaitent déjà parler à cette personne ou non et évaluez si votre modèle de notation porte ces prospects à la bonne note globale pour refléter ce niveau d’intérêt.

**Exemple 3b - Matrice de notation démographique :**

| **Matrice démographique** | **Priorité 1** | **Priorité 2** | **Priorité 3** |
| --- | --- | --- | --- |
| Valeurs élevées | 20 points | 10 points | 7 points |
| Valeurs de Medium | 10 points | 7 points | 3 points |
| Valeurs faibles | 5 points | 3 points | 1 point |

**Étape 3** - Recueillez les commentaires de vos équipes de vente locales ou régionales afin de développer une vue d&#39;ensemble. Vous remarquerez qu’aucune note individuelle n’est incluse dans l’exemple 3c. Cela permet à l&#39;équipe de vente de se concentrer sur la valeur relative des différents sujets pendant le processus de révision. Cependant, vous devez documenter votre modèle complet comme documents de base pour d’autres administrateurs et administratrices Marketo Engage.

* Verrouillez ce qui ne peut pas être ajusté pour la cohérence globale (ici, dans la colonne « Implémenter la rubrique »).
* Notez (ici, dans les colonnes « Priorité » et « Score ») les éléments ajustables en fonction des influences locales.

**Exemple 3c - Valeur relative des rubriques de notation :**

<table>
 <tr>
    <th>#</th>
    <th>Implémenter la rubrique</th>
    <th>Données démographiques/comportementales</th>
    <th>Rubrique</th>
    <th>Priorité</th>
    <th>Valeurs</th>
    <th>Notes</th>
 </tr>
 <tr>
    <td rowspan="6">1</td>
    <td rowspan="6"><b>OBLIGATOIRE</b></td>
    <td rowspan="6">Démographie</td>
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
    <td rowspan="3">Démographie</td>
    <td rowspan="3">Taille de l'entreprise (employés)</td>
    <td rowspan="3"><b>3</td>
    <td>&gt;1000 employés</td>
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
    <td rowspan="3">Comportemental</td>
    <td rowspan="3">Visites de pages sur votre site web</td>
    <td rowspan="3"><b>2</b></td>
    <td>&gt;Pages d’informations sur les produits</td>
    <td><b>Faible</b></td>
  </tr>
  <tr>
    <td>Pages de tarification</td>
    <td><b>Méthode</b></td>
  </tr>
  <tr>
    <td>Page de demande de démonstration</td>
    <td><b>Élevé</b></td>
  </tr>
</table>

## Quelle est la prochaine étape ?

* Téléchargez la [feuille d’exercice de notation de personne](./assets/build-person-scoring-model-and-local-flexibility-in-adobe-marketo-engage.docx){target=« _blank} pour développer votre modèle de notation hors ligne.
* Définissez le score de votre personne dans Marketo Engage. Consultez ce [tutoriel](https://experienceleague.adobe.com/fr/docs/marketo-learn/tutorials/lead-and-data-management/lead-scoring-watch){target=« _blank} et [démonstration](https://experienceleague.adobe.com/fr/docs/events/marketo-and-mochas-recordings/2023/lead-scoring){target=« _blank} pour commencer. Vous pouvez importer un programme de notation des prospects/personnes [modèle](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program){target=« _blank} à partir de la bibliothèque de référence Marketo Engage afin d’accélérer la création du programme.
* Créez deux versions du programme de notation :
   * Un programme central qui exécute tous les scores qui ne peuvent pas être mis à jour localement.
   * Une copie locale avec les éléments de score configurables.
* Configurez vos valeurs de notation en tant que jetons dans votre programme de notation. Cela garantit la cohérence même lorsque vous ajustez les scores au fil du temps.
   * Un exemple courant de scores segmentés en unités lexicales consiste à disposer d’un jeton pour les activités à forte valeur qui respectent automatiquement votre seuil, telles que la demande d’une démonstration ou la réservation d’une réunion avec votre équipe commerciale. Même si vous modifiez le score minimum requis pour atteindre votre seuil, vous pouvez facilement mettre à jour toutes les activités à forte valeur en même temps en mettant à jour un jeton.
* Ajustez votre campagne intelligente locale pour chaque emplacement :
   * Déterminez les données démographiques et les activités comportementales qui ne doivent être évaluées qu’une seule fois (par exemple, le secteur) et celles qui doivent l’être chaque fois qu’un prospect se qualifie (par exemple, il a participé à un webinaire). Cela permet de s’assurer que les contacts potentiels déclenchés par la modification de la valeur des données sont pertinents pour les ventes.
   * Assurez-vous que vos choix s’excluent mutuellement.
   * Effectuez vos mises à jour dans les deux étapes de flux afin que le score de personne soit mis à jour de manière identique au score démographique. Ainsi, le score de personne reste cohérent avec la combinaison du score comportemental et du score démographique.
* Testez la campagne intelligente une fois que vous avez terminé de créer votre programme. Par exemple, accédez à votre formulaire de démonstration, remplissez-le avec un e-mail de test, puis vérifiez le score de votre personne de test dans la base de données [&#128279;](https://experienceleague.adobe.com/fr/docs/marketo/using/getting-started-with-marketo/quick-wins/simple-scoring#step-view-the-person-info){target=« _blank}.
* Après avoir créé votre modèle, envisagez de configurer une alerte pour atteindre les ventes une fois que le score de la personne a atteint votre seuil de remise des ventes. En savoir plus sur la configuration d’une alerte avec ce [tutoriel](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert){target=« _blank}.

### Auteurs

{{christina-zuniga}}

{{katja-keesom}}

{{amy-chiu}}
