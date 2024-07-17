---
title: Dix bonnes pratiques pour le succès de [!DNL Adobe] [!DNL Campaign] pour les marketeurs
description: Découvrez les dix bonnes pratiques pour aider les utilisateurs de [!DNL Adobe] [!DNL Campaign] à déverrouiller et à accélérer la transformation des consommateurs numériques et une meilleure expérience pour leurs clients.
doc-type: article
solution: Campaign
feature-set: Campaign
feature: Personalization, Campaigns, Subscriptions, Deliverability
role: User
level: Beginner
jira: KT-11772
last-substantial-update: 2023-01-31T00:00:00Z
exl-id: add6ed84-892d-4901-9dd2-b0cba0c57290
source-git-commit: ec621f6e118292a3f8448c0e21abe8a1284cb10e
workflow-type: tm+mt
source-wordcount: '1262'
ht-degree: 77%

---

# Dix bonnes pratiques pour le succès de [!DNL [!DNL Adobe] [!DNL Campaign]] pour les marketeurs

Christian Klimczyk est un &quot;[!DNL Adobe] Nerd&quot; autodécrit avec sept ans d&#39;expertise [!DNL [!DNL Adobe] Experience Cloud], principalement axé sur [!DNL [!DNL Adobe] [!DNL Campaign]]. En tant que propriétaire de plateforme [!DNL Adobe] pour une grande société CPG, Christian et son équipe utilisent [!DNL [!DNL Campaign]] pour toutes les communications et interactions des consommateurs. Ils coordonnent et gèrent de manière transparente les exigences de réglementation élevées et les campagnes marketing client multicanaux par publipostage direct, e-mail et SMS/MMS.

Dans cet article, Christian partage ses bonnes pratiques pour aider les utilisateurs de [!DNL Adobe] [!DNL Campaign] à déverrouiller et à accélérer la transformation numérique des consommateurs et à offrir une meilleure expérience à leurs clients.


## 1. Créer un plan de diffusion et de marketing global et cohérent

La première étape pour garantir votre succès avec [!DNL [!DNL Adobe] [!DNL Campaign]] consiste à comprendre vos outils et les attentes de vos clients, ce qui est vrai dans n’importe quel type de marketing. Définissez et comprenez clairement les canaux que vous utilisez pour contacter vos client(e)s, sachez quand utiliser ces canaux et pourquoi.

