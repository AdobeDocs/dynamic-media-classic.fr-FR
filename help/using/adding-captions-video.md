---
title: Ajout de sous-titres à une vidéo
description: Découvrez comment ajouter des sous-titres à une vidéo dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 66a1ab20-6036-4c3d-bb66-dd06d917c7f2
topic: Content Management
level: Intermediate
source-git-commit: a30bc34b1943d63620cb12098b7bd2db4714086d
workflow-type: tm+mt
source-wordcount: '719'
ht-degree: 31%

---

# Ajout de sous-titres à une vidéo {#adding-captions-to-video}

Vous pouvez étendre la portée de vos vidéos aux marchés mondiaux en ajoutant des sous-titres aux vidéos ou aux visionneuses de vidéos adaptatives. En ajoutant des sous-titres vous évitez d’avoir à réenregistrer le son ou de recourir à des locuteurs natifs pour réenregistrer l’audio dans chacune des langues. La vidéo est lue dans la langue dans laquelle elle a été enregistrée. Les sous-titres en langue étrangère s’affichent pour que les personnes parlant d’autres langues puissent néanmoins comprendre la partie audio.

Les légendes élargissent également l’accessibilité en utilisant le sous-titrage télétexte pour les sourds ou les malentendants.

>[!NOTE]
>
>le lecteur vidéo utilisé doit prendre en charge l’affichage des sous-titres.

Pour configurer l’effet Légende et modifier le menu Légende lui-même, y compris le texte du menu pour l’une des visionneuses suivantes :

* `Universal_HTML5_Video` observateur
* `Universal_HTML5_MixedMedia_dark` observateur
* `Universal_HTML5_MixedMedia_light` observateur

Voir [Ajouter ou modifier un paramètre prédéfini de visionneuse de vidéos](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

Voir aussi [Ajout et modification de paramètres prédéfinis de visionneuse](application-setup.md#adding_and_editing_viewer_presets).

Adobe Dynamic Media Classic peut convertir les fichiers de sous-titres au format JSON (JavaScript Object Notation). Cette conversion signifie que vous pouvez intégrer le texte JSON dans une page Web comme transcription masquée mais complète de la vidéo. Les moteurs de recherche peuvent ensuite analyser et indexer le contenu pour faciliter la découverte des vidéos et donner aux clients plus de détails sur le contenu vidéo.

Voir [Diffuser du contenu statique (hors image)](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents.html?lang=en#image-serving-api) dans le *Aide de l’API Adobe Image Serving* pour plus d’informations sur l’utilisation de la fonction JSON dans une URL.

**Pour ajouter des sous-titres à une vidéo :**

1. À l’aide d’une application tierce en dehors d’Adobe Dynamic Media Classic, créez votre fichier de sous-titres vidéo en fonction du type de visionneuse que vous utilisez.

   | Type de visionneuse | Fichier de sous-titrage |
   |--- |--- |
   | HTML5 | Si vous utilisez une visionneuse de vidéos HTML5, assurez-vous que le fichier de sous-titrage que vous créez est conforme à la norme WebVTT (Web Video Text Tracks). Le fichier de sous-titrage a l’extension .vtt. D’autres informations sont disponibles sur la norme de sous-titrage WebVTT.<br><br>[Voir WebVTT](https://w3c.github.io/webvtt/): format de suivi de texte vidéo web. <br><br>De nombreux sites web offrent des outils et des services gratuits et gratuits que vous pouvez utiliser pour créer des fichiers de sous-titres WebVTT en dehors d’Adobe Dynamic Media Classic. <br><br>Suivez les instructions à l’écran d’un site pour créer et enregistrer votre fichier WebVTT. Une fois que vous avez terminé, copiez le contenu du fichier de sous-titres et collez-le dans un éditeur de texte brut, puis enregistrez-le avec l’extension de nom de fichier VTT. <br><br><b>Remarque :</b> Pour une prise en charge globale des sous-titres vidéo dans des langues autres que l’anglais, la norme WebVTT exige que vous créiez des fichiers .vtt et des appels distincts pour chaque langue que vous souhaitez prendre en charge. <br><br>En règle générale, vous attribuez au fichier de sous-titres VTT le même nom que le fichier vidéo et lui ajoutez des sous-titres. En procédant ainsi, vous pouvez automatiser aisément la génération des URL de vidéo en utilisant le système de gestion de contenu Web existant. |

1. Dans Adobe Dynamic Media Classic, téléchargez votre fichier de sous-titres WebVTT, DFXP ou SMPTE XML.

   Voir [Chargement de fichiers](uploading-files.md#uploading_files).

1. Dans le panneau Bibliothèque de fichiers situé sur le côté gauche, accédez au dossier de fichiers qui contient le fichier vidéo à associer au fichier de sous-titrage que vous avez téléchargé.
1. Dans le panneau de navigation des ressources, sélectionnez une seule ressource vidéo, puis sous l’image de miniature de la ressource, sélectionnez **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**.
1. Dans le tableau Liste des visionneuses , recherchez la visionneuse HTML5 nommée **Univeral_HTML5_Video**, **Universal_HTML5_MixedMedia_dark**, ou **Universal_HTML5_MixedMedia_light**, puis effectuez l’une des opérations suivantes :

   * Pour une expérience de visionneuse de vidéos contextuelle, sélectionnez **[!UICONTROL Copier l’URL]** à l’extrême droite du nom.

     Ajoutez l’URL copiée de la vidéo avec la syntaxe suivante afin de l’associer à l’URL copiée dans votre fichier de sous-titres :

     `&caption=<full Copy URL path to the caption file .vtt>,1`

     Notez que `,1` à la fin du chemin d’accès à l’URL de la légende. Immédiatement après l’extension de nom de fichier VTT dans le chemin d’accès, vous pouvez éventuellement activer ou désactiver le bouton de sous-titres dans la barre de lecteur vidéo en définissant sur `1` ou `0`, respectivement.

   * Pour une expérience de visionneuse de vidéos intégrée, sélectionnez **[!UICONTROL Code incorporé]** à l’extrême droite du nom.

     Dans la boîte de dialogue Code incorporé, sélectionnez **[!UICONTROL Copier dans le Presse-papiers]**.

     Pour le HTML5 `Universal_HTML5_Video`, `Universal_HTML5_MixedMedia_dark`, ou `Universal_HTML5_MixedMedia_light` visionneuses, ajoutez le code intégré copié avec ce qui suit :

     `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1"`

     Notez que `,1` à la fin du chemin de l’URL. Immédiatement après l’extension de nom de fichier VTT dans le chemin d’URL, vous pouvez éventuellement activer ou désactiver le bouton de légende sur la barre de lecteur vidéo en définissant sur `1` ou `0`, respectivement.
