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

Parfois, Adobe Dynamic Media Classic exige que vous chargiez un fichier de police pour saisir ou générer du texte dans une police particulière. Par exemple, pour composer le texte d’un modèle de calque dans une police donnée, téléchargez le fichier de polices. Pour afficher la numérotation des pages de la visionneuse de catalogue électronique dans une police spécifique, téléchargez le fichier de polices.

Adobe Dynamic Media Classic prend en charge les types de polices suivants :

* Ensemble des polices TrueType
* Polices PostScript®
* Polices OpenType/TrueType
* Polices OpenType/PostScript
* PhotoFonts

Une fois un fichier de police téléchargé, vous pouvez modifier son identifiant Adobe Dynamic Media Classic, son nom et ses informations de saisie dans l’écran Modifier les informations .

>[!NOTE]
>
>Adobe Dynamic Media Classic recommande de charger tous les styles de polices (gras, italique, gras/italique et standard) si vous envisagez d’utiliser des polices dans les calques de modèle. Adobe Dynamic Media Classic a besoin de ces styles de police pour traiter les requêtes. Il est également recommandé de télécharger tous les fichiers `PostScript/Adobe Type1` associés à une police, car certaines de ces polices contiennent des informations de crénage détaillées.

## Chargement des fichiers de polices {#uploading-font-files}

Téléchargez les fichiers de polices en procédant de la même façon que pour le téléchargement d’autres fichiers. Vous pouvez stocker des fichiers de polices dans n’importe quel dossier Adobe Dynamic Media Classic. (voir [Téléchargement de fichiers](uploading-files.md#uploading_your_files)).

## Modifier les informations du fichier de polices {#editing-font-file-information}

Vous pouvez modifier le nom de l’identifiant d’une police et ses informations de type. La modification d’un fichier de polices peut servir à effectuer des recherches et à identifier plus facilement les polices.

Dans le panneau de navigation, sélectionnez le fichier de police que vous souhaitez modifier dans la vue détaillée et choisissez Fichier > Modifier les informations. L’écran Editer les informations apparaît. Choisissez les options suivantes, puis sélectionnez **[!UICONTROL Envoyer]**.

* **[!UICONTROL Nom de la police]** : ce nom identifie la police lors de sa publication.

* **[!UICONTROL Nom du PostScript]** : il s’agit du nom PostScript complet de la police. Il indique généralement la graisse ou le style.

* **[!UICONTROL Nom RTF]** : ce nom apparaît dans un menu pop-up de l’éditeur RTF où les calques de texte du modèle sont créés.

* **[!UICONTROL Nom de famille de polices]** : ce nom répertorie le nom de la police sans l’indicateur de style, d’épaisseur ou de type de police.

* **[!UICONTROL Style de police]** : les options disponibles sont Gras, Gras, Italique et Gras-Italique.

* **[!UICONTROL Type de police]** : les options sont TrueType et Adobe Type 1. Si vous renommez ces polices, vous pouvez l’indiquer.

* **[!UICONTROL Abréviation du type de police]** : les options sont les suivantes :

   * **[!UICONTROL TTF]** : fichiers de polices TrueType utilisés pour le rendu PDF/PostScript et la diffusion d’images.

   * **[!UICONTROL AEM]** : fichiers de polices Adobe PostScript contenant des informations sur les mesures de polices Adobe et utilisés pour la diffusion d’images.

   * **[!UICONTROL PFM]** : fichiers de polices Adobe PostScript contenant des informations sur les mesures de polices binaires.

   * **[!UICONTROL PFB]** : fichiers de polices Adobe PostScript contenant des informations de contour de police binaire et utilisés pour le rendu et la diffusion d’images PDF/PostScript.
