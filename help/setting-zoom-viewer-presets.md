---
title: Configuration des paramètres prédéfinis de la visionneuse de zoom
seo-title: Configuration des paramètres prédéfinis de la visionneuse de zoom
description: 'null'
seo-description: Découvrez comment configurer les paramètres prédéfinis de la visionneuse de zoom.
uuid: 202d80cb-8282-45d4-89e8-942c8677aa93
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: 5023a933-e229-4d3c-8e91-3ac5e9f4970b
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 69%

---


# Configuration des paramètres prédéfinis de la visionneuse de zoom{#setting-up-zoom-viewer-presets}

Les paramètres prédéfinis de visionneuse de zoom déterminent le style, le comportement et l’aspect des visionneuses de zoom. Dynamic Media Classic offre de nombreuses options de personnalisation et d’habillage des visionneuses. Dynamic Media Classic est fourni avec des paramètres prédéfinis de visionneuse de zoom personnalisés, de visionneuse de zoom par défaut de base (rapide), de sortie et de sortie. Si vous êtes un administrateur, vous pouvez créer de nouveaux paramètres prédéfinis de visionneuse de zoom d’entreprise ou modifier un paramètre prédéfini par défaut et l’enregistrer ensuite sous un nouveau nom.

Toutes les visionneuses de zoom comportent des boutons permettant d’effectuer un zoom avant, un zoom arrière et un panoramique mais aussi de rétablir l’état initial de l’image après le zoom. L’aspect des boutons et de la fenêtre elle-même est fonction des paramètres prédéfinis de visionneuse de zoom actuellement sélectionnés. Vous pouvez configurer un paramètre prédéfini de visionneuse de zoom avec des couleurs, des bordures, des polices et des paramètres d’image différents. Dans le cas d’une visionneuse de zoom guidé, vous pouvez également choisir l’emplacement des cibles de zoom. Les cibles de zoom correspondent aux miniatures sur lesquelles les utilisateurs cliquent pour effectuer un zoom sur les zones que vous définissez.

## A propos des paramètres prédéfinis de la visionneuse de zoom {#about-zoom-viewer-presets}

Dynamic Media Classic offre ces paramètres prédéfinis de visionneuse de zoom :

* **Visionneuse de zoom : Élémentaire** Fournit un zoom de base sur l’image d’origine.

* **Visionneuse de zoom : Fenêtre déroulante** Affiche une seconde image de la zone agrandie en regard de l’image d’origine. Aucune commande n’est disponible. Il suffit de déplacer la sélection sur la zone à visualiser.

Pour déterminer la quantité totale de bande passante allouée à la visionneuse, n’oubliez pas que l’image principale et celle de la fenêtre déroulante sont toutes deux diffusées par la visionneuse. La taille de l’image de la fenêtre déroulante est déterminée par la taille de l’image principale (largeur et hauteur d’affichage) et par le facteur de zoom. Pour que la fenêtre déroulante ne devienne pas trop volumineuse, équilibrez ces deux valeurs : si la taille de l’image principale est importante, réduisez la valeur du facteur de zoom. (La Largeur de la fenêtre déroulante et la Hauteur de la fenêtre déroulante déterminent la taille de la fenêtre déroulante, mais pas la taille de l’image diffusée par la visionneuse.)

Par exemple, si la taille de l’image principale est de 350 x 350 pixels et que le facteur de zoom est de 3, la taille d’image de la fenêtre déroulante sera de 1 050 x 1 050 pixels. Si la taille de l’image principale est de 300 x 300 pixels et que le facteur de zoom est de 4, la taille d’image de la fenêtre déroulante sera de 1 200 x 1 200 pixels. Selon la valeur de qualité JPEG sélectionnée (une valeur comprise entre 80 et 90 est recommandée), il est possible de réduire sensiblement la taille du fichier. Selon la taille de l’image principale, un facteur de zoom de 2,5 à 4 est recommandé.

Dynamic Media Classic recommande les paramètres suivants pour les paramètres prédéfinis de visionneuse de zoom déroulante :

* **Taille** de l’image agrandie Environ 1 500 x 1 500 pixels, sans dépasser 2 000 x 2 000 pixels.

* **Taille** de l’image : 100 Ko ou moins, ne doit pas dépasser 150 Ko (compressez le fichier pour qu’il ne dépasse pas 150 Ko).

* **Visionneuse de zoom : Personnalisé** Fournit un zoom guidé ou non guidé avec des images, des visionneuses d’images avec plusieurs vues ou des séries d’échantillons de couleur.

## Création et modification de paramètres prédéfinis de la visionneuse de zoom {#creating-and-editing-zoom-viewer-presets}

Pour créer ou modifier un paramètre prédéfini de visionneuse de zoom, procédez comme suit :

1. Cliquez sur **Configuration** > **Paramètres prédéfinis de la visionneuse**.
1. Effectuez l’une des opérations suivantes :

   * **Création d’un paramètre prédéfini** Ajoute de clic. Dans la boîte de dialogue Ajouter un paramètre prédéfini de visionneuse, choisissez une plate-forme, choisissez une visionneuse de zoom, puis cliquez sur Ajouter. Entrez le nom du paramètre prédéfini dans la zone Nom du paramètre prédéfini.

   * **Modification d’un paramètre prédéfini** Sélectionnez un paramètre prédéfini de visionneuse de zoom, puis cliquez sur 
**Modifier**.

1. Spécifiez les paramètres de votre choix.

   Pour obtenir la description d’une option, cliquez sur l’icône d’information  adjacente.

   L’écran de prévisualisation affiche la visionneuse à mesure que vous actualisez et modifiez les paramètres.

1. Cliquez sur **Enregistrer** ou sur **Enregistrer sous**.
1. Sur l’écran Paramètres prédéfinis de la visionneuse, examinez le paramètre prédéfini de visionneuse de zoom libre ou guidé que vous venez de créer. If it needs adjusting, click **Edit**, change settings on the Configure Viewer screen, and click **Save**.

Pour plus d’informations sur la gestion des paramètres prédéfinis de visionneuse sur l’écran Paramètres prédéfinis de la visionneuse, voir [Paramètres prédéfinis de visionneuse](application-setup.md#viewer_presets).

>[!MORELIKETHIS]
>
>* [Création et modification de paramètres prédéfinis de la visionneuse](application-setup.md#adding_and_editing_viewer_presets)

