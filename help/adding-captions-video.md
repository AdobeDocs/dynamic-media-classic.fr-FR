---
title: Ajout de sous-titres aux vidéos
seo-title: Ajout de sous-titres aux vidéos
description: 'null'
seo-description: Découvrez comment ajouter des légendes à la vidéo
uuid: 4cc64469-4369-44a9-83db-63bad51aba8a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '909'
ht-degree: 64%

---


# Ajout de sous-titres aux vidéos{#adding-captions-to-video}

Vous pouvez étendre la portée de vos vidéos aux marchés mondiaux en ajoutant des sous-titres aux vidéos ou aux visionneuses de vidéos adaptatives. En ajoutant des sous-titres vous évitez d’avoir à réenregistrer le son ou de recourir à des locuteurs natifs pour réenregistrer l’audio dans chacune des langues. La vidéo est lue dans la langue dans laquelle elle a été enregistrée. Les sous-titres en langue étrangère s’affichent pour que les personnes parlant d’autres langues puissent néanmoins comprendre la partie audio.

Les légendes élargissent également l’accessibilité en utilisant le sous-titrage télétexte pour les sourds ou les malentendants.

>[!NOTE]
>
>le lecteur vidéo utilisé doit prendre en charge l’affichage des sous-titres.

Voir [Ajout ou modification d’un paramètre prédéfini de visionneuse de vidéos](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset) pour configurer l’effet de sous-titrage et modifier le menu de sous-titrage, y compris le texte du menu pour n’importe laquelle des visionneuses suivantes :

* `Universal_HTML5_Video` observateur.
* `Universal_HTML5_MixedMedia_dark` observateur.
* `Universal_HTML5_MixedMedia_light` observateur.

