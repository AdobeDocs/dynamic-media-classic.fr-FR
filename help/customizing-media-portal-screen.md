---
title: Personnalisation de l’écran du portail multimédia
description: Découvrez comment personnaliser l’écran du portail multimédia.
uuid: bd1a65a6-723b-49d0-8eac-849da00e0e1a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 8b000c25-c9c3-481e-9b25-96257471571f
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Administrator,Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 51%

---


# Personnalisation de l’écran du portail multimédia{#customizing-the-media-portal-screen}

Les paramètres de style du portail multimédia vous permettent de faire apparaître la marque de votre entreprise sur l’écran du portail multimédia sous forme de logo et de couleurs personnalisés. Grâce aux paramètres de style, vous pouvez faire figurer le tampon de votre société sur le portail multimédia. 

Pour accéder aux paramètres de style, choisissez **Configuration** > **Configuration de Media Portal** > **Paramètres de style**. Assurez-vous de cliquer sur **Enregistrer** pour enregistrer vos paramètres après les avoir définis. Vous pouvez cliquer sur **Restaurer** pour retrouver les paramètres par défaut. A mesure que vous configurez les options, le panneau de prévisualisation reflète vos choix.

**** LogoCliquez sur Parcourir et choisissez un graphique dans la fenêtre Sélectionner l&#39;image de logo.

**** ApplicationCréez un dégradé de couleurs mélangées en faisant des choix dans les menus Couleurs en dégradé d&#39;arrière-plan.

**** ArbreChoisissez une couleur de survol (couleur qui s&#39;affiche lorsque vous déplacez le pointeur sur un élément) et une couleur de sélection (couleur qui s&#39;affiche lorsque vous sélectionnez un élément).

**** AccordéonChoisissez les couleurs d’arrière-plan, un style de bordure et les couleurs de survol et de sélection pour l’accordéon qui s’affiche sur le côté droit de l’écran dans la vue des détails.

**Accordéon** HeaderChoisissez si vous souhaitez insérer du texte dans l’en-tête en accordéon en gras.

**** DatagridChoisissez les couleurs de la rangée d&#39;en-tête dans les grilles de données.

**** AlerteChoisissez une couleur d&#39;arrière-plan pour les zones de message d&#39;alerte.

**Barre de progressionChoisissez une couleur pour la barre qui indique la progression des téléchargements et des téléchargements.** 

Pour que les utilisateurs du portail multimédia puissent voir les paramètres de style que vous choisissez, ils doivent ajouter `?company=(company name)` à l’URL avec laquelle ils accèdent au portail multimédia. Par exemple, pour voir les paramètres de style, les utilisateurs du portail multimédia qui accèdent à l’entreprise PortalCo à l’adresse l’exemple suivant :

`https://s7sps1.scene7.com/MediaPortal`

utilise l’URL suivante à la place :

`https://s7sps1.scene7.com/MediaPortal?company=PortalCo`

L’inclusion du nom de l’entreprise dans l’URL permet au portail multimédia d’identifier l’entreprise à laquelle un utilisateur souhaite accéder et d’appliquer des paramètres de style de l’entreprise en question.

Vous pouvez en savoir plus sur la communication des changements d’URL aux utilisateurs du portail multimédia, et sur la définition d’un message de l’e-mail de bienvenue pour que les nouveaux utilisateurs reçoivent l’URL de portail multimédia correcte.

Voir [Définition du message de l’e-mail de bienvenue pour les utilisateurs du portail multimédia](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users).
