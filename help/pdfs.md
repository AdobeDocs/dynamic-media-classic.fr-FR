---
title: Utilisation de documents PDF
description: Découvrez comment utiliser des PDF dans Dynamic Media Classic.
uuid: 26d70d28-9393-49b1-9051-d70456deca67
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 5a073de3-6b1d-4c3e-8c03-9182f9f3874a
feature: Dynamic Media Classic,Asset Management
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 55%

---


# Utilisation de documents PDF{#working-with-pdfs}

Les fichiers PDF (Portable Document Format) sont le plus souvent utilisés dans Dynamic Media Classic pour créer des catalogues électroniques. Lorsque vous téléchargez un fichier PDF, Dynamic Media Classic pixellise les pages par défaut afin que les pages puissent être utilisées pour créer un média enrichi.

## Options de téléchargement des fichiers PDF {#pdf-upload-options}

Lorsque vous téléchargez un fichier PDF, vous pouvez le formater de différentes manières. Vous pouvez recadrer les pages, extraire des mots de recherche, spécifier une résolution en pixels par pouce et choisir un espace colorimétrique. Les fichiers PDF contiennent souvent une marge de rognage, des traits de coupe, des repères de montage et autres repères d’impression. Vous pouvez éliminer ces marques sur les côtés des pages lorsque vous téléchargez un fichier PDF.

Les options de téléchargement des fichiers PDF sont regroupées sous la section Options PDF de l’écran de téléchargement.

**Traitement**

Les options de traitement sont les suivantes :

**Pixelliser**  (par défaut) Pixellise les pages du fichier PDF et convertit les graphiques vectoriels en images bitmap. Choisissez cette option pour créer un catalogue électronique. 

**Extraire les** mots de rechercheExtrait les mots du fichier PDF afin que le fichier puisse être recherché par mot-clé dans une visionneuse de catalogue électronique.

**Extraire les** liensExtrait les liens des fichiers PDF et les convertit en zones cliquables utilisées dans une visionneuse de catalogue électronique.

**Générer automatiquement un catalogue électronique avec plusieurs pages** PDFAcrée automatiquement un catalogue électronique à partir du fichier PDF. Le catalogue électronique reprend le nom du fichier PDF que vous avez téléchargé (cette option n’est disponible que si vous pixellisez le fichier PDF au moment du téléchargement).

**Résolution**

Détermine le paramètre de résolution, qui définit le nombre de pixels affichés par pouce dans le fichier PDF. La valeur par défaut est de 150.

**Espace colorimétrique**

Dans le menu Espace colorimétrique, choisissez un espace pour le fichier PDF. La plupart des fichiers PDF contiennent des images en couleurs RVB et CMJN. L’espace colorimétrique RVB est préférable pour un affichage à l’écran.

**Détecter** automatiquementConserve l’espace colorimétrique du fichier PDF.

**Forcer comme** RGBConversion vers l’espace colorimétrique RVB.

**Forcer comme** CMJNonversion vers l’espace colorimétrique CMJN.

**Forcer comme** Niveaux de grisConvertit dans l’espace colorimétrique Niveaux de gris.

**Profil de couleurs**

Choisissez une option de profil de couleurs :

**Convertir en** conversions RVBonververs sRVB (rouge vert bleu standard). sRVB est l’espace colorimétrique recommandé pour l’affichage d’images sur les pages Web.

**Conserver l’** espace colorimétrique d’origineConserve l’espace colorimétrique d’origine.

**Personnalisé de >** ÀOuvre les menus afin que vous puissiez choisir un espace colorimétrique Convertir à partir de et Convertir en. Vous pouvez choisir un espace colorimétrique Photoshop standard ou un espace colorimétrique que vous avez téléchargé vers Dynamic Media Classic.

(voir [Profils ICC](icc-profiles.md#icc_profiles)).

## Suppression de l’espace blanc d’un fichier PDF  {#cropping-white-space-from-a-pdf-file}

1. Pour supprimer automatiquement les pixels d’espace blanc d’un fichier PDF au moment du téléchargement, sélectionnez le menu Recadrer, puis choisissez Rogner.
1. Spécifiez les options suivantes :

   **Rogner en fonction de** l’état Choisissez si vous souhaitez effectuer un rognage en fonction de la couleur ou de la transparence :

   **** CouleurChoisissez l&#39;option Couleur. Sélectionnez ensuite le menu Coin, puis choisissez l’angle du fichier PDF présentant la couleur qui correspond le mieux à l’espace blanc à rogner.

   **** TransparenceSélectionnez l&#39;option Transparence.

   **** ToléranceFaites glisser le curseur pour spécifier une tolérance comprise entre 0 et 1 :

   **Rognage en fonction de la** couleurIndiquez 0 pour rogner les pixels uniquement s’ils correspondent exactement à la couleur que vous avez sélectionnée dans l’angle du PDF. Les valeurs qui se rapprochent de 1 admettent un plus grand écart des couleurs.

   **Rognage basé sur la** transparenceSpécifiez 0 pour rogner les pixels uniquement s’ils sont entièrement transparents ; les valeurs plus proches de 1 permettent une plus grande transparence.

## Recadrage à partir des côtés des pages PDF {#cropping-from-the-sides-of-pdf-pages}

Vous pouvez supprimer manuellement les repères d’impression sur les côtés des pages d’un fichier PDF au moment du téléchargement.

1. Dans le menu Recadrer, choisissez Manuel.
1. Entrez les valeurs en pixels dans les zones de texte pour les bords supérieur, droit, inférieur et gauche de manière à recadrer à partir du haut, du bas et des côtés des pages.

La proportion de la page rognée dépend du paramètre de résolution px/pouce (pixels par pouce) que vous spécifiez pour le fichier PDF. Par exemple, si vous entrez 150 (valeur par défaut) comme résolution px/pouce et que vous rognez 75 pixels sur les côtés des pages, un demi-pouce est rogné sachant que, à une résolution de 150 pixels par pouce, 75 pixels correspondent à la moitié d’un pouce.
