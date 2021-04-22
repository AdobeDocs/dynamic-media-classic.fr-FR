---
title: Polices
description: Découvrez comment utiliser les polices dans Dynamic Media Classic.
uuid: bddec9c2-8530-4bbd-8db7-1562a347e482
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 97cecd6a-30aa-44fe-a611-fd71b02fd5ae
feature: Dynamic Media Classic
role: Business Practitioner
exl-id: 186f4c7f-16f6-42f5-bc0e-55362c55e794
translation-type: tm+mt
source-git-commit: 27d9a9b9f158846b54e4318119aec9e4dc9c4c0d
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 36%

---

# Polices{#fonts}

Dynamic Media Classic vous demande parfois de télécharger un fichier de police pour entrer ou rendre du texte dans une police particulière. Par exemple, pour composer le texte d’un modèle de calque dans une police donnée, téléchargez le fichier de polices. Pour afficher la numérotation des pages de la visionneuse de catalogue électronique dans une police spécifique, téléchargez le fichier de polices.

Dynamic Media Classic prend en charge les types de police suivants :

* Ensemble des polices TrueType
* PostScript® de polices
* Polices OpenType/TrueType
* Polices OpenType/PostScript
* PhotoFonts

Après avoir téléchargé un fichier de polices, vous pouvez modifier son ID Dynamic Media Classic, son nom et les informations de type dans l’écran Modifier les infos.

>[!NOTE]
>
>Dynamic Media Classic recommande de télécharger tous les styles de police (gras, italique, gras/italique et normal) si vous prévoyez d’utiliser des polices dans les calques de modèle. Dynamic Media Classic a besoin de ces styles de police pour traiter les requêtes. Il est également recommandé de télécharger tous les fichiers PostScript/Adobe Type 1 associés à une police dans la mesure où certaines polices contiennent des informations de crénage détaillées.

## Téléchargement de fichiers de polices  {#uploading-font-files}

Téléchargez les fichiers de polices en procédant de la même façon que pour le téléchargement d’autres fichiers. Vous pouvez stocker des fichiers de polices dans n’importe quel dossier Dynamic Media Classic. (voir [Téléchargement de fichiers](uploading-files.md#uploading_your_files)).

## Edition d’informations de fichiers de polices  {#editing-font-file-information}

Vous pouvez modifier le nom d’ID d’une police et ses informations de type. La modification d’un fichier de polices peut servir à effectuer des recherches et à identifier plus facilement les polices.

Dans le panneau de navigation, sélectionnez le fichier de polices à modifier dans la vue Affichage des détails, puis choisissez la commande Fichier > Modifier les informations. L’écran Editer les informations apparaît. Choisissez les options ci-dessous, puis sélectionnez le bouton Envoyer.

* **Nom**  de la police : ce nom identifie la police lors de sa publication.

* **Nom**  PostScript : il s’agit du nom PostScript complet pour la police. Il indique généralement la graisse ou le style.

* **Nom**  RTF : ce nom s&#39;affiche dans un menu contextuel de l&#39;éditeur RTF où sont créés les modèles de calques de texte.

* **Nom**  de la famille de polices : ce nom liste le nom de la police sans indicateur de style, de poids ou de type de police.

* **Style**  de police : les options sont Standard, Gras, Italique et Gras-Italique.

* **Type**  de police : les options sont TrueType et Adobe Type 1. Si vous renommez ces polices, vous pouvez l’indiquer.

* **Abréviation**  du type de police : les options sont les suivantes :

   * **Fichiers de police** TTFTrueType utilisés pour le rendu PDF/PostScript et la diffusion d’images.

   * **Fichiers de police PostScript** AFMAdobe contenant des informations sur les mesures de police de l’Adobe et utilisés pour la diffusion d’images.

   * **Fichiers de police PostScript** PFMAdobe contenant des informations binaires sur les mesures de police.

   * **Les fichiers de police PostScript** PFBAdobe qui contiennent des informations de contour de police binaires et sont utilisés pour le rendu PDF/PostScript et la diffusion d’images.
