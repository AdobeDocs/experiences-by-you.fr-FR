---
title: Organisation d’une nouvelle instance et établissement de conventions de dénomination
description: Découvrez comment configurer une bonne organisation dans votre instance de Marketo Engage, ce qui permet aux futurs marketeurs de votre entreprise de parcourir facilement les programmes, de modifier les ressources et d’extraire des rapports.
role: Admin
level: Beginner
doc-type: Article
solution: Marketo Engage
duration: 0
last-substantial-update: 2024-05-03T00:00:00Z
jira: KT-14813
thumbnail: KT-14813.jpeg
source-git-commit: 47ab8875bc4e41595cd40550330e43a88357b68d
workflow-type: tm+mt
source-wordcount: '1166'
ht-degree: 2%

---

# Organisation d’une nouvelle instance et établissement de conventions de dénomination

En tant qu’administrateur mettant en oeuvre une nouvelle instance de Marketo Engage, vous définissez les bases permettant aux futurs marketeurs de l’entreprise de naviguer facilement dans l’instance. Familiarisez-vous avec la structure de dossiers de l’arborescence et les conventions d’affectation des noms afin que votre instance reste ordonnée et configurée pour une réussite à long terme. Ce tutoriel comprend des exemples recommandés par Natalie Kremer, championne d’Adobe et de Marketo Engage (2019-2020), pour vous aider. [organiser les dossiers et nommer les ressources de manière cohérente ;](https://nation.marketo.com/t5/champion-program-blogs/keep-marketo-engage-organized-with-folders-and-naming/ba-p/245630){target="_blank"}.

## Pourquoi la structure des dossiers et l’application des conventions d’affectation des noms sont-elles nécessaires ?

Le fait de rester organisé dans votre instance vous permet, ainsi qu’à vos collègues, de suivre facilement les campagnes, les programmes et les ressources et de générer des rapports sur les performances du programme. Pour organiser l’arborescence de navigation dans votre instance et la créer à l’échelle, il est recommandé d’utiliser [dossiers](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/understanding-folders){target="_blank"}, [conventions de dénomination standard](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs#naming-schemes){target="_blank"}et les fonctionnalités telles que [clonage](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs#cloning){target="_blank"}.

## Organisation d’une instance de Marketo Engage

>[!VIDEO](https://video.tv.adobe.com/v/3421577/?quality=12&learn=on)

### Étape 1 - Configuration d’une structure de dossiers pour mettre vos programmes en ordre

La première étape pour organiser votre instance consiste à [configuration d’une structure de dossiers](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/create-new-campaign-folder.html) héberger votre programme et vos ressources de manière facile à trouver et ordonnée.

Voici quelques conseils rapides pour structurer les dossiers dans l’arborescence :

* Conserver une structure de dossiers plate pour la visibilité.
* Organisez vos dossiers pour refléter la structure de l’équipe de votre entreprise (par exemple, la région ou l’équipe) ou les initiatives (par exemple, les newsletters).
* Incluez des étiquettes temporelles pour activer la recherche et indiquer le timing approprié pour l’archivage (par exemple, 2024).
   * Il est recommandé aux administrateurs d’archiver les dossiers au moins une fois par an. Avec un nom de dossier annuel, vous pouvez facilement désactiver les campagnes dynamiques en direct et archiver l’ensemble du dossier à la fin de l’année.

Vous trouverez ci-dessous des exemples de mise en pratique de ces conseils.

**Nom du dossier dans l’arborescence**

>[!BEGINTABS]

>[!TAB Activités marketing]

![Activités marketing de dossiers](/help/marketo-tutorial-implementing-new-instance/assets/folders-marketing-activities.png)

>[!TAB Design Studio]

![Folder Design Studio](/help/marketo-tutorial-implementing-new-instance/assets/folders-design-studio.png)

>[!TAB Base]

![Base de données de dossiers](/help/marketo-tutorial-implementing-new-instance/assets/folders-database.png)

>[!ENDTABS]

### Etape 2 - Création de dossiers dans les programmes

Appliquons maintenant la structure de dossiers au niveau du programme. La bonne pratique consiste à placer les ressources locales dans des sous-dossiers afin de garder les programmes en ordre et de permettre aux utilisateurs internes de modifier ou de créer des rapports sur les programmes de manière efficace. Les sous-dossiers courants comprennent les emails, les landing pages, les campagnes dynamiques, les listes, les rapports, etc.

**Nom de dossier dans Programmes**
* Campagnes - *Dossier pour toutes les campagnes gérant les interactions et le suivi des états.*
* Ressources locales - *Dossier de toutes les ressources spécifiques à ce programme.*
   * E-mails
   * Pages de destination
   * Campagnes intelligentes
   * Listes - *Uniquement nécessaire lorsqu’il existe des listes spécifiques au programme.*
   * FORMS - *Uniquement nécessaire lorsqu’il existe un Forms spécifique au programme ; la plupart des Forms sont des ressources globales.*
   * Rapports - *Uniquement nécessaire lorsqu’il existe des rapports spécifiques au programme.*

### Étape 3 - Création de conventions de dénomination pour vos programmes et ressources

Une fois que vous disposez de la structure de dossiers dans l’arborescence, vous souhaiterez attribuer un nom cohérent aux programmes et aux ressources. C’est le cas lorsque la normalisation des conventions d’affectation des noms serait utile pour augmenter le processus d’affectation des noms en interne. Voici quelques composants que vous pouvez utiliser pour établir une convention d’affectation de nom afin d’assurer la fonctionnalité de recherche :

* Abréviation du type de programme - Email, Contenu, Formation, Webinaire, etc.
* Catégorie - Type de programme - Email autonome, Newsletter, etc.
* Dates : date de lancement du programme
* Brève description - Brève description du programme

Maintenant, plaçons les valeurs dans la formule et générons les noms des programmes pour différents types de programmes.

#### Formule de dénomination de programme

| **Abréviation du type de programme** | **AAAA** | **\-** | **MM** | **\-** | **DD(facultatif)** | **Catégorie** | **\-** | **Brève description du programme** |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| EM - Envoi de courrier électronique (programme de courrier électronique) | AAAA | \- | MM | \- | DD(facultatif) | Catégorie | \- | Brève description du programme |
| NL - Newsletter | AAAA | \- | MM | \- | DD(facultatif) | Catégorie | \- | Brève description du programme |
| ENG - Programme d’engagement | AAAA | \- | MM | \- | DD(facultatif) | Catégorie | \- | Brève description du programme |
| WBN - Webinaire | AAAA | \- | MM | \- | DD(facultatif) | Catégorie | \- | Brève description du programme |
| IW - Webinaire interactif | AAAA | \- | MM | \- | DD(facultatif) | Catégorie | \- | Brève description du programme |
| TS - Commerce | AAAA | \- | MM | \- | DD(facultatif) | Catégorie | \- | Brève description du programme |
| LE - Événement en direct (Roadshow) | AAAA | \- | MM | \- | DD(facultatif) | Catégorie | \- | Brève description du programme |
| UG - Groupe d’utilisateurs | AAAA | \- | MM | \- | DD(facultatif) | Catégorie | \- | Brève description du programme |
| WC - Contenu du site web | AAAA | \- | MM | \- | DD(facultatif) | Catégorie | \- | Brève description du programme |
| CS - Syndication de contenu | AAAA | \- | MM | \- | DD(facultatif) | Catégorie | \- | Brève description du programme |
| LI - Importation de liste | AAAA | \- | MM | \- | DD(facultatif) | Catégorie | \- | Brève description du programme |
| OA - Publicité en ligne | AAAA | \- | MM | \- | DD(facultatif) | Catégorie | \- | Brève description du programme |
| PPC - Paiement par clic | AAAA | \- | MM | \- | DD(facultatif) | Catégorie | \- | Brève description du programme |

| **Exemples** |
| --- |
| Contenu allégé ES 2023-10 - Livre blanc XYX |
| WC-2023-10 - Webinaire mensuel - Étude de cas ABC |

#### Formule de dénomination des ressources

Pour désigner les ressources par leur nom, il est préférable de ne pas répéter le nom du programme et d’utiliser des identifiants courts et génériques pour une utilisation ultérieure de clonage. Voici quelques conseils rapides à garder à l’esprit :

* Nommez les ressources en fonction de leur séquence dans le processus du programme.
* Utilisez &quot;-&quot; (trait d’union) pour séparer les composants d’affectation de nom au lieu de &quot;.&quot;(point) ou &quot;\_&quot; (trait de soulignement).
   * Pourquoi ? Marketo Engage utilise un point pour séparer le nom du programme du nom de la campagne. L’utilisation de &quot;\_&quot; vous empêche de le voir lorsque la ressource est liée par un hyperlien.
* Utilisez des acronymes standard dans les noms de ressources pour raccourcir la référence tout en permettant une reconnaissance facile.

En gardant ces informations à l’esprit, nous appliquerons ces conseils aux ressources suivantes et créerons des formules pour générer des noms :

##### Nommer les ressources en fonction de leur séquence dans le processus du programme

| **Séquence dans le processus du programme** | **\-** | **Description** |
| --- | --- | --- |
| 01 | \- | Description |
| 02 | \- | Description |
| 03 | \- | Description |

| **Exemples : Liste dynamique** |
| --- |
| 01-Envoyer un courrier électronique |
| 02-Ayant ouvert |
| 03-Clicked |
| Formulaire rempli 04 |
| 05-Influencé (Succès du programme) |
| 06-Désabonné |

##### Nommer les ressources avec l’abréviation de type de ressource

| **Abréviation du type de ressource** | **Type de ressource** | **\-** | **Description de l’objectif** |
| --- | --- | --- | --- |
| LP - Landing Page | LP | \- | Description de l’objectif |
| EMAIL - Email (sortant) | EMAIL | \- | Description de l’objectif |
| ALERTE - Alerte par email | ALERTE | \- | Description de l’objectif |
| WF - Formulaire web | WF | \- | Description de l’objectif |
| EXCL - Liste d’exclusion | EXCL | \- | Description de l’objectif |
| SLST - Liste dynamique | SLST | \- | Description de l’objectif |
| LST - Liste statique | LST | \- | Description de l’objectif |

| **Exemples** |
| --- |
| Enregistrement LP |
| LP-ThankYou |
| EMAIL-Outbound |
| EMAIL-Newsletter |
| EMAIL-Invitation |
| EMAIL-Reminder |
| EXCL-Concurrents |

##### Nommez les fichiers téléchargeables (.pdf) avec l’abréviation de type de ressource

| **Type de ressource** | **Description du contenu** | **\-** | **Abréviation du type de ressource** | **.** | **PDF** |
| --- | --- | --- | --- | --- | --- |
| WP - Livre blanc | Description du contenu | \- | WP | . | pdf |
| CS - Étude de cas | Description du contenu | \- | CS | . | pdf |
| DS - Feuille de données | Description du contenu | \- | DS | . | pdf |

| **Exemples : fichiers de PDF téléchargeables** |
| --- |
| XYZ-Gadget-DS.pdf |
| Acme-Company-CS.pdf |
| How-XYZ-Gadgets-make-life-easier-WP.pdf |

>[!CAUTION]
>
>Lorsque vous nommez des fichiers dans les exemples ci-dessus, n’utilisez pas d’espaces et évitez d’utiliser des traits de soulignement &quot;\_&quot;.

## Et après ?

* Téléchargez la feuille de calcul : [Organisation Marketo Engage et conventions de dénomination](./assets/adobe-marketo-engage-organization-and-naming-conventions.xlsx){target="_blank"} pour prendre en charge la création de la structure de dossiers et des conventions d’affectation des noms.
* Une fois que vous avez déterminé les composants nécessaires dans votre convention d’affectation des noms standard, pensez à créer des formules dans une feuille de calcul Google ou Microsoft Excel. Pour une utilisation ultérieure, il vous suffit de saisir vos valeurs dans la feuille de calcul pour générer vos noms de programme.
* Une fois que vous vous êtes aligné sur une structure de dossiers globale, il est temps d’analyser les modèles dont vous avez besoin en fonction des cas d’utilisation les plus fréquents et des demandes les plus courantes que votre équipe reçoit. Commencez ensuite à créer votre premier modèle de programme. Lisez la suite pour commencer à utiliser [Modèles de programme Adobe Marketo Engage](https://business.adobe.com/blog/how-to/get-started-with-marketo-engage-program-templates){target="_blank"}.

### Auteurs

{{natalie-kremer}}

{{amy-chiu}}