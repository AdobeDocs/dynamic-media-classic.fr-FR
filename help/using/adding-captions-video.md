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
source-git-commit: c4613c78347c4bda3d84747a72146617158c03b6
workflow-type: tm+mt
source-wordcount: '703'
ht-degree: 15%

---

# Ajout de sous-titres à une vidéo {#add-captions-to-video}

Étendez la portée de vos vidéos aux marchés mondiaux. Pour ce faire, vous pouvez ajouter des sous-titres à des vidéos uniques ou à des visionneuses de vidéos adaptatives. En ajoutant des sous-titres vous évitez d’avoir à réenregistrer le son ou de recourir à des locuteurs natifs pour réenregistrer l’audio dans chacune des langues. La vidéo est lue dans la langue dans laquelle elle a été enregistrée. Les sous-titres en langue étrangère s’affichent pour que les personnes parlant d’autres langues puissent néanmoins comprendre la partie audio.

Les légendes élargissent également l’accessibilité en utilisant le sous-titrage télétexte pour les sourds ou les malentendants.

>[!NOTE]
>
>Le lecteur vidéo utilisé doit prendre en charge l’affichage des sous-titres.

Pour configurer l’effet de légende et modifier le menu de légende lui-même, y compris le texte du menu pour l’une des visionneuses suivantes :

* Visionneuse `Universal_HTML5_Video`
* Visionneuse `Universal_HTML5_MixedMedia_dark`
* Visionneuse `Universal_HTML5_MixedMedia_light`

Voir [Ajout ou modification d’un paramètre prédéfini de visionneuse de vidéos](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

Voir aussi [Ajout et modification de paramètres prédéfinis de visionneuse](application-setup.md#adding_and_editing_viewer_presets).

Adobe Dynamic Media Classic peut convertir les fichiers de sous-titres au format JSON (JavaScript Object Notation). Cette conversion signifie que vous pouvez incorporer le texte JSON dans une page web sous la forme d’une transcription masquée complète de la vidéo. Les moteurs de recherche peuvent ensuite analyser et indexer le contenu pour rendre les vidéos plus facilement détectables et fournir aux clients et clientes plus de détails sur le contenu vidéo.

Pour plus d’informations sur l’utilisation de la fonction JSON dans une URL[&#x200B; voir &#x200B;](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents#image-serving-api)Diffuser du contenu statique (hors images)dans .

**Pour ajouter des sous-titres à une vidéo, procédez comme suit**

1. À l’aide d’une application tierce extérieure à Adobe Dynamic Media Classic, créez votre fichier de sous-titres vidéo en fonction du type de visionneuse que vous utilisez.

   | Type de visionneuse | Fichier de sous-titrage |
   |--- |--- |
   | HTML5 | Si vous utilisez une visionneuse de vidéos HTML5, assurez-vous que le fichier de sous-titrage que vous créez est conforme à la norme WebVTT (Web Video Text Tracks). L’extension de nom de fichier pour les sous-titres est `.VTT`. D’autres informations sont disponibles sur la norme de sous-titrage WebVTT.<br><br>[Voir WebVTT](https://w3c.github.io/webvtt/) : format de suivi de texte de vidéo web. <br><br>De nombreux sites Web proposent des outils et des services gratuits ou payants que vous pouvez utiliser pour créer des fichiers de sous-titres WebVTT. <br><br>Suivez les instructions à l’écran d’un site pour créer et enregistrer votre fichier WebVTT. Lorsque vous avez terminé, copiez le contenu du fichier de sous-titres et collez-le dans un éditeur de texte brut, puis enregistrez-le avec une extension de fichier VTT. <br><br><b>Remarque :</b> pour la prise en charge globale des sous-titres vidéo dans des langues autres que l’anglais, la norme WebVTT exige que vous créiez des fichiers `.VTT` et des appels distincts pour chaque langue que vous souhaitez prendre en charge. <br><br>En règle générale, vous souhaitez attribuer au fichier de sous-titres VTT le même nom qu’au fichier vidéo et vous lui ajoutez des sous-titres. Ainsi, vous pouvez automatiser plus facilement la génération des URL de vidéo à l’aide de votre système de gestion de contenu web existant. |

1. Dans Adobe Dynamic Media Classic, chargez votre fichier de sous-titres XML WebVTT, DFXP ou SMPTE.

   Voir [Charger des fichiers](uploading-files.md#uploading_files).

1. Dans le panneau Bibliothèque de ressources sur le côté gauche, accédez au dossier de ressources contenant le fichier vidéo à associer au fichier de sous-titres que vous avez chargé.
1. Dans le panneau de navigation des ressources, sélectionnez une seule ressource vidéo, puis, sous l’image miniature de la ressource, sélectionnez **[!UICONTROL Aperçu]** > **[!UICONTROL Liste de visionneuses]**.
1. Dans le tableau Liste des visionneuses, recherchez la visionneuse HTML5 nommée **Univeral_HTML5_Video**, **Universal_HTML5_MixedMedia_dark** ou **Universal_HTML5_MixedMedia_light**, puis effectuez l’une des opérations suivantes :

   * Pour une expérience de visionneuse de vidéos pop-up, sélectionnez **[!UICONTROL Copier l’URL]** à l’extrémité droite du nom.

     Ajoutez l’URL copiée de la vidéo avec la syntaxe suivante pour l’associer à l’URL copiée dans votre fichier de sous-titres :

     `&caption=<full Copy URL path to the caption file .vtt>,1`

     Notez la `,1` à la fin du chemin d’URL de la légende. Juste après l’extension de fichier VTT dans le chemin d’accès, vous avez la possibilité d’activer ou de désactiver le bouton de sous-titres dans la barre de lecteur vidéo en définissant la valeur sur `1` ou `0`, respectivement.

   * Pour une expérience de visionneuse de vidéos intégrée, sélectionnez **[!UICONTROL Code intégré]** à l’extrémité droite du nom.

     Dans la boîte de dialogue Code incorporé, sélectionnez **[!UICONTROL Copier dans le presse-papiers]**.

     Pour les visionneuses `Universal_HTML5_Video`, `Universal_HTML5_MixedMedia_dark` ou `Universal_HTML5_MixedMedia_light` d’HTML5, ajoutez le code intégré copié avec les éléments suivants :

     `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1"`

     Notez la `,1` à la fin du chemin de l’URL. Juste après l’extension de fichier VTT dans le chemin d’accès URL, vous avez la possibilité d’activer ou de désactiver le bouton de sous-titres dans la barre de lecteur vidéo en définissant la valeur sur `1` ou `0`, respectivement.
