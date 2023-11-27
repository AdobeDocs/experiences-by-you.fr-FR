---
title: Créer des modèles de code normalisés
description: Pour une mise en oeuvre de base (c’est-à-dire ce que votre entreprise considère comme les indicateurs de performance clés obligatoires pour tous) [!DNL Adobe Analytics] sites), votre organisation doit disposer d’une méthode de mise en oeuvre unique, si possible.
solution: Analytics
feature-set: Analytics
feature: Implementation Basics
topic: Administration
role: Admin
level: Beginner
doc-type: article
thumbnail: 10532.jpg
kt: 10532
exl-id: edd3df73-6d1a-4a26-a984-810cc7dd382f
source-git-commit: 058d26bd99ab060df3633fb32f1232f534881ca4
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 90%

---

# Créer des modèles de code normalisés

**QUOI :**[!DNL Adobe Analytics] pour une implémentation « de base » (c’est-à-dire ce que votre entreprise considère comme des indicateurs de performance clés obligatoires pour tous les sites ), votre organisation doit disposer d’une méthode d’implémentation unique, dans la mesure du possible. Par exemple, utilisez la même structure de couche de données sur plusieurs sites et utilisez le même code personnalisé/règle de gestionnaire de balises pour capturer des éléments tels que des recherches internes ou des informations de profil du visiteur.

**POURQUOI :** une implémentation de base répétable et évolutive permet d’ajouter de nouveaux éléments ou de nouveaux sites/applications dans un effort réduit et rationalisé, tout en préservant votre implémentation et en facilitant la résolution des problèmes. L’utilisation d’une méthode uniforme permet également aux nouveaux administrateurs/développeurs de se connecter et de comprendre ce avec quoi ils travaillent.

**COMMENT :** adoptez un modèle de format unique à transmettre aux développeurs lorsqu’un nouveau site ou une amélioration du balisage est en ligne. En règle générale, un document Word fonctionne bien quand vous pouvez mettre en avant les éléments suivants :

* Variables en cours d’implémentation, leur objectif et quand les définir. Par exemple :

| Variable AA | Description | Quand/où définir | Comment définir |
|--- |--- |--- |--- |
| eVar8 | Mots-clés de recherche interne | En arrivant sur la page de résultats de recherche interne | Couche de données |
| event8 | Nombre de recherches internes | En arrivant sur la page de résultats de recherche interne | Règle Launch |

* Précisions sur la définition. C’est là que vous spécifiez les objets de couche de données nécessaires, leur syntaxe ainsi que les règles TMS à configurer et les détails de la configuration des règles.
* Les cas de test pour vous tout vérifier sont couverts dans l’assurance qualité et toutes les variables que vous vous attendez à voir dans un cas de test réussi. Décrivez ce qu’une implémentation réussie doit inclure lorsque le développeur teste cette amélioration.

Idéalement, il suffira de modifier ce document pour le site suivant où vous mettez à jour les éléments de base tels que le nom de la propriété, la convention de nommage des pages, etc. Pas besoin de réinventer la roue à chaque fois, et vous pouvez gagner du temps.

## Auteurs

Ce document a été rédigé par :

![Christel Guidon](assets/Christel-Headshot-150.png)

Christel Guidon, Digital [!DNL Analytics] Platform Manager dans NortonLifeLock
[!DNL Adobe Analytics] Champion

![Rachel Fenwick](assets/Rachel-Fenwick-150.png)

Rachel Fenwick, conseillère principale chez [!DNL Adobe]
