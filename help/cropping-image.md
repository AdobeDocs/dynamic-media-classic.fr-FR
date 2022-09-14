---
title: Recadrage d’une image
description: Découvrez comment recadrer une image dans Adobe Dynamic Media Classic.
uuid: 84f199de-cbfc-4d06-877f-6e9148e82e15
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 99dfa476-4f11-4569-a27e-a76ed7787674
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: aec4c256-f5ed-4307-afec-dec848be95f9
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 35%

---

# Recadrage d’une image{#cropping-an-image}

Vous pouvez recadrer des images dans Adobe Dynamic Media Classic. Le système conserve les informations sur les images qui ont été recadrées, ce qui vous permet de rétablir leur état d’origine. Vous pouvez également recadrer une image et enregistrer la version recadrée sous un nouveau nom.

Vous pouvez recadrer une image afin d’en supprimer les bords blancs ou de ne garder qu’une partie de l’image.

>[!NOTE]
>
>Après le recadrage, vous pouvez sélectionner **[!UICONTROL Enregistrer sous]** et enregistrez une version recadrée de l’image sous un autre nom. Dans la fenêtre Enregistrer sous, sélectionnez **[!UICONTROL Enregistrer comme nouveau Principal]** pour enregistrer une seconde copie de l’image. Sélectionner **[!UICONTROL Enregistrer En Tant Que Vue Supplémentaire Du Principal]** vous pouvez donc enregistrer l’original et sa version recadrée sous un autre nom. Sélectionner **[!UICONTROL Remplacer l’original]** pour supprimer le fichier d’origine à partir duquel vous avez recadré votre image. Saisissez ensuite le nom de l’image, puis sélectionnez **[!UICONTROL Envoyer]**.

## Suppression de l’espace blanc autour d’une image à l’aide du recadrage {#crop-to-remove-white-space-around-an-image}

Vous pouvez éliminer les pixels transparents ou de couleur qui apparaissent au bord d’une image.

1. Pour recadrer une image, sélectionnez son survol **[!UICONTROL Modifier]** puis sélectionnez **[!UICONTROL Recadrer]** ou l’afficher dans le panneau de navigation de la vue Détails, puis sélectionnez l’option **[!UICONTROL Recadrer]** bouton .
1. Sur la page Éditeur de recadrage , effectuez l’une des opérations suivantes :

   * Pour rogner les pixels de couleur, accédez à **[!UICONTROL Rogner]** > **[!UICONTROL Couleur]**. Dans le **[!UICONTROL Recadrage automatique par couleur]** , sélectionnez **[!UICONTROL Coin]** et choisissez un coin avec la couleur d’arrière-plan que vous souhaitez recadrer. Puis saisissez un **[!UICONTROL Tolérance]** de 0 à 1. La valeur 0 permet de rogner les pixels uniquement s’ils correspondent exactement à la couleur sélectionnée dans l’angle de l’image. Les valeurs qui se rapprochent de 1 admettent un plus grand écart des couleurs. Sélectionner **[!UICONTROL Recadrer]**.
   * Pour rogner les pixels transparents, accédez à **[!UICONTROL Rogner]** > **[!UICONTROL Transparent]**. Dans le **[!UICONTROL Recadrage automatique par transparence]** , saisissez un paramètre de tolérance compris entre 0 et 1. Le paramètre 0 rogne les pixels uniquement s’ils sont transparents. Les valeurs plus proches de 1 permettent une plus grande transparence. Sélectionner **[!UICONTROL Recadrer]**.

1. Sélectionner **[!UICONTROL Enregistrer]**.

>[!NOTE]
>
>Pour rétablir l’état d’origine d’une image après l’avoir recadrée, affichez-la dans l’écran Éditeur de recadrage et sélectionnez **[!UICONTROL Réinitialiser]**.

## Sélection d’une zone à recadrer {#select-an-area-to-crop}

1. Pour recadrer une image, sélectionnez son survol **[!UICONTROL Modifier]** et choisissez **[!UICONTROL Recadrer]** ou l’afficher dans le panneau de navigation de la vue Détails, puis sélectionnez **[!UICONTROL Recadrer]**.

1. Dans la fenêtre Editeur de recadrage, placez la partie de l’image que vous ne souhaitez pas recadrer dans la zone de recadrage. Ce qui apparaît dans la zone est ce qui reste après avoir sélectionné **[!UICONTROL Enregistrer]** et recadrez l’image.
1. Pour modifier la zone de recadrage, effectuez l’une des opérations suivantes :

   * Faites glisser un côté ou un angle de la zone de recadrage. Maintenez la touche Maj enfoncée lorsque vous faites glisser la souris pour modifier la taille tout en conservant le format (la forme) de la zone de recadrage.
   * Spécifiez des valeurs en pixels dans les zones Taille.
   * Faites glisser la souris pour déplacer la zone de recadrage. Positionnez le pointeur dans les limites du cadre. Lorsque le pointeur prend la forme d’une flèche à quatre pointes, faites glisser la zone à l’emplacement voulu sur l’image.

1. Sélectionner **[!UICONTROL Enregistrer]**.

>[!NOTE]
>
>Pour rétablir l’état d’origine d’une image après l’avoir recadrée, affichez-la dans l’écran Éditeur de recadrage et sélectionnez **[!UICONTROL Réinitialiser]**.

>[!MORELIKETHIS]
>
>* [Options d’édition d’images lors du téléchargement](image-editing-options-upload.md#image-editing-options-at-upload)
>* [Recadrer l’espace blanc d’un fichier de PDF](pdfs.md#cropping_white_space_from_a_pdf_file)
>* [Recadrage à partir des côtés des pages de PDF](pdfs.md#cropping_from_the_sides_of_pdf_pages)

