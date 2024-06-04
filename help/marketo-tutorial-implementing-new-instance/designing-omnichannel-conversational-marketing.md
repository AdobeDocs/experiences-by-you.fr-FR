---
title: Concevoir un marketing conversationnel omnicanal avec Dynamic Chat
description: Commencez rapidement à concevoir du marketing conversationnel avec Adobe Dynamic Chat, le canal d’engagement conversationnel natif de Adobe Marketo Engage. Ce tutoriel propose des recettes pratiques pour mettre en oeuvre des cas d’utilisation tels que la réservation de réunions de vente, l’engagement dans le contenu du site web et la promotion d’événements/webinaires.
role: Admin
level: Beginner
doc-type: Article
duration: 0
last-substantial-update: 2024-05-23T00:00:00Z
jira: KT-14814
source-git-commit: 4ac24e1297287adbd6832030fda5590b696e45ed
workflow-type: tm+mt
source-wordcount: '1409'
ht-degree: 0%

---


# Concevoir un marketing conversationnel omnicanal avec Dynamic Chat

Pour les marketeurs, votre site web est essentiel pour générer des pistes, stimuler les conversions et accélérer les cycles de vente. L’interaction avec les visiteurs en temps réel sur votre site web permet à votre équipe de vente de qualifier les acheteurs plus efficacement. Adobe Dynamic Chat, le canal de chat natif de votre abonnement Adobe Marketo Engage, vous permet d’automatiser les conversations afin d’étendre les fonctionnalités des Marketo Engage.

Ce tutoriel décrit le processus de réflexion et les principaux cas d’utilisation partagés par Sara Barriuso, responsable des opérations marketing chez Cornerstone OnDemand, lors de la conférence &quot;Apprenez de vos pairs&quot;. Elle a expliqué comment son entreprise utilisait le Dynamic Chat pour optimiser les capacités des Marketo Engage.

## Intégrer l’engagement conversationnel dans votre stratégie de génération de demande

Les visiteurs parcourent votre site web pour une raison quelconque. Il peut s’agir de recherche de contenu sur vos produits ou services ou de recherche d’informations de contact pour parler à vos représentants commerciaux. Il peut également s’agir de vos clients qui recherchent des informations supplémentaires sur les produits. Chat permet aux visiteurs de votre site web de se qualifier en libre-service s’ils sont prêts à parler à votre équipe commerciale.

Quand Sara Barriuso a mis en place le Dynamic Chat, elle a été attirée par son intégration harmonieuse avec le Marketo Engage et le [déclencheurs d’activité prédéfinis](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-activities){target="_blank"} qui activent les programmes Marketo Engage et vice versa. Elle a développé ses stratégies d&#39;engagement conversationnel en ayant à l&#39;esprit trois segments d&#39;audience :

1. Perspectives inconnues : proposez de manière proactive des appels de démonstration pour générer de nouvelles pistes.
2. Pistes/clients connus : rallongez le temps passé par les visiteurs à parcourir le contenu et à offrir des appels de démonstration pour générer des opportunités d’achat et de vente croisée.
3. Prospects/clients : proposez des expériences personnalisées en étendant les efforts des campagnes marketing.


## Cas pratiques clés pour commencer à créer vos boîtes de dialogue

Pour mettre en oeuvre ces stratégies, Sara a construit ses Dialogues Dynamic Chat autour des cas pratiques suivants :

1. Dialogue tout attraper par défaut : offre une option initiale à tous les visiteurs, leur permettant d’accomplir leurs tâches plus efficacement.

2. Promotion de l’enregistrement des événements et des webinaires : incitez les visiteurs du site web à s’inscrire aux événements et aux webinaires afin de les orienter plus rapidement vers l’étape d’achat.

3. Extension de l&#39;engagement du contenu des campagnes : proposez un contexte supplémentaire ou répondez à des questions potentielles lorsque les visiteurs parcourent le contenu du site web.

Voyons ces cas pratiques en action, car Sara présente son processus, depuis la cartographie du flux conversationnel jusqu&#39;à la configuration des Dialogues et du ciblage en Dynamic Chat et en Marketo Engage.

### Cas d’utilisation 1 : dialogue fourre-tout par défaut pour tous les visiteurs du site

Ce dialogue fournit cinq options initiales parmi lesquelles les visiteurs du site peuvent choisir, ce qui crée une expérience autonome qui les aide à trouver les informations dont ils ont besoin en fonction de leur personnage. Pour commencer, vous pouvez explorer votre boîte de réception de courrier électronique &quot;Nous contacter&quot; afin d’identifier les thèmes communs et de les classer dans les options de dialogue qui s’appliquent aux visiteurs de votre site. Regardez la démonstration et suivez les étapes ci-dessous pour créer votre dialogue fourre-tout par défaut :

