---
title: Chargement des fichiers du PDF
description: Découvrez comment charger les fichiers de PDF associés à un catalogue électronique dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: a787d6b5-48c8-4cf7-b136-60ba3d3eb2f2
topic: Integrations, Development
level: Experienced
source-git-commit: 29752cf9eca0fc9bb760c721e1c3dc8e4ef912c3
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 30%

---

# Chargement des fichiers du PDF{#uploading-the-pdf-files}

En règle générale, les fichiers Adobe PDF sont la source d’un catalogue électronique. Ces fichiers contiennent toutes les informations sur l’image, les polices et les graphiques vectoriels. Néanmoins, rien ne vous empêche de créer un catalogue électronique à partir d’images. Après avoir préparé les fichiers de PDF à charger, dans la barre de navigation globale, sélectionnez **[!UICONTROL Télécharger]** pour commencer à charger les PDF.

Lorsque vous chargez un PDF pour l’extraction de page, Adobe applique la limite suivante :

| Type de limite de PDF | Limite imposée | Modification de la limite le 31 décembre 2022 |
| --- | --- | --- |
| Nombre maximum de pages qu’un PDF doit prendre en compte pour l’extraction | 5000 (pour les nouveaux chargements) | 100 (pour tous les PDF) |

Voir aussi [Limites de Dynamic Media](/help/using/limitations.md).

## Préparation des fichiers du PDF

Préparez les fichiers de votre PDF avant de les transférer vers Adobe Dynamic Media Classic :

