---
title: Personnalisation de l’écran du portail multimédia
description: Découvrez comment personnaliser l’écran Media Portal.
uuid: bd1a65a6-723b-49d0-8eac-849da00e0e1a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 8b000c25-c9c3-481e-9b25-96257471571f
feature: Dynamic Media Classic,Collaboration,Gestion des ressources
role: Admin,User
exl-id: b0c5f70a-2388-42aa-a1ed-fd745ff90518
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 46%

---

# Personnalisation de l’écran du portail multimédia{#customizing-the-media-portal-screen}

Les paramètres de style du portail multimédia vous permettent de faire apparaître la marque de votre entreprise sur l’écran du portail multimédia sous forme de logo et de couleurs personnalisés. Utilisez les paramètres de style pour placer la marque de votre entreprise sur Media Portal.

Pour accéder aux paramètres de style, choisissez **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de Media Portal]** > **[!UICONTROL Paramètres de style]**. Assurez-vous de cliquer sur **[!UICONTROL Enregistrer]** pour enregistrer vos paramètres après les avoir définis. Vous pouvez cliquer sur **[!UICONTROL Restaurer]** pour retrouver les paramètres par défaut. A mesure que vous configurez les options, le panneau de prévisualisation reflète vos choix.

* **Logo**  : cliquez sur  **** Parcourir et sélectionnez un graphique dans la fenêtre Sélectionner l’image du logo.

* **Application**  : créez un dégradé de couleurs en effectuant des choix dans les menus Couleurs du dégradé de l’arrière-plan.

* **Arborescence**  : choisissez une couleur de survol (la couleur qui s’affiche lorsque vous placez le pointeur sur un élément) et une couleur de sélection (la couleur qui s’affiche lorsque vous sélectionnez un élément).

* **Accordéon**  : choisissez les couleurs d’arrière-plan, le style de la bordure, le survol et les couleurs sélectionnées pour l’accordéon qui s’affiche sur le côté droit de l’écran en mode Détails.

* **En-tête d’accordéon**  : choisissez si vous souhaitez insérer du texte dans le gras de l’en-tête d’accordéon.

* **Grille de données**  : choisissez les couleurs de la rangée d’en-tête dans les grilles de données.

* **Alerte**  : sélectionnez une couleur d’arrière-plan pour les zones de message d’alerte.

* **Barre de progression**  : choisissez une couleur pour la barre qui indique la progression des chargements et des téléchargements.

Pour que les utilisateurs du portail multimédia voient les paramètres de style que vous avez choisis, ils doivent ajouter `?company=(company name)` à l’URL avec laquelle ils accèdent au portail multimédia. Par exemple, pour voir les paramètres de style, les utilisateurs du portail multimédia qui accèdent à l’entreprise PortalCo à l’adresse l’exemple suivant :

`https://s7sps1.scene7.com/MediaPortal`

Utilisez plutôt l’URL suivante :

`https://s7sps1.scene7.com/MediaPortal?company=PortalCo`

L’inclusion du nom de l’entreprise dans l’URL permet au portail multimédia d’identifier l’entreprise à laquelle un utilisateur souhaite accéder et d’appliquer des paramètres de style de l’entreprise en question.

Vous pouvez en savoir plus sur la communication des changements d’URL aux utilisateurs du portail multimédia, et sur la définition d’un message de l’e-mail de bienvenue pour que les nouveaux utilisateurs reçoivent l’URL de portail multimédia correcte.

Voir [Définition du message de l’e-mail de bienvenue pour les utilisateurs du portail multimédia](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users).