>[!VIDEO](https://video.tv.adobe.com/v/3429194/?learn=on)

>[!BEGINTABS]

>[!TAB Dynamic Chat]

#### Phase 1

1. Créez le dialogue et créez un lien de test.
2. Ajoutez un objectif pour effectuer le suivi des conversions (envoi de requête de démonstration, par exemple).
3. Demandez à 2 ou 3 personnes de le tester et de recueillir des commentaires.

#### Phase 2

1. Dans &quot;Audience&quot;, ajoutez une URL de page web dans &quot;Cible&quot; pour indiquer où le dialogue s’affichera.
2. Dans &quot;Paramètres&quot;, ajoutez le nom, la description, la priorité et la langue de la campagne.
3. Cliquez sur &quot;Publier&quot;

>[!TAB Marketo Engage]

#### Phase 1

1. Créez votre campagne de suivi dynamique.
2. Dans &quot;Liste dynamique&quot;, utilisez un déclencheur &quot;Atteindre l’objectif de dialogue&quot;. Utilisez le même objectif (par exemple, Demo Request) que celui utilisé pour Dialogue.
3. Dans &quot;Flux&quot;, incluez une étape &quot;Modifier l’état du programme&quot; pour effectuer le suivi de la conversion.
4. La source s’affichera comme &quot;dynamicChat&quot;. Vous pouvez créer une campagne dynamique pour mettre à jour la source vers un nom qui vous semble logique.

#### Phase 2

1. Testez à nouveau votre suivi de campagne dynamique lorsqu’il est actif.

>[!ENDTABS]

#### Niveau supérieur : marketing basé sur les comptes

Vous pouvez améliorer davantage le dialogue fourre-tout par défaut en incorporant du contenu ciblé par le secteur, ce qui rend les conversations encore plus utiles aux visiteurs. Par exemple, proposez des livres blancs ou des études de cas spécifiques au secteur à télécharger pour vos visiteurs. Regardez la démonstration et suivez les étapes ci-dessous pour créer un dialogue fourre-tout par défaut pour le marketing basé sur les comptes :

>[!VIDEO](https://video.tv.adobe.com/v/3429195/?learn=on)

>[!BEGINTABS]

>[!TAB Dynamic Chat]

1. Cloner le &quot;dialogue par défaut&quot; et le renommer.
2. Dans &quot;Concepteur de flux&quot;, adaptez les messages de dialogue au secteur cible (un seul flux + la question initiale).
3. Demandez à 2 ou 3 personnes de tester le Dialogue et de recueillir leurs commentaires.
4. Créez un lien de test et partagez-le.
5. Dans &quot;Audience&quot;, ajoutez une URL de page web où le dialogue s’affichera et mettra à jour la cible vers le secteur que vous souhaitez.
6. Dans &quot;Paramètres&quot;, ajoutez le nom de la campagne, la priorité de la description et la langue.
7. Cliquez sur &quot;Publier&quot;.

>[!TAB Marketo Engage]

1. Créez votre campagne de suivi dynamique et testez l’objectif.
2. Rétestez le suivi de la campagne dynamique après la publication de la boîte de dialogue.

>[!ENDTABS]

### Cas d’utilisation 2 : promotion de l’enregistrement d’événement et de webinaire

Les événements et les webinaires sont des tactiques marketing populaires pour les entreprises B2B afin de générer de la demande. Ils offrent des expériences attrayantes et des informations riches qui attirent des clients potentiels. La connexion des visiteurs de votre site web aux événements et aux webinaires à venir vous permet de qualifier les clients potentiels encore plus rapidement. La création de ce dialogue est peu coûteuse et nécessite peu d’efforts. Il peut rapidement démontrer son succès, ce qui vous permet d’obtenir l’aide des parties prenantes marketing pour ajouter un engagement conversationnel à votre plan d’automatisation omnicanal. Regardez la démonstration et suivez les étapes ci-dessous pour créer votre dialogue de promotion d’événement/webinaire :

>[!VIDEO](https://video.tv.adobe.com/v/3429196/?learn=on)

>[!BEGINTABS]

>[!TAB Dynamic Chat]

#### Phase 1

Créez un modèle pour le dialogue &quot;enregistrement d’événement&quot; pour une utilisation continue de la campagne.

#### Phase 2

1. Cloner le modèle.
2. Copier et coller du texte dans le message Dialogue pour un nouvel événement
3. Mettez à jour les paramètres UTM utilisés dans votre lien d’événement (par exemple utm_medium=website&amp;utm_source=adobe).
4. Créez un lien de test, cliquez sur &quot;Publier&quot; et partagez-le avec le demandeur.
5. Examen par les pairs et application des commentaires.


>[!TAB Marketo Engage]

#### Phase 1

1. Créez votre campagne de suivi dynamique dans le modèle de programme webinaire/d’événement et testez-le.

#### Phase 2

1. Ajoutez le nom de votre campagne au suivi de la campagne dynamique dans Marketo Engage et testez-la.

>[!ENDTABS]


#### Niveau supérieur : enregistrer les personnes connues

Vous pouvez offrir une expérience encore meilleure aux visiteurs du site web en les enregistrant pour vos événements et vos webinaires sans qu’ils remplissent un formulaire. Les expériences personnalisées créent de la confiance et montrent aux visiteurs que vous vous souvenez d’eux. Voyons comment mettre à niveau votre événement et votre promotion de webinaire Dialogue en action.

>[!NOTE]
>Veuillez prendre en compte les risques potentiels de sécurité inhérents à certains Etats/pays protecteurs et mettre en oeuvre cette personnalisation avec précaution en consultant votre équipe juridique.

>[!VIDEO](https://video.tv.adobe.com/v/3429197/?learn=on)

>[!BEGINTABS]

>[!TAB Dynamic Chat]

1. Cloner la boîte de dialogue de promotion Événement/Webinaire.
2. Dans le Concepteur de flux, une fois que l’utilisateur a répondu &quot;Oui&quot;, ajoutez une carte de questions &quot;Vous avez déjà partagé votre adresse électronique avec nous. Souhaitez-vous le conserver pour les détails de l’événement ?&quot;
3. S’ils répondent &quot;Oui&quot;, ajoutez une carte de message &quot;Vous recevrez un email de confirmation dans votre email avec les détails de l’événement/du webinaire&quot;.
4. S&#39;ils répondent &quot;Non&quot;, ajoutez une carte de message &quot;Veuillez remplir le formulaire sur la page d&#39;inscription&quot;.
5. Créez un lien de test, cliquez sur &quot;Publier&quot; et partagez-le avec le demandeur.
6. Dans l’onglet Audience , ajoutez [email n&#39;est pas vide].

>[!TAB Marketo Engage]

1. Ajoutez ce nouveau dialogue au suivi de la campagne dynamique dans Marketo Engage et testez-le.

>[!ENDTABS]

### Cas d’utilisation 3 : extension de l’engagement du contenu d’une campagne

Imaginez une fenêtre captivante qui attire votre oeil et vous attire dans un magasin. Si un réceptionniste vous aide alors à sélectionner des produits ou à répondre à vos questions, vous pouvez vous sentir plus à l&#39;aise pour faire un achat. Pour répliquer cette expérience en ligne, la boîte de dialogue de votre Dynamic Chat peut s’afficher sur les pages web où vos campagnes marketing orientent les visiteurs. Lorsque les utilisateurs interagissent avec le contenu web, Dynamic Chat affiche immédiatement les conversations pertinentes, suggérant du contenu supplémentaire ou répondant à des questions potentielles. Pour ce faire, utilisez les déclencheurs d’automatisation pour activer les campagnes de Dynamic Chat en fonction de l’engagement des utilisateurs dans les programmes de Marketo Engage. Maintenant, voyons comment donner vie à ce cas pratique.

>[!VIDEO](https://video.tv.adobe.com/v/3429199/?learn=on)

Extension de l&#39;engagement du contenu Campaign - Configuration :

>[!VIDEO](https://video.tv.adobe.com/v/3429200/?learn=on)

>[!BEGINTABS]

>[!TAB Dynamic Chat]

1. Générez de nouvelles pistes pour vos campagnes par courrier électronique et les points de contact des campagnes sur les réseaux sociaux. Dans cet exemple, l&#39;enquête de l&#39;index de santé Talent est hébergée sur le site web de la marque.
2. Cloner un modèle de dialogue existant (dialogue fourre-tout par défaut, par exemple) pour créer trois boîtes de dialogue pour les scénarios suivants et mettre à jour l’&quot;URL cible&quot; dans l’onglet &quot;Audience&quot; en conséquence :
   * Lorsque des visiteurs web sont venus de vos canaux marketing et arrivent sur votre page web.
   * Sur la page de remerciement
   * Tout visiteur qui revient sur votre site web dans les 45 jours suivant la campagne marketing (reciblage)

>[!ENDTABS]

## Et après ?

* Mappez votre flux de conversation dans [Concepteur de diffusion](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer){target="_blank"} ou un diagramme de flux hors ligne.
* Créez un dialogue fourre-tout par défaut en Dynamic Chat.
* Activez les conversations après l’engagement de la campagne à l’aide de déclencheurs d’automatisation dans Marketo Engage.


## Auteurs

{{sara-barriuso}}

{{amy-chiu}}