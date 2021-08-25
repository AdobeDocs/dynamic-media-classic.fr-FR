---
title: Recadrage d’une image
description: Découvrez comment recadrer une image dans Dynamic Media Classic.
uuid: 84f199de-cbfc-4d06-877f-6e9148e82e15
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 99dfa476-4f11-4569-a27e-a76ed7787674
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: aec4c256-f5ed-4307-afec-dec848be95f9
source-git-commit: 976f739e5233ae9da24b06cffa729353a7d03c46
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 35%

---

# Recadrage d’une image{#cropping-an-image}

Vous pouvez recadrer des images dans Dynamic Media Classic. Le système conserve les informations sur les images qui ont été recadrées, ce qui vous permet de rétablir leur état d’origine. Vous pouvez également recadrer une image et enregistrer la version recadrée sous un nouveau nom.

Vous pouvez recadrer une image afin d’en supprimer les bords blancs ou de ne garder qu’une partie de l’image.

>[!NOTE]
>
>Une fois le recadrage effectué, vous pouvez sélectionner **[!UICONTROL Enregistrer sous]** et enregistrer une version recadrée de l’image sous un autre nom. Dans la fenêtre Enregistrer sous, sélectionnez **[!UICONTROL Enregistrer comme nouveau Principal]** pour enregistrer une seconde copie de l’image. Sélectionnez **[!UICONTROL Enregistrer en tant que vue supplémentaire du Principal]** afin que vous puissiez enregistrer l’original et sa version recadrée sous un autre nom. Sélectionnez **[!UICONTROL Remplacer l’original]** pour supprimer le fichier d’origine à partir duquel vous avez recadré votre image. Saisissez ensuite le nom de l’image, puis sélectionnez **[!UICONTROL Submit]**.

## Suppression de l’espace blanc autour d’une image à l’aide du recadrage {#crop-to-remove-white-space-around-an-image}

Vous pouvez éliminer les pixels transparents ou de couleur qui apparaissent au bord d’une image.

1. Pour recadrer une image, cliquez sur son bouton de survol **[!UICONTROL Modifier]**, puis sélectionnez **[!UICONTROL Recadrer]** ou affichez-la dans le panneau de navigation en mode Détails et sélectionnez le bouton **[!UICONTROL Recadrer]**.
1. Sur la page Éditeur de recadrage , effectuez l’une des opérations suivantes :

   * Pour rogner les pixels de couleur, accédez à **[!UICONTROL Rogner]** > **[!UICONTROL Couleur]**. Dans la boîte de dialogue **[!UICONTROL Recadrage automatique par couleur]**, sélectionnez le menu **[!UICONTROL Coin]** et choisissez un coin avec la couleur d’arrière-plan que vous souhaitez recadrer. Saisissez ensuite un paramètre **[!UICONTROL Tolérance]** compris entre 0 et 1. La valeur 0 permet de rogner les pixels uniquement s’ils correspondent exactement à la couleur sélectionnée dans l’angle de l’image. Les valeurs qui se rapprochent de 1 admettent un plus grand écart des couleurs. Sélectionnez **[!UICONTROL Recadrer]**.
   * Pour rogner les pixels transparents, accédez à **[!UICONTROL Rogner]** > **[!UICONTROL Transparent]**. Dans la boîte de dialogue **[!UICONTROL Recadrage automatique par transparence]** , saisissez un paramètre de tolérance compris entre 0 et 1. Le paramètre 0 rogne les pixels uniquement s’ils sont transparents. Les valeurs plus proches de 1 permettent une plus grande transparence. Sélectionnez **[!UICONTROL Recadrer]**.

1. Sélectionnez **[!UICONTROL Enregistrer]**.

>[!NOTE]
>
>Pour restaurer l’état d’origine d’une image après l’avoir recadrée, affichez-la dans l’écran Éditeur de recadrage et sélectionnez **[!UICONTROL Réinitialiser]**.

## Sélection d’une zone à recadrer {#select-an-area-to-crop}

1. Pour recadrer une image, cliquez sur son bouton de survol **[!UICONTROL Modifier]**, puis sélectionnez **[!UICONTROL Recadrer]** ou affichez-la dans le panneau de navigation en mode Détails et sélectionnez **[!UICONTROL Recadrer]**.

1. Dans la fenêtre Editeur de recadrage, placez la partie de l’image que vous ne souhaitez pas recadrer dans la zone de recadrage. Tout ce qui apparaît dans la zone est ce qui reste après avoir sélectionné **[!UICONTROL Enregistrer]** et recadré l’image.
1. Pour modifier la zone de recadrage, effectuez l’une des opérations suivantes :

   * Faites glisser un côté ou un angle de la zone de recadrage. Maintenez la touche Maj enfoncée lorsque vous faites glisser la souris pour modifier la taille tout en conservant le format (la forme) de la zone de recadrage.
   * Spécifiez des valeurs en pixels dans les zones Taille.
   * Faites glisser la souris pour déplacer la zone de recadrage. Positionnez le pointeur dans les limites du cadre. Lorsque le pointeur prend la forme d’une flèche à quatre pointes, faites glisser la zone à l’emplacement voulu sur l’image.

1. Sélectionnez **[!UICONTROL Enregistrer]**.

>[!NOTE]
>
>Pour restaurer l’état d’origine d’une image après l’avoir recadrée, affichez-la dans l’écran Éditeur de recadrage et sélectionnez **[!UICONTROL Réinitialiser]**.

>[!MORELIKETHIS]
>
>* [Options d’édition d’images lors du téléchargement](image-editing-options-upload.md#image-editing-options-at-upload)
>* [Recadrer l’espace blanc d’un fichier PDF](pdfs.md#cropping_white_space_from_a_pdf_file)
>* [Recadrage à partir des côtés des pages PDF](pdfs.md#cropping_from_the_sides_of_pdf_pages)

