---
title: 'Démarrage rapide : visionneuse de médias mixtes'
description: Une introduction et un démarrage rapide pour les visionneuses de médias mixtes afin de vous aider à démarrer rapidement dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/mixed_media_sets
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: 757893ae-7507-42a0-a67b-f6542e7231c7
topic: Content Management
level: Beginner
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 16%

---

# Démarrage rapide : Visionneuses de supports variés{#quick-start-mixed-media-sets}

Les visionneuses de médias mixtes offrent aux utilisateurs une expérience de visionnage intégrée. Les visionneuses de supports variés peuvent contenir des images, des visionneuses d’images, des séries d’échantillons, des visionneuses à 360° et des vidéos. Les utilisateurs peuvent sélectionner différents onglets dans la visionneuse de médias mixtes pour afficher les éléments dans les différentes visionneuses. Si aucun onglet n’est sélectionné, tous les fichiers s’affichent dans la ligne d’échantillons.

Les paramètres prédéfinis de visionneuse de médias mixtes incluent des options de communauté permettant aux utilisateurs finaux d’incorporer du code, de copier des URL et d’établir un lien vers le site web principal. Les utilisateurs peuvent utiliser ces options pour partager des informations sur les produits sur leurs sites web personnels ou leurs sites de réseaux sociaux.

Ce démarrage rapide d’une visionneuse de médias mixtes est conçu pour vous aider à maîtriser rapidement les techniques des visionneuses de médias mixtes dans Adobe Dynamic Media Classic.

## &#x200B;1. Chargez les images, les fichiers d’échantillon et les vidéos

Commencez par télécharger les images, fichiers d’échantillons et vidéos pour les visionneuses de supports variés. Comme les utilisateurs peuvent zoomer sur les images dans la visionneuse de médias mixtes, veillez à tenir compte de cette fonctionnalité lors du choix des images. Assurez-vous que les images font au moins 2 000 pixels dans leur plus grande taille.

Sur la barre de navigation générale, sélectionnez **[!UICONTROL Télécharger]** pour télécharger des fichiers depuis votre ordinateur vers un dossier d’Adobe Dynamic Media Classic.

Voir [Charger vos fichiers](uploading-files.md#uploading-your-files).

## &#x200B;2. Création d’une visionneuse de médias à utiliser dans la visionneuse de médias mixtes

Vous pouvez ajouter des images, des visionneuses d’images, des visionneuses d’échantillons, à 360° et des vidéos à votre visionneuse de médias mixtes. Préparez les visionneuses de médias avant de les ajouter à la visionneuse de médias mixtes.

Voir [Création d’une visionneuse d’images](creating-image-set.md#creating-an-image-set), [Création d’une visionneuse d’échantillons](creating-swatch-set.md#creating-a-swatch-set) et [Création d’une visionneuse à 360°](creating-spin-set.md#creating-a-spin-set).

## &#x200B;3. Création d’une visionneuse de médias mixtes

Sur la barre de navigation générale, accédez à **[!UICONTROL Créer]** > **[!UICONTROL Visionneuses de médias mixtes]**. Faites glisser les images, les visionneuses d’échantillons, les visionneuses d’images et les vidéos vers la page Visionneuse de médias mixtes. Pour ajouter une bande sonore, faites glisser un fichier audio sur la zone Bande sonore.

Voir [&#x200B; Création d’une visionneuse de médias mixtes &#x200B;](creating-mixed-media-set.md#creating-a-mixed-media-set).

## &#x200B;4. Configuration des paramètres prédéfinis de visionneuse de médias mixtes

Adobe Dynamic Media Classic est fourni avec les paramètres prédéfinis de visionneuse par défaut pour les visionneuses de médias mixtes. L’administration peut créer ou modifier des paramètres prédéfinis de visionneuse de médias mixtes.

Lors de la configuration d’un paramètre prédéfini de visionneuse de médias mixtes, ajoutez les paramètres prédéfinis de visionneuse pour toutes les autres ressources de votre visionneuse. Par exemple, si votre visionneuse de médias mixtes comprend des vidéos, ajoutez un paramètre prédéfini de visionneuse de vidéos à celui-ci. Vous pouvez également ajouter une bande sonore à la visionneuse. Cette bande sonore est lue lorsque la visionneuse est ouverte mais pas lorsqu’une vidéo est active.

Voir [Configuration d’un paramètre prédéfini de visionneuse de médias mixtes](setting-mixed-media-set-viewer.md#setting-up-a-mixed-media-set-viewer-preset) et [Création et modification de paramètres prédéfinis de visionneuse](application-setup.md#adding-and-editing-viewer-presets).

Voir aussi [Paramètres prédéfinis de la visionneuse](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) vidéo de formation.

## &#x200B;5. Prévisualisation d’une visionneuse de médias mixtes

Sélectionnez le bouton **[!UICONTROL Aperçu]** de la visionneuse de médias mixtes. Vous pouvez sélectionner les icônes de miniature et d’échantillon pour examiner votre visionneuse de médias mixtes dans la visionneuse de médias mixtes. Différentes visionneuses sont disponibles dans les menus Paramètres prédéfinis.

Voir [Aperçu d’une ressource](previewing-asset.md#previewing-an-asset).

## &#x200B;6. Publication d’une visionneuse de médias mixtes

La publication d’une visionneuse de médias mixtes la place sur les serveurs Adobe Dynamic Media Classic et active la chaîne URL.

Avec les visionneuses de supports variés, vous devez publier sur un **serveur de vidéo** et un **serveur d’images**. Utilisez **Serveur vidéo** pour publier les vidéos que vous avez marquées pour publication. De plus, vous utilisez **Image Server** pour publier les ressources connexes, telles que les miniatures vidéo, et définir des informations pour toute visionneuse de vidéos adaptative.

Voir [&#x200B; Publication d’une visionneuse de médias mixtes &#x200B;](publishing-mixed-media-set.md#publishing-a-mixed-media-set).

## &#x200B;7. Liaison d’une visionneuse de médias mixtes à une page web

Adobe Dynamic Media Classic active les appels d’URL pour les visionneuses de médias mixtes après leur publication. Vous pouvez copier ces URL à partir de la page Aperçu .

Sélectionnez la visionneuse de médias mixtes, puis sélectionnez **[!UICONTROL Aperçu]**. Dans la page Aperçu, sélectionnez un paramètre prédéfini de visionneuse de médias mixtes, puis sélectionnez l’**[!UICONTROL URL de copie]**. Voir [Liaison de visionneuses de médias mixtes à des pages web](linking-mixed-media-set-web.md#linking-a-mixed-media-set-to-a-web-page).
