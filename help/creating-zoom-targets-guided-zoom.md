---
title: Création de cibles de zoom pour un zoom guidé
description: Découvrez comment créer des cibles de zoom pour un zoom guidé.
uuid: 501ea37b-adc5-4290-87eb-52a3501e5d26
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: e7b4673c-8681-4741-912e-9a31cf106449
feature: Dynamic Media Classic, Visionneuses, Zoom
role: Professionnel
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '738'
ht-degree: 68%

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

## Création et modification de cibles de zoom  {#creating-and-editing-zoom-targets}

Créez et modifiez des cibles de zoom sur l’écran Editeur de cible de zoom. Pour ouvrir cet écran, sélectionnez une image et procédez de l’une des façons suivantes :

* Cliquez sur le bouton de survol **[!UICONTROL Modifier]** et choisissez Cibles de zoom.
* Dans le panneau de navigation, affichez l’image dans **[!UICONTROL Vue de détails]**, puis cliquez sur **[!UICONTROL Cibles de zoom]**.

Dans l’écran Editeur de Cible de zoom, cliquez sur le bouton **[!UICONTROL Sélectionner la Cible]** (flèche) pour sélectionner une cible avant de modifier sa taille ou sa position. Cliquez sur **[!UICONTROL Ajouter des Cibles]** (rectangle) pour créer une cible de zoom sur l’image. L’écran Editeur de cible de zoom propose également des outils permettant de supprimer, de copier et de nommer des cibles de zoom.

### Création d’une cible de zoom  {#creating-a-zoom-target}

Pour créer une cible de zoom, ouvrez l’écran Editeur de cible de zoom et procédez comme suit :

1. Cliquez sur **[!UICONTROL Ajouter des Cibles]** (rectangle), déplacez le pointeur sur l’image, puis cliquez à l’endroit où vous souhaitez que la cible de zoom se trouve.

   Une image miniature de la cible de zoom apparaît dans le panneau situé sur la droite de l’écran.

1. Cliquez sur **[!UICONTROL Sélectionner la Cible]** (flèche), cliquez sur pour sélectionner la cible de zoom que vous avez créée, puis ajustez la taille et la position de la cible.

   * ****
RedimensionnementDéplacez le pointeur sur un coin de la cible de zoom et faites-le glisser pour agrandir ou rétrécir la cible.

   * ****
PositionnementDéplacez le pointeur sur la cible de zoom et faites-le glisser vers un autre emplacement.

1. Indiquez le nom de la cible de zoom dans le champ Nom. 

   >[!NOTE]
   >
   >les informations que vous indiquez dans la zone Nom sont bien plus que cela. Lorsque les utilisateurs déplacent le pointeur sur la cible de zoom, ils voient ces informations. Entrez donc, dans cette zone Nom, une brève description de la cible de zoom pour que les utilisateurs sachent sur quoi ils peuvent zoomer.

1. (Facultatif) Saisissez des données utilisateur dans le champ Données utilisateur. Ce champ, destiné aux concepteurs Web, permet d’ajouter des informations à la cible de zoom.
1. Cliquez sur **[!UICONTROL Enregistrer]**.

   Les coordonnées et le niveau de zoom de la cible de zoom sont enregistrés. Une miniature de votre cible de zoom, avec le nom que vous avez indiqué, apparaît dans le panneau situé sur la droite de l’écran.

>[!NOTE]
>
>Pour voir à quoi ressemblent vos cibles de zoom dans une visionneuse de zoom, cliquez sur le bouton Prévisualiser sur l’écran Editeur de cible de zoom et choisissez une visionneuse de zoom sur l’écran Prévisualiser. Pour plus d’informations sur cet écran, voir [Prévisualisation d’images avec différentes visionneuses de zoom](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers).

### Modification de cibles de zoom  {#editing-zoom-targets}

Utilisez ces techniques sur l’écran Editeur de cible de zoom pour modifier des cibles de zoom :

* ****
RepositionnementAvec le bouton Sélectionner la Cible (la flèche), cliquez sur la cible pour la sélectionner. Ensuite, faites glisser la cible vers un autre emplacement.

* ****
RedimensionnementAvec le bouton Sélectionner la Cible (la flèche), cliquez sur la cible pour la sélectionner. Ensuite, déplacez le pointeur vers un coin de la cible de zoom et faites-le glisser pour élargir ou rétrécir la cible.

* ****
SuppressionCliquez sur l’image miniature de la cible située sur le côté droit de l’écran. Cliquez ensuite sur **[!UICONTROL Supprimer la Cible]**.

* ****
Attribution d’un nouveau nomCliquez sur l’image miniature de la cible située sur le côté droit de l’écran. Entrez ensuite un nom dans le champ de texte **[!UICONTROL Nom]**, puis cliquez sur **[!UICONTROL Enregistrer]**.

### Copie de cibles de zoom {#copying-zoom-targets}

Vous pouvez copier des cibles de zoom d’une image à une autre. Copiez des cibles lorsque deux images présentent du contenu similaire et que leurs cibles de zoom se trouvent aux mêmes emplacements. Pour copier des cibles de zoom vers une autre image, procédez comme suit :

1. Sur l’écran Editeur de cible de zoom, ouvrez l’image contenant les cibles de zoom à copier.
1. Cliquez sur **[!UICONTROL Copier les Cibles dans]**.
1. Dans la boîte de dialogue Sélectionner les images, sélectionnez une image et cliquez sur **[!UICONTROL Sélectionner]**.

