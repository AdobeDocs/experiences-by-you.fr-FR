---
title: Concevoir du marketing conversationnel omnicanal avec Dynamic Chat
description: Découvrez rapidement comment concevoir le marketing conversationnel avec Adobe Dynamic Chat, le canal d’engagement conversationnel natif de Adobe Marketo Engage. Ce tutoriel propose des recettes exploitables pour implémenter des cas d’utilisation tels que la réservation de réunions de vente, l’engagement de contenu de site web et la promotion d’événements/de webinaires.
role: Admin
level: Beginner
doc-type: Article
solution: Marketo Engage
duration: 0
last-substantial-update: 2024-05-23T00:00:00Z
jira: KT-14814
exl-id: 160dfb25-9f54-4dce-a08a-4a8d3c4c5368
source-git-commit: 1205848b1985a99b91f9d4d25e1a79f0df379589
workflow-type: tm+mt
source-wordcount: '1458'
ht-degree: 0%

---

# Conception de marketing conversationnel omnicanal avec Dynamic Chat

Pour les spécialistes du marketing, votre site web est essentiel pour générer des prospects, stimuler les conversions et accélérer les cycles de vente. Interagir avec les visiteurs en temps réel sur votre site web permet à votre équipe de vente de qualifier les acheteurs plus efficacement. Adobe Dynamic Chat, le canal de conversation natif de votre abonnement Adobe Marketo Engage, vous permet d’automatiser les conversations afin d’étendre les fonctionnalités de Marketo Engage.

Ce tutoriel décrit le processus de réflexion et les principaux cas d’utilisation partagés par Sara Barriuso, responsable des opérations marketing chez Cornerstone OnDemand, lors de la session « Apprenez de vos pairs ». Elle a expliqué comment son organisation utilisait Dynamic Chat pour optimiser les fonctionnalités de Marketo Engage.

## Intégrer l&#39;engagement conversationnel dans votre stratégie de génération de demande

Les visiteurs et visiteuses parcourent votre site web pour une raison. Il est possible qu’il recherche du contenu sur vos produits ou services, ou des coordonnées pour s’adresser à vos représentants commerciaux. Il peut également s’agir de vos clients qui recherchent des informations supplémentaires sur les produits. Le chat permet aux visiteurs de votre site Web de se mettre en libre-service et de s&#39;autoqualifier s&#39;ils sont prêts à parler à votre équipe de vente.

Lorsque Sara Barriuso a implémenté Dynamic Chat, elle a été séduite par son intégration transparente à Marketo Engage et par les [déclencheurs d’activité préconfigurés](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-activities){target="_blank"} qui activent les programmes Marketo Engage et vice versa. Elle a élaboré ses stratégies d’engagement conversationnel en tenant compte de trois segments d’audience :

1. Prospects inconnus : proposer de manière proactive des appels de démonstration pour générer de nouveaux prospects.
2. Leads/clients connus : allongez le temps passé par les visiteurs à parcourir le contenu et proposez des appels de démonstration pour générer des opportunités de vente incitative et de vente croisée.
3. Prospects/clients : proposent des expériences personnalisées en étendant les efforts des campagnes marketing.


## Cas d’utilisation clés pour commencer à créer vos boîtes de dialogue

Pour mettre en œuvre ces stratégies, Sara a créé ses dialogues Dynamic Chat autour des cas d’utilisation suivants :

1. Boîte de dialogue fourre-tout par défaut : donnez une option initiale à tous les visiteurs et visiteuses, en les guidant pour accomplir leurs tâches plus efficacement.

2. Promotion de l’inscription aux événements et webinaires : incitez les visiteurs et visiteuses du site à s’inscrire aux événements et webinaires pour les faire passer plus rapidement par la phase d’achat.

3. Étendre l’engagement du contenu de la campagne : offrez un contexte supplémentaire ou répondez à des questions potentielles lorsque les visiteurs parcourent le contenu du site web.

Voyons ces cas pratiques en action comme Sara présente son processus, de la cartographie du flux conversationnel à la configuration des boîtes de dialogue et du ciblage dans Dynamic Chat et Marketo Engage.

### Cas d’utilisation 1 : boîte de dialogue fourre-tout par défaut pour tous les visiteurs du site

Cette boîte de dialogue propose cinq options initiales aux visiteurs du site, ce qui crée une expérience autoguidée qui les aide à trouver les informations dont ils ont besoin en fonction de leur personnalité. Pour commencer, vous pouvez explorer votre boîte de réception e-mail « Contactez-nous » pour identifier les thèmes communs et les classer en options de boîte de dialogue qui s’appliquent aux visiteurs de votre site. Regardez la démonstration et suivez les étapes ci-dessous pour créer votre boîte de dialogue fourre-tout par défaut :

