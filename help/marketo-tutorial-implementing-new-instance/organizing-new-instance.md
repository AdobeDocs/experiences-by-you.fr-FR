---
title: Organisation d’une nouvelle instance et définition des conventions d’affectation de noms
description: Découvrez comment configurer une bonne organisation au sein de votre instance Marketo Engage, ce qui permettra aux futurs spécialistes du marketing de votre organisation de parcourir facilement les programmes, de modifier les ressources et d’extraire des rapports.
role: Admin
level: Beginner
doc-type: Article
solution: Marketo Engage
duration: 0
last-substantial-update: 2024-05-03T00:00:00Z
jira: KT-14813
thumbnail: KT-14813.jpeg
exl-id: 19b3de9e-53f3-4308-b46e-7b8f756c30a0
source-git-commit: cae626cb3958ebcda16ac30b0a487ebfe06d50f4
workflow-type: tm+mt
source-wordcount: '1166'
ht-degree: 2%

---

# Organiser une nouvelle instance et établir des conventions de nommage

En tant qu’administrateur ou administratrice mettant en œuvre une nouvelle instance de Marketo Engage, vous jetez les bases qui permettront aux futurs professionnels du marketing au sein de l’organisation de parcourir facilement l’instance. Familiarisez-vous avec l’arborescence, la structure des dossiers et les conventions de nommage pour que votre instance reste ordonnée et configurée pour un succès à long terme. Ce tutoriel comprend des exemples recommandés par Adobe et Natalie Kremer, championne de Marketo Engage (2019-2020), pour vous aider à [organiser les dossiers et nommer les ressources de manière cohérente](https://nation.marketo.com/t5/champion-program-blogs/keep-marketo-engage-organized-with-folders-and-naming/ba-p/245630){target="_blank"}.

## Pourquoi est-il nécessaire de structurer des dossiers et d’appliquer des conventions de nommage ?

Lorsque vous restez organisé dans votre instance, vous et vos collègues pouvez facilement suivre les campagnes, les programmes et les ressources, et générer des rapports sur les performances des programmes. Pour organiser l’arborescence de navigation dans votre instance et la créer à grande échelle, il est recommandé d’utiliser des [dossiers](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/understanding-folders){target="_blank"}, [conventions de nommage standard](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs#naming-schemes){target="_blank"} et des fonctionnalités telles que [clonage](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs#cloning){target="_blank"}.

## Organisation d’une instance Marketo Engage

>[!VIDEO](https://video.tv.adobe.com/v/3421577/?quality=12&learn=on)

### Étape 1 - Configurer une structure de dossiers pour mettre vos programmes en ordre

La première étape pour organiser votre instance consiste à [configurer une structure de dossiers](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/create-new-campaign-folder.html?lang=fr) héberger votre programme et vos ressources de manière facile à trouver et ordonnée.

Voici quelques conseils rapides pour structurer les dossiers dans l’arborescence :

* Conserver une structure de dossiers plate pour la visibilité.
* Structurez vos dossiers de manière à refléter la structure de l’équipe de votre entreprise (par exemple, la région ou l’équipe) ou les initiatives (par exemple, les newsletters).
* Inclure des étiquettes temporelles pour permettre la recherche et signaler le moment approprié pour l’archivage (par exemple, 2024).
   * Il est recommandé aux administrateurs d’archiver les dossiers au moins une fois par an. À l’aide d’un nom de dossier annuel, vous pouvez facilement désactiver les campagnes dynamiques en direct et archiver l’ensemble du dossier à la fin de l’année.

Vous trouverez ci-dessous des exemples de dossiers pour mettre ces conseils en pratique.

**Nom du dossier dans l’arborescence**

>[!BEGINTABS]

>[!TAB Activités marketing]

![Activités marketing Dossiers](/help/marketo-tutorial-implementing-new-instance/assets/folders-marketing-activities.png)

>[!TAB  Design Studio ]

![Folder Design Studio](/help/marketo-tutorial-implementing-new-instance/assets/folders-design-studio.png)

>[!TAB Base de données]

![Base de données des dossiers](/help/marketo-tutorial-implementing-new-instance/assets/folders-database.png)

>[!ENDTABS]

### Etape 2 - Créer des dossiers dans les programmes

Appliquons maintenant la structure de dossiers au niveau du programme. Il est recommandé de placer les ressources locales dans des sous-dossiers pour garder les programmes bien ordonnés et permettre aux utilisateurs internes de modifier les programmes ou de créer des rapports sur ceux-ci de manière efficace. Les sous-dossiers courants comprennent les e-mails, les pages de destination, les campagnes intelligentes, les listes, les rapports, etc.

**Nom de dossier dans Programmes**

* Campagnes - *Dossier pour toutes les campagnes gérant les interactions et le tracking des statuts.*
* Assets locale - *Dossier pour toutes les ressources spécifiques à ce programme.*

   * E-mails
   * Pages de destination
   * Campagnes intelligentes
   * Listes - *Uniquement nécessaire lorsqu’il existe des listes spécifiques au programme.*
   * Forms - *Nécessaire uniquement lorsqu’il existe un Forms spécifique au programme ; la plupart des Forms sont des Assets globaux.*
   * Rapports : *uniquement nécessaire lorsqu’il existe des rapports spécifiques au programme*.

### Étape 3 - Créer des conventions de nommage pour vos programmes et ressources

Une fois que vous disposez de la structure de dossiers dans l’arborescence, vous souhaiterez nommer les programmes et les ressources de manière cohérente. C’est à ce moment que la normalisation des conventions de nommage serait utile pour étendre le processus de nommage en interne. Voici quelques composants que vous pouvez utiliser pour établir une convention de nommage afin d’assurer la recherche :

* Abréviation du type de programme : e-mail, contenu, culture, webinaire, etc.
* Catégorie - Type de programme - E-mail autonome, newsletter, etc.
* Dates - Date de lancement du programme
* Description courte - Brève description du programme

Maintenant, plaçons les valeurs dans la formule et générons les noms des programmes pour divers types de programmes.

#### Formule De Dénomination Du Programme

| **Abréviation du type de programme** | **AAAA** | **\-** | **MM** | **\-** | **DD(Facultatif)** | **Catégorie** | **\-** | **Brève description du programme** |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| AEM - Envoi d’e-mail (programme d’e-mail) | AAAA | \- | MM | \- | DD(Facultatif) | Catégorie | \- | Brève description du programme |
| NL - Newsletter | AAAA | \- | MM | \- | DD(Facultatif) | Catégorie | \- | Brève description du programme |
| ENG - Programme de mobilisation | AAAA | \- | MM | \- | DD(Facultatif) | Catégorie | \- | Brève description du programme |
| WBN - Webinaire | AAAA | \- | MM | \- | DD(Facultatif) | Catégorie | \- | Brève description du programme |
| IW - Webinaire interactif | AAAA | \- | MM | \- | DD(Facultatif) | Catégorie | \- | Brève description du programme |
| TS - Salon professionnel | AAAA | \- | MM | \- | DD(Facultatif) | Catégorie | \- | Brève description du programme |
| LE - Événement en direct (Roadshow) | AAAA | \- | MM | \- | DD(Facultatif) | Catégorie | \- | Brève description du programme |
| ID d’utilisateur - Groupe d’utilisateurs | AAAA | \- | MM | \- | DD(Facultatif) | Catégorie | \- | Brève description du programme |
| WC - Contenu du site Web | AAAA | \- | MM | \- | DD(Facultatif) | Catégorie | \- | Brève description du programme |
| CS - Syndication de contenu | AAAA | \- | MM | \- | DD(Facultatif) | Catégorie | \- | Brève description du programme |
| LI - Importation de liste | AAAA | \- | MM | \- | DD(Facultatif) | Catégorie | \- | Brève description du programme |
| OA - Advertising en ligne | AAAA | \- | MM | \- | DD(Facultatif) | Catégorie | \- | Brève description du programme |
| PPC - Paiement par clic | AAAA | \- | MM | \- | DD(Facultatif) | Catégorie | \- | Brève description du programme |

| **Exemples** |
| --- |
| Livre blanc ES 2023-10 Gated Content - XYX |
| WC-2023-10- Webinaire mensuel - Etude de cas ABC |

#### Formule de dénomination des ressources

En descendant d’un niveau pour nommer les ressources, il est préférable de ne pas répéter le nom du programme et d’utiliser des identifiants courts et génériques pour une utilisation ultérieure de clonage. Voici quelques conseils rapides à garder à l’esprit :

* Numérotez les ressources en fonction de leur ordre dans le processus du programme.
* Utilisez « - » (trait d’union) pour séparer les composants de dénomination au lieu de « . »(point) ou « \ » (trait de soulignement).
   * Pourquoi ? Marketo Engage utilise un point pour séparer le nom du programme du nom de la campagne. L’utilisation de « \_ » vous empêche de le voir lorsque la ressource comporte un lien hypertexte.
* Utilisez des acronymes standard dans les noms de ressources pour raccourcir la référence et toujours permettre une reconnaissance facile.

Dans cette optique, nous appliquerons ces conseils aux ressources suivantes et créerons des formules pour générer des noms :

##### Nommez les ressources en fonction de la séquence dans le processus du programme.

| **Séquence dans le processus du programme** | **\-** | **Description** |
| --- | --- | --- |
| 01 | \- | Description |
| 02 | \- | Description |
| 03 | \- | Description |

| **Exemples : liste dynamique** |
| --- |
| 01-Envoyer un e-mail |
| 02-Ouvert |
| 03-Clicked |
| 04-Formulaire rempli |
| 05-Influencé (Succès du programme) |
| 06-Désabonné |

##### Nommer les ressources à l’aide de l’abréviation de type de ressource

| **Abréviation du type de ressource** | **Type de ressource** | **\-** | **Description de l’objectif** |
| --- | --- | --- | --- |
| LP - Landing Page | LP | \- | Description de l’objectif |
| E-MAIL - E-mail (sortant) | EMAIL | \- | Description de l’objectif |
| ALERTE - Alerte par e-mail | ALERTE | \- | Description de l’objectif |
| WF - Web Form | WF | \- | Description de l’objectif |
| EXCL - Liste d&#39;exclusion | EXCL | \- | Description de l’objectif |
| SLST - Liste dynamique | LISTE | \- | Description de l’objectif |
| LST - Liste statique | LST | \- | Description de l’objectif |

| **Exemples** |
| --- |
| LP-Registration |
| LP-Merci |
| E-MAIL sortant |
| EMAIL-Newsletter |
| INVITATION PAR E-MAIL |
| E-MAIL-Reminder |
| EXCL-Concurrents |

##### Nommez les fichiers téléchargeables (.pdf) en utilisant l’abréviation du type de ressource.

| **Type de ressource** | **Description du contenu** | **\-** | **Abréviation du type de ressource** | **,** | **PDF** |
| --- | --- | --- | --- | --- | --- |
| WP - Livre blanc | Description du contenu | \- | WP | . | pdf |
| CS - Étude de cas | Description du contenu | \- | CS | . | pdf |
| DS - Fiche produit | Description du contenu | \- | DS | . | pdf |

| **Exemples : fichiers PDF téléchargeables** |
| --- |
| XYZ-Gadget-DS.pdf |
| Acme-Company-CS.pdf |
| How-XYZ-Gadgets-make-life-easier-WP.pdf |

>[!CAUTION]
>
>Lorsque vous nommez des fichiers dans les exemples ci-dessus, n’utilisez pas d’espaces et évitez d’utiliser des traits de soulignement « \_ »

## Quelle est la suite ?

* Téléchargez la feuille de calcul : [Organisation Marketo Engage et conventions de nommage](./assets/adobe-marketo-engage-organization-and-naming-conventions.xlsx){target="_blank"} pour prendre en charge la création de la structure de dossiers et des conventions de nommage.
* Une fois que vous avez déterminé les composants nécessaires dans votre convention d’affectation des noms standard, pensez à créer des formules dans une feuille de calcul Google Sheet ou Microsoft Excel. Pour une utilisation ultérieure, il vous suffit d’entrer vos valeurs dans la feuille de calcul pour générer les noms de vos programmes.
* Une fois que vous vous êtes aligné sur une structure de dossiers globale, il est temps de réfléchir aux modèles dont vous avez besoin en fonction des cas d’utilisation les plus fréquents et des demandes les plus courantes que votre équipe reçoit. Commencez ensuite à créer votre premier modèle de programme. Lisez la suite pour commencer à utiliser les [modèles de programme Adobe Marketo Engage](https://business.adobe.com/fr/blog/how-to/get-started-with-marketo-engage-program-templates){target="_blank"}.

### Auteurs

{{natalie-kremer}}

{{amy-chiu}}
