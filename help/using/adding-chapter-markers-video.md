---
title: Ajout de marqueurs de chapitre à la vidéo
description: Découvrez comment ajouter des marqueurs de chapitre à une vidéo dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: a9250841-2dba-4fdc-8a6e-91b2fecef72f
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 24%

---

# Ajout de marqueurs de chapitre à la vidéo {#adding-chapter-markers-to-video}

Vous pouvez faciliter la lecture et la navigation dans vos vidéos au format long en ajoutant des marqueurs de chapitre aux vidéos uniques ou aux visionneuses de vidéos adaptatives. Lorsqu’un utilisateur lit la vidéo, il peut sélectionner les marqueurs de chapitre dans la chronologie de la vidéo (également appelée barre vidéo). Cela leur permet de naviguer facilement jusqu’à leur point ciblé ou d’accéder immédiatement à de nouveaux contenus, à des démonstrations, à des tutoriels, etc.

>[!NOTE]
>
>Le lecteur vidéo utilisé doit prendre en charge l’utilisation des marques de chapitre.

Voir [Ajout ou modification d’un paramètre prédéfini de visionneuse de vidéos](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset) si vous souhaitez configurer les points de repère de navigation des chapitres et le texte pop-up du titre du chapitre pour la visionneuse de `Universal_HTML5_Video` (HTML5).

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

Dans l’exemple ci-dessus, `Chapter 1` est l’identifiant de repère et est facultatif. L’heure de repère de `00:00:000 --> 01:04:364` indique l’heure de début et de fin du chapitre, au format 00 :00:. Les trois derniers chiffres sont les millisecondes et peuvent être laissés sur 000, selon vos préférences. Le titre du chapitre de `The bicycle store behind it all` est la description réelle du contenu du chapitre. L’identifiant de repère, l’heure de départ du repère, ainsi que le titre du chapitre apparaissent tous dans un pop-up du lecteur vidéo lorsque le pointeur survole un point de repère visuel dans la chronologie de la vidéo.

Puisque vous utilisez une visionneuse de vidéos HTML5, assurez-vous que le fichier de chapitre que vous créez est conforme à la norme WebVTT (Web Video Text Tracks). L’extension de nom de fichier de chapitres est `.VTT`. D’autres informations sont disponibles sur la norme de sous-titrage WebVTT.

Voir [WebVTT : format de suivi de texte de vidéo web](https://w3c.github.io/webvtt/).

**Pour ajouter des marqueurs de chapitre à une vidéo, procédez comme suit**

1. À l’aide d’un simple éditeur de texte en dehors d’Adobe Dynamic Media Classic, créez votre fichier de chapitres vidéo.

   >[!NOTE]
   >
   >Pour la prise en charge globale des chapitres vidéo dans des langues autres que l’anglais, la norme WebVTT exige que vous créiez des fichiers `.VTT` et des appels distincts pour chaque langue que vous souhaitez prendre en charge.

1. Enregistrez le fichier VTT en codage UTF8 pour éviter tout problème de rendu des caractères dans le texte du titre du chapitre.

   En règle générale, vous souhaitez donner au fichier VTT de chapitre le même nom qu’au fichier vidéo et l’ajouter avec `chapters`. Ainsi, vous pouvez automatiser plus facilement la génération des URL de vidéo à l’aide de votre système de gestion de contenu web existant.

1. Dans Adobe Dynamic Media Classic, chargez votre fichier de chapitres WebVTT.

   Voir [Charger des fichiers](uploading-files.md#uploading_files).

1. Dans le panneau Bibliothèque de ressources sur le côté gauche, accédez au dossier de ressources contenant le fichier vidéo à associer au fichier de chapitres que vous avez chargé.
1. Dans le panneau de navigation des ressources, sélectionnez une seule ressource vidéo, puis, sous l’image miniature de la ressource, sélectionnez **[!UICONTROL Aperçu]** > **[!UICONTROL Liste de visionneuses]**.
1. Dans le tableau Liste des visionneuses, recherchez la visionneuse HTML5 nommée **Univeral_HTML5_Video**, puis effectuez l’une des opérations suivantes :

   * Pour une expérience de visionneuse de vidéos pop-up, sélectionnez **[!UICONTROL Copier l’URL]** à l’extrémité droite du nom.

     Ajoutez l’URL copiée de la vidéo avec la syntaxe suivante pour l’associer à l’URL copiée dans votre fichier de sous-titres :

     `&navigation=*<full Copy URL path to the chapter navigation file .vtt>*`

   * Pour une expérience de visionneuse de vidéos intégrée, sélectionnez **[!UICONTROL Code intégré]** à l’extrémité droite du nom.

     Dans la boîte de dialogue Code incorporé, sélectionnez **[!UICONTROL Copier dans le presse-papiers]**.

     Pour la visionneuse `Universal_HTML5_Video` HTML5, ajoutez le code intégré copié avec les éléments suivants :

     `videoViewer.setParam("navigation","*<full Copy URL path to the chapter navigation file .vtt>*"`
