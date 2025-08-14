---
title: Chargement des fichiers de modèle
description: Découvrez comment télécharger des fichiers de modèle dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: a105c18a-7e06-43cb-938c-a3bcdc3e9d22
topic: Content Management
level: Experienced
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 32%

---

# Chargement des fichiers de modèle{#uploading-template-files}

Chargez les fichiers dont vous avez besoin pour votre modèle dans Adobe Dynamic Media Classic avant de commencer à créer le modèle. Vous pouvez créer des modèles à partir d’un PSD Adobe® Photoshop® ou d’un fichier image. Les images TIFF et PNG sont recommandées en raison de leur prise en charge de la transparence.

>[!NOTE]
>
>Adobe Dynamic Media Classic recommande d’utiliser des images TIFF ou PSD transparentes dans vos modèles à la taille exacte que vous souhaitez leur afficher sur votre site web. Lorsque vous publiez le modèle, appelez l’image avec un paramètre d’image prédéfini qui soit de la même taille. Si vous prenez soin de définir correctement la taille, il sera inutile de redimensionner (rééchantillonner) le modèle par rapport à la taille à laquelle il a été créé.

Les modèles peuvent être créés à partir de fichiers Adobe Photoshop PSD ou de fichiers d’images. 

Pour obtenir des instructions détaillées sur le téléchargement de fichiers, voir [Télécharger des fichiers](uploading-files.md#uploading_files). Tenez compte des remarques suivantes lors du téléchargement de fichiers de modèle :

* Si vous téléchargez un fichier PSD, vous pouvez créer un modèle à partir de ce fichier. Adobe Dynamic Media Classic crée une image distincte pour chaque calque dans PSD. Dans la boîte de dialogue Charger les options de la tâche, sélectionnez **[!UICONTROL Options de Photoshop]**, **[!UICONTROL Conserver les calques]** et **[!UICONTROL Créer un modèle]**. Choisissez ensuite une option dans la liste déroulante **[!UICONTROL Dénomination de calque]** pour nommer les images créées par Adobe Dynamic Media Classic à partir des calques dans PSD.
(voir [Options de téléchargement des fichiers PSD](psd-files.md#psd_upload_options)).
<!-- THERE IS NO LONGER AN IMAGE EDITING OPTIONS MENU * If you are uploading images, you can create a mask from its clipping path. This option applies to images created with image-editing applications in which a clipping path was created. In the Upload Job Options dialog box, select Image Editing Options and select the Create Mask From Clipping Path option. 
See [Image editing options at upload](image-editing-options-upload.md#image-editing-options-at-upload). -->

>[!MORELIKETHIS]
>
>* [Chargez vos fichiers](uploading-files.md#uploading_your_files)
>* [Utiliser des fichiers PSD](psd-files.md#working_with_psd_files)
