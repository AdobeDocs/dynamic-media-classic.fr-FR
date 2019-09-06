---
title: Ajout de marques de chapitre à la vidéo
seo-title: Ajout de marques de chapitre à la vidéo
description: 'null'
seo-description: Découvrez comment ajouter des marques de chapitre à une vidéo.
uuid: 4 e 1 e 6 daf-afc 6-49 d 9-ac 90-183 fe 2 a 903 b 2
contentOwner: admin
content-type: référence
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/video
discoiquuid: 8 bc 5 e 552-2 abb -41 f 0-89 d 2-bdf 3 ae 5 d 96 c 2
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Ajout de marques de chapitre à la vidéo{#adding-chapter-markers-to-video}

Vous pouvez rendre vos vidéos de forme longue plus faciles à regarder et à parcourir en ajoutant des marques de chapitre aux vidéos uniques ou aux visionneuses de vidéos adaptatives. Lorsqu’un utilisateur lit la vidéo, il peut cliquer sur les marques de chapitre du montage vidéo (également connues sous le nom de barre visuelle) pour accéder facilement à son point ciblé ou accéder immédiatement au nouveau contenu, à des démonstrations, des didacticiels, etc.

>[!NOTE]
>
>Le lecteur vidéo utilisé doit prendre en charge l’utilisation des marques de chapitre.

Voir [Ajout ou modification d’un paramètre prédéfini de visionneuse de vidéos](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset) pour configurer les indices de navigation des chapitres et le texte contextuel des titres de chapitres pour la visionneuse `Universal_HTML5_Video` (HTML5).

Voir aussi [Ajout et modification des paramètres prédéfinis de visionneuse](application-setup.md#adding_and_editing_viewer_presets).

Vous créez une liste de chapitres pour votre vidéo un peu de la même façon que vous créez des légendes. Autrement dit, vous créez un fichier WebVTT. Notez, toutefois, que ce fichier doit être distinct de tout fichier de sous-titrage WebVTT que vous pouvez également utiliser ; vous ne pouvez pas combiner des légendes et des chapitres dans un fichier WebVTT.

Vous pouvez utiliser l’exemple suivant comme exemple du format utilisé pour créer un fichier WebVTT avec une navigation de chapitre :

```as3
WEBVTT 
Chapter 1 
00:00.000 --> 01:04.364 
The bicycle store behind it all. 
Chapter 2 
01:04.364 --> 02:00.944 
Creative Cloud. 
Chapter 3 
02:00.944 --> 03:02.937 
Ease of management for a working solution. 
Chapter 4 
03:02.937 --> 03:35.000 
Cost-efficient access to rapidly evolving technology.
```

In the example above, `Chapter 1` is the cue identifier and is optional. La période de réplication `00:00:000 --> 01:04:364` correspond aux heures de début et de fin du chapitre au format 00:00:000. Les trois derniers chiffres sont les millisecondes et peuvent être laissés sur 000, selon vos préférences. The chapter title of `The bicycle store behind it all` is the actual description of the chapter’s contents. L’identifiant de duplication, l’heure de départ, ainsi que le titre de chapitre s’affichent tous dans une fenêtre contextuelle du lecteur vidéo lorsqu’un utilisateur place le pointeur de la souris sur un point de repère visuel dans le montage de la vidéo.

Puisque vous utilisez une visionneuse de vidéos HTML5, assurez-vous que le fichier de chapitre que vous créez est conforme à la norme WebVTT (Web Video Text Tracks). L’extension du fichier de chapitre est .vtt. D’autres informations sont disponibles sur la norme de sous-titrage WebVTT.

See [WebVTT: The Web Video Text Tracks format](https://dev.w3.org/html5/webvtt/).

**Pour ajouter des marques de chapitre à la vidéo**

1. Dans un éditeur de texte simple externe à Scene7 Publishing System, créez votre fichier de chapitre vidéo.

   >[!NOTE]
   >
   >Pour une prise en charge internationale des chapitres vidéo dans d’autres langues que l’anglais, n’oubliez pas que la norme WebVTT exige que vous créiez des fichiers .vtt et des appels distincts pour chaque langue à prendre en charge.

1. Enregistrer le fichier .vtt dans le codage UTF8 pour éviter tout problème lié au rendu des caractères dans le texte des titres de chapitres.

   Generally, you want to name the chapter VTT file the same name as the video file, and append it with `chapters`. En procédant ainsi, vous pouvez automatiser aisément la génération des URL de vidéo en utilisant le système de gestion de contenu Web existant.

1. Dans Scene7 Publishing System, transférez votre fichier de chapitre WebVTT.

   Voir [Téléchargement de fichiers](uploading-files.md#uploading_files).

1. Dans le panneau Bibliothèque de fichiers situé sur le côté gauche, accédez au dossier de fichiers qui contient le fichier vidéo à associer au fichier de chapitre que vous avez transféré.
1. Dans le panneau de navigation dans les fichiers, sélectionnez un fichier vidéo puis, sous l’image miniature du fichier, cliquez sur **Prévisualiser** &gt; **Liste des visionneuses**.
1. Dans le tableau Liste des visionneuses, recherchez la visionneuse HTML5 nommée **Univeral_HTML5_Video**, puis effectuez l’une des opérations suivantes :

   * Pour une expérience de visionneuse contextuelle, cliquez sur **Copier l’URL** à l’extrémité droite de son nom.

      Annexez l’URL copiée de la vidéo avec la syntaxe suivante pour l’associer à l’URL copiée dans le fichier de sous-titrage :

      `&navigation=*<full Copy URL path to the chapter navigation file .vtt>*`

   * Pour une expérience de visionneuse de vidéos intégrée, cliquez sur **Code intégré** à l’extrémité droite de son nom.

      Dans la boîte de dialogue du code intégré, cliquez sur **Copier dans le Presse-papiers**.

      For the HTML5 `Universal_HTML5_Video` viewer, append the copied embed code with the following:

      `videoViewer.setParam("navigation","*<full Copy URL path to the chapter navigation file .vtt>*”`

