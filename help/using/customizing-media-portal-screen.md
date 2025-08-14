---
title: Personnalisation de l’écran du portail multimédia
description: Découvrez comment personnaliser l’écran du portail multimédia dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: b0c5f70a-2388-42aa-a1ed-fd745ff90518
topic: Collaboration, Content Management
level: Intermediate
source-git-commit: 00591bdbe721035e25d3dea245a2110f978d19aa
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 17%

---

# Personnalisation de l’écran du portail multimédia{#customizing-the-media-portal-screen}

Les paramètres de style du portail multimédia vous permettent de faire apparaître la marque de votre entreprise sur l’écran du portail multimédia sous forme de logo et de couleurs personnalisés. Utilisez les paramètres de style pour placer l’image de marque de votre entreprise sur le portail multimédia.

Pour accéder aux paramètres de style, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de Media Portal]** > **[!UICONTROL Paramètres de style]**. Veillez à sélectionner **[!UICONTROL Enregistrer]** pour enregistrer vos paramètres une fois qu’ils ont été définis. Vous pouvez sélectionner **[!UICONTROL Restaurer]** pour rétablir les paramètres par défaut. Lorsque vous effectuez vos choix, le panneau Aperçu vous montre leur apparence.

* **[!UICONTROL Logo]** : sélectionnez **[!UICONTROL Parcourir]**, puis choisissez un graphique dans la fenêtre Sélectionner une image de logo.

* **[!UICONTROL Application]** : créez un dégradé de couleurs en effectuant des choix dans les menus des Couleurs de dégradé d’arrière-plan.

* **[!UICONTROL Arborescence]** : choisissez une couleur de survol et une couleur de sélection.

* **[!UICONTROL Accordéon]** : sélectionnez les couleurs d’arrière-plan, un style de bordure, ainsi que les couleurs de survol et sélectionnées pour l’accordéon qui s’affiche sur le côté droit de l’écran en mode Détails.

* **[!UICONTROL En-tête d’accordéon]** : indiquez si le texte doit être en gras dans l’en-tête d’accordéon.

* **[!UICONTROL Grille de données]** : choisissez les couleurs de la ligne d’en-tête dans les grilles de données.

* **[!UICONTROL Alerte]** : choisissez une couleur d’arrière-plan pour les zones de message d’alerte.

* **[!UICONTROL Barre de progression]** : choisissez la couleur de la barre qui indique la progression des chargements et des téléchargements.

Pour que les utilisateurs du portail multimédia voient les paramètres de style que vous avez choisis, ils doivent ajouter `?company=(company name)` à l’URL avec laquelle ils accèdent au portail multimédia. Par exemple, pour afficher les paramètres de style, les utilisateurs du portail multimédia qui accèdent à la société PortalCo peuvent accéder aux éléments suivants :

`https://s7sps1.scene7.com/MediaPortal`

Utilisez plutôt l’URL suivante :

`https://s7sps1.scene7.com/MediaPortal?company=PortalCo`

L’inclusion du nom de la société dans l’URL permet à Media Portal de reconnaître la société à laquelle un utilisateur souhaite accéder et d’appliquer les paramètres de style de la société en conséquence.

Vous pouvez en savoir plus sur la communication des changements d’URL aux utilisateurs du portail multimédia, et sur la définition d’un message de l’e-mail de bienvenue pour que les nouveaux utilisateurs reçoivent l’URL de portail multimédia correcte.

Voir [Définition du message de l’e-mail de bienvenue pour les utilisateurs du portail multimédia](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users).
