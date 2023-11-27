---
title: Créer des conventions d’affectation de noms normalisées
description: Les conventions de nommage normalisées s’appliquent à la fois au nom de variable lui-même lorsqu’il est activé dans l’interface utilisateur d’administration d’AA et aux valeurs transmises à la dimension.
solution: Analytics
feature-set: Analytics
feature: Implementation Basics
topic: Administration
role: Admin
level: Beginner
doc-type: article
thumbnail: 10531.jpg
kt: 10531
exl-id: 79cec21e-2b52-4e7b-88ad-db137a8cef4e
source-git-commit: 058d26bd99ab060df3633fb32f1232f534881ca4
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 80%

---

# Créer des conventions d’affectation de noms normalisées

**QUOI :** Les conventions d’appellation normalisées s’appliquent aux deux noms de variable lorsqu’ils sont activés dans la variable [!DNL Adobe Analytics] (AA) Interface utilisateur d’administration et valeurs transmises à la dimension. (c’est-à-dire que les noms de page seraient « nom de page (v1) » comme nom de variable et que les valeurs de nom de page transmises doivent être uniformes et suivre une structure/hiérarchie spécifique telle que « nom_site|page_accueil » ou « nom_site|recherche|résultats_recherche »).

**POURQUOI :** les conventions de nommage sont un excellent moyen de conserver une uniformité et de faciliter la compréhension de l’interface pour vos utilisateurs. Si vous les créez à partir du début et que vous les appliquez dans la plateforme et le code, elles seront plus faciles à mettre à l’échelle.

**COMMENT :** l’interface et le document de balisage doivent correspondre à la fois au « Nom » et à la « Description ». Ainsi, vos utilisateurs n’auront plus à extraire un document Excel et pourront comprendre directement vos données dans l’interface. Il est également recommandé de conserver tous les éléments en minuscules pour garantir la cohérence.

Il est toujours préférable de préserver la cohérence des noms de page sur l’ensemble de la plateforme (ou des noms d’écran pour les applications). Par exemple, vous pouvez définir « propriété:section:sous-section:sous sous-section:nom de page unique » dans une variable/dimension. Si tous ces champs sont distincts dans votre couche de données, vous pouvez même créer le nom de page directement dans votre fichier JS/Launch. Si tous ces éléments sont définis dans leurs propres dimensions, vous pouvez ventiler plus facilement des propriétés ou des zones spécifiques de votre site/application et mieux comprendre le trafic et les flux.

Tout ce qui permet aux utilisateurs de trouver et de comprendre plus facilement les données, y compris des données aussi simples que des conventions d’affectation de noms, augmentera l’utilisation des [!DNL Adobe Analytics] et fournir de meilleures informations pour l’entreprise.

## Auteurs

Ce document a été rédigé par :

![Christel Guidon](assets/Christel-Headshot-150.png)

Christel Guidon, Digital [!DNL Analytics] Platform Manager dans NortonLifeLock
[!DNL Adobe Analytics] Champion

![Rachel Fenwick](assets/Rachel-Fenwick-150.png)

Rachel Fenwick, conseillère principale chez [!DNL Adobe]
