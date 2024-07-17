---
title: Créer des modèles de code normalisés
description: Pour une mise en oeuvre de base (c’est-à-dire ce que votre entreprise considère comme des indicateurs de performance clés obligatoires pour tous les  [!DNL Adobe Analytics] sites), votre organisation doit disposer d’une méthode de mise en oeuvre unique si possible.
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
ht-degree: 0%

---

# Créer des modèles de code normalisés

**QUOI :** Pour une mise en oeuvre &quot;de base&quot; (c’est-à-dire ce que votre entreprise considère comme des indicateurs de performance clés obligatoires pour tous les [!DNL Adobe Analytics] sites), votre organisation doit disposer d’une méthode de mise en oeuvre unique si possible. Par exemple, utilisez la même structure de couche de données sur plusieurs sites et utilisez le même code personnalisé/règle de gestionnaire de balises pour capturer des éléments tels que des recherches internes ou des informations de profil du visiteur.

**POURQUOI :** L’ajout d’une mise en oeuvre de base répétable et évolutive simplifie l’ajout de nouveaux éléments ou de nouveaux sites/applications tout en simplifiant et en simplifiant votre mise en oeuvre et en simplifiant le dépannage. L’utilisation d’une méthode uniforme permet également aux nouveaux administrateurs/développeurs de se connecter et de comprendre leur fonctionnement.

**COMMENT :** Adoptez un modèle de format unique à remettre aux développeurs lorsqu’un nouveau site ou une amélioration du balisage est en ligne. En règle générale, un document Word fonctionne bien où vous pouvez mettre en avant les éléments suivants :

* Variables en cours de mise en oeuvre, leur objectif et le moment où les définir. Par exemple :

| Variable AA | Description | Quand/où définir | Comment définir |
|--- |--- |--- |--- |
| eVar8 | Mots-clés de recherche interne | À l’entrée de la page de résultats de recherche interne | couche de données |
| event8 | Nombre de recherches internes | À l’entrée de la page de résultats de recherche interne | Règle de lancement |

* Découvrez comment définir. C’est là que vous spécifiez les objets de couche de données nécessaires, leur syntaxe ainsi que les règles TMS à configurer et les détails de la configuration des règles.
* Les cas de test pour vous assurer sont couverts dans l’assurance qualité et toutes les variables que vous prévoyez de voir dans un cas de test réussi. Décrivez ce qu’une mise en oeuvre réussie doit inclure lorsque le développeur teste cette amélioration.

Idéalement, il suffira de modifier ce document pour le site suivant où vous mettez à jour les éléments de base tels que le nom de la propriété, la convention d’appellation des pages, etc. Pas besoin de réinventer la roue à chaque fois, et vous pouvez gagner du temps.

## Auteurs

Ce document a été co-écrit par :

![Christel Guidon](assets/Christel-Headshot-150.png)

Christel Guidon, responsable de la plateforme numérique [!DNL Analytics] chez NortonLifeLock
[!DNL Adobe Analytics] champion

![Rachel Fenwick](assets/Rachel-Fenwick-150.png)

Rachel Fenwick, conseillère principale à [!DNL Adobe]
