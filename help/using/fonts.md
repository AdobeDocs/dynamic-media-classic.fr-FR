---
title: Polices
description: Découvrez comment utiliser les polices dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
feature: Dynamic Media Classic
role: User
exl-id: 186f4c7f-16f6-42f5-bc0e-55362c55e794
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 23%

---

# Polices{#fonts}

Il arrive qu’Adobe Dynamic Media Classic vous demande de charger un fichier de police pour saisir ou effectuer le rendu du texte dans une police donnée. Par exemple, pour composer le texte d’un modèle de calque dans une police donnée, téléchargez le fichier de polices. Pour afficher la numérotation des pages de la visionneuse de catalogue électronique dans une police spécifique, téléchargez le fichier de polices.

Adobe Dynamic Media Classic prend en charge les types de police suivants :

* Ensemble des polices TrueType
* Polices PostScript®
* Polices OpenType/TrueType
* Polices OpenType/PostScript
* PhotoFonts

Une fois le fichier de police chargé, vous pouvez modifier son Adobe Dynamic Media Classic ID, le nom de la police et les informations de type dans l’écran Modifier les informations.

>[!NOTE]
>
>Adobe Dynamic Media Classic recommande de charger tous les styles de police (gras, italique, gras/italique et normal) si vous prévoyez d’utiliser des polices dans les calques de modèle. Adobe Dynamic Media Classic a besoin de ces styles de police pour traiter les demandes. Tout télécharger `PostScript/Adobe Type1` les fichiers associés à une police sont également recommandés, car certaines de ces polices contiennent des informations détaillées sur le crénage.

## Chargement des fichiers de polices {#uploading-font-files}

Téléchargez les fichiers de polices en procédant de la même façon que pour le téléchargement d’autres fichiers. Vous pouvez stocker les fichiers de polices dans n’importe quel dossier Adobe Dynamic Media Classic. (voir [Téléchargement de fichiers](uploading-files.md#uploading_your_files)).

## Modifier les informations du fichier de polices {#editing-font-file-information}

Vous pouvez modifier le nom d’identifiant d’une police et ses informations de type. La modification d’un fichier de polices peut servir à effectuer des recherches et à identifier plus facilement les polices.

Dans le panneau Parcourir, sélectionnez le fichier de police à modifier dans la vue Détails, puis choisissez Fichier > Modifier les informations. L’écran Editer les informations apparaît. Choisissez les options suivantes, puis sélectionnez **[!UICONTROL Envoyer]**.

* **[!UICONTROL Nom de la police]**: ce nom identifie la police lors de sa publication.

* **[!UICONTROL Nom PostScript]**: il s’agit du nom PostScript complet de la police. Il indique généralement la graisse ou le style.

* **[!UICONTROL Nom RTF]**: ce nom apparaît dans un menu contextuel de l’éditeur RTF où sont créées les calques de texte de modèle.

* **[!UICONTROL Nom de famille de polices]**: ce nom répertorie le nom de la police sans indicateur de style, de poids ou de type de police.

* **[!UICONTROL Style de police]**: les options sont les suivantes : brut, gras, italique et gras-italique.

* **[!UICONTROL Type de police]**: les options sont TrueType et Adobe Type 1. Si vous renommez ces polices, vous pouvez l’indiquer.

* **[!UICONTROL Abréviation du type de police]**: les options sont les suivantes :

   * **[!UICONTROL TTF]**: fichiers de police TrueType utilisés pour le rendu PDF/PostScript et la diffusion d’images.

   * **[!UICONTROL AFM]**: fichiers de police Adobe PostScript contenant des informations sur les mesures de police de l’Adobe et utilisés pour la diffusion d’images.

   * **[!UICONTROL PFM]**: fichiers de polices Adobe PostScript contenant des informations de mesure de polices binaires.

   * **[!UICONTROL PFB]**: fichiers de polices Adobe PostScript contenant des informations de contour de police binaires et utilisés pour le rendu PDF/PostScript et la diffusion d’images.
