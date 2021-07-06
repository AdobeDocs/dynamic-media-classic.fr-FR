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
role: User
exl-id: 186f4c7f-16f6-42f5-bc0e-55362c55e794
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 36%

---

# Polices{#fonts}

Parfois, Dynamic Media Classic nécessite de charger un fichier de police pour saisir ou effectuer le rendu du texte dans une police donnée. Par exemple, pour composer le texte d’un modèle de calque dans une police donnée, téléchargez le fichier de polices. Pour afficher la numérotation des pages de la visionneuse de catalogue électronique dans une police spécifique, téléchargez le fichier de polices.

Dynamic Media Classic prend en charge les types de police suivants :

* Ensemble des polices TrueType
* Polices PostScript®
* Polices OpenType/TrueType
* Polices OpenType/PostScript
* PhotoFonts

Une fois le fichier de police chargé, vous pouvez modifier son identifiant Dynamic Media Classic, son nom et saisir des informations dans l’écran Modifier les informations.

>[!NOTE]
>
>Dynamic Media Classic recommande de charger tous les styles de police (gras, italique, gras/italique et normal) si vous prévoyez d’utiliser des polices dans les calques de modèle. Dynamic Media Classic a besoin de ces styles de police pour traiter les demandes. Il est également recommandé de télécharger tous les fichiers PostScript/Adobe Type 1 associés à une police dans la mesure où certaines polices contiennent des informations de crénage détaillées.

## Téléchargement de fichiers de polices {#uploading-font-files}

Téléchargez les fichiers de polices en procédant de la même façon que pour le téléchargement d’autres fichiers. Vous pouvez stocker les fichiers de polices dans n’importe quel dossier Dynamic Media Classic. (voir [Téléchargement de fichiers](uploading-files.md#uploading_your_files)).

## Edition d’informations de fichiers de polices {#editing-font-file-information}

Vous pouvez modifier le nom d’identifiant d’une police et ses informations de type. La modification d’un fichier de polices peut servir à effectuer des recherches et à identifier plus facilement les polices.

Dans le panneau de navigation, sélectionnez le fichier de polices à modifier dans la vue Affichage des détails, puis choisissez la commande Fichier > Modifier les informations. L’écran Editer les informations apparaît. Choisissez les options ci-dessous, puis sélectionnez le bouton Envoyer.

* **Nom de la police**  : ce nom identifie la police lors de sa publication.

* **Nom PostScript**  : il s’agit du nom PostScript complet de la police. Il indique généralement la graisse ou le style.

* **Nom RTF**  : ce nom apparaît dans un menu contextuel de l’éditeur RTF où sont créées les calques de texte de modèle.

* **Nom de famille de polices**  : ce nom répertorie le nom de la police sans indicateur de style, de poids ou de type de police.

* **Style de police**  : les options sont les suivantes : clair, gras, italique et gras-italique.

* **Type de police**  : les options sont TrueType et Adobe Type 1. Si vous renommez ces polices, vous pouvez l’indiquer.

* **Abréviation**  du type de police : les options sont les suivantes :

   * **** Fichiers de police TTFrueType utilisés pour le rendu PDF/PostScript et la diffusion d’images.

   * **** Fichiers de polices PostScript AFMAdobe contenant des informations sur les mesures de polices d’Adobe et utilisés pour la diffusion d’images.

   * **** Fichiers de police PDF PostScript Adobe contenant des informations de mesure de police binaire.

   * **** Fichiers de police PDF PostScript Adobe contenant des informations de contour de police binaires et utilisés pour le rendu PDF/PostScript et la diffusion d’images.
