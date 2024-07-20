---
title: Utilisation de PDF
description: Découvrez comment utiliser des PDF dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 02892514-61fe-48ba-a2e3-eeb30580a1e4
topic: Integrations, Development
level: Experienced
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '726'
ht-degree: 26%

---

# Utilisation de PDF{#working-with-pdfs}

Les fichiers PDF (Portable Document Format) sont le plus souvent utilisés dans Adobe Dynamic Media Classic pour créer des catalogues électroniques. Lorsque vous chargez un fichier de PDF, Adobe Dynamic Media Classic pixellise les pages par défaut afin que les pages puissent être utilisées pour créer du contenu multimédia.

Lorsque vous chargez un PDF pour l’extraction de page, Adobe applique la limite suivante :

| Type de limite | Limite imposée | Modification de la limite le 31 décembre 2022 |
| --- | --- | --- |
| Nombre maximum de pages qu’un PDF doit prendre en compte pour l’extraction | 5000 (pour les nouveaux chargements) | 100 (pour tous les PDF) |

Voir aussi [Limites de Dynamic Media](/help/using/limitations.md).

## Options de téléchargement des fichiers PDF {#pdf-upload-options}

Lorsque vous téléchargez un fichier PDF, vous pouvez le formater de différentes manières. Vous pouvez recadrer les pages, extraire des mots de recherche, spécifier une résolution en pixels par pouce et choisir un espace colorimétrique. Les fichiers de PDF contiennent souvent une marge de rognage, des marques de recadrage, des marques d’enregistrement et d’autres marques d’imprimante. Vous pouvez éliminer ces marques sur les côtés des pages lorsque vous téléchargez un fichier PDF.

Les options de téléchargement de fichiers de PDF sont disponibles sur la page Télécharger sous les options du PDF.

### Options de traitement

**[!UICONTROL Pixelliser]** : (par défaut) Pixellise les pages du fichier du PDF et convertit les graphiques vectoriels en images bitmap. Pour créer un catalogue électronique, sélectionnez cette option.

**[!UICONTROL Extraire les mots de recherche]** : extrait les mots du fichier du PDF afin que les mots-clés du fichier puissent être recherchés dans une visionneuse de catalogue électronique.

**[!UICONTROL Extract Links]** : extrait les liens des fichiers du PDF et les convertit en zones cliquables utilisées dans une visionneuse de catalogue électronique.

**[!UICONTROL Générer automatiquement un catalogue électronique avec un PDF de plusieurs pages]** : crée automatiquement un catalogue électronique à partir du fichier du PDF. Le catalogue électronique reprend le nom du fichier PDF que vous avez téléchargé (cette option n’est disponible que si vous pixellisez le fichier PDF au moment du téléchargement).

### Résolution

Détermine le paramètre de résolution, qui définit le nombre de pixels affichés par pouce dans le fichier PDF. La valeur par défaut est de 150.

### Options d’espace colorimétrique

Dans le menu Espace colorimétrique, choisissez un espace pour le fichier PDF. La plupart des fichiers PDF contiennent des images en couleurs RVB et CMJN. L’espace colorimétrique RVB est préférable pour un affichage à l’écran.

* **[!UICONTROL Détecter automatiquement]** : conserve l’espace colorimétrique du fichier de PDF.

* **[!UICONTROL Forcer comme RGB]** : convertit l’espace colorimétrique du RGB.

* **[!UICONTROL Forcer comme CMJN]** : convertit l’espace colorimétrique CMJN.

* **[!UICONTROL Forcer comme Niveaux de gris]** : convertit l’espace colorimétrique Niveaux de gris en Niveaux de gris.

### Options Profil de couleurs

* **[!UICONTROL Convert To sRGB]** : convertit en sRVB (Standard Red Green Blue). sRVB est l’espace colorimétrique recommandé pour l’affichage des images sur une page Web.

* **[!UICONTROL Conserver l’espace colorimétrique d’origine]** : conserve l’espace colorimétrique d’origine.

* **[!UICONTROL Personnalisé de]** > **[!UICONTROL À]** : ouvre les menus afin que vous puissiez choisir un espace colorimétrique Convertir à partir de et Convertir en. Vous pouvez choisir un espace colorimétrique Photoshop standard ou un espace colorimétrique que vous avez chargé dans Adobe Dynamic Media Classic.

(voir aussi [Profils ICC](/help/using/icc-profiles.md#icc_profiles)).

## Recadrer l’espace blanc d’un fichier de PDF {#cropping-white-space-from-a-pdf-file}

Vous pouvez recadrer automatiquement les pixels d’espace blanc d’un fichier de PDF au fur et à mesure de son téléchargement.

1. Sélectionnez le menu Recadrer et choisissez Rogner.
1. Spécifiez les options suivantes :

   * **[!UICONTROL Rogner en fonction de]** : choisissez si vous souhaitez recadrer en fonction de la couleur ou de la transparence :

      * **[!UICONTROL Color]** : choisissez l’option Color. Sélectionnez ensuite le menu **[!UICONTROL Coin]** et choisissez l’angle du PDF dont la couleur représente le mieux l’espace blanc à recadrer.

      * **[!UICONTROL Transparence]** : sélectionnez l’option Transparence.

   * **[!UICONTROL Tolérance]** : faites glisser le curseur pour spécifier une tolérance comprise entre 0 et 1.

   * **[!UICONTROL Rognage en fonction de la couleur]** : indiquez 0 pour rogner les pixels uniquement s’ils correspondent exactement à la couleur que vous avez sélectionnée dans le coin du PDF. Les valeurs qui se rapprochent de 1 admettent un plus grand écart des couleurs.

   * **[!UICONTROL Rognage en fonction de la transparence]** : spécifiez 0 pour rogner les pixels uniquement s’ils sont transparents ; les nombres plus proches de 1 permettent une plus grande transparence.

## Recadrage à partir des côtés des pages de PDF {#cropping-from-the-sides-of-pdf-pages}

Vous pouvez supprimer manuellement les repères d’impression des côtés des pages d’un fichier de PDF au fur et à mesure de son chargement.

1. Dans le menu Recadrer, sélectionnez **[!UICONTROL Manuel]**.
1. Entrez les valeurs en pixels dans les zones de texte pour les bords supérieur, droit, inférieur et gauche de manière à recadrer à partir du haut, du bas et des côtés des pages.

La proportion de la page rognée dépend du paramètre de résolution px/pouce (pixels par pouce) que vous spécifiez pour le fichier PDF. Supposons, par exemple, que vous saisissiez 150 (valeur par défaut) comme paramètre de résolution PX/Inch. Ensuite, vous recadrez 75 pixels à partir des côtés des pages. Dans ce cas, 0,5 po est recadré. À 150 pixels par pouce, 75 pixels égale un demi-pouce.
