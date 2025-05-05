---
title: Résolution de problèmes pour les spécialistes du marketing
description: Connaître les erreurs les plus courantes peut vous aider à résoudre plus rapidement les problèmes et améliorer votre productivité. Ces conseils de dépannage vous aident à résoudre efficacement des erreurs similaires lorsqu’elles se produisent.
solution: Campaign Standard
feature-set: Campaign
feature: Workflows
role: User
level: Beginner, Intermediate, Experienced
doc-type: Article
last-substantial-update: 2023-05-18T00:00:00Z
jira: KT-13256
thumbnail: KT-13256.jpeg
exl-id: 1f27e284-73e3-4f28-988e-51163775eec8
source-git-commit: 02e3a6dfa59df45113242bd8e874e18e9e1efd58
workflow-type: tm+mt
source-wordcount: '711'
ht-degree: 2%

---

# Dépannage pour les marketeurs : 5 erreurs courantes de workflow et de diffusion

Par : [Suraj Patra](https://www.linkedin.com/in/suraj-p-51612053/){target="_blank"}, consultant principal, Meijer

En tant qu&#39;ingénieur principal et expert client de [!DNL Adobe] produits Experience Cloud depuis cinq ans, je permet aux utilisateurs d&#39;entreprise de [Meijer](https://www.meijer.com/){target="_blank"}, une chaîne de supercentres américaine fondée en 1934, d&#39;exécuter des campagnes marketing et transactionnelles complexes avec ACS. Parmi les projets sur lesquels j’ai travaillé, citons les campagnes personnalisées pour stocker les offres et les détails de commande pour la personnalisation, l’intégration à l’Audience Manager [!DNL Adobe] et les informations sur les clients pour l’ingestion de segments.

En utilisant ACS, j&#39;ai rencontré des erreurs qui peuvent prendre du temps et être frustrantes à résoudre. Connaître les erreurs les plus courantes peut vous aider à résoudre plus rapidement les problèmes et améliorer votre productivité. Vous trouverez ci-dessous mes conseils de dépannage pour vous aider à résoudre efficacement des erreurs similaires lorsqu’elles se produisent.

## Erreur de correspondance du type de données

**Code d’erreur :**
`PGS-220000 PostgreSQL error: ERROR: operator does not exist: character varying = bigint`

**Cause :**
Ces types d&#39;erreurs apparaissent dans un workflow lorsque vous essayez de vous réconcilier à l&#39;aide de champs de différents types de données. Par exemple, lorsque vous téléchargez un fichier à l’aide d’un fichier de chargement comportant un champ de chaîne et que vous essayez de réconcilier le champ de chaîne avec un champ de profil dont le type de données est int.

![data-type-mismatch-error](/help/_assets/kt-13256/data-type-mismatch.png)

**Solution :**
Remplacez le type de données du champ de l&#39;activité &quot;Chargement de fichier&quot; par celui avec lequel vous faites correspondre. Ouvrez l&#39;activité &quot;Chargement de fichier&quot;. Accédez à l&#39;onglet &quot;DÉFINITION DES COLONNES&quot; et modifiez le type de données du champ de votre choix.


![data-type-mismatch-solution](/help/_assets/kt-13256/data-type-mismatch-solution.png)

## Erreur du Personalization de diffusion

**Code d’erreur :**
`The schema for profiles specified in the transition ('') is not compatible with the schema defined in the delivery template ('nms:recipient'). They should be identical.`

**Cause :**
Cette erreur s’affiche lorsque vous envoyez un email à une adresse, mais que l’email ou tout autre identifiant n’est pas réconcilié avec un profil. Pour envoyer une communication par email, l&#39;email ou l&#39;identifiant doit toujours être associé à un profil.

![ workflow avec activité de réconciliation](/help/_assets/kt-13256/del-persn-error-wf.png)

**Solution :**
Un identifiant commun doit exister à partir du fichier chargé avec la table des destinataires. Cette clé commune relie le fichier de chargement à la table des destinataires dans l&#39;activité de réconciliation. Les emails ne peuvent pas être envoyés aux enregistrements qui n&#39;existent pas dans la table des destinataires et qui nécessitent cette étape de réconciliation dans le workflow. Ce faisant, vous réconciliez l’activité de chargement de fichier entrant avec un identifiant comme l’ID d’email du profil. Le schéma `nms:recipient` fait référence à la table des profils et la réconciliation des enregistrements entrants avec le profil le rend disponible lors de la préparation des emails.

Reportez-vous à la capture d&#39;écran de l&#39;activité de réconciliation comme illustré ci-dessous.

![ workflow avec détail de réconciliation](/help/_assets/kt-13256/del-persn-error-wf-solution.png)

En savoir plus sur [reconciliation](https://experienceleague.adobe.com/docs/campaign-standard/using/managing-processes-and-data/data-management-activities/reconciliation.html?lang=fr).

## Erreur du jeu de données de champ commun

**Code d’erreur :**
`The document types of inbound events (''and'') are incompatible (step 'Exclusion'). Unable to perform the operation. `

**Cause :**
Ce problème se produit lors de l’utilisation de l’ **activité d’exclusion** dans les workflows ACS, lors de l’exécution d’une exclusion basée sur l’identifiant, lorsque le jeu de Principal et l’ensemble exclu n’ont pas les mêmes noms de champ.


![Erreur du jeu de données de champ commun](/help/_assets/kt-13256/dataset-error.png)

**Solution :**

Cette erreur peut être résolue de deux manières différentes :

1. Utilisez le même nom de champ dans le champ principal et le champ exclu et utilisez ce champ comme ID

   OR

2. Utilisez la méthode d&#39;exclusion JOINS pour sélectionner le champ sur lequel vous souhaitez exclure les enregistrements.

![Erreur du jeu de données de champ commun - Solution ](/help/_assets/kt-13256/dataset-error-solution.png)

## Nom du champ Erreur de suppression

**Code d’erreur :**
`XTK-170036 Unable to parse expression 'i__name'`

**Cause :**

Les points d&#39;échec peuvent se produire dans une **activité d&#39;enrichissement**. L’une des plus courantes est affichée ci-dessous.

![Nom du champ Erreur de suppression](/help/_assets/kt-13256/field-name-dropped-error.png)

Cela se produit lorsque vous modifiez manuellement le nom d’une expression dans l’activité. L’image montre que l’expression a été modifiée de `name ` à `i__name`.

**Solution :**

Vous pouvez résoudre cette erreur de trois façons :

1. Remplacez le nom par l’expression qui était présente à l’origine.

2. Si vous souhaitez utiliser un nouveau nom, modifiez les valeurs de l&#39; **activité d&#39;enrichissement**.

3. Si vous ne vous souvenez pas de ce qui a changé, il est préférable de recréer l’activité.

## Erreur de suppression de la table temporaire 

**Code d’erreur :**
`XTK-170024 The temporary schema "temp:deliveryEmail1" is not defined in the current context.`

**Cause :**
Il s’agit d’une erreur courante dans les workflows complexes impliquant un enrichissement ou une autre activité. Cela signifie probablement que certains workflows d’activité ne sont pas correctement enregistrés lors de plusieurs modifications apportées au workflow.

![Erreur de suppression de table temporaire ](/help/_assets/kt-13256/temp-table-dropped-error.png)

**Solution :**
Cette erreur peut se produire de nombreuses façons, il n’existe donc pas de solution simple. S’il s’agit d’un workflow simple, il serait préférable de reconfigurer l’activité. Dans un workflow complexe, il est préférable de copier les activités du workflow dans un nouveau workflow, de les enregistrer et de les réexécuter.
