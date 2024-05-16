---
title: Chargement des fichiers de modèle
description: Découvrez comment charger des fichiers de modèle dans Adobe Dynamic Media Classic.
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

Transférez les fichiers dont vous avez besoin pour votre modèle dans Adobe Dynamic Media Classic avant de commencer à créer le modèle. Vous pouvez créer des modèles à partir d’un PSD Adobe® Photoshop® ou d’un fichier image. Les images TIFF et PNG sont recommandées en raison de leur prise en charge de la transparence.

>[!NOTE]
>
>Adobe Dynamic Media Classic recommande d’utiliser des images de TIFF ou de PSD transparentes dans vos modèles à la taille exacte que vous souhaitez afficher sur votre site Web. Lorsque vous publiez le modèle, appelez l’image avec un paramètre d’image prédéfini qui soit de la même taille. Si vous prenez soin de définir correctement la taille, il sera inutile de redimensionner (rééchantillonner) le modèle par rapport à la taille à laquelle il a été créé.

Les modèles peuvent être créés à partir de fichiers Adobe Photoshop PSD ou de fichiers d’images. 

Pour obtenir des instructions détaillées sur le téléchargement de fichiers, voir [Chargement de fichiers](uploading-files.md#uploading_files). Tenez compte des remarques suivantes lors du téléchargement de fichiers de modèle :

* Si vous téléchargez un fichier de PSD, vous pouvez en créer un modèle. Adobe Dynamic Media Classic crée une image distincte pour chaque calque du PSD. Dans la boîte de dialogue Télécharger les options de la tâche, sélectionnez **[!UICONTROL Options Photoshop]**, puis sélectionnez **[!UICONTROL Conserver les calques]** et **[!UICONTROL Créer un modèle]**. Sélectionnez ensuite une option dans la liste **[!UICONTROL Nom de calque]** Liste déroulante pour nommer les images qu’Adobe Dynamic Media Classic crée à partir des calques du PSD.
(voir [Options de téléchargement des fichiers PSD](psd-files.md#psd_upload_options)).
<!-- THERE IS NO LONGER AN IMAGE EDITING OPTIONS MENU * If you are uploading images, you can create a mask from its clipping path. This option applies to images created with image-editing applications in which a clipping path was created. In the Upload Job Options dialog box, select Image Editing Options and select the Create Mask From Clipping Path option. 
See [Image editing options at upload](image-editing-options-upload.md#image-editing-options-at-upload). -->

>[!MORELIKETHIS]
>
>* [Chargement des fichiers](uploading-files.md#uploading_your_files)
>* [Utilisation de fichiers de PSD](psd-files.md#working_with_psd_files)
