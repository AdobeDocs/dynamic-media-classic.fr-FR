---
title: Recadrage d’une image
description: Découvrez comment recadrer une image.
uuid: 84f199de-cbfc-4d06-877f-6e9148e82e15
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 99dfa476-4f11-4569-a27e-a76ed7787674
feature: Dynamic Media Classic,Asset Management
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '559'
ht-degree: 85%

---


# Recadrage d’une image{#cropping-an-image}

Vous pouvez recadrer des images dans Dynamic Media Classic. Le système conserve les informations sur les images qui ont été recadrées, ce qui vous permet de rétablir leur état d’origine. Vous pouvez également recadrer une image et enregistrer la version recadrée sous un nouveau nom.

Vous pouvez recadrer une image afin d’en supprimer les bords blancs ou de ne garder qu’une partie de l’image.

>[!NOTE]
>
>une fois l’image recadrée, vous pouvez cliquer sur le bouton Enregistrer en tant que, et ainsi enregistrer la version recadrée de l’image sous un autre nom. Dans la fenêtre Enregistrer en tant que, choisissez l’option Enregistrer sous nouvelle image originale pour sauvegarder une seconde copie de l’image. Choisissez l’option Enregistrer une vue supplémentaire de l’image originale pour enregistrer l’original et sa version recadrée sous un nom différent. Choisissez l’option Remplacer l’original pour supprimer le fichier original qui a servi à recadrer l’image. Ensuite, nommez l’image, puis cliquez sur le bouton Envoyer.

## Suppression de l’espace blanc autour d’une image à l’aide du recadrage  {#crop-to-remove-white-space-around-an-image}

Vous pouvez éliminer les pixels transparents ou de couleur qui apparaissent au bord d’une image.

1. Pour recadrer une image, cliquez sur son bouton de survol Modifier et choisissez Recadrer ou affichez l’image dans le panneau de navigation en mode Affichage des détails et cliquez sur le bouton Recadrer. L’écran Editeur de recadrage s’ouvre.
1. Effectuez l’une des opérations suivantes :

   * Pour rogner des pixels de couleur, sélectionnez le menu Rogner et choisissez Couleur. La boîte de dialogue Recadrage automatique par couleur s’affiche. Dans le menu Coin, choisissez un angle dont vous souhaitez rogner la couleur d’arrière-plan. Ensuite, spécifiez une valeur de tolérance comprise entre 0 et 1. La valeur 0 permet de rogner les pixels uniquement s’ils correspondent exactement à la couleur sélectionnée dans l’angle de l’image. Les valeurs qui se rapprochent de 1 admettent un plus grand écart des couleurs. Cliquez sur le bouton Recadrer.
   * Pour rogner des pixels transparents, sélectionnez le menu Rogner et choisissez Transparent. La boîte de dialogue Recadrage auto par transparence s’affiche. Spécifiez une valeur de tolérance comprise entre 0 et 1. La valeur 0 permet de rogner les pixels uniquement s’ils sont entièrement transparents. Les valeurs plus proches de 1 permettent une plus grande transparence. Cliquez sur Recadrer.

1. Cliquez sur **Enregistrer**.

>[!NOTE]
>
>pour restaurer l’état d’origine d’une image après l’avoir recadrée, affichez l’image dans l’écran Editeur de recadrage, puis cliquez sur le bouton Réinitialiser.

## Sélection d’une zone à recadrer  {#select-an-area-to-crop}

1. Pour recadrer une image, cliquez sur son bouton de survol Modifier et choisissez **Recadrer** ou affichez-la dans le panneau de navigation de la vue de détails, puis cliquez sur **Recadrer**.

1. Dans la fenêtre Editeur de recadrage, placez la partie de l’image que vous ne souhaitez pas recadrer dans la zone de recadrage. Ce qui apparaît dans la zone reste lorsque vous cliquez sur **Enregistrer** et que vous recadrez l’image.
1. Pour modifier la zone de recadrage, effectuez l’une des opérations suivantes :

   * Faites glisser un côté ou un angle de la zone de recadrage. Maintenez la touche Maj enfoncée lorsque vous faites glisser la souris pour modifier la taille tout en conservant le format (la forme) de la zone de recadrage.
   * Spécifiez des valeurs en pixels dans les zones Taille.
   * Faites glisser la souris pour déplacer la zone de recadrage. Positionnez le pointeur dans les limites du cadre. Lorsque le pointeur prend la forme d’une flèche à quatre pointes, faites glisser la zone à l’emplacement voulu sur l’image.

1. Cliquez sur **Enregistrer**.

>[!NOTE]
>
>pour restaurer l’état d’origine d’une image après l’avoir recadrée, affichez l’image dans l’écran Editeur de recadrage, puis cliquez sur le bouton Réinitialiser.

>[!MORELIKETHIS]
>
>* [Options d’édition d’images au téléchargement](image-editing-options-upload.md#image-editing-options-at-upload)
>* [Suppression de l’espace blanc d’un fichier PDF](pdfs.md#cropping_white_space_from_a_pdf_file)
>* [Recadrage à partir des côtés des pages PDF](pdfs.md#cropping_from_the_sides_of_pdf_pages)

