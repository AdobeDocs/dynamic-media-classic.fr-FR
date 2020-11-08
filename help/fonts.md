---
title: Polices
seo-title: Polices
description: 'null'
seo-description: Découvrez comment utiliser les polices dans Dynamic Media Classic.
uuid: bddec9c2-8530-4bbd-8db7-1562a347e482
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 97cecd6a-30aa-44fe-a611-fd71b02fd5ae
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 40%

---


# Polices{#fonts}

Dans certains cas, Dynamic Media Classic vous demande de télécharger un fichier de police pour entrer ou rendre du texte dans une police particulière. Par exemple, pour composer le texte d’un modèle de calque dans une police donnée, téléchargez le fichier de polices. Pour afficher la numérotation des pages de la visionneuse de catalogue électronique dans une police spécifique, téléchargez le fichier de polices.

Dynamic Media Classic prend en charge les types de police suivants :

* Ensemble des polices TrueType
* PostScript® de polices
* Polices OpenType/TrueType
* Polices OpenType/PostScript
* PhotoFonts

Après avoir téléchargé un fichier de polices, vous pouvez modifier son identifiant Dynamic Media Classic, son nom et les informations de type dans l’écran Modifier les infos.

>[!NOTE]
>
>Dynamic Media Classic recommande de télécharger tous les styles de police (gras, italique, gras/italique et normal) si vous prévoyez d’utiliser des polices dans les calques de modèle. Dynamic Media Classic a besoin de ces styles de police pour traiter les requêtes. Il est également recommandé de télécharger tous les fichiers PostScript/Adobe Type 1 associés à une police dans la mesure où certaines polices contiennent des informations de crénage détaillées.

## Téléchargement de fichiers de polices {#uploading-font-files}

Téléchargez les fichiers de polices en procédant de la même façon que pour le téléchargement d’autres fichiers. Vous pouvez stocker des fichiers de polices dans n’importe quel dossier Dynamic Media Classic. (voir [Téléchargement de fichiers](uploading-files.md#uploading_your_files)).

## Edition d’informations de fichiers de polices {#editing-font-file-information}

Vous pouvez modifier l’ID d’une police ainsi que les informations de type correspondantes. La modification d’un fichier de polices peut servir à effectuer des recherches et à identifier plus facilement les polices.

Dans le panneau de navigation, sélectionnez le fichier de polices à modifier dans la vue Affichage des détails, puis choisissez la commande Fichier > Modifier les informations. L’écran Editer les informations apparaît. Choisissez les options ci-dessous, puis sélectionnez le bouton Envoyer.

**Nom** de la police Ce nom identifie la police lors de sa publication.

**Nom** PostScript Ce nom correspond au nom PostScript complet de la police. Il indique généralement la graisse ou le style.

**Nom** RTF Ce nom s’affiche dans un menu contextuel de l’éditeur RTF où sont créés les modèles de calques de texte.

**Nom** de la famille de polices Ce nom liste le nom de la police sans indicateur de style, de poids ou de type de police.

**Style** de police Les options sont les suivantes : Normal, Gras, Italique et Gras-Italique.

**Type** de police Les options sont TrueType et Type d&#39;Adobe 1. Si vous renommez ces polices, vous pouvez l’indiquer.

**Abréviation** du type de police Les options sont les suivantes :

**Fichiers de police TTF** TrueType utilisés pour le rendu PDF/PostScript et la diffusion d’images.

**Les fichiers de police AFM** Adobe PostScript qui contiennent des informations sur les mesures de police de l’Adobe et sont utilisés pour la diffusion d’images.

**Fichiers de police Adobe PostScript PFM** qui contiennent des informations binaires sur les mesures de police.

**Les fichiers de police PFB** Adobe PostScript qui contiennent des informations de contour de police binaires et sont utilisés pour le rendu PDF/PostScript et la diffusion d’images.
