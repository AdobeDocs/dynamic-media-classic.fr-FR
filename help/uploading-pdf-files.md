---
title: Chargement des fichiers du PDF
description: Découvrez comment charger les fichiers de PDF associés à un catalogue électronique dans Adobe Dynamic Media Classic.
uuid: 9e178bb2-ac09-427a-b61a-aad4e87a5837
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0097cba5-c886-4115-bc35-7ae7a500202f
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: a787d6b5-48c8-4cf7-b136-60ba3d3eb2f2
source-git-commit: 92a28b7868e03802f4ef1c113ec3f8b34f57ed56
workflow-type: tm+mt
source-wordcount: '827'
ht-degree: 38%

---

# Chargement des fichiers du PDF{#uploading-the-pdf-files}

En règle générale, les fichiers Adobe PDF sont la source d’un catalogue électronique. Ces fichiers contiennent toutes les informations sur l’image, les polices et les graphiques vectoriels. Néanmoins, rien ne vous empêche de créer un catalogue électronique à partir d’images. Après avoir préparé les fichiers de PDF à charger, dans la barre de navigation globale, sélectionnez **[!UICONTROL Télécharger]** pour commencer à charger les PDF.

Lorsque vous chargez un PDF pour l’extraction de page, Adobe applique la limite suivante :

| Type de limite de PDF | Limite imposée | Modification de la limite le 31 décembre 2022 |
| --- | --- | --- |
| Nombre maximum de pages qu’un PDF doit prendre en compte pour l’extraction | 5000 (pour les nouveaux chargements) | 100 |

Voir aussi [Limites de Dynamic Media](/help/limitations.md).

<!-- 
>[!NOTE]
>
>When you upload a PDF for page extraction, Adobe imposes the following best practice guideline and enforced limit.d
>
>* Maximum page size of a PDF to be considered for extraction
>   * Best practice: 100
>   * Enforced limit: 1000 (for refresh uploads) -->

## Préparation des fichiers du PDF {#preparing-your-pdf-files}

Préparez les fichiers de votre PDF avant de les transférer vers Adobe Dynamic Media Classic :

