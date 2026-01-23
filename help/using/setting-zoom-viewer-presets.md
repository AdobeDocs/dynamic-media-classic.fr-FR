---
title: Configurer les paramètres prédéfinis de la visionneuse Zoom
description: Découvrez comment configurer les paramètres prédéfinis de visionneuse Zoom dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: ddaaff6c-5447-408e-9c92-bcdfd1a0e72e
topic: Content Management
level: Intermediate
source-git-commit: c4613c78347c4bda3d84747a72146617158c03b6
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 40%

---

# Configurer les paramètres prédéfinis de la visionneuse Zoom{#setting-up-zoom-viewer-presets}

Les paramètres prédéfinis de la visionneuse Zoom déterminent le style, le comportement et l’aspect de vos visionneuses Zoom. Adobe Dynamic Media Classic offre de nombreuses options pour personnaliser et appliquer l’habillage aux visionneuses. Adobe Dynamic Media Classic est fourni avec les paramètres prédéfinis de base par défaut (rapide), de fenêtre déroulante et de visionneuse Zoom personnalisée. Si vous êtes administrateur, vous pouvez créer des paramètres prédéfinis de visionneuse Zoom d’entreprise ou modifier un paramètre prédéfini par défaut et l’enregistrer sous un nouveau nom.

Toutes les visionneuses de zoom comportent des boutons permettant d’effectuer un zoom avant, un zoom arrière et un panoramique mais aussi de rétablir l’état initial de l’image après le zoom. L’apparence de ces boutons et de la fenêtre elle-même dépend de votre choix de Paramètres prédéfinis de la visionneuse Zoom. Vous pouvez configurer un paramètre prédéfini de visionneuse de zoom avec des couleurs, des bordures, des polices et des paramètres d’image différents. Lors de la configuration d’une visionneuse avec zoom guidé, vous pouvez également choisir l’emplacement des cibles de zoom. Les cibles de zoom correspondent aux miniatures sur lesquelles les utilisateurs cliquent pour effectuer un zoom sur les zones que vous définissez.

## A propos des paramètres prédéfinis de la visionneuse de zoom {#about-zoom-viewer-presets}

Adobe Dynamic Media Classic propose les paramètres prédéfinis de visionneuse Zoom suivants :

* **Visionneuse Zoom : de base** : fournit un zoom de base sur l’image d’origine.

* **Visionneuse Zoom : Fenêtre déroulante** : affiche une seconde image de la zone zoomée en regard de l’image d’origine. Aucune commande n’est disponible. Il suffit de déplacer la sélection sur la zone à visualiser.

Pour déterminer la quantité totale de bande passante allouée à la visionneuse, n’oubliez pas que l’image principale et celle de la fenêtre déroulante sont toutes deux diffusées par la visionneuse. La taille de l’image déroulante est déterminée à l’aide de la taille de l’image principale (largeur et hauteur de la scène) et du facteur de zoom. Pour que la fenêtre déroulante ne devienne pas trop volumineuse, équilibrez ces deux valeurs : si la taille de l’image principale est importante, réduisez la valeur du facteur de zoom. (La Largeur de la fenêtre déroulante et la Hauteur de la fenêtre déroulante déterminent la taille de la fenêtre déroulante, mais pas la taille de l’image diffusée par la visionneuse.)

Par exemple, si la taille de l’image principale est de 350 x 350 pixels et que le facteur de zoom est de 3, la taille d’image de la fenêtre déroulante sera de 1 050 x 1 050 pixels. Si la taille de l’image principale est de 300 x 300 pixels et que le facteur de zoom est de 4, la taille d’image de la fenêtre déroulante sera de 1 200 x 1 200 pixels. Selon la valeur de qualité JPEG sélectionnée (une valeur comprise entre 80 et 90 est recommandée), il est possible de réduire sensiblement la taille du fichier. Selon la taille de l’image principale, un facteur de zoom de 2,5 à 4 est recommandé.

Adobe Dynamic Media Classic recommande les paramètres suivants pour les paramètres prédéfinis de visionneuse Zoom volant :

* **Taille de l’image agrandie** : environ 1 500 x 1 500 pixels, sans dépasser 2 000 x 2 000 pixels.

* **Taille de l’image** : 100 Ko ou moins, ne pas dépasser 150 Ko (compressez le fichier pour le conserver en dessous de 150 Ko).

* **Visionneuse Zoom : personnalisée** : permet un zoom guidé ou non avec des images, des visionneuses d’images avec plusieurs vues ou des visionneuses d’échantillons de couleurs.

## Création et modification des paramètres prédéfinis de la visionneuse Zoom {#creating-and-editing-zoom-viewer-presets}

1. Sur la barre de navigation générale, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Paramètres prédéfinis de la visionneuse]**.
1. Effectuez l’une des opérations suivantes :

   * **Créer un paramètre prédéfini** : sélectionnez **[!UICONTROL Ajouter]**. Dans la boîte de dialogue Ajouter un paramètre prédéfini de visionneuse, sélectionnez une plateforme, une visionneuse Zoom, puis sélectionnez **[!UICONTROL Ajouter]**. Saisissez le nom du paramètre prédéfini dans la zone Nom du paramètre prédéfini .

   * **Modification d’un paramètre prédéfini** : sélectionnez un paramètre prédéfini de visionneuse pour zoom, puis sélectionnez **[!UICONTROL Modifier]**.

1. Spécifiez les paramètres de votre choix.

   Pour afficher la description d’une option, sélectionnez l’icône **[!UICONTROL Info-bulle]** à côté de l’option.

   La page Aperçu affiche la visionneuse lorsque vous mettez à jour et modifiez des paramètres.

1. Sélectionnez **[!UICONTROL Enregistrer]** ou **[!UICONTROL Enregistrer sous]**.
1. Sur la page Paramètres prédéfinis de la visionneuse, examinez le paramètre prédéfini de la visionneuse Zoom ou le paramètre prédéfini de la visionneuse Zoom guidé que vous avez créé. Si vous devez l’ajuster, sélectionnez **[!UICONTROL Modifier]**, modifiez les paramètres sur la page `Configure Viewer`, puis sélectionnez **[!UICONTROL Enregistrer]**.

Pour plus d’informations sur la gestion des paramètres prédéfinis de visionneuse sur l’écran Paramètres prédéfinis de la visionneuse, voir [Paramètres prédéfinis de visionneuse](application-setup.md#viewer_presets).

>[!MORELIKETHIS]
>
>* [Création et modification des paramètres prédéfinis de visionneuse](application-setup.md#adding_and_editing_viewer_presets)
