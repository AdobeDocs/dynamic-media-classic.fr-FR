---
title: Polices
seo-title: Polices
description: 'null'
seo-description: Découvrez comment utiliser les polices dans Dynamic Media Classic.
uuid: bddec 9 c 2-8530-4 bbd -8 db 7-1562 a 347 e 482
contentOwner: admin
content-type: référence
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/support_ files
discoiquuid: 97 cecd 6 a -30 aa -44 fe-a 611-fd 71 b 02 fd 5 ae
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Polices{#fonts}

Dans certains cas, Scene7 Publishing System requiert le téléchargement d’un fichier de polices pour la saisie ou la restitution du texte dans une police particulière. Par exemple, pour composer le texte d’un modèle de calque dans une police donnée, téléchargez le fichier de polices. Pour afficher la numérotation des pages de la visionneuse de catalogue électronique dans une police spécifique, téléchargez le fichier de polices.

Dynamic Media Classic prend en charge les types de police suivants :

* Ensemble des polices TrueType
* Polices postscript®
* Polices OpenType/TrueType
* Polices OpenType/PostScript
* PhotoFonts

Une fois que le fichier de polices a été téléchargé, vous pouvez modifier son ID SPS, le nom de la police et les informations de type dans l’écran Modifier les infos.

>[!NOTE]
>
>Dynamic Media Classic recommande de télécharger tous les styles de police (gras, italique, gras/italique et normal) si vous prévoyez d'utiliser des polices dans des calques de modèle. Dynamic Media Classic requiert ces styles de police pour traiter les requêtes. Il est également recommandé de télécharger tous les fichiers PostScript/Adobe Type 1 associés à une police dans la mesure où certaines polices contiennent des informations de crénage détaillées.

## Téléchargement de fichiers de polices {#uploading-font-files}

Téléchargez les fichiers de polices en procédant de la même façon que pour le téléchargement d’autres fichiers. Vous pouvez stocker des fichiers de polices dans n’importe quel dossier SPS (voir [Téléchargement de fichiers](uploading-files.md#uploading_your_files)).

## Edition d’informations de fichiers de polices {#editing-font-file-information}

Vous pouvez modifier l’ID d’une police ainsi que les informations de type correspondantes. La modification d’un fichier de polices peut servir à effectuer des recherches et à identifier plus facilement les polices.

Dans le panneau de navigation, sélectionnez le fichier de polices à modifier dans la vue Affichage des détails, puis choisissez la commande Fichier &gt; Modifier les informations. L’écran Editer les informations apparaît. Choisissez les options ci-dessous, puis sélectionnez le bouton Envoyer.

**Nom de la police** Ce nom identifie la police lorsqu'elle est publiée.

**Nom postscript** Ce nom correspond au nom postscript complet de la police. Il indique généralement la graisse ou le style.

**Nom RTF** Ce nom apparaît dans un menu contextuel de l'éditeur RTF dans lequel sont créées les calques de texte de modèle.

**Nom de la famille de polices** Ce nom répertorie le nom de la police sans l'indicateur de style, de poids ou de police.

**Style de police** Les options sont les suivantes : Normal, Gras, Italique et Gras-Italique.

**Type** de police Les options sont truetype et Adobe Type - 1. Si vous renommez ces polices, vous pouvez l’indiquer.

**Abréviation de type de police** Les options sont les suivantes :

**Fichiers de polices TTF** truetype utilisés pour le rendu PDF/postscript et la diffusion d'images.

**Fichiers de polices AFM** Adobe postscript contenant des informations Adobe Font Metrics et utilisés pour la diffusion d'images.

**Fichiers de police PFM** Adobe postscript contenant des informations binaires sur les polices.

**Fichiers de police PFB** Adobe postscript contenant des informations de contour de police binaires et utilisés pour le rendu PDF/postscript et la diffusion d'images.
