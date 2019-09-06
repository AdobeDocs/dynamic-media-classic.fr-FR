---
title: Téléchargement des fichiers PDF
seo-title: Téléchargement des fichiers PDF
description: 'null'
seo-description: Découvrez comment télécharger les fichiers PDF associés à un catalogue électronique.
uuid: 9 e 178 bb 2-ac 09-427 a-b 61 a-aad 4 e 87 a 5837
contentOwner: admin
content-type: référence
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
discoiquuid: 0097 cba 5-c 886-4115-bc 35-7 ae 7 a 500202 f
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Téléchargement des fichiers PDF{#uploading-the-pdf-files}

En règle générale, un catalogue électronique est créé à partir de fichiers Adobe PDF ; ces fichiers contiennent l’ensemble des informations relatives aux images, ainsi que les polices et les graphiques vectoriels. Néanmoins, rien ne vous empêche de créer un catalogue électronique à partir d’images. Après avoir préparé vos fichiers PDF pour le téléchargement, cliquez sur le bouton Télécharger de la barre de navigation globale pour lancer le téléchargement des fichiers.

## Préparation des fichiers PDF {#preparing-your-pdf-files}

Préparez vos fichiers PDF avant de les télécharger vers Scene7 Publishing System :

* Placez tous les fichiers dans le même dossier sur votre ordinateur ou votre réseau pour faciliter leur téléchargement.
* Nommez les fichiers selon un ordre alphanumérique, par page. L’organisation des pages selon un ordre donné facilite leur bon assemblage après le téléchargement des fichiers.
* Examinez les pages PDF afin de vérifier si elles contiennent des traits de coupe, des repères de montage ou des gammes de couleurs. Ces marques indiquent où couper le papier lorsque les documents sont imprimés et doivent impérativement être supprimées avant le placement du catalogue électronique sur le Web. Dynamic Media Classic propose des options de suppression des marques lorsque vous téléchargez des fichiers PDF.
* Si vous souhaitez que les utilisateurs puissent effectuer des recherches par mot-clé dans votre catalogue électronique, déterminez si vos fichiers PDF sont aplatis. Il est impossible d’extraire des mots de recherche dans des fichiers PDF aplatis. Pour savoir si un fichier PDF est aplati, essayez de sélectionner le texte qu’il contient. Si le texte n’est pas sélectionnable, le fichier PDF est aplati. Les utilisateurs ne peuvent donc pas effectuer de recherches par mot-clé dans votre catalogue électronique.
* Les fichiers PDF étant destinés à l’impression, ils contiennent le plus souvent des images CMJN. Par défaut, Scene7 Publishing System peut détecter les images CMJN et les convertir à l’aide d’un profil de couleurs CMJN interne. Vous pouvez cependant utiliser un profil de couleurs personnalisé pour convertir les images CMJN.

   (voir [Profils ICC](icc-profiles.md#icc_profiles)).

## Options recommandées pour le téléchargement des fichiers PDF {#best-practice-pdf-upload-options}

Pour obtenir des informations détaillées sur les différentes méthodes de téléchargement, voir [Téléchargement de fichiers](uploading-files.md#uploading_your_files).

Sélectionnez les fichiers à télécharger, puis sélectionnez ces options PDF *recommandées* :

**Recadrez** le menu Recadrer, puis choisissez Manuel si les pages contiennent des traits de coupe, des repères de montage ou d'autres marques. Indiquez les valeurs de recadrage (en nombre de pixels) à partir des bords supérieur, droit, inférieur et gauche des pages. En règle générale, les traits de coupe sont définis sur une marge d’un demi-pouce. Supposons que vous choisissiez une résolution de 150 pixels par pouce (valeur recommandée), si vous entrez 75, 75, 75, 75 dans les zones de texte Bord supérieur, Droite, Bord inférieur et Gauche, les marges sont recadrées d’un demi-pouce (à 150 ppp, la moitié d’un pouce équivaut à 75 pixels).

**Traitement** Sélectionnez le menu Traitement et choisissez Pixelliser. Il est nécessaire de pixelliser le fichier PDF afin que toutes les pages et les images soient affichées dans le catalogue électronique.

**Extraire les mots de recherche (facultatif)** Sélectionnez cette option si vous souhaitez que les utilisateurs puissent effectuer des recherches par mot-clé dans votre catalogue électronique.

**Générer automatiquement un catalogue électronique à partir de plusieurs pages PDF (facultatif)** Sélectionnez cette option pour créer automatiquement un catalogue électronique lors du téléchargement. L’écran de catalogue électronique s’affiche alors directement, et vous pouvez commencer à travailler sur votre catalogue électronique sans avoir à sélectionner préalablement les fichiers PDF et la commande Créer. Le catalogue électronique prend le nom du fichier PDF.

**La résolution** dynamique de Media Classic recommande 150 pixels par pouce.

**Colorspace** Dynamic Media Classic recommande de choisir Détecter automatiquement. En règle générale, les fichiers PDF destinés à l’impression sont créés dans l’espace colorimétrique CMJN, tandis que ceux conçus pour le Web le sont dans l’espace RVB. Si un fichier PDF utilise les deux espaces colorimétriques, vous pouvez opter pour l’utilisation de l’un de ces espaces en choisissant l’option Forcer comme RVB ou Forcer comme CMJN. Les fichiers PDF utilisent les deux espaces de couleurs lorsqu’ils contiennent des graphiques CMJN et des images RVB, par exemple. Si vous avez téléchargé un profil ICC, son nom s’affiche dans le menu Espace colorimétrique, où vous pouvez le sélectionner à votre convenance.

(voir [Profils ICC](icc-profiles.md#icc_profiles)).

**Profil de couleurs** Choisissez une option Profil de couleurs :

**Convertir
en SRVB** Convertit en SRVB (rouge vert vert standard). SRVB est l’espace colorimétrique recommandé pour l’affichage d’images sur les pages Web.

**Conserver l'espace colorimétrique original** Conserve l'espace colorimétrique d'origine.

**Personnalisé De &gt; Pour** ouvrir les menus, vous pouvez choisir un espace colorimétrique Convertir à partir de et Convertir en couleurs. Vous pouvez choisir un espace colorimétrique Photoshop standard ou un espace colorimétrique téléchargé sur SPS.

(voir [Profils ICC](icc-profiles.md#icc_profiles)).

>[!NOTE]
>
>pour plus d’informations sur toutes les options PDF, voir [Options de téléchargement des fichiers PDF](pdfs.md#pdf_upload_options).

