---
title: Création de cibles de zoom pour un zoom guidé
description: Découvrez comment créer des cibles de zoom pour un zoom guidé dans Dynamic Media Classic.
uuid: 501ea37b-adc5-4290-87eb-52a3501e5d26
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: e7b4673c-8681-4741-912e-9a31cf106449
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: ffb799ba-1cf1-48e0-91a8-dea758139140
source-git-commit: 976f739e5233ae9da24b06cffa729353a7d03c46
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 44%

---

# Création de cibles de zoom pour un zoom guidé{#creating-zoom-targets-for-guided-zoom}

Les cibles de zoom permettent d’orienter les utilisateurs vers certaines sections d’une image. Outre le zoom en forme libre, les visionneuses peuvent sélectionner une miniature de la cible de zoom et effectuer un zoom sur la partie de l’image sur laquelle vous souhaitez qu’elles se concentrent. Les cibles de zoom sont un bon moyen de mettre en valeur les sections attrayantes ou intéressantes d’une image.

![Création de cibles de zoom pour un zoom guidé](/help/assets/zo_guided_zoom.png)

## A propos des cibles de zoom {#about-zoom-targets}

Le taux de zoom maximal applicable aux cibles de zoom est de 100 %. Le taux de zoom minimal varie selon la taille de la visionneuse et de l’image, comme indiqué dans le tableau ci-après.

| Taille de l’image | Taille de la visionneuse | Facteur de zoom |
| --- | --- | --- |
| Grande | Plus petite | Taux minimal plus petit |
| Petite | Plus grande | Taux minimal plus grand |

Vous pouvez ajuster la taille de la visionneuse de zoom à celle utilisée sur votre page Web. Si vous souhaitez que cette modification soit permanente, changez la taille de la visionneuse sur l’écran Configuration (si vous êtes un administrateur) Voir [Configuration des paramètres prédéfinis de la visionneuse de zoom](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets).

## Création et modification de cibles de zoom {#creating-and-editing-zoom-targets}

Créez et modifiez des cibles de zoom sur l’écran Editeur de cible de zoom. Pour ouvrir cet écran, sélectionnez une image et procédez de l’une des façons suivantes :

* sélectionnez le bouton de survol **[!UICONTROL Modifier]** et choisissez Cibles de zoom.
* Dans le panneau de navigation, affichez l’image dans la **[!UICONTROL vue Détails]**, puis sélectionnez **[!UICONTROL Cibles de zoom]**.

Dans l’écran Éditeur de cible de zoom, sélectionnez le bouton **[!UICONTROL Sélectionner la cible]** (flèche) pour sélectionner une cible avant de modifier sa taille ou sa position. Pour créer une cible de zoom sur l’image, sélectionnez **[!UICONTROL Ajouter des cibles]** (rectangle). La page Éditeur de cible de zoom propose également des outils pour supprimer, copier et nommer des cibles de zoom.

### Création d’une cible de zoom {#creating-a-zoom-target}

Pour créer une cible de zoom, ouvrez la page Éditeur de cible de zoom et procédez comme suit :

1. Sélectionnez **[!UICONTROL Ajouter des cibles]** (rectangle), déplacez le pointeur sur l’image, puis sélectionnez l’emplacement de la cible de zoom.

   Une image miniature de la cible de zoom apparaît dans le panneau situé sur la droite de l’écran.

1. Sélectionnez **[!UICONTROL Cible]** (flèche), puis sélectionnez la cible de zoom que vous avez créée et ajustez la taille et la position de la cible.

   * **Redimensionner**  : déplace le pointeur sur un coin de la cible de zoom et faites-le glisser pour agrandir ou rétrécir la cible.

   * **Position**  : déplace le pointeur sur la cible de zoom et le fait glisser vers un autre emplacement.

1. Indiquez le nom de la cible de zoom dans le champ Nom. 

   >[!NOTE]
   >
   >les informations que vous indiquez dans la zone Nom sont bien plus que cela. Lorsque les utilisateurs déplacent le pointeur sur la cible de zoom, ils voient ces informations. Entrez donc, dans cette zone Nom, une brève description de la cible de zoom pour que les utilisateurs sachent sur quoi ils peuvent zoomer.

1. (Facultatif) Saisissez des données utilisateur dans le champ Données utilisateur. Ce champ, destiné aux concepteurs Web, permet d’ajouter des informations à la cible de zoom.
1. Sélectionnez **[!UICONTROL Enregistrer]**.

   Les coordonnées et le niveau de zoom de la cible de zoom sont enregistrés. Une miniature de votre cible de zoom, avec le nom que vous avez indiqué, apparaît dans le panneau situé sur la droite de l’écran.

>[!NOTE]
>
>Pour voir à quoi ressemblent vos cibles de zoom dans une visionneuse de zoom, sélectionnez le bouton **[!UICONTROL Aperçu]** dans l’écran Éditeur de cible de zoom et choisissez une visionneuse de zoom dans l’écran Aperçu. Pour plus d’informations sur cet écran, voir [Aperçu des images avec différentes visionneuses de zoom](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers).

### Modification des cibles de zoom {#editing-zoom-targets}

Pour modifier des cibles de zoom, utilisez les techniques suivantes sur la page Éditeur de cible de zoom :

* **Repositionnement**  : à l’aide du bouton Sélectionner la cible (la flèche), sélectionnez la cible. Ensuite, faites glisser la cible vers un autre emplacement.

* **Redimensionner**  : à l’aide du bouton Sélectionner la cible (la flèche), sélectionnez la cible. Pour agrandir ou réduire la cible, déplacez le pointeur sur un coin de la cible de zoom et faites-le glisser.

* **Supprimer**  : sélectionnez la miniature de la cible sur le côté droit de l’écran. Sélectionnez ensuite **[!UICONTROL Supprimer la cible]**.

* **Renommer**  : sélectionnez l’image miniature de la cible sur le côté droit de l’écran. Saisissez ensuite un nom dans le champ de texte **[!UICONTROL Nom]** et sélectionnez **[!UICONTROL Enregistrer]**.

### Copie de cibles de zoom {#copying-zoom-targets}

Vous pouvez copier des cibles de zoom d’une image à une autre. Copiez des cibles lorsque deux images présentent du contenu similaire et que leurs cibles de zoom se trouvent aux mêmes emplacements. Pour copier des cibles de zoom sur une autre image, procédez comme suit :

1. Sur l’écran Editeur de cible de zoom, ouvrez l’image contenant les cibles de zoom à copier.
1. Sélectionnez **[!UICONTROL Copier Les Cibles Dans]**.
1. Dans la boîte de dialogue Sélectionner les images, sélectionnez une image, puis **[!UICONTROL Sélectionner]**.
