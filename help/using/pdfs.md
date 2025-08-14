---
title: Utiliser des PDF
description: Découvrez comment utiliser des fichiers PDF dans Adobe Dynamic Media Classic.
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

# Utiliser des PDF{#working-with-pdfs}

Les fichiers PDF (Portable Document Format) sont le plus souvent utilisés dans Adobe Dynamic Media Classic pour créer des catalogues électroniques. Lorsque vous chargez un fichier PDF, Adobe Dynamic Media Classic pixellise ou pixellise les pages par défaut afin que les pages puissent être utilisées pour créer des médias riches.

Lorsque vous téléchargez un PDF pour l’extraction de page, Adobe applique la limite suivante :

| Type de limite | Limite imposée | Modification de la limite au 31 décembre 2022 |
| --- | --- | --- |
| Nombre maximal de pages qu’un PDF doit prendre en compte pour l’extraction | 5000 (pour les nouveaux chargements) | 100 (pour tous les PDF) |

Voir aussi [Limites de Dynamic Media](/help/using/limitations.md).

## Options de téléchargement des fichiers PDF {#pdf-upload-options}

Lorsque vous téléchargez un fichier PDF, vous pouvez le formater de différentes manières. Vous pouvez recadrer les pages, extraire des mots de recherche, spécifier une résolution en pixels par pouce et choisir un espace colorimétrique. Les fichiers PDF contiennent souvent une marge de rognage, des traits de coupe, des repères de montage et d’autres repères d’impression. Vous pouvez éliminer ces marques sur les côtés des pages lorsque vous téléchargez un fichier PDF.

Les options de chargement de fichiers PDF se trouvent sur la page Charger sous Options PDF.

### Options de traitement

**[!UICONTROL Pixelliser]** : (par défaut) pixellise les pages du fichier PDF et convertit les graphiques vectoriels en images bitmap. Pour créer un catalogue électronique, choisissez cette option.

**[!UICONTROL Extraire les mots-clés]** : extrait les mots du fichier PDF afin que les mots-clés du fichier puissent être recherchés dans une visionneuse de catalogue électronique.

**[!UICONTROL Extraire les liens]** : extrait les liens des fichiers PDF et les convertit en zones cliquables utilisées dans une visionneuse de catalogue électronique.

**[!UICONTROL Générer automatiquement un catalogue électronique avec le PDF à plusieurs pages]** : crée automatiquement un catalogue électronique à partir du fichier PDF. Le catalogue électronique reprend le nom du fichier PDF que vous avez téléchargé (cette option n’est disponible que si vous pixellisez le fichier PDF au moment du téléchargement).

### Résolution

Détermine le paramètre de résolution, qui définit le nombre de pixels affichés par pouce dans le fichier PDF. La valeur par défaut est de 150.

### Options d’espace colorimétrique

Dans le menu Espace colorimétrique, choisissez un espace pour le fichier PDF. La plupart des fichiers PDF contiennent des images en couleurs RVB et CMJN. L’espace colorimétrique RVB est préférable pour un affichage à l’écran.

* **[!UICONTROL Détecter automatiquement]** : conserve l’espace colorimétrique du fichier PDF.

* **[!UICONTROL Forcer comme RGB]** : permet de convertir les couleurs dans l’espace colorimétrique RGB.

* **[!UICONTROL Forcer comme CMJN]** : permet de convertir les couleurs dans l’espace colorimétrique CMJN.

* **[!UICONTROL Forcer comme Niveaux de gris]** : permet de convertir en niveaux de gris l’espace colorimétrique.

### Options Profil de couleurs

* **[!UICONTROL Convertir en sRGB]** : permet de convertir le format sRGB (rouge standard, vert, bleu). sRGB est l’espace colorimétrique recommandé pour afficher les images sur une page web.

* **[!UICONTROL Conserver l’espace colorimétrique d’origine]** : conserve l’espace colorimétrique d’origine.

* **[!UICONTROL Personnaliser à partir de]** > **[!UICONTROL À]** : ouvre les menus afin que vous puissiez choisir un espace colorimétrique Convertir à partir de et Convertir en . Vous pouvez choisir un espace colorimétrique Photoshop standard ou un espace colorimétrique que vous avez téléchargé sur Adobe Dynamic Media Classic.

(voir aussi [Profils ICC](/help/using/icc-profiles.md#icc_profiles)).

## Recadrer un espace blanc dans un fichier PDF {#cropping-white-space-from-a-pdf-file}

Vous pouvez supprimer automatiquement les pixels représentant des espaces blancs d’un fichier PDF au fur et à mesure de son chargement.

1. Sélectionnez le menu Recadrer et choisissez Rogner.
1. Spécifiez les options suivantes :

   * **[!UICONTROL Rogner en fonction de]** : choisissez de recadrer en fonction de la couleur ou de la transparence :

      * **[!UICONTROL Couleur]** : sélectionnez l’option Couleur. Sélectionnez ensuite le menu **[!UICONTROL Coin]** et choisissez l’angle du PDF présentant la couleur qui représente le mieux l’espace blanc à rogner.

      * **[!UICONTROL Transparence]** : sélectionnez l’option Transparence.

   * **[!UICONTROL Tolérance]** : faites glisser le curseur pour définir une tolérance comprise entre 0 et 1.

   * **[!UICONTROL Rognage en fonction de la couleur]** : spécifiez 0 pour rogner les pixels uniquement s’ils correspondent exactement à la couleur que vous avez sélectionnée dans le coin du PDF. Les valeurs qui se rapprochent de 1 admettent un plus grand écart des couleurs.

   * **[!UICONTROL Rognage en fonction de la transparence]** : spécifiez 0 pour rogner les pixels uniquement s’ils sont transparents ; les nombres plus proches de 1 permettent une plus grande transparence.

## Recadrer à partir des bords des pages PDF {#cropping-from-the-sides-of-pdf-pages}

Vous pouvez supprimer manuellement les repères d’impression sur les côtés des pages d’un fichier PDF au fur et à mesure de son chargement.

1. Dans le menu Recadrer, sélectionnez **[!UICONTROL Manuel]**.
1. Entrez les valeurs en pixels dans les zones de texte pour les bords supérieur, droit, inférieur et gauche de manière à recadrer à partir du haut, du bas et des côtés des pages.

La proportion de la page rognée dépend du paramètre de résolution px/pouce (pixels par pouce) que vous spécifiez pour le fichier PDF. Supposons, par exemple, que vous entriez 150 (valeur par défaut) comme paramètre Résolution PX/Pouce . Vous pouvez ensuite recadrer 75 pixels des côtés des pages. Dans ce cas, 0,5 po. est recadré. À 150 pixels par pouce, 75 pixels équivalent à un demi-pouce.
