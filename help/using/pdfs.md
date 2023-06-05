---
title: Utilisation de PDF
description: Découvrez comment utiliser des PDF dans Adobe Dynamic Media Classic.
uuid: 26d70d28-9393-49b1-9051-d70456deca67
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 5a073de3-6b1d-4c3e-8c03-9182f9f3874a
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 02892514-61fe-48ba-a2e3-eeb30580a1e4
source-git-commit: 38d7f8d6e5888e1c5ba9260ada45b79fb16b338f
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 36%

---

# Utilisation de PDF{#working-with-pdfs}

Les fichiers PDF (Portable Document Format) sont le plus souvent utilisés dans Adobe Dynamic Media Classic pour créer des catalogues électroniques. Lorsque vous chargez un fichier de PDF, Adobe Dynamic Media Classic pixellise les pages par défaut afin que les pages puissent être utilisées pour créer du contenu multimédia.

Lorsque vous chargez un PDF pour l’extraction de page, Adobe applique la limite suivante :

| Type de limite | Limite imposée | Modification de la limite le 31 décembre 2022 |
| --- | --- | --- |
| Nombre maximum de pages qu’un PDF doit prendre en compte pour l’extraction | 5000 (pour les nouveaux chargements) | 100 (pour tous les PDF) |

Voir aussi [Limites de Dynamic Media](/help/using/limitations.md).

## Options de téléchargement des fichiers PDF {#pdf-upload-options}

Lorsque vous téléchargez un fichier PDF, vous pouvez le formater de différentes manières. Vous pouvez recadrer les pages, extraire des mots de recherche, spécifier une résolution en pixels par pouce et choisir un espace colorimétrique. Les fichiers PDF contiennent souvent une marge de rognage, des traits de coupe, des repères de montage et autres repères d’impression. Vous pouvez éliminer ces marques sur les côtés des pages lorsque vous téléchargez un fichier PDF.

Les options de téléchargement de fichiers de PDF sont disponibles sur la page Télécharger sous les options du PDF.

### Options de traitement

**[!UICONTROL Pixelliser]** - (Par défaut) Pixellise les pages du fichier du PDF et convertit les graphiques vectoriels en images bitmap. Pour créer un catalogue électronique, sélectionnez cette option.

**[!UICONTROL Extraction de mots de recherche]** - Extrait les mots du fichier du PDF afin que le fichier puisse être recherché par mot-clé dans une visionneuse de catalogue électronique.

**[!UICONTROL Extraction de liens]** - Extrait les liens des fichiers du PDF et les convertit en zones cliquables utilisées dans une visionneuse de catalogue électronique.

**[!UICONTROL Génération automatique d’un catalogue électronique avec un PDF de plusieurs pages]** : crée automatiquement un catalogue électronique à partir du fichier du PDF. Le catalogue électronique reprend le nom du fichier PDF que vous avez téléchargé (cette option n’est disponible que si vous pixellisez le fichier PDF au moment du téléchargement).

### Résolution

Détermine le paramètre de résolution, qui définit le nombre de pixels affichés par pouce dans le fichier PDF. La valeur par défaut est de 150.

### Espace colorimétrique options

Dans le menu Espace colorimétrique, choisissez un espace pour le fichier PDF. La plupart des fichiers PDF contiennent des images en couleurs RVB et CMJN. L’espace colorimétrique RVB est préférable pour un affichage à l’écran.

* **[!UICONTROL Détecter automatiquement]** - Conserve l’espace colorimétrique du fichier de PDF.

* **[!UICONTROL Forcer comme RGB]** : convertit l’espace colorimétrique du RGB.

* **[!UICONTROL Forcer comme CMJN]** : convertit l’espace colorimétrique CMJN.

* **[!UICONTROL Forcer comme Niveaux de gris]** - Applique l’espace colorimétrique Niveaux de gris.

### Options Profil de couleurs

* **[!UICONTROL Convertir en sRVB]** - Convertit en sRVB (Standard Red Green Blue). sRVB est l’espace colorimétrique recommandé pour l’affichage d’images sur les pages Web.

* **[!UICONTROL Conserver l’espace colorimétrique original]** - Conserve l’espace colorimétrique d’origine.

* **[!UICONTROL Personnalisé à partir de]** > **[!UICONTROL À]** - Ouvre les menus pour vous permettre de choisir un espace colorimétrique Convertir à partir de et Convertir en . Vous pouvez choisir un espace colorimétrique Photoshop standard ou un espace colorimétrique que vous avez chargé dans Adobe Dynamic Media Classic.

(voir aussi [Profils ICC](/help/using/icc-profiles.md#icc_profiles)).

## Recadrer l’espace blanc d’un fichier de PDF {#cropping-white-space-from-a-pdf-file}

1. Pour supprimer automatiquement les pixels d’espace blanc d’un fichier PDF au moment du téléchargement, sélectionnez le menu Recadrer, puis choisissez Rogner.
1. Spécifiez les options suivantes :

   * **[!UICONTROL Rogner en fonction de]** - Choisissez si vous souhaitez recadrer en fonction de la couleur ou de la transparence :

      * **[!UICONTROL Couleur]** - Choisissez l’option Couleur . Sélectionnez ensuite le **[!UICONTROL Coin]** et choisissez l’angle du PDF avec la couleur qui représente le mieux l’espace blanc que vous souhaitez recadrer.

      * **[!UICONTROL Transparence]** - Sélectionnez l’option Transparence .
   * **[!UICONTROL Tolérance]** - Faites glisser le curseur pour spécifier une tolérance comprise entre 0 et 1.

   * **[!UICONTROL Rognage en fonction de la couleur]** - Indiquez 0 pour rogner les pixels uniquement s’ils correspondent exactement à la couleur sélectionnée dans le coin du PDF. Les valeurs qui se rapprochent de 1 admettent un plus grand écart des couleurs.

   * **[!UICONTROL Rognage en fonction de la transparence]** - Indiquez 0 pour rogner les pixels uniquement s’ils sont transparents ; Les valeurs plus proches de 1 permettent une plus grande transparence.


## Recadrage à partir des côtés des pages de PDF {#cropping-from-the-sides-of-pdf-pages}

Vous pouvez supprimer manuellement les repères d’impression sur les côtés des pages d’un fichier PDF au moment du téléchargement.

1. Dans le menu Recadrer, sélectionnez **[!UICONTROL Manuel]**.
1. Entrez les valeurs en pixels dans les zones de texte pour les bords supérieur, droit, inférieur et gauche de manière à recadrer à partir du haut, du bas et des côtés des pages.

La proportion de la page rognée dépend du paramètre de résolution px/pouce (pixels par pouce) que vous spécifiez pour le fichier PDF. Supposons, par exemple, que vous saisissiez 150 (valeur par défaut) comme paramètre de résolution PX/Inch. Ensuite, vous recadrez 75 pixels à partir des côtés des pages. Dans ce cas, 0,5 po est recadré. À 150 pixels par pouce, 75 pixels égale un demi-pouce.
