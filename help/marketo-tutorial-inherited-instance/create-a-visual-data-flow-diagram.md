---
title: Création d’un diagramme de flux de données pour comprendre votre Tech stack marketing
description: Découvrez comment créer un diagramme de "plomb et sources de données" pour comprendre l’univers des données, pour contrôler et organiser efficacement l’instance.
feature-set: Marketo Engage
feature: Administration
role: Admin
level: Intermediate, Experienced
doc-type: Tutorial
last-substantial-update: 2023-10-16T00:00:00Z
jira: KT-13877
thumbnail: KT-13877.jpeg
hide: false
exl-id: 088bdcf1-4e49-44a7-ac78-a03742ff680b
source-git-commit: 1205848b1985a99b91f9d4d25e1a79f0df379589
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 2%

---

# Créer un diagramme de flux de données pour comprendre votre tech stack marketing

En tant qu’administrateur qui prend le contrôle d’une instance [!DNL Marketo Engage] active depuis des années, c’est comme une mission impossible à contrôler et à organiser efficacement l’instance. Lorsque [!DNL Adobe] [!DNL Marketo Champion] (2019) Kelly Jo Horton, est entrée dans une instance établie de longue date, elle s&#39;est attaquée à ce défi en [créant un diagramme de &quot;Lead and data sources&quot;](https://nation.marketo.com/t5/employee-blogs/understand-your-marketing-technology-and-data-create-this/ba-p/296774){target="_blank"} pour se familiariser avec l&#39;univers des données. Dans ce tutoriel, vous apprendrez à créer votre propre diagramme de flux de données en vous basant sur les exemples partagés par Kelly Jo Horton. Connaissons votre écosystème MarTech !

## Pourquoi créer un diagramme d’architecture pour votre instance héritée ?

1. **Familiarisez-vous avec le tech stack marketing que vous avez hérité d’une instance en direct.** Tous les responsables des opérations marketing/responsables des opérations de plateforme sont encouragés à effectuer cet exercice lorsqu’ils commencent dans une nouvelle entreprise. Ce processus de création permet aux utilisateurs administrateurs de visualiser l’image complète des données et activités envoyées à partir des intégrations externes vers [!DNL Marketo Engage] et de résoudre facilement les erreurs de l’API.
2. **Familiarisez-vous avec les principales parties prenantes qui gèrent les intégrations externes.** Une astuce que Kelly Jo Horton utilise pour identifier rapidement les parties prenantes est de référencer la liste des utilisateurs de l’API.
   1. **Accédez à l’onglet &quot;Intégration>LaunchPoint&quot; dans la section &quot;Admin&quot;.** En savoir plus sur la manière d’accéder à l’onglet &quot;LaunchPoint&quot; : [Création d’un service personnalisé à utiliser avec l’API REST](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-a-custom-service-for-use-with-rest-api.html){target="_blank"}.
   2. Recherchez les statistiques d’utilisation de l’API par utilisateur de l’API dans l’onglet Intégration > Services web de la section Informations sur l’appel de l’API . En cliquant sur le numéro d’appel de l’API, vous pouvez afficher les appels individuels spécifiques effectués par chaque utilisateur.

## Comment effectuer cet exercice de diagramme de flux de données visuel

### Étape 1 : diagramme d’état actuel

Créez un diagramme &quot;Etat actuel&quot;. Voici un exemple :

![Diagramme d’état actuel](/help/marketo-tutorial-inherited-instance/_assets/data-flow-diagram/Current_State_Lead_Data_Sources_KellyJo_Horton.png){align="center"}


### Étape 2 : futur diagramme d’état

Créez un diagramme &quot;Etat de l’avenir&quot; qui peut être utilisé lors de la présentation de la feuille de route de la technologie et des systèmes aux parties prenantes non techniques. Voici un exemple :

![Schéma d’état futur](/help/marketo-tutorial-inherited-instance/_assets/data-flow-diagram/Future-State-Lead-Data-Sources-KellyJo-Horton.png){align="center"}

### Étape 3 : version technique

