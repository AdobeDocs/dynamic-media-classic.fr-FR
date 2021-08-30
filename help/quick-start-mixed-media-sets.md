---
title: '"Démarrage rapide : Visionneuse de médias mixtes"'
description: Présentation et démarrage rapide des visionneuses de médias mixtes pour vous aider à démarrer rapidement dans Adobe Dynamic Media Classic.
uuid: 0ef033d5-b053-4d7c-b1e1-1980f899fd88
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/mixed_media_sets
discoiquuid: 2708d077-94fc-4045-8992-ad3589ed9cfd
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: 757893ae-7507-42a0-a67b-f6542e7231c7
source-git-commit: 36f9aa3c2b4dc66e4cb851c2ce6837ae0ad4f64c
workflow-type: tm+mt
source-wordcount: '641'
ht-degree: 38%

---

# Démarrage rapide : Visionneuses de supports variés{#quick-start-mixed-media-sets}

Les visionneuses de supports variés offrent aux utilisateurs une expérience de visualisation intégrée. Les visionneuses de supports variés peuvent contenir des images, des visionneuses d’images, des séries d’échantillons, des visionneuses à 360° et des vidéos. Les utilisateurs peuvent sélectionner différents onglets dans la visionneuse de supports variés pour afficher les éléments dans les différentes visionneuses. Si aucun onglet n’est sélectionné, tous les fichiers s’affichent dans la ligne d’échantillons.

Les paramètres prédéfinis de visionneuse de supports variés incluent des options de la communauté permettant aux utilisateurs finals d’incorporer du code, de copier des URL et de créer des liens vers le site Web principal. Les utilisateurs peuvent utiliser ces options pour partager des informations de produits sur leur site Web personnel ou sur des sites de réseaux sociaux.

Cette section de démarrage rapide des visionneuses de médias mixtes est conçue pour vous aider à maîtriser rapidement les techniques de visionneuse de médias mixtes dans Adobe Dynamic Media Classic.

## 1. Chargement des images, des fichiers d’échantillon et des vidéos

Commencez par télécharger les images, fichiers d’échantillons et vidéos pour les visionneuses de supports variés. Comme les utilisateurs peuvent zoomer sur les images dans la visionneuse de médias mixtes, veillez à tenir compte de cette fonctionnalité lors du choix des images. Assurez-vous que la taille des images est d’au moins 2 000 pixels.

Dans la barre de navigation globale, sélectionnez **[!UICONTROL Télécharger]** pour charger des fichiers depuis votre ordinateur vers un dossier sur Adobe Dynamic Media Classic.

Voir [Télécharger vos fichiers](uploading-files.md#uploading-your-files).

## 2. Création de visionneuses de médias à utiliser dans la visionneuse de médias mixtes

Vous pouvez ajouter des images, des visionneuses d’images, des séries d’échantillons, des visionneuses à 360° et des vidéos à votre visionneuse de supports variés. Préparez les visionneuses de supports avant de les ajouter à la visionneuse de supports variés.

Voir [Création d’une visionneuse d’images](creating-image-set.md#creating-an-image-set), [Création d’une série d’échantillons](creating-swatch-set.md#creating-a-swatch-set) et [Création d’une visionneuse à 360°](creating-spin-set.md#creating-a-spin-set).

## 3. Création d’une visionneuse de médias mixtes

Dans la barre de navigation globale, accédez à **[!UICONTROL Créer]** > **[!UICONTROL Visionneuses de médias mixtes]**. Faites glisser les images, les séries d’échantillons, les visionneuses d’images et les vidéos sur la page Visionneuse de supports variés. Pour ajouter une bande sonore, faites glisser un fichier audio sur la zone Bande sonore.

Voir [Création d’une visionneuse de médias mixtes](creating-mixed-media-set.md#creating-a-mixed-media-set).

## 4. Configuration des paramètres prédéfinis de la visionneuse de supports variés

Adobe Dynamic Media Classic est fourni avec des paramètres prédéfinis de visionneuse par défaut pour les visionneuses de médias mixtes. Les administrateurs peuvent créer ou modifier ces paramètres prédéfinis.

Lors de la configuration d’un paramètre prédéfini de visionneuse de médias mixtes, ajoutez les paramètres prédéfinis de visionneuse pour toutes les autres ressources de votre visionneuse. Par exemple, si votre visionneuse de supports variés contient des vidéos, ajoutez un paramètre prédéfini de visionneuse de vidéos à celui de la visionneuse de supports variés. Vous pouvez également ajouter une bande sonore à la visionneuse. Cette bande sonore est lue lorsque la visionneuse est ouverte mais pas lorsqu’une vidéo est active.

Voir [Configuration d’un paramètre prédéfini de visionneuse de médias mixtes](setting-mixed-media-set-viewer.md#setting-up-a-mixed-media-set-viewer-preset) et [Création et modification de paramètres prédéfinis de visionneuse](application-setup.md#adding-and-editing-viewer-presets).

## 5. Aperçu d’une visionneuse de médias mixtes

Sélectionnez le bouton **[!UICONTROL Aperçu]** de la visionneuse de médias mixtes. Vous pouvez sélectionner les icônes de miniature et d’échantillon pour examiner votre visionneuse de médias mixtes dans la visionneuse de médias mixtes. Différentes visionneuses sont disponibles dans les menus Paramètres prédéfinis.

Voir [Aperçu d’une ressource](previewing-asset.md#previewing-an-asset).

## 6. Publication d’une visionneuse de médias mixtes

La publication d’une visionneuse de médias mixtes la place sur les serveurs Dynamic Media Classic Adobe et active la chaîne URL.

Avec les visionneuses de supports variés, vous devez publier sur un **serveur de vidéo** et un **serveur d’images**. Utilisez le **serveur de vidéo** pour publier les vidéos réelles que vous avez marquées pour publication De plus, vous utilisez **Image Server** pour publier des ressources connexes, telles que les miniatures vidéo, et définir des informations pour toute visionneuse de vidéos adaptative.

Voir [Publication d’une visionneuse de médias mixtes](publishing-mixed-media-set.md#publishing-a-mixed-media-set).

## 7. Liaison d’une visionneuse de médias mixtes à une page web

Adobe Dynamic Media Classic active les appels URL pour les visionneuses de médias mixtes une fois que vous les avez publiées. Vous pouvez copier ces URL à partir de la page Aperçu .

Sélectionnez la visionneuse de médias mixtes, puis sélectionnez **[!UICONTROL Aperçu]**. Dans la page Aperçu, sélectionnez un paramètre prédéfini de visionneuse de médias mixtes, puis sélectionnez **[!UICONTROL Copier l’URL]**. (voir [Liaison d’une visionneuse de supports variés à une page Web](linking-mixed-media-set-web.md#linking-a-mixed-media-set-to-a-web-page)).