Voir aussi [Ajout et modification des paramètres prédéfinis de visionneuse](application-setup.md#adding_and_editing_viewer_presets).

Dynamic Media Classic permet de convertir des fichiers de sous-titrage au format JSON (JavaScript Object Notation). Cette conversion signifie que vous pouvez intégrer le texte JSON dans une page Web comme transcription masquée mais complète de la vidéo. Les moteurs de recherche peuvent ensuite analyser et indexer le contenu pour rendre les vidéos plus facilement détectables et fournir aux utilisateurs des informations supplémentaires concernant le contenu de la vidéo.

See [Serving static (non-image) contents](https://docs.adobe.com/content/help/en/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents.html) in the *Adobe Image Serving API Help* for more information about using the JSON function in a URL.

**Ajout de sous-titres aux vidéos**

1. A l’aide d’une application tierce extérieure à Dynamic Media Classic, créez votre fichier de sous-titrage vidéo en fonction du type de visionneuse que vous utilisez.

   | Type de visionneuse | Fichier de sous-titrage |
   |--- |--- |
   | HTML5 | Si vous utilisez une visionneuse de vidéos HTML5, assurez-vous que le fichier de sous-titrage que vous créez est conforme à la norme WebVTT (Web Video Text Tracks). Le fichier de sous-titrage a l’extension .vtt. D’autres informations sont disponibles sur la norme de sous-titrage WebVTT.<br><br>[Voir WebVTT](https://dev.w3.org/html5/webvtt/): Format Suivi de texte de vidéo Web. <br><br>Il existe des outils et services gratuits et payants que vous pouvez utiliser pour créer des fichiers de sous-titrage en dehors de Dynamic Media Classic. Par exemple, pour créer un fichier de sous-titrage vidéo simple sans aucun style, vous pouvez utiliser l’outil gratuit de création et de modification de sous-titrage en ligne suivant : <br><br>[WebVTT Caption Maker](https://testdrive-archive.azurewebsites.net/Graphics/CaptionMaker/Default.html) <br><br>Pour un résultat optimal, utilisez l’outil dans Internet Explorer 9 ou version ultérieure, Google Chrome ou Safari. <br><br>Dans l’outil, dans le champ <b>Enter URL of video file</b> (entrer l’URL du fichier vidéo), collez l’URL du fichier vidéo, puis cliquez sur <b>Load</b> (Charger). <br><br>Par exemple, si vous utilisez une URL Dynamic Media Classic pour votre fichier vidéo, dans DMC, cliquez sur un fichier vidéo individuel en doublon (et non sur une visionneuse de vidéos adaptative ou une vidéo de Principal) pour l’ouvrir dans la Vue de détails. Dans le panneau droit de la vue Détails, développez la liste URL et code intégré. Ensuite, sous le groupe Mobile, à droite de Mobile (progressive), cliquez sur Copier l’URL. This process gives you the URL to the video file itself which you can then paste into the <b>Enter URL of video file</b> field. Internet Explorer, Chrome ou Safari peuvent alors lire la vidéo en mode natif. Suivez maintenant les instructions à l’écran du site pour créer et enregistrer votre fichier WebVTT. Ensuite, copiez le contenu du fichier de sous-titrage et collez-le dans un éditeur de texte brut, puis enregistrez-le au format .vtt. <br><br><b>Remarque :</b> Pour une prise en charge globale des sous-titres vidéo dans des langues autres que l’anglais, sachez que la norme WebVTT exige que vous créiez des fichiers .vtt et des appels distincts pour chaque langue à prendre en charge. <br><br>En règle générale, vous attribuez au fichier VTT de sous-titrage le même nom que le fichier vidéo et vous lui ajoutez le mot captions. En procédant ainsi, vous pouvez automatiser aisément la génération des URL de vidéo en utilisant le système de gestion de contenu Web existant. |

1. Dans Dynamic Media Classic, téléchargez votre fichier de sous-titrage WebVTT, DFXP ou SMPTE XML.

   Voir [Téléchargement de fichiers](uploading-files.md#uploading_files).

1. Dans le panneau Bibliothèque de fichiers situé sur le côté gauche, accédez au dossier de fichiers qui contient le fichier vidéo à associer au fichier de sous-titrage que vous avez téléchargé.
1. Dans le panneau de navigation dans les fichiers, sélectionnez un fichier vidéo puis, sous l’image miniature du fichier, cliquez sur **[!UICONTROL Prévisualiser]** > **[!UICONTROL Liste des visionneuses]**.
1. In the Viewer List table, find the HTML5 viewer named **Univeral_HTML5_Video**, **Universal_HTML5_MixedMedia_dark**, or **Universal_HTML5_MixedMedia_light**, then do one of the following:

   * Pour une expérience de visionneuse contextuelle, cliquez sur **[!UICONTROL Copier l’URL]** à l’extrémité droite de son nom.

      Annexez l’URL copiée de la vidéo avec la syntaxe suivante pour l’associer à l’URL copiée dans le fichier de sous-titrage :

      `&caption=<full Copy URL path to the caption file .vtt>,1`

      Note the `,1` at the end of the caption URL path. Immédiatement après l’extension de fichier .vtt dans le chemin d’accès, vous avez la possibilité d’activer ou de désactiver le bouton de sous-titrage dans la barre du lecteur vidéo en le définissant sur `1` ou sur `0`, respectivement.

   * Pour une expérience de visionneuse de vidéos intégrée, cliquez sur **[!UICONTROL Code intégré]** à l’extrémité droite de son nom.

      Dans la boîte de dialogue du code intégré, cliquez sur **[!UICONTROL Copier dans le Presse-papiers]**.

      For the HTML5 `Universal_HTML5_Video`, `Universal_HTML5_MixedMedia_dark`, or `Universal_HTML5_MixedMedia_light` viewers, append the copied embed code with the following:

      `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1”`

      Note the `,1` at the end of the URL path. Immédiatement après l’extension de fichier .vtt dans le chemin d’accès de l’URL, vous avez la possibilité d’activer ou de désactiver le bouton de sous-titrage dans la barre du lecteur vidéo en le définissant sur `1` ou sur `0`, respectivement.

