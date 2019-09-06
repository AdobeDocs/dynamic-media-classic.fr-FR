---
title: Utilisation de documents PDF
seo-title: Utilisation de documents PDF
description: 'null'
seo-description: Découvrez comment travailler avec des fichiers PDF dans Dynamic Media Classic.
uuid: 26 d 70 d 28-9393-49 b 1-9051-d 70456 deca 67
contentOwner: admin
content-type: référence
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/master_ files
discoiquuid: 5 a 073 de 3-6 b 1 d -4 c 3 e -8 c 03-9182 f 9 f 3874 a
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Utilisation de documents PDF{#working-with-pdfs}

Les fichiers PDF (Portable Document Format) sont généralement utilisés dans Dynamic Media Classic pour créer des catalogues électroniques. Lorsque vous téléchargez un fichier PDF, Dynamic Media Classic pixellise les pages par défaut, de sorte que les pages puissent être utilisées pour créer un média enrichi.

## Options de téléchargement des fichiers PDF {#pdf-upload-options}

Lorsque vous téléchargez un fichier PDF, vous pouvez le formater de différentes manières. Vous pouvez recadrer les pages, extraire des mots de recherche, spécifier une résolution en pixels par pouce et choisir un espace colorimétrique. Les fichiers PDF contiennent souvent une marge de rognage, des traits de coupe, des repères de montage et autres repères d’impression. Vous pouvez éliminer ces marques sur les côtés des pages lorsque vous téléchargez un fichier PDF.

Les options de téléchargement des fichiers PDF sont regroupées sous la section Options PDF de l’écran de téléchargement.

**Traitement**

Les options de traitement sont les suivantes :

**Pixelliser** (par défaut) Pixellise les pages du fichier PDF et convertit les graphiques vectoriels en images bitmap. Choisissez cette option pour créer un catalogue électronique. 

**Extraire les mots de recherche** Extrait les mots du fichier PDF de sorte que le fichier puisse être recherché par mot-clé dans une visionneuse de catalogue électronique.

**Extraction des liens** Extrait les liens des fichiers PDF et les convertit en zones cliquables utilisées dans une visionneuse de catalogue électronique.

**Générer automatiquement un catalogue électronique avec plusieurs pages PDF** Crée automatiquement un catalogue électronique à partir du fichier PDF. Le catalogue électronique reprend le nom du fichier PDF que vous avez téléchargé (cette option n’est disponible que si vous pixellisez le fichier PDF au moment du téléchargement).

**Résolution**

Détermine le paramètre de résolution, qui définit le nombre de pixels affichés par pouce dans le fichier PDF. La valeur par défaut est de 150.

**Espace colorimétrique**

Dans le menu Espace colorimétrique, choisissez un espace pour le fichier PDF. La plupart des fichiers PDF contiennent des images en couleurs RVB et CMJN. L’espace colorimétrique RVB est préférable pour un affichage à l’écran.

**Détecter automatiquement** l'espace colorimétrique du fichier PDF.

**Forcer comme** conversions RVB dans l'espace colorimétrique RVB.

**Forcer comme** conversions CMJN dans l'espace colorimétrique CMJN.

**Forcer comme conversions en niveaux de gris** dans l'espace colorimétrique Niveaux de gris.

**Profil de couleurs**

Choisissez une option de profil de couleurs :

**Convertir en srvb** Convertit en srvb (rouge vert vert standard). sRVB est l’espace colorimétrique recommandé pour l’affichage d’images sur les pages Web.

**Conserver l'espace colorimétrique original** Conserve l'espace colorimétrique d'origine.

**Personnalisé De &gt; Pour** ouvrir les menus, vous pouvez choisir un espace colorimétrique Convertir à partir de et Convertir en couleurs. Vous pouvez choisir un espace colorimétrique Photoshop standard ou un espace colorimétrique téléchargé sur SPS.

(voir [Profils ICC](icc-profiles.md#icc_profiles)).

## Suppression de l’espace blanc d’un fichier PDF {#cropping-white-space-from-a-pdf-file}

1. Pour supprimer automatiquement les pixels d’espace blanc d’un fichier PDF au moment du téléchargement, sélectionnez le menu Recadrer, puis choisissez Rogner.
1. Spécifiez les options suivantes :

   **Rogner selon** le choix de recadrer selon la couleur ou la transparence :

   **Couleur** Choisissez l'option Couleur. Sélectionnez ensuite le menu Coin, puis choisissez l’angle du fichier PDF présentant la couleur qui correspond le mieux à l’espace blanc à rogner.

   **Transparence** Choisissez l'option Transparence.

   **Tolérance** Faites glisser le curseur pour définir une valeur de tolérance comprise entre 0 et 1 :

   **Rognage selon la couleur** Indiquez 0 pour rogner les pixels uniquement s'ils correspondent exactement à la couleur sélectionnée dans l'angle du PDF. Les valeurs qui se rapprochent de 1 admettent un plus grand écart des couleurs.

   **Rognage selon la transparence** Indiquez 0 pour rogner les pixels uniquement s'ils sont entièrement transparents ; les valeurs plus proches de 1 permettent une plus grande transparence.

## Recadrage à partir des côtés des pages PDF {#cropping-from-the-sides-of-pdf-pages}

Vous pouvez supprimer manuellement les repères d’impression sur les côtés des pages d’un fichier PDF au moment du téléchargement.

1. Dans le menu Recadrer, choisissez Manuel.
1. Entrez les valeurs en pixels dans les zones de texte pour les bords supérieur, droit, inférieur et gauche de manière à recadrer à partir du haut, du bas et des côtés des pages.

La proportion de la page rognée dépend du paramètre de résolution px/pouce (pixels par pouce) que vous spécifiez pour le fichier PDF. Par exemple, si vous entrez 150 (valeur par défaut) comme résolution px/pouce et que vous rognez 75 pixels sur les côtés des pages, un demi-pouce est rogné sachant que, à une résolution de 150 pixels par pouce, 75 pixels correspondent à la moitié d’un pouce.