>[!VIDEO](https://video.tv.adobe.com/v/3454849/?captions=fre_fr&learn=on)

>[!BEGINTABS]

>[!TAB Tab]

#### Phase 1

1. Créez la boîte de dialogue et un lien de test.
2. Ajoutez un objectif pour effectuer le suivi des conversions (par exemple, envoi de la demande de démonstration).
3. Demandez à 2 ou 3 personnes de le tester et de recueillir leurs commentaires.

#### Phase 2

1. Dans « Audience », ajoutez une URL de page web dans « Target » pour indiquer où la boîte de dialogue s’affichera.
2. Dans « Paramètres », ajoutez le nom, la description, la priorité et la langue de la campagne.
3. Cliquez sur Publier.

>[!TAB Tab&#x200B;]

#### Phase 1

1. Créez votre campagne intelligente de suivi.
2. Dans Liste dynamique, utilisez un déclencheur « Atteint l’objectif de la boîte de dialogue ». Utilisez le même objectif (par exemple, Demande de démonstration) que celui de la boîte de dialogue
3. Dans « Flux », incluez une étape « Modifier le statut du programme » pour suivre la conversion.
4. La source s’affichera en tant que « dynamicChat ». Vous pouvez créer une campagne intelligente pour mettre à jour la source vers un nom qui vous semble logique.

#### Phase 2

1. Testez à nouveau votre campagne intelligente de suivi lorsqu’elle sera en ligne.

>[!ENDTABS]

#### Niveau supérieur : marketing basé sur les comptes

Vous pouvez améliorer la Boîte de dialogue fourre-tout par défaut en incorporant du contenu ciblé par le secteur, ce qui rend les conversations encore plus utiles pour les visiteurs et les visiteuses. Par exemple, proposez des livres blancs ou des études de cas spécifiques à un secteur que vos visiteurs peuvent télécharger. Regardez la démonstration et suivez les étapes ci-dessous pour créer une boîte de dialogue fourre-tout par défaut pour le marketing basé sur les comptes :

>[!VIDEO](https://video.tv.adobe.com/v/3429195/?learn=on)

>[!BEGINTABS]

>[!TAB Tab]

1. Clonez la « Boîte de dialogue par défaut » et renommez-la.
2. Dans « Stream Designer », adaptez les messages de la boîte de dialogue au secteur cible (un seul flux + la question initiale).
3. Demandez à 2 ou 3 personnes de tester la boîte de dialogue et de collecter les commentaires.
4. Créer un lien de test et le partager.
5. Dans « Audience », ajoutez une URL de page web où la boîte de dialogue s’affichera et mettra à jour la cible selon le secteur que vous souhaitez.
6. Dans « Paramètres », ajoutez le nom de la campagne, la priorité de description et la langue.
7. Cliquez sur « Publier ».

>[!TAB Tab&#x200B;]

1. Créez votre campagne intelligente de suivi et testez l’objectif.
2. Testez à nouveau la campagne intelligente de suivi après avoir publié la boîte de dialogue.

>[!ENDTABS]

### Cas d’utilisation 2 : promotion de l’enregistrement à l’événement et au webinaire

Les événements et webinaires sont des tactiques marketing populaires pour les entreprises B2B afin de générer de la demande. Ils offrent des expériences attrayantes et des informations riches qui attirent les clients potentiels. La connexion des visiteurs et visiteuses de votre site web aux événements et webinaires à venir vous permet de qualifier les clientes et clients potentiels encore plus rapidement. La création de cette boîte de dialogue demande peu d’efforts et est peu coûteuse. Elle peut rapidement s’avérer efficace et vous aider à obtenir le soutien des parties prenantes marketing pour ajouter l’engagement conversationnel à votre plan d’automatisation omnicanal. Regardez la démonstration et suivez les étapes ci-dessous pour créer votre boîte de dialogue de promotion d’événement/webinaire :

>[!VIDEO](https://video.tv.adobe.com/v/3429196/?learn=on)

>[!BEGINTABS]

>[!TAB Tab]

#### Phase 1

1. Créez un modèle de boîte de dialogue « enregistrement d’événement » pour une utilisation continue de la campagne.

#### Phase 2

1. Clonez le modèle.
2. Copiez et collez du texte dans le message de la boîte de dialogue pour un nouvel événement.
3. Mettez à jour les paramètres UTM utilisés dans votre lien d’événement (par exemple, utm_medium=website&amp;utm_source=adobe).
4. Créez un lien de test, cliquez sur « Publier », puis partagez-le avec le demandeur.
5. Examen par les pairs et application des commentaires.


>[!TAB Tab&#x200B;]

#### Phase 1

1. Créez votre campagne intelligente de suivi dans le modèle de programme de webinaire/événement et testez-la.

#### Phase 2

1. Ajoutez le nom de votre campagne à la campagne intelligente de suivi dans Marketo Engage et testez-la.

>[!ENDTABS]


#### Niveler vers le haut : enregistrer les personnes connues

Vous pouvez offrir une expérience encore meilleure aux visiteurs et visiteuses du site Web en les inscrivant à vos événements et webinaires sans leur demander de remplir un formulaire. Les expériences personnalisées renforcent la confiance et montrent aux visiteurs que vous vous souvenez d’eux. Découvrons comment améliorer votre événement et la promotion du webinaire Dialogue en action.

>[!NOTE]
>Veuillez tenir compte des risques de sécurité potentiels encourus par certains États/pays protecteurs et mettre en œuvre cette personnalisation avec soin en consultant votre équipe juridique.

>[!VIDEO](https://video.tv.adobe.com/v/3429197/?learn=on)

>[!BEGINTABS]

>[!TAB Tab]

1. Clonez la boîte de dialogue de promotion d’événement/de webinaire.
2. Dans Stream Designer, une fois que l&#39;utilisateur a répondu « Oui », ajoutez une carte de questions « Vous avez déjà partagé votre adresse e-mail avec nous. Voulez-vous conserver ceci pour les détails de l’événement ? »
3. S’ils répondent « Oui », ajoutez une carte de message « Vous recevrez un e-mail de confirmation dans votre e-mail contenant les détails de l’événement/du webinaire ».
4. S&#39;ils répondent « Non », ajoutez une carte de message « Veuillez remplir le formulaire sur la page d&#39;inscription ».
5. Créez un lien de test, cliquez sur « Publier », puis partagez-le avec le demandeur.
6. Dans l’onglet Audience , ajoutez [l’e-mail n’est pas vide].

>[!TAB Tab&#x200B;]

1. Ajoutez cette nouvelle boîte de dialogue à la campagne intelligente de suivi dans Marketo Engage et testez-la.

>[!ENDTABS]

### Cas d’utilisation 3 : extension de l’engagement du contenu de campagne

Imaginez qu’un écran de fenêtre captivant attire votre attention et vous entraîne dans un magasin. Si une réceptionniste vous aide ensuite à choisir des produits ou répond à vos questions, vous vous sentirez peut-être plus à l&#39;aise de faire un achat. Pour répliquer cette expérience en ligne, vous pouvez afficher la boîte de dialogue Dynamic Chat sur les pages web vers lesquelles vos campagnes marketing dirigent les visiteurs. Lorsque les utilisateurs et utilisatrices consultent le contenu web, Dynamic Chat affiche immédiatement les conversations pertinentes, suggérant du contenu supplémentaire ou répondant à des questions potentielles. Pour ce faire, utilisez des déclencheurs d’automatisation pour activer les campagnes Dynamic Chat en fonction de l’interaction client dans les programmes Marketo Engage. Maintenant, voyons comment donner vie à ce cas d’utilisation.

>[!VIDEO](https://video.tv.adobe.com/v/3429199/?learn=on)

Extension de l’engagement de contenu de Campaign - Configuration :

>[!VIDEO](https://video.tv.adobe.com/v/3429200/?learn=on)

>[!BEGINTABS]

>[!TAB Tab]

1. Générez de nouveaux leads pour vos campagnes via les points de contact des e-mails et des campagnes sociales. Dans cet exemple, l’enquête de l’indice de santé Talent est hébergée sur le site web de la marque.
2. Clonez un modèle de boîte de dialogue existant (par exemple, une boîte de dialogue fourre-tout par défaut) pour créer trois boîtes de dialogue pour les scénarios suivants et mettez à jour l’« URL cible » dans l’onglet « Audience » en conséquence :
   * Lorsque les visiteurs et visiteuses web proviennent de vos canaux marketing et accèdent à votre page web.
   * Sur la page de remerciement
   * Tous les visiteurs et visiteuses qui reviennent sur votre site web dans les 45 jours suivant l’engagement dans la campagne marketing (reciblage)

>[!ENDTABS]

## Quelle est la prochaine étape ?

* Mappez votre flux de conversation dans [Stream Designer](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer){target="_blank"} ou un diagramme de flux hors ligne.
* Créez une boîte de dialogue fourre-tout par défaut dans Dynamic Chat.
* Activez les conversations après l’engagement de campagne à l’aide de déclencheurs d’automatisation dans Marketo Engage.


## Auteurs

{{sara-barriuso}}

{{amy-chiu}}