[!DNL Adobe] [!DNL Campaign] est un outil flexible qui vous permet d’exécuter et d’orchestrer des communications de différentes manières. [La moitié des client(e)s utilisent trois à cinq canaux lors de chaque parcours d’achat ](https://www.mckinsey.com/capabilities/operations/our-insights/redefine-the-omnichannel-approach-focus-on-what-truly-matters). Il est donc essentiel de comprendre et de planifier l’utilisation de ces canaux pour accomplir tout le potentiel de votre plateforme et interagir avec vos client(e)s.

## 2. Documenter et comprendre vos données des client(e)s

<!-- Sandra, this paragraph opens as if it's going to discuss the advantages of segmentation, but it left me hanging. So, I hit the Hubspot link and dug into it a bit, and it seemed to me like the juicy information is this quote: 

"A study by Hubspot revealed that 30% of the marketers who participated in it used market segmentation techniques to improve email engagement. Segmented campaigns had 14.31% higher open rates and saw 101% more clicks than non-segmented campaigns.

"Email marketers who segmented their audience before campaigning stated that the revenue generated increased to up to 760%. Targeted and segmented emails bring in 58% of all revenue." [Link](https://www.notifyvisitors.com/blog/segmentation-statistics/) 

I added that second paragraph about 760% revenue and broke up the rest of the section, touched it up to help make the Hubspot example a little more impactful. If I altered this section too much, you can reject the change. It didn't have mistakes, but it felt like it didn't tie the segment example strongly enough to the point about data design. See if this is okay...-->

Selon une [étude de Hubspot](https://www.linkedin.com/pulse/customer-segmentation-effective-b2b-business-industry-sabreen), les campagnes segmentées auraient un taux d’ouverture supérieur de 14,31 % et enregistreraient 101 % de clics de plus que les campagnes non segmentées. Les spécialistes marketing par e-mail qui ont segmenté leur audience avant de lancer leur campagne ont déclaré que les recettes générées ont augmenté jusqu’à 760 %.

Dans [!DNL Adobe] [!DNL Campaign], vous pouvez orchestrer la segmentation rapidement et facilement. Toutefois, pour rationaliser et faciliter ce processus, les opérateurs et opératrices de campagne et les professionnel(le)s du marketing doivent avoir une compréhension documentée de leurs données sous-jacentes lors de la conception et de la demande de la création et de l’exécution d’une campagne. Il est essentiel que vous compreniez vos données actuelles et que vous déterminiez comment anticiper les données dont vous pourriez avoir besoin lors d’un partenariat avec les administrateurs et les développeurs qui prennent en charge votre instance [!DNL [!DNL Campaign]].

Vos campagnes sont aussi efficaces que les structures de données sous-jacentes qui les constituent. La connaissance et la documentation de cette structure de données aident également en cas de problèmes lors de l’intégration de plateformes ou de l’accès à une plateforme de données clientes.

## 3. Planifier le timing de vos campagnes

Comme vos client(e)s, vous avez une routine quotidienne. L’envoi et l’orchestration de vos campagnes doivent correspondre à ce rythme. Sinon, vous risquez de ne pas atteindre vos client(e)s, étant donné que [85 % des e-mails envoyés ne sont jamais ouverts et 98 % n’obtiennent pas de clic publicitaire](https://www.validity.com/resource-center/state-of-email-2021/).

Si, par exemple, vos client(e)s consultent leur téléphone le matin à la recherche des meilleures offres, envisagez de leur envoyer une promotion par SMS. S’ils ou elles naviguent la nuit en quête de la prochaine tendance, pensez à envoyer un e-mail de relance avec un code promo pour une livraison gratuite. Il est également important d’utiliser l’outil de carte thermique dans [!DNL [!DNL Campaign]] pour suivre le moment où vos workflows et envois s’exécutent. La coordination et la facilitation des communications entre plusieurs marques peut s’avérer difficile. [Garder un oeil sur et connaître le rythme, la cadence et le timing de vos emails](https://experienceleaguecommunities.adobe.com/t5/adobe-campaign-classic-blogs/predictive-send-time-optimization-with-adobe-campaign/ba-p/561554?profile.language=fr) est inestimable pour la stabilité et la force globales de votre message et de votre instance [!DNL Campaign].

## 4. Utiliser la personnalisation là où elle est importante

De nos jours, les consommateurs et consommatrices s’attendent à un certain niveau de personnalisation dans les messages qu’ils reçoivent. [80 % des client(e)s sont plus susceptibles d’acheter auprès d’une marque qui fournit des expériences personnalisées](https://us.epsilon.com/power-of-me). Leur nom dans la ligne d’objet est attrayant. Cependant, la personnalisation peut aller beaucoup plus loin. Vous pouvez inclure les produits qu’ils ont parcourus, les connecter à des produits similaires ou continuer à renforcer la cohésion de l’expérience et l’aspect de votre marque. Chaque détail compte et favorise l’engagement et les taux d’ouverture de vos messages.

## 5. Posséder un inventaire sain de ressources de création

Les ressources de création sont l’essence qui alimente votre moteur de diffusion de campagne efficace et bien huilé. Plus vous atteignez vos client(e)s et plus vous adaptez et plus vous faites évoluer vos processus de marketing, plus vous avez besoin de contenu créatif. Les consommateurs et consommatrices s’attendent à cela.

Votre rapidité dépend de la prochaine diffusion que votre équipe peut configurer. Cela nécessite souvent du contenu nouveau et passionnant. [!DNL [!DNL Adobe] [!DNL Campaign]] facilite la configuration des modèles, la réception et la préparation de ces diffusions. Toutefois, il est essentiel d’avoir un pipeline de création sain, car, selon un [rapport Litmus](https://www.litmus.com/resources/state-of-email/), 58 % des spécialistes marketing ont remarqué que la création d’une campagne par e-mail prend deux semaines ou plus.

## 6. Comprendre et gérer les abonnements et les préférences

La gestion et la maintenance des préférences d’abonnement peuvent rapidement s’avérer déroutantes, ce qui entraîne divers niveaux de risque. Neuf consommateurs ou consommatrices sur dix déclarent qu’avoir une expérience négative les rend moins susceptibles d’acheter auprès d’une marque à l’avenir, telle que recevoir un message erroné sur un canal auquel on ne répond pas. À plus grande échelle, vous pourriez vous exposer à des risques et amendes liés à la réglementation et à la conformité.

Ayez une stratégie à l&#39;avant-garde pour gérer les opt-ins et cultiver cet écosystème en constante évolution grâce à l&#39;utilisation experte de [!DNL [!DNL Adobe] [!DNL Campaign]] et d&#39;autres outils de technologie marketing. Il s’agit généralement de l’un des principaux indicateurs de réussite d’une campagne. Une planification minutieuse génère donc des dividendes inestimables à mesure que votre stratégie de campagne se développe jusqu’à maturité.

## 7. Comprendre et planifier la délivrabilité

La _délivrabilité_ s’apparente souvent à un concept compliqué, voire mystique. La planification stratégique est une règle fondamentale de la délivrabilité. Préchauffer les adresses IP et et se forger une bonne réputation prend du temps. Cette réputation peut se dégrader rapidement, ce qui complique la réparation des dommages subis. En effet, **un e-mail sur six n’atteint pas la boîte de réception**.

Des problèmes de délivrabilité peuvent être dus à de nombreux facteurs, qu’ils soient techniques ou liés à la façon dont les consommateurs et consommatrices réagissent à votre marketing. En gardant à l’esprit la [délivrabilité](https://business.adobe.com/fr/products/campaign/email-deliverability.html) lors de la création et de l’exécution des campagnes, ainsi que dans le processus de rétrospective, vous pouvez veiller au maintien d’un environnement sain et stable et continuer à offrir des expériences positives aux client(e)s.

## 8. Planifier et développer un processus de rétrospective de campagne

Bien que la diffusion et l’orchestration des campagnes puissent exiger beaucoup de travail, il est également important, voire plus, d’examiner ce que vous avez accompli et de réévaluer vos processus et la segmentation de vos campagnes. Tenez des rétrospectives de campagne toutes les deux à quatre semaines, selon l’échelle et la vitesse d’exécution de vos campagnes.

La création d’un ensemble modélisé de questions peut contribuer à alimenter une conversation approfondie et réfléchie sur la façon d’améliorer les délais de campagne, le contenu créatif ou la segmentation, parmi de nombreux autres sujets. Parfois, vous ne pouvez vous améliorer et devenir plus efficace que si vous tirez des enseignements de vos expériences passées.

## 9. Tester et itérer

Quand on essaie de nouvelles choses, on ne réussit pas toujours du premier coup. Il est donc essentiel de tester et d’itérer vos processus et tactiques. Essayez de trouver un groupe de client(e)s qui ne sont pas forcément intéressé(e)s ou qui pourraient l’être. Adoptez une nouvelle approche créative. Essayez un nouvel appel à l’action. Changer simplement pour changer n’est pas productif, mais plusieurs petites expériences précises au fil du temps peuvent aboutir à des gains futurs potentiellement importants pour vous et vos client(e)s.

## 10. Soyez aussi flexible que possible

Le marché change et évolue à un rythme toujours plus effréné. Il est primordial d’encourager vos équipes de campagne à rester aussi flexibles et rapides que possible afin de rester compétitif et de continuer à répondre aux attentes croissantes des client(e)s.

[35 % des responsables du marketing numérique estiment que les plus grands défis viennent de l’intérieur de leur organisation.](https://www.gartner.com/en/newsroom/press-releases/gartner-says-35--of-digital-marketing-leaders-believe-the-bigges). Pour ce faire, suivez des formations sur quelques plates-formes, approfondissez votre compréhension des flux de données et de la structure ou d’autres solutions [!DNL Adobe] et créez des plans d’urgence pour les campagnes. Cet état d’esprit peut être atteint de plusieurs façons, mais un engagement global en faveur de la flexibilité et de la planification est essentiel pour obtenir un succès à court et à long terme.