* Pour faciliter le téléchargement des fichiers, placez tous les fichiers dans le même dossier sur votre ordinateur ou votre réseau.
* Nommez les fichiers selon un ordre alphanumérique, par page. L’organisation des pages selon un ordre donné facilite leur bon assemblage après le téléchargement des fichiers.
* Pour déterminer si les pages de PDF contiennent des marques de recadrage, des cibles d’enregistrement ou des barres de couleurs, examinez les pages. Ces marques indiquent où couper le papier lorsque les documents sont imprimés et doivent impérativement être supprimées avant le placement du catalogue électronique sur le Web. Adobe Dynamic Media Classic fournit des options de recadrage des marques lorsque vous chargez des fichiers PDF.
* Si vous souhaitez que les visiteurs effectuent des recherches par mot-clé dans votre catalogue électronique, découvrez si vos fichiers de PDF sont &quot;aplatis&quot;. Il est impossible d’extraire des mots de recherche dans des fichiers PDF aplatis. Pour savoir si un PDF est aplati, essayez de sélectionner le texte à l’intérieur. Si vous ne pouvez pas sélectionner de texte, le PDF est aplati et les visiteurs ne peuvent pas effectuer de recherche par mot-clé dans votre catalogue électronique.
* Les fichiers PDF étant destinés à l’impression, ils contiennent le plus souvent des images CMJN. Par défaut, Adobe Dynamic Media Classic peut détecter intelligemment ces images CMJN et les convertir à l’aide d’un profil colorimétrique CMJN interne. Vous pouvez cependant utiliser un profil de couleurs personnalisé pour convertir les images CMJN.

  Voir [Profils ICC (International Color Consortium)](icc-profiles.md#icc_profiles).

## Options recommandées pour le téléchargement des fichiers PDF {#best-practice-pdf-upload-options}

Pour obtenir des informations détaillées sur les différentes méthodes de téléchargement, voir [Téléchargement de fichiers](uploading-files.md#uploading_your_files).

Sélectionnez les fichiers à charger, puis sélectionnez-les. *bonne pratique* Options de PDF :

* **Options de recadrage**: dans la boîte de dialogue Télécharger les options de la tâche, sélectionnez **[!UICONTROL Options de recadrage]**. Si les pages du PDF contiennent des marques de recadrage, des marques d’enregistrement ou d’autres marques, dans la variable **[!UICONTROL Recadrer]** liste déroulante, choisissez **[!UICONTROL Manuel]**. Saisissez le nombre de pixels à recadrer à partir des côtés supérieur, droit, inférieur et gauche des pages. Les marques de recadrage sont souvent définies sur une marge de 50 cm. Supposons que vous choisissiez **[!UICONTROL 150]** (recommandé) comme résolution de pixel par pouce. Ensuite, saisissez 75, 75, 75, 75 dans les zones de texte Haut, Droite, Bas et Gauche. Dans ce cas, elle recadre un demi-pouce des marges (à 150 ppp, la moitié de 1 équivaut à 75 pixels).

* **Traitement**: dans la boîte de dialogue Télécharger les options de la tâche, sélectionnez **[!UICONTROL Options de PDF]**. Dans le **[!UICONTROL Traitement]** liste déroulante, choisissez **[!UICONTROL Pixelliser]**. Il est nécessaire de pixelliser le fichier PDF afin que toutes les pages et les images soient affichées dans le catalogue électronique.

* **Extraire les mots de recherche (facultatif)**: dans la boîte de dialogue Télécharger les options de la tâche, sélectionnez **[!UICONTROL Options de PDF]**. Dans la liste déroulante Extraire , choisissez **[!UICONTROL Mots de recherche]** si vous souhaitez que vos visiteurs puissent effectuer des recherches par mot-clé dans votre catalogue électronique.

* **Génération automatique d’un catalogue électronique à partir de plusieurs PDF de page (facultatif)**: dans la boîte de dialogue Télécharger les options de la tâche, sélectionnez **[!UICONTROL Options de PDF]**. Cliquez sur **[!UICONTROL Génération automatique d’un catalogue électronique à partir de plusieurs PDF de page]** vous pouvez ainsi créer automatiquement un catalogue électronique lors du téléchargement. L’écran de catalogue électronique s’affiche alors directement, et vous pouvez commencer à travailler sur votre catalogue électronique sans avoir à sélectionner préalablement les fichiers PDF et la commande Créer. Le catalogue électronique prend le nom du fichier PDF.

* **Résolution**: dans la boîte de dialogue Télécharger les options de la tâche, sélectionnez **[!UICONTROL Options de PDF]**. Dans le **[!UICONTROL Résolution]** , saisissez une valeur. Adobe Dynamic Media Classic recommande 150 pixels par pouce.

* **Colorspace**: dans la boîte de dialogue Télécharger les options de la tâche, sélectionnez **[!UICONTROL Options de PDF]**. Dans la liste déroulante Espace colorimétrique, choisissez **[!UICONTROL Détecter automatiquement]**. En règle générale, les fichiers PDF destinés à l’impression sont créés dans l’espace colorimétrique CMJN, tandis que ceux conçus pour le Web le sont dans l’espace RVB. Si un fichier PDF utilise les deux espaces colorimétriques, vous pouvez opter pour l’utilisation de l’un de ces espaces en choisissant l’option Forcer comme RVB ou Forcer comme CMJN. Les fichiers PDF utilisent les deux espaces de couleurs lorsqu’ils contiennent des graphiques CMJN et des images RVB, par exemple. Si vous avez téléchargé un profil ICC, son nom s’affiche dans le menu Espace colorimétrique, où vous pouvez le sélectionner à votre convenance.

  Voir [Profils ICC (International Color Consortium)](/help/using/icc-profiles.md).

* **Options de profil colorimétrique**: dans la boîte de dialogue Télécharger les options de la tâche, sélectionnez **[!UICONTROL Options de profil colorimétrique]**, puis sélectionnez une option de profil de couleurs :

   * **Conserver l’espace colorimétrique original**: conserve l’espace colorimétrique d’origine.

   * **Personnaliser de > à**: ouvre des sous-menus afin que vous puissiez choisir un **[!UICONTROL Convertir depuis]** et **[!UICONTROL Convertir en]** espace colorimétrique. Vous pouvez choisir un espace colorimétrique Photoshop standard ou un espace colorimétrique que vous avez chargé dans Adobe Dynamic Media Classic.

<!-- * **Convert To SRGB**: Converts to SRGB (Standard Red Green Blue). SRGB is the recommended color space for displaying images on Web pages. -->

Voir [Profils ICC (International Color Consortium)](icc-profiles.md#icc_profiles).

>[!NOTE]
>
>pour plus d’informations sur toutes les options PDF, voir [Options de téléchargement des fichiers PDF](pdfs.md#pdf_upload_options).
