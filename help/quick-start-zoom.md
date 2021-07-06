---
title: '"Démarrage rapide : Zoom"'
description: Introduction et démarrage rapide pour zoomer pour vous aider à démarrer rapidement.
uuid: 31eda632-3469-4f90-885b-e90c6a2e5e75
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: 559c986d-313d-46df-a5ff-0b49316ad3a7
feature: Dynamic Media Classic,Visionneuses,Zoom
role: User
exl-id: eae35207-000c-4ced-b9ab-714c2384a9e7
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 41%

---

# Démarrage rapide : Zoom{#quick-start-zoom}

Zoom permet d’afficher de manière interactive les détails haute résolution des images. Vous pouvez, par exemple, voir les couleurs, les options, les angles et les détails d’une image dans une visionneuse intégrée, entièrement configurable et dynamique. Cette visionneuse peut être incorporée à une page Web ou s’afficher dans une fenêtre contextuelle. Vous pouvez contrôler les images à distance et effectuer un panoramique à haute résolution afin de les examiner de plus près. La fonction de zoom permet à vos clients de bénéficier d’une expérience de visualisation plus interactive, instructive et dynamique. 

Dynamic Media Classic propose également un zoom guidé, qui permet de mettre en évidence les fonctionnalités importantes d’une image. Vous pouvez par exemple créer une cible de zoom pour un logo afin d’attirer l’attention des utilisateurs sur ce dernier. Lorsque les utilisateurs cliquent sur cette cible de zoom, ils effectuent un zoom sur le logo.

Toutes les images de zoom sont créées et servies à partir d’images originales uniques, de graphiques et d’attributs gérés par des bases de données. Le zoom de Dynamic Media Classic réduit considérablement le temps et les coûts de production et de diffusion des images. Vous pouvez utiliser les visionneuses de zoom pour effectuer un zoom avant ou arrière sur les images. La visionneuse de zoom comporte des boutons sur lesquels il suffit de cliquer pour effectuer un zoom et un panoramique ; à cela s’ajoute la possibilité d’effectuer un panoramique par glissement sur l’écran. Des paramètres prédéfinis de visionneuse de zoom permettent de configurer la visionneuse utilisée pour effectuer un zoom sur les images.

Ce didacticiel de mise en route Zoom est conçu pour être opérationnel rapidement avec les techniques de zoom de Dynamic Media Classic. Suivez les étapes 1 à 6. Chaque étape se termine par un renvoi à une rubrique contenant de plus amples informations.

## 1. Chargement des images de zoom

Commencez par télécharger vos images de zoom vers Dynamic Media Classic. Pour un zoom optimal, Dynamic Media Classic recommande que la taille des images soit d’au moins 2 000 pixels.

Dans la barre de navigation globale, cliquez sur **[!UICONTROL Télécharger]** pour télécharger des images de votre ordinateur ou réseau vers un dossier de Dynamic Media Classic. (voir [Téléchargement des images de zoom](uploading-zoom-images.md#uploading_zoom_images)).

## 2. Création de cibles de zoom pour un zoom guidé

Les cibles de zoom vous permettent de mettre en valeur des sections particulières d’une image. Vous pouvez, par exemple, attirer l’attention des utilisateurs sur les sections d’une image qui la caractérisent ou la distinguent. Les cibles de zoom s’affichent sous la forme de miniatures, à côté de l’image, dans la fenêtre de la visionneuse de zoom. La sélection d’une de ces miniatures de cible de zoom permet d’effectuer un zoom automatique sur la section de l’image que vous définissez.

Pour créer une cible de zoom, cliquez sur **[!UICONTROL Modifier]** et sélectionnez Cibles de zoom ou ouvrez une image dans le panneau Parcourir en mode Détails, puis cliquez sur **[!UICONTROL Cibles de zoom]**. Utilisez ensuite les outils de zoom de la page Éditeur de cible de zoom pour isoler une partie de l’image en tant que cible. (voir [Création de cibles de zoom pour un zoom guidé](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom)).

## 3. Configuration des paramètres prédéfinis de la visionneuse de zoom

Les paramètres prédéfinis de visionneuse de zoom déterminent le style et le comportement des visionneuses de zoom. Vous pouvez configurer des paramètres prédéfinis de visionneuse de zoom en tant qu’administrateur. Dynamic Media Classic est fourni avec les paramètres prédéfinis de visionneuse de zoom par défaut.

Pour créer un paramètre prédéfini de visionneuse de zoom, dans la barre de navigation globale, cliquez sur **[!UICONTROL Configuration]** > **[!UICONTROL Paramètres prédéfinis de la visionneuse]**. Sur la page Paramètres prédéfinis de la visionneuse, cliquez sur **[!UICONTROL Ajouter]**, choisissez une plateforme et une visionneuse de zoom, puis cliquez sur **[!UICONTROL Ajouter]**. Sélectionnez ensuite les options de la page Configurer la visionneuse .

Dynamic Media Classic propose des options **[!UICONTROL Paramètre prédéfini de la visionneuse de zoom]** qui vous permettent de sélectionner le style du bouton et l’aspect global de la visionneuse. Vous avez également la possibilité de personnaliser les paramètres de zoom pour votre site Web (voir [Configuration des paramètres prédéfinis de la visionneuse de zoom](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets)).

## 4. Aperçu des images à l’aide de la visionneuse de zoom

Vous pouvez prévisualiser des images dans une visionneuse de zoom afin de vérifier le résultat obtenu lorsque vous effectuez un zoom sur les images.

Pour explorer les différents paramètres prédéfinis de la visionneuse de zoom et la manière dont ils présentent l’expérience de zoom, sélectionnez une image dans le panneau de navigation, puis cliquez sur **[!UICONTROL Aperçu]**. Cliquez sur **[!UICONTROL Paramètres prédéfinis]** > **[!UICONTROL Zoom]**, puis sélectionnez un paramètre prédéfini avec les menus Zoom .

Les boutons de zoom apparaissent. Vous pouvez alors vérifier l’aspect des images de zoom sur votre site Web. Cliquez sur les boutons de zoom (et les cibles de zoom) pour tester les paramètres du paramètre prédéfini de la visionneuse de zoom que vous avez choisi. (voir [Prévisualisation d’images avec différentes visionneuses de zoom](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers)).

## 5. Publication des images de zoom

Lorsque vous publiez vos images de zoom, elles sont placées sur les serveurs d’images Dynamic Media afin qu’elles puissent être diffusées sur votre site web et dans votre application. Dans le cadre du processus de publication, Dynamic Media Classic active les chaînes URL. Ces chaînes URL appellent des images de zoom des serveurs d’images Dynamic Media vers votre site web ou votre application.

Sur la barre de navigation générale, cliquez sur **[!UICONTROL Publier]**, Dans la boîte de dialogue Publier, cliquez sur **[!UICONTROL Envoyer la publication]**. (voir [Publication des images de zoom](publishing-zoom-images.md#publishing_zoom_images)).

## 6. Liaison de visionneuses de zoom à une page web

Dynamic Media Classic crée les chaînes d’légende URL nécessaires pour zoomer sur les images et les active lorsque vous publiez des images sur les serveurs d’images Dynamic Media. Vous pouvez copier ces chaînes URL à partir de la page **[!UICONTROL Aperçu]**. Une fois copiées, les chaînes URL peuvent être utilisées dans vos applications et sur vos sites Web (voir [Liaison des visionneuses de zoom à une page Web](linking-zoom-viewers-web-pages.md#linking_zoom_viewers_to_your_web_pages)).
