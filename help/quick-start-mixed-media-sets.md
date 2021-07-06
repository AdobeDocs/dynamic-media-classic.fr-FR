---
title: '"Démarrage rapide : Visionneuse de médias mixtes"'
description: Présentation et démarrage rapide des visionneuses de médias mixtes pour vous aider à démarrer rapidement.
uuid: 0ef033d5-b053-4d7c-b1e1-1980f899fd88
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/mixed_media_sets
discoiquuid: 2708d077-94fc-4045-8992-ad3589ed9cfd
feature: Dynamic Media Classic,Visionneuses,Combiner une visionneuse de médias
role: User
exl-id: 757893ae-7507-42a0-a67b-f6542e7231c7
source-git-commit: f99832bc9660a16b06e63b19f9ead1267dab0f35
workflow-type: tm+mt
source-wordcount: '637'
ht-degree: 52%

---

# Démarrage rapide : Visionneuses de supports variés{#quick-start-mixed-media-sets}

Les visionneuses de supports variés offrent aux utilisateurs une expérience de visualisation intégrée. Les visionneuses de supports variés peuvent contenir des images, des visionneuses d’images, des séries d’échantillons, des visionneuses à 360° et des vidéos. Les utilisateurs peuvent cliquer sur divers onglets de la visionneuse de supports variés pour visualiser les objets des différentes visionneuses. Si aucun onglet n’est sélectionné, tous les fichiers s’affichent dans la ligne d’échantillons.

Les paramètres prédéfinis de visionneuse de supports variés incluent des options de la communauté permettant aux utilisateurs finals d’incorporer du code, de copier des URL et de créer des liens vers le site Web principal. Les utilisateurs peuvent utiliser ces options pour partager des informations de produits sur leur site Web personnel ou sur des sites de réseaux sociaux.

Cette section de démarrage rapide des visionneuses de médias mixtes est conçue pour vous aider à maîtriser rapidement les techniques de visionneuse de médias mixtes dans Dynamic Media Classic.

## 1. Téléchargement des images, des fichiers d’échantillon et des vidéos

Commencez par télécharger les images, fichiers d’échantillons et vidéos pour les visionneuses de supports variés. Comme les utilisateurs peuvent zoomer sur les images dans la visionneuse de médias mixtes, veillez à tenir compte de cette fonctionnalité lors du choix des images. Assurez-vous que la taille des images est d’au moins 2 000 pixels.

Dans la barre de navigation globale, cliquez sur **[!UICONTROL Télécharger]** pour charger des fichiers depuis votre ordinateur vers un dossier de Dynamic Media Classic.

(voir [Téléchargement de fichiers](uploading-files.md#uploading-your-files)).

## 2. Création de visionneuses de médias à utiliser dans la visionneuse de médias mixtes

Vous pouvez ajouter des images, des visionneuses d’images, des séries d’échantillons, des visionneuses à 360° et des vidéos à votre visionneuse de supports variés. Préparez les visionneuses de supports avant de les ajouter à la visionneuse de supports variés.

Voir les sections [Création d’une visionneuse d’images](creating-image-set.md#creating-an-image-set), [Création d’une série d’échantillons](creating-swatch-set.md#creating-a-swatch-set) et [Création d’une visionneuse à 360°](creating-spin-set.md#creating-a-spin-set).

## 3. Création d’une visionneuse de médias mixtes

Dans la barre de navigation globale, cliquez sur **[!UICONTROL Créer]** > **[!UICONTROL Visionneuses de médias mixtes]**. Faites glisser les images, les séries d’échantillons, les visionneuses d’images et les vidéos sur la page Visionneuse de supports variés. Pour ajouter une bande sonore, faites glisser un fichier audio sur la zone Bande sonore.

Reportez-vous à la section [Création d’une visionneuse de supports variés](creating-mixed-media-set.md#creating-a-mixed-media-set).

## 4. Configuration des paramètres prédéfinis de la visionneuse de supports variés

Dynamic Media Classic est fourni avec des paramètres prédéfinis de visionneuse par défaut pour les visionneuses de médias mixtes. Les administrateurs peuvent créer ou modifier ces paramètres prédéfinis.

Lors de la configuration d’un paramètre prédéfini de visionneuse de médias mixtes, ajoutez les paramètres prédéfinis de visionneuse pour toutes les autres ressources de votre visionneuse. Par exemple, si votre visionneuse de supports variés contient des vidéos, ajoutez un paramètre prédéfini de visionneuse de vidéos à celui de la visionneuse de supports variés. Vous pouvez également ajouter une bande sonore à la visionneuse. Cette bande sonore est lue lorsque la visionneuse est ouverte mais pas lorsqu’une vidéo est active.

Reportez-vous aux sections [Configuration d’un paramètre prédéfini de visionneuse de supports variés](setting-mixed-media-set-viewer.md#setting-up-a-mixed-media-set-viewer-preset) et [Création et modification de paramètres prédéfinis de la visionneuse](application-setup.md#adding-and-editing-viewer-presets).

## 5. Aperçu d’une visionneuse de médias mixtes

Cliquez sur le bouton **[!UICONTROL Aperçu]** de la visionneuse de médias mixtes. Vous pouvez cliquer sur les icônes de miniature et d’échantillon pour examiner votre visionneuse de supports variés. Différentes visionneuses sont disponibles dans les menus Paramètres prédéfinis.

Voir [Prévisualisation d’un fichier](previewing-asset.md#previewing-an-asset)

## 6. Publication d’une visionneuse de médias mixtes

La publication d’une visionneuse de médias mixtes la place sur les serveurs Dynamic Media Classic et active la chaîne URL.

Avec les visionneuses de supports variés, vous devez publier sur un **serveur de vidéo** et un **serveur d’images**. Utilisez le **serveur de vidéo** pour publier les vidéos réelles que vous avez marquées pour publication De plus, vous utilisez **Image Server** pour publier des ressources connexes, telles que les miniatures vidéo, et définir des informations pour toute visionneuse de vidéos adaptative.

Reportez-vous à la section [Publication d’une visionneuse de supports variés](publishing-mixed-media-set.md#publishing-a-mixed-media-set).

## 7. Liaison d’une visionneuse de médias mixtes à une page web

Dynamic Media Classic active les appels URL pour les visionneuses de médias mixtes une fois que vous les avez publiées. Vous pouvez copier ces URL à partir de la page Aperçu .

Sélectionnez la visionneuse de médias mixtes, puis cliquez sur **[!UICONTROL Aperçu]**. Dans la page Aperçu, sélectionnez un paramètre prédéfini de visionneuse de médias mixtes, puis cliquez sur **[!UICONTROL Copier l’URL]**. (voir [Liaison d’une visionneuse de supports variés à une page Web](linking-mixed-media-set-web.md#linking-a-mixed-media-set-to-a-web-page)).
