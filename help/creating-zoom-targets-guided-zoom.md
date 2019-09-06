---
title: Création de cibles de zoom pour un zoom guidé
seo-title: Création de cibles de zoom pour un zoom guidé
description: 'null'
seo-description: Découvrez comment créer des cibles de zoom pour le zoom guidé.
uuid: 501 ea 37 b-adc 5-4290-87 eb -52 a 3501 e 5 d 26
contentOwner: admin
content-type: référence
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/zoom
discoiquuid: e 7 b 4673 c -8681-4741-912 e -9 a 31 cf 106449
translation-type: tm+mt
source-git-commit: 2f99190eb0c346b87402e69c4067e94365042339

---


# Création de cibles de zoom pour un zoom guidé{#creating-zoom-targets-for-guided-zoom}

Les cibles de zoom permettent d’orienter les utilisateurs vers certaines sections d’une image. Les utilisateurs peuvent effectuer un zoom libre mais aussi cliquer sur une miniature de cible de zoom afin d’effectuer un zoom sur la section de l’image à privilégier. Les cibles de zoom sont un bon moyen de mettre en valeur les sections attrayantes ou intéressantes d’une image.

![Création de cibles de zoom pour un zoom guidé](/help/assets/zo_guided_zoom.png)

## A propos des cibles de zoom {#about-zoom-targets}

Le taux de zoom maximal applicable aux cibles de zoom est de 100 %. Le taux de zoom minimal varie selon la taille de la visionneuse et de l’image, comme indiqué dans le tableau ci-après.

| Taille de l’image | Taille de la visionneuse | Facteur de zoom |
|--- |--- |--- |
| Grande | Plus petite | Taux minimal plus petit |
| Petite | Plus grande | Taux minimal plus grand |

Vous pouvez ajuster la taille de la visionneuse de zoom à celle utilisée sur votre page Web. Si vous souhaitez que cette modification soit permanente, changez la taille de la visionneuse sur l’écran Configuration (si vous êtes un administrateur) (voir [Configuration des paramètres prédéfinis de la visionneuse de zoom](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets)).

## Création et modification de cibles de zoom {#creating-and-editing-zoom-targets}

Créez et modifiez des cibles de zoom sur l’écran Editeur de cible de zoom. Pour ouvrir cet écran, sélectionnez une image et procédez de l’une des façons suivantes :

* Click the rollover **Edit** button and choose Zoom Targets.
* In the Browse Panel, display the image in Detail view and click **Zoom Targets**.

On the Zoom Target Editor screen, click **Select Targe** t button (the arrow) to select a target before changing its size or position. Click **Add Targets** (the rectangle) to create a zoom target on the image. L’écran Editeur de cible de zoom propose également des outils permettant de supprimer, de copier et de nommer des cibles de zoom.

### Création d’une cible de zoom {#creating-a-zoom-target}

Pour créer une cible de zoom, ouvrez l’écran Editeur de cible de zoom et procédez comme suit :

1. Click **Add Targets** (the rectangle), move the pointer over the image, and click where you want to the zoom target to be.

   Une image miniature de la cible de zoom apparaît dans le panneau situé sur la droite de l’écran.

1. Click **Select Target** (the arrow), click to select the zoom target you created, and adjust the size and position of the target.

   **Redimensionnez** le pointeur sur un coin de la cible de zoom et faites-le glisser pour élargir ou réduire la cible.

   **Positionnement** Déplacez le pointeur sur la cible de zoom et faites-le glisser vers un autre emplacement.

1. Indiquez le nom de la cible de zoom dans le champ Nom. 

   >[!NOTE]
   >
   >les informations que vous indiquez dans la zone Nom sont bien plus que cela. Lorsque les utilisateurs déplacent le pointeur sur la cible de zoom, ils voient ces informations. Entrez donc, dans cette zone Nom, une brève description de la cible de zoom pour que les utilisateurs sachent sur quoi ils peuvent zoomer.

1. (Facultatif) Saisissez des données utilisateur dans le champ Données utilisateur. Ce champ, destiné aux concepteurs Web, permet d’ajouter des informations à la cible de zoom.
1. Cliquez sur **Enregistrer**.

   Les coordonnées et le niveau de zoom de la cible de zoom sont enregistrés. Une miniature de votre cible de zoom, avec le nom que vous avez indiqué, apparaît dans le panneau situé sur la droite de l’écran.

>[!NOTE]
>
>Pour voir à quoi ressemblent vos cibles de zoom dans une visionneuse de zoom, cliquez sur le bouton Prévisualiser sur l’écran Editeur de cible de zoom et choisissez une visionneuse de zoom sur l’écran Prévisualiser. Pour plus d’informations sur cet écran, voir [Prévisualisation d’images avec différentes visionneuses de zoom](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers).

### Modification de cibles de zoom {#editing-zoom-targets}

Utilisez ces techniques sur l’écran Editeur de cible de zoom pour modifier des cibles de zoom :

**Repositionnement** avec le bouton Sélectionner cible (la flèche), cliquez sur la cible pour la sélectionner. Ensuite, faites glisser la cible vers un autre emplacement.

**Redimensionnement** avec le bouton Sélectionner cible (la flèche), cliquez sur la cible pour la sélectionner. Ensuite, déplacez le pointeur vers un coin de la cible de zoom et faites-le glisser pour élargir ou rétrécir la cible.

**Suppression** de l'image de miniature de la cible sur le côté droit de l'écran. Cliquez ensuite sur Supprimer la cible.

**Attribution d'un nouveau nom** à la miniature de la cible sur la droite de l'écran. Ensuite, entrez un nom dans la zone Nom et cliquez sur Enregistrer.

### Copie de cibles de zoom {#copying-zoom-targets}

Vous pouvez copier des cibles de zoom d’une image à une autre. Copiez des cibles lorsque deux images présentent du contenu similaire et que leurs cibles de zoom se trouvent aux mêmes emplacements. Pour copier des cibles de zoom vers une autre image, procédez comme suit :

1. Sur l’écran Editeur de cible de zoom, ouvrez l’image contenant les cibles de zoom à copier.
1. Cliquez **sur Copier les cibles vers**.
1. In the Select Images dialog box, select an image and click **Select**.

