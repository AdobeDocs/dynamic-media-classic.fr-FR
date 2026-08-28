---
title: Chargement des fichiers PDF
description: Découvrez comment télécharger les fichiers PDF associés à un catalogue électronique dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: a787d6b5-48c8-4cf7-b136-60ba3d3eb2f2
topic: Integrations, Development
level: Experienced
autotag-review: '2026-05-13T20:17:17.647Z'
TQID: 'https://experienceleague.adobe.com/SNoRYiCgjJK2TBx6X7HAzv3Xqet64-lm4oSOcat7DfM'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 4035cd307a13d1174f8b66fb1cd1ab39138d1310
workflow-type: tm+mt
source-wordcount: 838
ht-degree: 18%

---

# Chargement des fichiers PDF{#uploading-the-pdf-files}

Les fichiers Adobe PDF constituent la source d’un catalogue électronique. Ces fichiers contiennent toutes les informations sur l’image, les polices et les graphiques vectoriels. Néanmoins, rien ne vous empêche de créer un catalogue électronique à partir d’images. Une fois que vous avez préparé les fichiers PDF à charger, sur la barre de navigation générale, sélectionnez **[!UICONTROL Charger]** pour commencer à charger les fichiers PDF.

Lorsque vous téléchargez un PDF pour l’extraction de page, Adobe applique la limite suivante :

| Type de limite PDF | Limite imposée | Modification de la limite au 31 décembre 2022 |
| --- | --- | --- |
| Nombre maximal de pages qu’un PDF doit prendre en compte pour l’extraction | 5000 (pour les nouveaux chargements) | 100 (pour tous les PDF) |

Voir aussi [Limites de Dynamic Media](/help/using/limitations.md).

## Préparation des fichiers PDF

Préparez vos fichiers PDF avant de les charger vers Adobe Dynamic Media Classic :

