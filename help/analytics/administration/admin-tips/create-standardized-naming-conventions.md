---
title: Créer des conventions de nommage normalisées
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
source-git-commit: c568ed0a06551d910b6f533698ec47c15adecf6c
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---

# Créer des conventions de nommage normalisées

**QUOI :** les conventions de nommage normalisées s’appliquent à la fois au nom de variable lui-même lorsqu’il est activé dans l’interface utilisateur d’administration d’[!DNL Adobe Analytics] (AA) et aux valeurs transmises à la dimension. (c’est-à-dire que les noms de page seraient « nom de page (v1) » comme nom de variable et que les valeurs de nom de page transmises doivent être uniformes et suivre une structure/hiérarchie spécifique telle que « nom_site|page_accueil » ou « nom_site|recherche|résultats_recherche »).

**POURQUOI :** conventions de nommage sont un excellent moyen de conserver une uniformité et de faciliter la compréhension de l’interface pour vos utilisateurs. Si vous les créez depuis le début et que vous les appliquez dans la plateforme et le code, elles seront plus faciles à mettre à l’échelle.

**COMMENT :** l’interface et le document de balisage doivent correspondre à la fois au « Nom » et à la « Description ». Ainsi, vos utilisateurs n’auront plus à extraire un document Excel et pourront comprendre directement vos données dans l’interface. Il est également recommandé de conserver tous les éléments en minuscules pour garantir la cohérence.

Il est toujours préférable de conserver des noms de page cohérents sur l’ensemble de la plateforme (ou des noms d’écran pour les applications). Par exemple, vous pouvez définir « `property:section:sub section:sub sub section:unique page name` » dans une variable/dimension. Si tous ces champs sont distincts dans votre couche de données, vous pouvez même créer le nom de page directement dans votre fichier JS/Launch. Si tous ces éléments sont définis dans leurs propres dimensions, vous pouvez ventiler plus facilement des propriétés ou des zones spécifiques de votre site/application et mieux comprendre le trafic et les flux.

Tout ce qui permet aux utilisateurs de trouver et de comprendre plus facilement les données, y compris des informations aussi simples que des conventions de nommage, accroît l’utilisation des [!DNL Adobe Analytics] et fournit de meilleures informations pour l’entreprise.

## Auteurs

Ce document a été coécrit par :

![Christel Guidon](assets/Christel-Headshot-150.png)

Christel Guidon, responsable de la plateforme Digital [!DNL Analytics] chez NortonLifeLock
[!DNL Adobe Analytics] Champion

![ Rachel Fenwick ](assets/Rachel-Fenwick-150.png)

Rachel Fenwick, conseillère principale chez [!DNL Adobe]
