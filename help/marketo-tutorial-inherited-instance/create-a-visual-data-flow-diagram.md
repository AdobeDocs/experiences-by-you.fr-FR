---
title: Créer un diagramme de flux de données pour comprendre votre Tech stack marketing
description: Découvrez comment créer un diagramme de « Lead et sources de données » pour comprendre l’univers des données, vérifier et nettoyer l’instance efficacement.
feature-set: Marketo Engage
feature: Administration
role: Admin
level: Intermediate, Experienced
doc-type: Tutorial
last-substantial-update: 2023-10-16T00:00:00Z
jira: KT-13877
thumbnail: KT-13877.jpeg
exl-id: 088bdcf1-4e49-44a7-ac78-a03742ff680b
source-git-commit: d78210c6d6f5ec22430770c752495959303a9519
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 1%

---

# Créer un diagramme de flux de données pour comprendre votre tech stack marketing

En tant qu’administrateur prenant en charge une instance [!DNL Marketo Engage] active depuis des années, il est comme une mission impossible d’effectuer un audit et de nettoyer l’instance efficacement. Lorsque [!DNL Adobe] [!DNL Marketo Champion] (2019), Kelly Jo Horton, a mis en place une instance de longue date, elle a relevé ce défi en [créant un diagramme de « Lead et sources de données »](https://nation.marketo.com/t5/employee-blogs/understand-your-marketing-technology-and-data-create-this/ba-p/296774){target="_blank"} pour se familiariser avec l&#39;univers des données. Dans ce tutoriel, vous apprendrez à créer votre propre diagramme de flux de données en vous appuyant sur les exemples partagés par Kelly Jo Horton. Apprenons à connaître votre écosystème MarTech !

## Pourquoi créer un diagramme d’architecture pour votre instance héritée ?

1. **Familiarisez-vous avec le tech stack marketing hérité d’une instance active.** Tous les responsables des opérations marketing/responsables des opérations de plateforme sont encouragés à effectuer cet exercice lors du démarrage dans une nouvelle entreprise. Ce processus de création permet aux utilisateurs administrateurs d’avoir une vue d’ensemble des données et activités envoyées depuis les intégrations externes vers [!DNL Marketo Engage] et de résoudre facilement les erreurs d’API.
2. **Familiarisez-vous avec les principales parties prenantes qui gèrent les intégrations externes.** Une astuce que Kelly Jo Horton utilise pour identifier rapidement les parties prenantes est de référencer la liste des utilisateurs d’API.
   1. **Accédez à l’onglet « Intégration > LaunchPoint » dans la section « Administration ».** En savoir plus sur la navigation vers l’onglet « LaunchPoint » : [Créer un service personnalisé à utiliser avec l’API REST](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-a-custom-service-for-use-with-rest-api.html){target="_blank"}.
   2. Recherchez les statistiques d’utilisation de l’API par utilisateur de l’API dans l’onglet Intégration > Services web de la section Informations sur l’appel API . En cliquant sur le numéro d’appel API, vous pouvez afficher les appels individuels spécifiques effectués par chaque utilisateur.

## Comment effectuer cet exercice de diagramme de flux de données visuelles

### Étape 1 : Diagramme d’état actuel

Créez un diagramme « État actuel ». Voici un exemple :

![diagramme d’état actuel](/help/marketo-tutorial-inherited-instance/_assets/data-flow-diagram/Current_State_Lead_Data_Sources_KellyJo_Horton.png){align="center"}


### Étape 2 : Diagramme d’état futur

Créez un diagramme « État futur » qui peut être utilisé lors de la présentation de la feuille de route des technologies et des systèmes aux parties prenantes non techniques. Voici un exemple :

![Diagramme d’état futur](/help/marketo-tutorial-inherited-instance/_assets/data-flow-diagram/Future-State-Lead-Data-Sources-KellyJo-Horton.png){align="center"}

### Etape 3 : Version Technique

Créez une version technique qui affiche des détails tels que le nom d&#39;utilisateur de l&#39;API pour chaque intégration, une brève description du type de données transmises à [!DNL Marketo Engage] ou extraites de [!DNL Marketo Engage], ainsi qu&#39;un diagramme détaillé de tous les flux et déclencheurs de middleware. Voici un exemple :

![Version technique ](/help/marketo-tutorial-inherited-instance/_assets/data-flow-diagram/Lead-Data-Source-Diagram-KellyJo-Horton.png){align="center"}


## Quelle est la prochaine étape ?

**Prise en main avec des exemples :**
Téléchargez l’un des exemples de diagrammes de flux de données pour cartographier l’état actuel de votre tech stack marketing, de votre personne et de votre flux de données, ou créez un diagramme pour votre univers de données à partir de zéro lorsque vous auditez l’instance :


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
         <strong>Calques détaillés par catégorie fonctionnelle </strong>   
         </a>
      </div>
      </td>
      <td style="border: 0;">
         <div style="text-align: center;">
         <a href="./_assets/downloads/Lead_Data_Source.zip">
           </strong> de flux de Source de données et de lead <strong>  
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
          <img alt="Diagramme d’état actuel et d’état futur" src="./_assets/Thumbnail_Current-Future State Lead_Data Sources_KellyJo_Horton.png"/>
         </a>
      </div>
      </td>
      <td style="border: 0;">
         <div>
         <a href="./_assets/downloads/Detailed_Layers_by_Functional_Category_Stacked_Technologies.zip">
         <img alt="Diagramme détaillé des calques par catégorie fonctionnelle" src="./_assets/Thumbnail_Detailed_Layers_by_Functional_Category_Stacked_Technologies_KellyJo_Horton.png" />
       </a>
         </div>
      </td>
       <td style="border: 0;">
         <div>
            <a href="./_assets/downloads/Lead_Data_Source.zip">
         <img alt="Diagramme de flux de Source de leads et de données" src="./_assets/Thumbnail_Lead-Data Source Diagram_KellyJo_Horton.png" />
         </a>
         </div>
      </td>
     <td style="border: 0;">
         <div>
            <a href="./_assets/downloads/Simple_World_Class_Stage_Stack.zip">
             <img alt="Diagramme simplifié" src="./_assets/Thumbnail_Simple_World_Class_Stage_Stack.png" />
         </a>
         </div>
      </td>
</table>

Voici quelques outils que vous pouvez utiliser : draw.io (Google Docs), [!DNL Adobe] XD, Figma, Gliffy (dans Confluence)

**Et s’il existe déjà des diagrammes d’architecture ?** Les nouveaux membres de l’équipe peuvent avoir des points de vue différents. Il est important que les nouveaux administrateurs [!DNL Marketo Engage] effectuent cet exercice dans le cadre de leur processus d’intégration et le partagent avec d’autres personnes.

## Auteurs

**Kelly Jo Horton**\
[!DNL Adobe] Champion Marketo (2019)
*Partenaire client senior chez Etumos*

![ Kelly Jo Horton ](/help/marketo-tutorial-inherited-instance/_assets/authors/Customer_Author_Kelly_Jo_Horton.png){width="30%"}

**Amy Chiu**
*Responsable marketing, adoption et rétention,[!DNL Adobe]*

![ Amy Chiu ](/help/marketo-tutorial-inherited-instance/_assets/authors/Adobe_Author_Amy_Chiu.png){width=30%}