* Pour simplifier le chargement des fichiers, placez tous les fichiers dans le même dossier sur votre ordinateur ou votre réseau.
* Nommez les fichiers selon un ordre alphanumérique, par page. Organiser les pages simplifie leur placement dans l’ordre approprié une fois les fichiers chargés.
* Pour voir si les pages PDF contiennent des traits de coupe, des cibles d’enregistrement ou des barres de couleurs, examinez les pages. Ces marques déterminent où couper le papier lors de l&#39;impression des documents ; elles doivent être supprimées avant la publication en ligne de votre catalogue électronique. Adobe Dynamic Media Classic fournit des options pour le recadrage de marques lorsque vous chargez des fichiers PDF.
* Si vous souhaitez que les visiteurs puissent rechercher votre catalogue électronique par mot-clé, déterminez si vos fichiers PDF sont « aplatis ». Il est impossible d’extraire des mots de recherche dans des fichiers PDF aplatis. Pour déterminer si un PDF est aplati, essayez de sélectionner le texte qu’il contient. Si vous ne pouvez pas sélectionner de texte, le PDF est aplati et les visiteurs ne peuvent pas effectuer de recherche par mot-clé dans votre catalogue électronique.
* Étant destinés à l’impression, les fichiers PDF contiennent généralement des images CMJN. Par défaut, Adobe Dynamic Media Classic détecte ces images CMJN et les convertit à l’aide d’un profil colorimétrique CMJN interne. Vous pouvez cependant utiliser un profil de couleurs personnalisé pour convertir les images CMJN.

  Voir [Profils ICC (International Color Consortium)](icc-profiles.md#icc_profiles).

## Options recommandées pour le téléchargement des fichiers PDF {#best-practice-pdf-upload-options}

Pour obtenir des informations détaillées sur les différentes méthodes de téléchargement, voir [Téléchargement de fichiers](uploading-files.md#uploading_your_files).

Sélectionnez les fichiers à charger, puis choisissez les *bonnes pratiques* Options PDF suivantes :

* **Options de recadrage** : dans la boîte de dialogue Charger les options de la tâche, sélectionnez **[!UICONTROL Options de recadrage]**. Si les pages PDF contiennent des traits de coupe, des repères de montage ou d’autres repères, dans la liste déroulante **[!UICONTROL Recadrer]**, choisissez **[!UICONTROL Manuel]**. Saisissez le nombre de pixels à recadrer à partir des côtés supérieur, droit, inférieur et gauche des pages. Les marques de recadrage sont souvent définies sur une marge de 0,5 pouce. Supposons que vous choisissiez **[!UICONTROL 150]** (recommandé) comme résolution en pixels par pouce. Ensuite, entrez 75, 75, 75, 75 dans les zones de texte Haut, Droite, Bas et Gauche. Cela supprime 0,5 pouce des marges (à 150 ppp, 0,5 est égal à 75 pixels).

* **Traitement** : dans la boîte de dialogue Charger les options de la tâche, sélectionnez **[!UICONTROL Options de PDF]**. Dans la liste déroulante **[!UICONTROL Traitement]**, choisissez **[!UICONTROL Pixelliser]**. Il est nécessaire de pixelliser le fichier PDF afin que toutes les pages et les images soient affichées dans le catalogue électronique.

* **Extraire les mots de recherche (facultatif)** : dans la boîte de dialogue Charger les options de la tâche, sélectionnez **[!UICONTROL Options de PDF]**. Dans la liste déroulante **[!UICONTROL Extraire]**, choisissez **[!UICONTROL Mots de recherche]** si vous souhaitez que vos visiteurs puissent effectuer une recherche par mot-clé dans votre catalogue électronique.

* **Générer automatiquement un catalogue électronique à partir d’un PDF à plusieurs pages (facultatif)** : dans la boîte de dialogue Charger les options de la tâche, sélectionnez **[!UICONTROL Options de PDF]**. Cliquez sur **[!UICONTROL Générer automatiquement un catalogue électronique à partir de PDF à plusieurs pages]** afin de créer automatiquement un catalogue électronique lors du chargement. Vous pouvez accéder directement à l’écran Catalogue électronique et commencer à travailler sur votre catalogue électronique sans sélectionner au préalable les fichiers PDF et la commande Créer. Le catalogue électronique prend le nom du fichier PDF.

* **Résolution** : dans la boîte de dialogue Charger les options de la tâche, sélectionnez **[!UICONTROL Options de PDF]**. Dans le champ de texte **[!UICONTROL Résolution]**, saisissez une valeur. Adobe Dynamic Media Classic recommande 150 pixels par pouce.

* **Colorspace** : dans la boîte de dialogue Charger les options de la tâche, sélectionnez **[!UICONTROL Options de PDF]**. Dans la liste déroulante Espace colorimétrique , choisissez **[!UICONTROL Détecter automatiquement]**. En règle générale, les fichiers PDF destinés à l’impression sont créés dans l’espace colorimétrique CMJN, tandis que ceux conçus pour le Web le sont dans l’espace RVB. Si un fichier PDF utilise les deux espaces colorimétriques, vous pouvez opter pour l’utilisation de l’un de ces espaces en choisissant l’option Forcer comme RVB ou Forcer comme CMJN. Les fichiers PDF utilisent les deux espaces colorimétriques ; par exemple, lorsque les graphiques de page utilisent un espace colorimétrique CMJN, mais que les images utilisent un espace colorimétrique RGB. Si vous avez téléchargé un profil ICC, son nom s’affiche dans le menu Espace colorimétrique, où vous pouvez le sélectionner à votre convenance.

  Voir [Profils ICC (International Color Consortium)](/help/using/icc-profiles.md).

* **Options de profil de couleurs** : dans la boîte de dialogue Charger les options de la tâche, sélectionnez **[!UICONTROL Options de profil de couleurs]**, puis choisissez une option de profil de couleurs :

  * **Conserver l’espace colorimétrique d’origine** : conserve l’espace colorimétrique d’origine.

  * **Personnaliser de > À** : ouvre les sous-menus afin que vous puissiez choisir un espace colorimétrique **[!UICONTROL Convertir de]** et **[!UICONTROL Convertir en]**. Vous pouvez choisir un espace colorimétrique Photoshop standard ou un espace colorimétrique que vous avez téléchargé sur Adobe Dynamic Media Classic.

<!-- * **Convert To SRGB**: Converts to SRGB (Standard Red Green Blue). SRGB is the recommended color space for displaying images on Web pages. -->

Voir [Profils ICC (International Color Consortium)](icc-profiles.md#icc_profiles).

>[!NOTE]
>
>pour plus d’informations sur toutes les options PDF, voir [Options de téléchargement des fichiers PDF](pdfs.md#pdf_upload_options).
