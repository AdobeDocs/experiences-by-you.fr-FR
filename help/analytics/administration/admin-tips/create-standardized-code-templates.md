---
title: Créer des modèles de code normalisés
description: Pour une implémentation de base (c’est-à-dire ce que votre entreprise considère comme des indicateurs de performance clés obligatoires pour tous les sites [!DNL Adobe Analytics]), votre organisation doit disposer d’une méthode d’implémentation unique, dans la mesure du possible.
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
product_v2:
  - id: e55547f1-a1ff-40c6-8978-026e40ab7fa4
    internal-label: Analytics
feature_v2:
  - id: a421fb65-2c82-457a-921c-28c46b697a39
    internal-label: Analytics basics
subfeature_v2:
  - id: c24fe15a-643a-47bd-8278-5e027df49785
    internal-label: Implementation basics
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
source-git-commit: 749b293ab38b8ea5a5f72517bd5c3455399137c2
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 0%
---
# Créer des modèles de code normalisés

**QUOI :** pour une implémentation « de base » (c’est-à-dire ce que votre entreprise considère comme des indicateurs de performance clés obligatoires pour tous les sites [!DNL Adobe Analytics]), votre organisation doit disposer d’une méthode d’implémentation unique, dans la mesure du possible. Par exemple, utilisez la même structure de couche de données sur plusieurs sites et utilisez le même code personnalisé/règle de gestionnaire de balises pour capturer des éléments tels que des recherches internes ou des informations de profil du visiteur.

**POURQUOI :** une implémentation de base répétable et évolutive permet d’ajouter de nouveaux éléments ou de nouveaux sites/applications dans un effort réduit et rationalisé, tout en préservant votre implémentation et en facilitant la résolution des problèmes. L’utilisation d’une méthode uniforme permet également aux nouveaux administrateurs/développeurs de se connecter et de comprendre ce avec quoi ils travaillent.

**COMMENT :** adoptez un modèle de format unique à transmettre aux développeurs lorsqu’un nouveau site ou une amélioration du balisage est en ligne. En règle générale, un document Word fonctionne bien lorsque vous pouvez mettre en avant les éléments suivants :

* Variables en cours d’implémentation, leur objectif et quand les définir. Par exemple :

| Variable AA | Description | Quand/où définir | Comment définir |
|--- |--- |--- |--- |
| EVAR8 | Mots-clés de recherche interne | Lors de la destination de la page de résultats de recherche interne | couche de données |
| event8 | Nombre de recherches internes | Lors de la destination de la page de résultats de recherche interne | Règle Launch |

* Détails sur la définition. C’est là que vous spécifiez les objets de couche de données nécessaires, leur syntaxe, ainsi que les règles TMS à configurer et les détails de la configuration des règles.
* Les cas de test pour vous assurer sont couverts dans l’assurance qualité et toutes les variables que vous vous attendez à voir dans un cas de test réussi. Décrivez ce qu’une implémentation réussie doit inclure lorsque le développeur teste cette amélioration.

Idéalement, il suffira de modifier ce document pour le site suivant où vous mettez à jour les éléments de base tels que le nom de la propriété, la convention de nommage des pages, etc. Pas besoin de réinventer la roue à chaque fois, et vous pouvez gagner du temps.

## Auteurs

Ce document a été coécrit par :

![Christel Guidon](assets/Christel-Headshot-150.png)

Christel Guidon, responsable de la plateforme Digital [!DNL Analytics] chez NortonLifeLock
[!DNL Adobe Analytics] Champion

![&#x200B; Rachel Fenwick &#x200B;](assets/Rachel-Fenwick-150.png)

Rachel Fenwick, conseillère principale chez [!DNL Adobe]