Créez une version technique qui affiche des détails tels que le nom d’utilisateur de l’API pour chaque intégration, une brève description du type de données transmises à [!DNL Marketo Engage] ou extraites de [!DNL Marketo Engage], ainsi qu’un diagramme détaillé des flux et déclencheurs de middleware.  Voici un exemple :

![Version technique](/help/marketo-tutorial-inherited-instance/_assets/data-flow-diagram/Lead-Data-Source-Diagram-KellyJo-Horton.png){align="center"}


## Quelle est la suite ?

**Commencer avec des exemples :**
Téléchargez l’un des exemples de diagrammes de flux de données pour déterminer l’état actuel de votre tech stack marketing, de votre personne et de votre flux de données, ou créez un diagramme pour votre univers de données à partir de zéro lorsque vous audaciez l’instance :


<table style="table-layout:fixed">
   <tr>  
      <td style="border: 0;">
      <div style="text-align: center;">
          <a href="./_assets/downloads/Current_Future_State_Lead_Data_Sources.zip">
            <strong>État actuel et état futur</strong>
         </a>
      </div>
      </td>
      <td style="border: 0;">
      <div style="text-align: center;">
         <a href="./_assets/downloads/Detailed_Layers_by_Functional_Category_Stacked_Technologies.zip">
         <strong> Calques détaillés par catégorie fonctionnelle </strong>   
         </a>
      </div>
      </td>
      <td style="border: 0;">
         <div style="text-align: center;">
         <a href="./_assets/downloads/Lead_Data_Source.zip">
           <strong>Flux de piste et de Source de données </strong>  
         </a>
         </div>
       </td> 
       <td style="border: 0;">
         <div style="text-align: center;">
         <a href="./_assets/downloads/Simple_World_Class_Stage_Stack.zip">
          <strong>Diagramme simplifié</strong>  
         </a>
         </div>
        </td>  
   </tr>
   <tr>
    <td style="border: 0;">
         <div>
          <img alt="Diagramme État actuel et futur" src="./_assets/Thumbnail_Current-Future State Lead_Data Sources_KellyJo_Horton.png"/>
         </a>
      </div>
      </td>
      <td style="border: 0;">
         <div>
         <a href="./_assets/downloads/Detailed_Layers_by_Functional_Category_Stacked_Technologies.zip">
         <img alt="Calques détaillés par diagramme de catégorie fonctionnelle" src="./_assets/Thumbnail_Detailed_Layers_by_Functional_Category_Stacked_Technologies_KellyJo_Horton.png" />
       </a>
         </div>
      </td>
       <td style="border: 0;">
         <div>
            <a href="./_assets/downloads/Lead_Data_Source.zip">
         <img alt="Diagramme de flux de prospect et de Source de données" src="./_assets/Thumbnail_Lead-Data Source Diagram_KellyJo_Horton.png" />
         </a>
         </div>
      </td>
     <td style="border: 0;">
         <div>
            <a href="./_assets/downloads/Simple_World_Class_Stage_Stack.zip">
             <img alt="Schéma simplifié" src="./_assets/Thumbnail_Simple_World_Class_Stage_Stack.png" />
         </a>
         </div>
      </td>
</table>

Voici quelques outils que vous pouvez utiliser : draw.io (Google Docs), [!DNL Adobe] XD, Figma, Gliffy (in Confluence)

**Que se passe-t-il s’il existe déjà des diagrammes d’architecture ?** Les nouveaux membres de l’équipe peuvent avoir des perspectives différentes. Il est utile que les nouveaux administrateurs [!DNL Marketo Engage] effectuent cet exercice dans le cadre de leur processus d’intégration et le partagent avec d’autres personnes.

## Auteurs

**Kelly Jo Horton**\
[!DNL Adobe] Champion Marketo (2019)
*Partenaire client senior à Etumos*

![Kelly Jo Horton](/help/marketo-tutorial-inherited-instance/_assets/authors/Customer_Author_Kelly_Jo_Horton.png){width="30%"}

**Amy Chiu**
*Gestionnaire marketing d’adoption et de rétention,[!DNL Adobe]*

(/help/marketo-tutorial-inherited-instance/_assets/authors/[!DNL Adobe]_Author_Amy_Chiu.png){width=30%}
