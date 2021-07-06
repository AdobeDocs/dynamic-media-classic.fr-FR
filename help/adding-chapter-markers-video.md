---
title: Ajout de marques de chapitre à la vidéo
description: Découvrez comment ajouter des marqueurs de chapitre à une vidéo.
uuid: 4e1e6daf-afc6-49d9-ac90-183fe2a903b2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 8bc5e552-2abb-41f0-89d2-bdf3ae5d96c2
feature: Dynamic Media Classic,Visionneuses,Vidéo
role: User
exl-id: a9250841-2dba-4fdc-8a6e-91b2fecef72f
source-git-commit: 885fcd16559d31d3b9bad88705b4b6bec18515ee
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 51%

---

# Ajout de marques de chapitre à la vidéo{#adding-chapter-markers-to-video}

Vous pouvez rendre vos vidéos de forme longue plus faciles à regarder et à parcourir en ajoutant des marques de chapitre aux vidéos uniques ou aux visionneuses de vidéos adaptatives. Lorsqu’un utilisateur lit la vidéo, il peut cliquer sur les marqueurs de chapitre dans la chronologie de la vidéo (également appelée défilement vidéo). Cela leur permet de naviguer facilement jusqu’à leur point ciblé ou d’accéder immédiatement à un nouveau contenu, à des démonstrations, à des tutoriels, etc.

>[!NOTE]
>
>Le lecteur vidéo utilisé doit prendre en charge l’utilisation des marques de chapitre.

Voir [Ajout ou modification d’un paramètre prédéfini de visionneuse de vidéos](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset) si vous souhaitez configurer les points de repère de navigation du chapitre et le texte contextuel du titre du chapitre pour la visionneuse `Universal_HTML5_Video` (HTML5).

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

Dans l’exemple ci-dessus, `Chapter 1` est l’identifiant de repère et est facultatif. L’heure de repère `00:00:000 --> 01:04:364` spécifie l’heure de début et l’heure de fin du chapitre, au format 00:00:000. Les trois derniers chiffres sont les millisecondes et peuvent être laissés sur 000, selon vos préférences. Le titre du chapitre `The bicycle store behind it all` est la description réelle du contenu du chapitre. L’identifiant de repère, l’heure de repère de départ et le titre du chapitre apparaissent tous dans une fenêtre contextuelle du lecteur vidéo lorsque le pointeur est placé sur un point de repère visuel dans la chronologie de la vidéo.

Puisque vous utilisez une visionneuse de vidéos HTML5, assurez-vous que le fichier de chapitre que vous créez est conforme à la norme WebVTT (Web Video Text Tracks). L’extension de nom de fichier de chapitre est .VTT. D’autres informations sont disponibles sur la norme de sous-titrage WebVTT.

Voir [WebVTT : Le Texte De La Vidéo Web Effectue Le Suivi Du Format](https://w3c.github.io/webvtt/).

**Pour ajouter des marques de chapitre à la vidéo:**

1. À l’aide d’un éditeur de texte simple en dehors de Dynamic Media Classic, créez votre fichier de chapitres vidéo.

   >[!NOTE]
   >
   >Pour une prise en charge globale des chapitres vidéo dans des langues autres que l’anglais, la norme WebVTT exige que vous créiez des fichiers .vtt et des appels distincts pour chaque langue que vous souhaitez prendre en charge.

1. Enregistrez le fichier VTT en codage UTF8 afin d’éviter tout problème de rendu des caractères dans le texte du titre du chapitre.

   En règle générale, vous attribuez au fichier de chapitres VTT le même nom que le fichier vidéo et lui ajoutez `chapters`. En procédant ainsi, vous pouvez automatiser aisément la génération des URL de vidéo en utilisant le système de gestion de contenu Web existant.

1. Dans Dynamic Media Classic, téléchargez votre fichier de chapitres WebVTT.

   Voir [Téléchargement de fichiers](uploading-files.md#uploading_files).

1. Dans le panneau Bibliothèque de fichiers situé sur le côté gauche, accédez au dossier de fichiers qui contient le fichier vidéo à associer au fichier de chapitre que vous avez transféré.
1. Dans le panneau de navigation dans les fichiers, sélectionnez un fichier vidéo puis, sous l’image miniature du fichier, cliquez sur **[!UICONTROL Prévisualiser]** > **[!UICONTROL Liste des visionneuses]**.
1. Dans le tableau Liste des visionneuses, recherchez la visionneuse HTML5 nommée **Univeral_HTML5_Video**, puis effectuez l’une des opérations suivantes :

   * Pour une expérience de visionneuse contextuelle, cliquez sur **[!UICONTROL Copier l’URL]** à l’extrémité droite de son nom.

      Ajoutez l’URL copiée de la vidéo avec la syntaxe suivante afin de l’associer à l’URL copiée dans votre fichier de sous-titres :

      `&navigation=*<full Copy URL path to the chapter navigation file .vtt>*`

   * Pour une expérience de visionneuse de vidéos intégrée, cliquez sur **[!UICONTROL Code intégré]** à l’extrémité droite de son nom.

      Dans la boîte de dialogue du code intégré, cliquez sur **[!UICONTROL Copier dans le Presse-papiers]**.

      Pour la visionneuse HTML5 `Universal_HTML5_Video`, ajoutez le code intégré copié avec ce qui suit :

      `videoViewer.setParam("navigation","*<full Copy URL path to the chapter navigation file .vtt>*”`
