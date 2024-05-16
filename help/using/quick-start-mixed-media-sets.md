---
title: "Démarrage rapide : visionneuse de médias mixtes"
description: Présentation et démarrage rapide des visionneuses de médias mixtes pour vous aider à démarrer rapidement dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/mixed_media_sets
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: 757893ae-7507-42a0-a67b-f6542e7231c7
topic: Content Management
level: Beginner
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 16%

---

# Démarrage rapide : Visionneuses de supports variés{#quick-start-mixed-media-sets}

Les visionneuses de médias mixtes offrent aux utilisateurs une expérience de visionnage intégrée. Les visionneuses de supports variés peuvent contenir des images, des visionneuses d’images, des séries d’échantillons, des visionneuses à 360° et des vidéos. Les utilisateurs peuvent sélectionner différents onglets dans la visionneuse de supports variés pour afficher les éléments dans les différentes visionneuses. Si aucun onglet n’est sélectionné, tous les fichiers s’affichent dans la ligne d’échantillons.

Les paramètres prédéfinis de visionneuse de médias mixtes incluent des options de communauté permettant aux utilisateurs finaux d’incorporer du code, de copier des URL et de créer un lien vers le site web principal. Les utilisateurs peuvent utiliser ces options pour partager des informations sur les produits sur leurs sites Web personnels ou sur les réseaux sociaux.

Ce didacticiel de supports variés est conçu pour vous aider à maîtriser rapidement les techniques de visionneuse de supports variés dans Adobe Dynamic Media Classic.

## 1. Chargement des images, des fichiers d’échantillon et des vidéos

Commencez par télécharger les images, fichiers d’échantillons et vidéos pour les visionneuses de supports variés. Comme les utilisateurs peuvent zoomer sur les images dans la visionneuse de médias mixtes, veillez à tenir compte de cette fonctionnalité lors du choix des images. Assurez-vous que la taille des images est d’au moins 2 000 pixels.

Dans la barre de navigation globale, sélectionnez **[!UICONTROL Télécharger]** pour charger des fichiers depuis votre ordinateur vers un dossier sur Adobe Dynamic Media Classic.

Voir [Chargement des fichiers](uploading-files.md#uploading-your-files).

## 2. Créez une visionneuse de médias à utiliser dans la visionneuse de médias mixtes.

Vous pouvez ajouter des images, des visionneuses d’images, des séries d’échantillons, des visionneuses à 360° et des vidéos à votre visionneuse de médias mixtes. Préparez les visionneuses de médias avant de les ajouter à la visionneuse de médias mixtes.

Voir [Création d’une visionneuse d’images](creating-image-set.md#creating-an-image-set), [Création d’une série d’échantillons](creating-swatch-set.md#creating-a-swatch-set), et [Création d’une visionneuse à 360°](creating-spin-set.md#creating-a-spin-set).

## 3. Création d’une visionneuse de médias mixtes

Dans la barre de navigation globale, accédez à **[!UICONTROL Build]** > **[!UICONTROL Visionneuses de médias mixtes]**. Faites glisser les images, les séries d’échantillons, les visionneuses d’images et les vidéos sur la page Visionneuse de supports variés. Pour ajouter une bande sonore, faites glisser un fichier audio sur la zone Bande sonore.

Voir [Création d’une visionneuse de médias mixtes](creating-mixed-media-set.md#creating-a-mixed-media-set).

## 4. Configuration des paramètres prédéfinis de la visionneuse de médias mixtes

Adobe Dynamic Media Classic est fourni avec des paramètres prédéfinis de visionneuse par défaut pour les visionneuses de médias mixtes. Les administrateurs peuvent créer ou modifier des paramètres prédéfinis de visionneuse de médias mixtes.

Lors de la configuration d’un paramètre prédéfini de visionneuse de médias mixtes, ajoutez les paramètres prédéfinis de visionneuse pour toutes les autres ressources de votre visionneuse. Par exemple, si votre visionneuse de médias mixtes contient des vidéos, ajoutez un paramètre prédéfini de visionneuse de vidéos au paramètre prédéfini de visionneuse de médias mixtes. Vous pouvez également ajouter une bande sonore à la visionneuse. Cette bande sonore est lue lorsque la visionneuse est ouverte mais pas lorsqu’une vidéo est active.

Voir [Configuration d’un paramètre prédéfini de visionneuse de médias mixtes](setting-mixed-media-set-viewer.md#setting-up-a-mixed-media-set-viewer-preset) et [Création et modification de paramètres prédéfinis de visionneuse](application-setup.md#adding-and-editing-viewer-presets).

Voir aussi [Paramètres prédéfinis de la visionneuse](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) vidéo de formation.

## 5. Aperçu d’une visionneuse de médias mixtes

Sélectionnez la visionneuse de supports variés **[!UICONTROL Aperçu]** bouton . Vous pouvez sélectionner les icônes de miniature et d’échantillon pour examiner votre visionneuse de médias mixtes dans la visionneuse de médias mixtes. Différentes visionneuses sont disponibles dans les menus Paramètres prédéfinis.

Voir [Aperçu d’une ressource](previewing-asset.md#previewing-an-asset).

## 6. Publication d’une visionneuse de médias mixtes

La publication d’une visionneuse de médias mixtes la place sur les serveurs Adobe Dynamic Media Classic et active la chaîne URL.

Avec les visionneuses de supports variés, vous devez publier sur un **serveur de vidéo** et un **serveur d’images**. Utilisation **Serveur vidéo** pour publier les vidéos réelles que vous avez marquées pour publication. Et vous utilisez **Serveur d’images** pour publier des ressources connexes, telles que des miniatures vidéo, et définir des informations pour toute visionneuse de vidéos adaptative.

Voir [Publication d’une visionneuse de médias mixtes](publishing-mixed-media-set.md#publishing-a-mixed-media-set).

## 7. Liaison d’une visionneuse de médias mixtes à une page web

Adobe Dynamic Media Classic active les appels URL pour les visionneuses de médias mixtes une fois que vous les avez publiées. Vous pouvez copier ces URL à partir de la page Aperçu .

Sélectionnez la visionneuse de médias mixtes, puis sélectionnez **[!UICONTROL Aperçu]**. Dans la page Aperçu, sélectionnez un paramètre prédéfini de visionneuse de médias mixtes, puis sélectionnez le paramètre **[!UICONTROL Copier l’URL]**. Voir [Lier des visionneuses de médias mixtes à des pages Web](linking-mixed-media-set-web.md#linking-a-mixed-media-set-to-a-web-page).
