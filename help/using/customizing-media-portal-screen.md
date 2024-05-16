---
title: Personnalisation de l’écran Media Portal
description: Découvrez comment personnaliser l’écran Media Portal dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: b0c5f70a-2388-42aa-a1ed-fd745ff90518
topic: Collaboration, Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 16%

---

# Personnalisation de l’écran Media Portal{#customizing-the-media-portal-screen}

Les paramètres de style du portail multimédia vous permettent de faire apparaître la marque de votre entreprise sur l’écran du portail multimédia sous forme de logo et de couleurs personnalisés. Utilisez les paramètres de style pour placer la marque de votre entreprise sur Media Portal.

Pour accéder aux paramètres de style, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de Media Portal]** > **[!UICONTROL Paramètres de style]**. Veillez à sélectionner **[!UICONTROL Enregistrer]** pour enregistrer vos paramètres une fois que vous les avez créés. Vous pouvez sélectionner **[!UICONTROL Restaurer]** pour rétablir les paramètres par défaut. Au fur et à mesure de vos choix, le panneau Aperçu vous montre comment ils apparaissent.

* **[!UICONTROL Logo]**: sélectionnez **[!UICONTROL Parcourir]**, puis sélectionnez un graphique dans la fenêtre Sélectionner l’image du logo .

* **[!UICONTROL Application]**: créez un dégradé de couleurs en effectuant des choix dans les menus des couleurs du dégradé de fond.

* **[!UICONTROL Arbre]**: choisissez une couleur de survol (la couleur qui s’affiche lorsque vous placez le pointeur sur un élément) et une couleur de sélection (la couleur qui s’affiche lorsque vous sélectionnez un élément).

* **[!UICONTROL Accordéon]**: choisissez les couleurs d’arrière-plan, un style de bordure, ainsi que le survol et les couleurs sélectionnées pour l’accordéon qui s’affiche sur le côté droit de l’écran en mode Détails.

* **[!UICONTROL En-tête d’accordéon]**: choisissez si le texte doit être inséré dans le gras de l’en-tête de l’accordéon.

* **[!UICONTROL Datagrid]**: choisissez les couleurs de la rangée d’en-tête dans les grilles de données.

* **[!UICONTROL Alerte]**: sélectionnez une couleur d’arrière-plan pour les zones de message d’alerte.

* **[!UICONTROL Barre de progression]**: choisissez une couleur pour la barre qui indique la progression des chargements et des téléchargements.

Pour que les utilisateurs de Media Portal voient les paramètres de style que vous choisissez, ils doivent ajouter `?company=(company name)` à l’URL avec laquelle ils accèdent au portail multimédia. Par exemple, pour afficher les paramètres de style, les utilisateurs du portail multimédia qui accèdent à la société PortalCo à l’adresse suivante :

`https://s7sps1.scene7.com/MediaPortal`

Utilisez plutôt l’URL suivante :

`https://s7sps1.scene7.com/MediaPortal?company=PortalCo`

L’inclusion du nom de l’entreprise dans l’URL permet à Media Portal de reconnaître la société à laquelle un utilisateur souhaite accéder et d’appliquer les paramètres de style de l’entreprise en conséquence.

Vous pouvez en savoir plus sur la communication des changements d’URL aux utilisateurs du portail multimédia, et sur la définition d’un message de l’e-mail de bienvenue pour que les nouveaux utilisateurs reçoivent l’URL de portail multimédia correcte.

Voir [Définition du message de l’e-mail de bienvenue pour les utilisateurs du portail multimédia](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users).
