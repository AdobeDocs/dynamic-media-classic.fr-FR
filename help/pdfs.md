---
title: Utilisation de PDF
description: Découvrez comment utiliser des PDF dans Adobe Dynamic Media Classic.
uuid: 26d70d28-9393-49b1-9051-d70456deca67
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 5a073de3-6b1d-4c3e-8c03-9182f9f3874a
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 02892514-61fe-48ba-a2e3-eeb30580a1e4
source-git-commit: 3185824deca4d4b3c5549bda2e47f179094110e7
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Utilisation de PDF{#working-with-pdfs}

Les fichiers PDF (Portable Document Format) sont le plus souvent utilisés dans Adobe Dynamic Media Classic pour créer des catalogues électroniques. Lorsque vous chargez un fichier PDF, Adobe Dynamic Media Classic pixellise les pages par défaut afin que les pages puissent être utilisées pour créer du contenu multimédia enrichi.

## Options de téléchargement des fichiers PDF {#pdf-upload-options}

Lorsque vous téléchargez un fichier PDF, vous pouvez le formater de différentes manières. Vous pouvez recadrer les pages, extraire des mots de recherche, spécifier une résolution en pixels par pouce et choisir un espace colorimétrique. Les fichiers PDF contiennent souvent une marge de rognage, des traits de coupe, des repères de montage et autres repères d’impression. Vous pouvez éliminer ces marques sur les côtés des pages lorsque vous téléchargez un fichier PDF.

Les options de téléchargement de fichiers PDF sont disponibles sur la page Télécharger sous les options PDF.

### Options de traitement

**[!UICONTROL Pixelliser]**  : (par défaut) extrait les pages du fichier PDF et convertit les graphiques vectoriels en images bitmap. Pour créer un catalogue électronique, sélectionnez cette option.

**[!UICONTROL Extraire les mots de recherche]**  : extrait les mots du fichier PDF afin que le fichier puisse être recherché par mot-clé dans une visionneuse de catalogue électronique.

**[!UICONTROL Extraire les liens]**  : extrait les liens des fichiers PDF et les convertit en zones cliquables utilisées dans une visionneuse de catalogue électronique.

**[!UICONTROL Générer automatiquement un catalogue électronique avec un PDF de plusieurs pages]**  : crée automatiquement un catalogue électronique à partir du fichier PDF. Le catalogue électronique reprend le nom du fichier PDF que vous avez téléchargé (cette option n’est disponible que si vous pixellisez le fichier PDF au moment du téléchargement).

### Résolution

Détermine le paramètre de résolution, qui définit le nombre de pixels affichés par pouce dans le fichier PDF. La valeur par défaut est de 150.

### Espace colorimétrique options

Dans le menu Espace colorimétrique, choisissez un espace pour le fichier PDF. La plupart des fichiers PDF contiennent des images en couleurs RVB et CMJN. L’espace colorimétrique RVB est préférable pour un affichage à l’écran.

* **[!UICONTROL Détecter automatiquement]**  : conserve l’espace colorimétrique du fichier PDF.

* **[!UICONTROL Forcer comme RVB]**  : convertit l’espace colorimétrique RVB.

* **[!UICONTROL Forcer comme CMJN]**  : convertit l’espace colorimétrique CMJN.

* **[!UICONTROL Forcer comme Niveaux de gris]**  : convertit l’espace colorimétrique Niveaux de gris.

### Options Profil de couleurs

* **[!UICONTROL Convertir en sRVB]**  : convertit en sRVB (rouge vert bleu standard). sRVB est l’espace colorimétrique recommandé pour l’affichage d’images sur les pages Web.

* **[!UICONTROL Conserver l’espace colorimétrique d’origine]**  : conserve l’espace colorimétrique d’origine.

* **[!UICONTROL Personnaliser à partir de]**  >  **[!UICONTROL vers]**  : ouvre les menus afin que vous puissiez sélectionner un espace colorimétrique Convertir à partir de et Convertir en. Vous pouvez choisir un espace colorimétrique Photoshop standard ou un espace colorimétrique que vous avez chargé dans Adobe Dynamic Media Classic.

(voir aussi [Profils ICC](/help/icc-profiles.md#icc_profiles)).

## Recadrer l’espace blanc d’un fichier PDF {#cropping-white-space-from-a-pdf-file}

1. Pour supprimer automatiquement les pixels d’espace blanc d’un fichier PDF au moment du téléchargement, sélectionnez le menu Recadrer, puis choisissez Rogner.
1. Spécifiez les options suivantes :

   * **[!UICONTROL Rogner en fonction de]**  : choisissez si vous souhaitez recadrer en fonction de la couleur ou de la transparence :

      * **[!UICONTROL Couleur]**  : choisissez l’option Couleur. Sélectionnez ensuite le menu **[!UICONTROL Coin]** et choisissez l’angle du PDF dont la couleur représente le mieux l’espace blanc à recadrer.

      * **[!UICONTROL Transparence]**  : sélectionnez l’option Transparence.
   * **[!UICONTROL Tolérance]**  : faites glisser le curseur pour spécifier une tolérance comprise entre 0 et 1.

   * **[!UICONTROL Rognage en fonction de la couleur]**  : indiquez 0 pour rogner les pixels uniquement s’ils correspondent exactement à la couleur sélectionnée dans le coin du PDF. Les valeurs qui se rapprochent de 1 admettent un plus grand écart des couleurs.

   * **[!UICONTROL Rognage en fonction de la transparence]**  : spécifiez 0 pour rogner les pixels uniquement s’ils sont transparents. Les valeurs plus proches de 1 permettent une plus grande transparence.


## Recadrage à partir des côtés des pages PDF {#cropping-from-the-sides-of-pdf-pages}

Vous pouvez supprimer manuellement les repères d’impression sur les côtés des pages d’un fichier PDF au moment du téléchargement.

1. Dans le menu Recadrer, sélectionnez **[!UICONTROL Manuel]**.
1. Entrez les valeurs en pixels dans les zones de texte pour les bords supérieur, droit, inférieur et gauche de manière à recadrer à partir du haut, du bas et des côtés des pages.

La proportion de la page rognée dépend du paramètre de résolution px/pouce (pixels par pouce) que vous spécifiez pour le fichier PDF. Par exemple, si vous saisissez 150 (valeur par défaut) comme paramètre de résolution PX/Inch et que vous recadrez 75 pixels des côtés des pages, un demi-pouce est rogné ; à 150 pixels par pouce, 75 pixels égale un demi-pouce.
