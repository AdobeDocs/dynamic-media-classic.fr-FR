---
title: Recadrage d’une image
description: Découvrez comment recadrer une image dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: aec4c256-f5ed-4307-afec-dec848be95f9
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 31%

---

# Recadrage d’une image{#cropping-an-image}

Vous pouvez recadrer des images dans Adobe Dynamic Media Classic. Le système conserve les informations sur les images qui ont été recadrées, ce qui vous permet de rétablir leur état d’origine. Vous pouvez également recadrer une image et enregistrer la version recadrée sous un nouveau nom.

Vous pouvez recadrer une image afin d’en supprimer les bords blancs ou de ne garder qu’une partie de l’image.

>[!NOTE]
>
>Après le recadrage, vous pouvez sélectionner **[!UICONTROL Enregistrer sous]** et enregistrer une version recadrée de l’image sous un autre nom. Dans la fenêtre Enregistrer sous, sélectionnez **[!UICONTROL Enregistrer en tant que nouveau Principal]** pour enregistrer une seconde copie de l’image. Sélectionnez **[!UICONTROL Enregistrer en tant que vue d’ajout du Principal]** afin de pouvoir enregistrer l’original et sa version recadrée sous un autre nom. Sélectionnez **[!UICONTROL Remplacer l’original]** pour supprimer le fichier d’origine à partir duquel vous avez recadré votre image. Saisissez ensuite le nom de l’image, puis sélectionnez **[!UICONTROL Envoyer]**.

## Suppression de l’espace blanc autour d’une image à l’aide du recadrage {#crop-to-remove-white-space-around-an-image}

Vous pouvez éliminer les pixels transparents ou de couleur qui apparaissent au bord d’une image.

1. Pour recadrer une image, sélectionnez son bouton de survol **[!UICONTROL Modifier]**, puis sélectionnez **[!UICONTROL Recadrer]**, ou affichez-la dans le panneau Parcourir dans la vue Détail et sélectionnez le bouton **[!UICONTROL Recadrer]**.
1. Dans la page Éditeur de recadrage, effectuez l’une des opérations suivantes :

   * Pour rogner les pixels de couleur, accédez à **[!UICONTROL Rogner]** > **[!UICONTROL Couleur]**. Dans la boîte de dialogue **[!UICONTROL Recadrage automatique par couleur]**, sélectionnez le menu **[!UICONTROL Coin]** et choisissez un coin avec la couleur d’arrière-plan à recadrer. Entrez ensuite un paramètre **[!UICONTROL Tolérance]** compris entre 0 et 1. La valeur 0 permet de rogner les pixels uniquement s’ils correspondent exactement à la couleur sélectionnée dans l’angle de l’image. Les valeurs qui se rapprochent de 1 admettent un plus grand écart des couleurs. Sélectionnez **[!UICONTROL Recadrer]**.
   * Pour rogner les pixels transparents, accédez à **[!UICONTROL Rogner]** > **[!UICONTROL Transparent]**. Dans la boîte de dialogue **[!UICONTROL Recadrage automatique par transparence]**, saisissez un paramètre de tolérance compris entre 0 et 1. Le paramètre 0 recadre les pixels uniquement s’ils sont transparents. Les valeurs plus proches de 1 permettent une plus grande transparence. Sélectionnez **[!UICONTROL Recadrer]**.

1. Sélectionnez **[!UICONTROL Enregistrer]**.

>[!NOTE]
>
>Pour restaurer l’état d’origine d’une image après l’avoir recadrée, affichez l’image dans l’écran de l’éditeur de recadrage et sélectionnez **[!UICONTROL Réinitialiser]**.

## Sélection d’une zone à recadrer {#select-an-area-to-crop}

1. Pour recadrer une image, sélectionnez son bouton de survol **[!UICONTROL Modifier]**, puis choisissez **[!UICONTROL Recadrer]** ou affichez-la dans le panneau Parcourir dans le mode Détail et sélectionnez **[!UICONTROL Recadrer]**.

1. Dans la fenêtre Éditeur de recadrage , placez la partie de l’image que vous ne souhaitez pas recadrer dans la zone de recadrage. Ce qui apparaît dans la zone est ce qui restera après avoir sélectionné **[!UICONTROL Enregistrer]** et recadré l’image.
1. Pour modifier la zone de recadrage, effectuez l’une des opérations suivantes :

   * Faites glisser un côté ou un angle de la zone de recadrage. Maintenez la touche Maj enfoncée tout en faisant glisser pour modifier la taille, mais conservez les proportions (la forme) de la zone de recadrage.
   * Spécifiez des valeurs en pixels dans les zones Taille.
   * Faites glisser la souris pour déplacer la zone de recadrage. Positionnez le pointeur dans les limites du cadre. Lorsque le pointeur prend la forme d’une flèche à quatre pointes, faites glisser la zone à l’emplacement voulu sur l’image.

1. Sélectionnez **[!UICONTROL Enregistrer]**.

>[!NOTE]
>
>Pour restaurer l’état d’origine d’une image après l’avoir recadrée, affichez l’image dans l’écran de l’éditeur de recadrage et sélectionnez **[!UICONTROL Réinitialiser]**.

>[!MORELIKETHIS]
>
>* [Options de modification d’images lors du chargement](image-editing-options-upload.md#image-editing-options-at-upload)
>* [Recadrer un espace blanc dans un fichier PDF](pdfs.md#cropping_white_space_from_a_pdf_file)
>* [Recadrer sur les côtés des pages PDF](pdfs.md#cropping_from_the_sides_of_pdf_pages)
