---
title: Téléchargement des fichiers PDF
description: Découvrez comment télécharger les fichiers PDF associés à un catalogue électronique.
uuid: 9e178bb2-ac09-427a-b61a-aad4e87a5837
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0097cba5-c886-4115-bc35-7ae7a500202f
feature: Dynamic Media Classic, Visionneuses, Catalogue électronique
role: Business Practitioner
exl-id: a787d6b5-48c8-4cf7-b136-60ba3d3eb2f2
translation-type: tm+mt
source-git-commit: 7456226cf6469f40e66ff327475d4c605b6d6e13
workflow-type: tm+mt
source-wordcount: '699'
ht-degree: 56%

---

# Téléchargement des fichiers PDF{#uploading-the-pdf-files}

En règle générale, les fichiers Adobe PDF sont la source d’un catalogue électronique. Ces fichiers contiennent toutes les informations sur les images, les polices et les graphiques vectoriels. Néanmoins, rien ne vous empêche de créer un catalogue électronique à partir d’images. Après avoir préparé vos fichiers PDF pour le téléchargement, cliquez sur le bouton Télécharger de la barre de navigation globale pour lancer le téléchargement des fichiers.

## Préparation des fichiers PDF  {#preparing-your-pdf-files}

Préparez vos fichiers PDF avant de les télécharger vers Dynamic Media Classic :

* Pour faciliter le téléchargement des fichiers, placez tous les fichiers dans le même dossier sur votre ordinateur ou votre réseau.
* Nommez les fichiers selon un ordre alphanumérique, par page. L’organisation des pages selon un ordre donné facilite leur bon assemblage après le téléchargement des fichiers.
* Pour savoir si les pages PDF contiennent des traits de coupe, des cibles d’enregistrement ou des barres de couleurs, examinez les pages. Ces marques indiquent où couper le papier lorsque les documents sont imprimés et doivent impérativement être supprimées avant le placement du catalogue électronique sur le Web. Dynamic Media Classic propose des options de recadrage des marques lorsque vous téléchargez des fichiers PDF.
* Si vous souhaitez que les utilisateurs puissent effectuer des recherches par mot-clé dans votre catalogue électronique, déterminez si vos fichiers PDF sont aplatis. Il est impossible d’extraire des mots de recherche dans des fichiers PDF aplatis. Pour savoir si un fichier PDF est aplati, essayez de sélectionner le texte qu’il contient. Si le texte n’est pas sélectionnable, le fichier PDF est aplati. Les utilisateurs ne peuvent donc pas effectuer de recherches par mot-clé dans votre catalogue électronique.
* Les fichiers PDF étant destinés à l’impression, ils contiennent le plus souvent des images CMJN. Par défaut, Dynamic Media Classic peut détecter intelligemment ces images CMJN et les convertir à l’aide d’un profil de couleurs CMJN interne. Vous pouvez cependant utiliser un profil de couleurs personnalisé pour convertir les images CMJN.

   (voir [Profils ICC](icc-profiles.md#icc_profiles)).

## Options recommandées pour le téléchargement des fichiers PDF  {#best-practice-pdf-upload-options}

Pour obtenir des informations détaillées sur les différentes méthodes de téléchargement, voir [Téléchargement de fichiers](uploading-files.md#uploading_your_files).

Sélectionnez les fichiers à télécharger, puis sélectionnez ces options PDF *recommandées* :

* ****
RecadrerSélectionnez le menu Recadrer et choisissez Manuel si les pages contiennent des traits de coupe, des repères de montage ou d&#39;autres marques. Indiquez les valeurs de recadrage (en nombre de pixels) à partir des bords supérieur, droit, inférieur et gauche des pages. Les traits de coupe sont souvent définis sur une marge d’un demi-pouce. Supposons que vous choisissiez 150 pixels par pouce (résolution recommandée) et que vous saisissez 75, 75, 75, 75 dans les zones de texte Haut, Droite, Bas et Gauche. Dans ce cas, elle rogne un demi-pouce des marges (à 150 ppp, la moitié de 1 équivaut à 75 pixels).

* ****
TraitementSélectionnez le menu Traitement, puis choisissez Pixelliser. Il est nécessaire de pixelliser le fichier PDF afin que toutes les pages et les images soient affichées dans le catalogue électronique.

* **Extraire les mots de recherche (facultatif)**
Sélectionnez cette option si vous souhaitez que les utilisateurs puissent effectuer des recherches par mot-clé dans votre catalogue électronique.

* **Générer automatiquement un catalogue électronique à partir de plusieurs pages PDF (facultatif)**
Sélectionnez cette option pour créer automatiquement un catalogue électronique lors du téléchargement. L’écran de catalogue électronique s’affiche alors directement, et vous pouvez commencer à travailler sur votre catalogue électronique sans avoir à sélectionner préalablement les fichiers PDF et la commande Créer. Le catalogue électronique prend le nom du fichier PDF.

* ****
RésolutionDynamic Media Classic recommande 150 pixels par pouce.

* ****
ColorspaceDynamic Media Classic recommande de choisir Détecter automatiquement. En règle générale, les fichiers PDF destinés à l’impression sont créés dans l’espace colorimétrique CMJN, tandis que ceux conçus pour le Web le sont dans l’espace RVB. Si un fichier PDF utilise les deux espaces colorimétriques, vous pouvez opter pour l’utilisation de l’un de ces espaces en choisissant l’option Forcer comme RVB ou Forcer comme CMJN. Les fichiers PDF utilisent les deux espaces de couleurs lorsqu’ils contiennent des graphiques CMJN et des images RVB, par exemple. Si vous avez téléchargé un profil ICC, son nom s’affiche dans le menu Espace colorimétrique, où vous pouvez le sélectionner à votre convenance.

   (voir [Profils ICC](icc-profiles.md#icc_profiles)).

* **Profil**
de couleursChoisissez une option de Profil de couleurs :

* **Convertir en**
conversions SRGBConververs SRVB (Standard Red Green Blue). SRVB est l’espace colorimétrique recommandé pour l’affichage d’images sur les pages Web.

* **Conserver l’**
espace colorimétrique d’origineConserve l’espace colorimétrique d’origine.

* **Personnalisé de >**
ÀOuvre les menus afin que vous puissiez choisir un espace colorimétrique Convertir à partir de et Convertir en. Vous pouvez choisir un espace colorimétrique Photoshop standard ou un espace colorimétrique que vous avez téléchargé vers Dynamic Media Classic.

(voir [Profils ICC](icc-profiles.md#icc_profiles)).

>[!NOTE]
>
>pour plus d’informations sur toutes les options PDF, voir [Options de téléchargement des fichiers PDF](pdfs.md#pdf_upload_options).