* Pour faciliter le téléchargement des fichiers, placez tous les fichiers dans le même dossier sur votre ordinateur ou votre réseau.
* Nommez les fichiers selon un ordre alphanumérique, par page. L’organisation des pages selon un ordre donné facilite leur bon assemblage après le téléchargement des fichiers.
* Pour déterminer si les pages de PDF contiennent des marques de recadrage, des cibles d’enregistrement ou des barres de couleurs, examinez les pages. Ces marques indiquent où couper le papier lorsque les documents sont imprimés et doivent impérativement être supprimées avant le placement du catalogue électronique sur le Web. Adobe Dynamic Media Classic fournit des options de recadrage des marques lorsque vous chargez des fichiers PDF.
* Si vous souhaitez que les utilisateurs puissent effectuer des recherches par mot-clé dans votre catalogue électronique, déterminez si vos fichiers PDF sont aplatis. Il est impossible d’extraire des mots de recherche dans des fichiers PDF aplatis. Pour savoir si un fichier PDF est aplati, essayez de sélectionner le texte qu’il contient. Si vous ne pouvez pas sélectionner de texte, le PDF est aplati et les visiteurs ne peuvent pas effectuer de recherche par mot-clé dans votre catalogue électronique.
* Les fichiers PDF étant destinés à l’impression, ils contiennent le plus souvent des images CMJN. Par défaut, Adobe Dynamic Media Classic peut détecter intelligemment ces images CMJN et les convertir à l’aide d’un profil colorimétrique CMJN interne. Vous pouvez cependant utiliser un profil de couleurs personnalisé pour convertir les images CMJN.

   Voir [Profils ICC (International Color Consortium)](icc-profiles.md#icc_profiles).

## Options recommandées pour le téléchargement des fichiers PDF {#best-practice-pdf-upload-options}

Pour obtenir des informations détaillées sur les différentes méthodes de téléchargement, voir [Téléchargement de fichiers](uploading-files.md#uploading_your_files).

Sélectionnez les fichiers à télécharger, puis sélectionnez ces options PDF *recommandées* :

* **Options de recadrage** - Dans la boîte de dialogue Télécharger les options de la tâche, sélectionnez **[!UICONTROL Options de recadrage]**. Si les pages du PDF contiennent des marques de recadrage, des marques d’enregistrement ou d’autres marques, dans la variable **[!UICONTROL Recadrer]** liste déroulante, choisissez **[!UICONTROL Manuel]**. Indiquez les valeurs de recadrage (en nombre de pixels) à partir des bords supérieur, droit, inférieur et gauche des pages. Les marques de recadrage sont souvent définies sur une marge d’un demi-pouce. Supposons que vous choisissiez **[!UICONTROL 150]** (recommandé) en tant que résolution en pixels par pouce, et saisissez 75, 75, 75, 75 dans les zones de texte Haut, Droite, Bas et Gauche. Dans ce cas, elle recadre un demi-pouce des marges (à 150 ppp, la moitié de 1 équivaut à 75 pixels).

* **Traitement** - Dans la boîte de dialogue Télécharger les options de la tâche, sélectionnez **[!UICONTROL Options de PDF]**. Dans le **[!UICONTROL Traitement]** liste déroulante, choisissez **[!UICONTROL Pixelliser]**. Il est nécessaire de pixelliser le fichier PDF afin que toutes les pages et les images soient affichées dans le catalogue électronique.

* **Extraire les mots de recherche (facultatif)** - Dans la boîte de dialogue Télécharger les options de la tâche, sélectionnez **[!UICONTROL Options de PDF]**. Dans la liste déroulante Extraire , choisissez **[!UICONTROL Mots de recherche]** si vous souhaitez que vos visiteurs puissent effectuer des recherches par mot-clé dans votre catalogue électronique.

* **Génération automatique d’un catalogue électronique à partir de plusieurs PDF de page (facultatif)** - Dans la boîte de dialogue Télécharger les options de la tâche, sélectionnez **[!UICONTROL Options de PDF]**. Sélectionner **[!UICONTROL Génération automatique d’un catalogue électronique à partir de plusieurs PDF de page]** pour créer automatiquement un catalogue électronique lors du téléchargement. L’écran de catalogue électronique s’affiche alors directement, et vous pouvez commencer à travailler sur votre catalogue électronique sans avoir à sélectionner préalablement les fichiers PDF et la commande Créer. Le catalogue électronique prend le nom du fichier PDF.

* **Résolution** - Dans la boîte de dialogue Télécharger les options de la tâche, sélectionnez **[!UICONTROL Options de PDF]**. Dans le **[!UICONTROL Résolution]** , saisissez une valeur. Adobe Dynamic Media Classic recommande 150 pixels par pouce.

* **Espace colorimétrique** - Dans la boîte de dialogue Télécharger les options de la tâche, sélectionnez **[!UICONTROL Options de PDF]**. Dans la liste déroulante Espace colorimétrique, choisissez **[!UICONTROL Détecter automatiquement]**. En règle générale, les fichiers PDF destinés à l’impression sont créés dans l’espace colorimétrique CMJN, tandis que ceux conçus pour le Web le sont dans l’espace RVB. Si un fichier PDF utilise les deux espaces colorimétriques, vous pouvez opter pour l’utilisation de l’un de ces espaces en choisissant l’option Forcer comme RVB ou Forcer comme CMJN. Les fichiers PDF utilisent les deux espaces de couleurs lorsqu’ils contiennent des graphiques CMJN et des images RVB, par exemple. Si vous avez téléchargé un profil ICC, son nom s’affiche dans le menu Espace colorimétrique, où vous pouvez le sélectionner à votre convenance.

   Voir [Profils ICC (International Color Consortium)](/help/icc-profiles.md).

* **Options de profil colorimétrique** - Dans la boîte de dialogue Télécharger les options de la tâche, sélectionnez **[!UICONTROL Options de profil colorimétrique]**, puis sélectionnez une option de profil de couleurs :

   * **Conserver l’espace colorimétrique original** - Conserve l’espace colorimétrique d’origine.

   * **Personnaliser de > à** - Ouvre les sous-menus afin que vous puissiez choisir un **[!UICONTROL Convertir à partir de]** et **[!UICONTROL Convertir en]** espace colorimétrique. Vous pouvez choisir un espace colorimétrique Photoshop standard ou un espace colorimétrique que vous avez chargé dans Adobe Dynamic Media Classic.

<!-- * **Convert To SRGB** - Converts to SRGB (Standard Red Green Blue). SRGB is the recommended color space for displaying images on web pages. -->

Voir [Profils ICC (International Color Consortium)](icc-profiles.md#icc_profiles).

>[!NOTE]
>
>pour plus d’informations sur toutes les options PDF, voir [Options de téléchargement des fichiers PDF](pdfs.md#pdf_upload_options).
