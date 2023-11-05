---
title: Déployer de la vidéo sur vos sites Web et sites mobiles
description: Découvrez comment déployer des vidéos sur vos sites web et sites mobiles à partir d’Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 3df22d48-edb5-4927-aefb-104b53f81f1a
topic: Content Management
level: Intermediate
source-git-commit: 51c05c62448b39a75facb2e90cc9da5d0f26ab45
workflow-type: tm+mt
source-wordcount: '1708'
ht-degree: 33%

---

# Déployer de la vidéo sur vos sites Web et sites mobiles{#deploying-video-to-your-websites-and-mobile-sites}

Les sites web, les sites mobiles et les applications de bureau accèdent au contenu du serveur Adobe Dynamic Media Classic, y compris aux vidéos, à l’aide de chaînes d’URL ou de code incorporé. Adobe Dynamic Media Classic active ces chaînes URL lors du processus de publication. Pour placer la chaîne URL ou le code intégré de votre vidéo dans vos pages web, pages mobiles et applications de bureau, copiez-la depuis Adobe Dynamic Media Classic.

>[!NOTE]
>
>l’URL ou le code intégré n’est actif(ve) qu’une fois le fichier publié.

## Publier de la vidéo {#publishing-video}

La publication d’une vidéo permet aux serveurs Adobe Dynamic Media Classic de diffuser de la vidéo sur votre site web, site mobile ou application.

Vous pouvez utiliser deux méthodes différentes pour publier une vidéo :

* **Publier des vidéos automatiquement et instantanément lors du téléchargement** - Dans le cadre du processus de chargement de vidéo, Adobe Dynamic Media Classic peut publier automatiquement les vidéos lorsqu’elles sont chargées et codées. Cette capacité de publication instantanée signifie qu’il n’est pas nécessaire de publier les vidéos séparément après coup.

* **Publication d’une vidéo manuellement après le transfert** - Si vous ne souhaitez pas publier les vidéos immédiatement, vous pouvez les publier manuellement à tout moment.

Une fois les vidéos publiées, Adobe Dynamic Media Classic active les chaînes URL de votre code d’application ou de votre page de HTML.

**Publication d’une vidéo:**

1. Effectuez l’une des opérations suivantes :

   * Pour publier des vidéos automatiquement et instantanément lors du téléchargement, sur la page Télécharger, sélectionnez **[!UICONTROL Publier après le téléchargement]**. Vous avez terminé ; il ne reste plus aucune étape à exécuter.
   * Pour publier des vidéos manuellement après le chargement, dans le panneau de navigation, sélectionnez les vidéos, puis, dans la barre de navigation globale, sélectionnez **Publier**.

## Liaison d’une URL de vidéo à un site mobile ou à un site web {#linking-a-video-url-to-a-mobile-site-or-a-website}

Lorsque vous publiez une vidéo, vous pouvez obtenir l’URL associée à utiliser sur votre site web, votre site mobile ou votre application de bureau. Utilisez l’URL de la vidéo lorsque vous souhaitez afficher la vidéo dans une fenêtre contextuelle ou modale au haut de la page Web.

Lorsqu’un client sélectionne le lien, son appareil, sa bande passante et sa taille d’écran sont automatiquement détectés. S’il s’agit d’un ordinateur, la vidéo adéquate s’affiche dans une visionneuse prédéfinie ; dans le cas d’un smartphone ou d’une tablette, elle s’affiche dans le lecteur vidéo natif du périphérique en question.

Voir aussi [Incorporation de la visionneuse de vidéos dans une page web](deploying-video-websites-mobile-sites.md#embedding_the_video_viewer_on_a_web_page).

**Liaison d’une URL de vidéo à un site Web ou à un site mobile:**

1. Dans le panneau de navigation des ressources, dans la **[!UICONTROL Afficher]** liste déroulante, sélectionnez **[!UICONTROL Vidéo]**, ou **[!UICONTROL Visionneuse de vidéos adaptative]**.
1. Dans le panneau Bibliothèque de fichiers sur la gauche, accédez au dossier Fichiers qui contient la vidéo ou la vidéo adaptative que vous souhaitez lier.
1. Au-dessus du panneau de navigation dans les fichiers, à droite de la barre d’outils, effectuez l’une des opérations suivantes :

   * Sélectionner **[!UICONTROL Affichage de la grille]** ou **[!UICONTROL Mode Liste]**. Dans le panneau de navigation des fichiers, cliquez deux fois sur la miniature vidéo d’un fichier pour l’ouvrir en mode Affichage des détails. Dans le panneau URL et code intégré à droite, sous Diffusion en flux continu HTTP, sélectionnez **[!UICONTROL Copier l’URL]** à droite de la visionneuse que vous souhaitez. Il est recommandé de copier l’URL associée à la variable `Universal_HTML5_Video` visionneuse.
   * Sélectionner **[!UICONTROL Affichage de la grille]**. Dans le panneau de navigation des ressources, sélectionnez une seule ressource, puis sous l’image miniature, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**.

     Dans la page Liste des visionneuses, sous la colonne Actions du tableau, sélectionnez **[!UICONTROL Copier l’URL]**. Il est recommandé de copier l’URL associée à la variable `Universal_HTML5_Video` visionneuse.

   * Sélectionner **[!UICONTROL Mode Liste]**. Dans le panneau de navigation des ressources, sélectionnez une seule ressource, puis, à droite de l’image miniature, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**.

     Dans la page Liste des visionneuses, sous la colonne Actions du tableau, sélectionnez **[!UICONTROL Copier l’URL]**. Il est recommandé de copier l’URL associée à la variable `Universal_HTML5_Video` visionneuse.

   * Sélectionner **[!UICONTROL Affichage de la grille]**, **[!UICONTROL Mode Liste]**, ou **[!UICONTROL Affichage des détails]**. Dans la même barre d’outils, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**.

     Dans la page Liste des visionneuses, sous la colonne Actions du tableau, sélectionnez **[!UICONTROL Copier l’URL]**. Il est recommandé de copier l’URL associée à la variable `Universal_HTML5_Video` visionneuse.

1. Collez l’URL de vidéo HTML5 sur vos sites Web et mobile.

## Incorporation de la visionneuse de vidéos dans une page web {#embedding-the-video-viewer-on-a-web-page}

Utilisez la fonction Intégrer le code lorsque vous souhaitez lire la vidéo incorporée sur une page Web. Vous copiez le code intégré dans le Presse-papiers afin de pouvoir le coller dans vos pages Web. Vous ne pouvez pas modifier le code dans la boîte de dialogue Code intégré.

Voir aussi [Liaison d’une URL de vidéo à un site mobile ou à un site web](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

**Incorporation de la visionneuse de vidéos sur une page Web:**

1. Dans la liste déroulante Afficher du panneau de navigation des ressources, sélectionnez **[!UICONTROL Vidéo]**, ou **[!UICONTROL Visionneuse de vidéos adaptative]**.
1. Dans le panneau Bibliothèque de fichiers sur la gauche, accédez au dossier Fichiers qui contient la vidéo ou la visionneuse de vidéos adaptative dont vous voulez copier le code intégré.
1. Au-dessus du panneau de navigation dans les fichiers, à droite de la barre d’outils, effectuez l’une des opérations suivantes :

   * Sélectionner **[!UICONTROL Affichage de la grille]** ou **[!UICONTROL Mode Liste]**. Dans le panneau de navigation des fichiers, cliquez deux fois sur la miniature vidéo d’un fichier pour l’ouvrir en mode Affichage des détails. Dans le panneau URL et code intégré à droite, sous Diffusion en flux continu HTTP, sélectionnez **[!UICONTROL Code incorporé]** à droite de la visionneuse que vous souhaitez. Pour une bonne pratique, sélectionnez **[!UICONTROL Code incorporé]** qui est associé à la variable `Universal_HTML5_Video` visionneuse.
   * Sélectionner **[!UICONTROL Affichage de la grille]**. Dans le panneau de navigation des ressources, sélectionnez une seule ressource, puis sous l’image de miniature vidéo, sélectionnez **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**.

     Dans la page Liste des visionneuses, sous la colonne Actions du tableau, sélectionnez **[!UICONTROL Code incorporé]**. Pour une bonne pratique, sélectionnez **[!UICONTROL Code incorporé]** qui est associé à la variable `Universal_HTML5_Video` visionneuse.

   * Sélectionner **[!UICONTROL Mode Liste]**. Dans le panneau de navigation des ressources, sélectionnez une seule ressource, puis, à droite de l’image miniature, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**.

     Dans la page Liste des visionneuses, sous la colonne Actions du tableau, sélectionnez **[!UICONTROL Code incorporé]**. Pour une bonne pratique, sélectionnez **[!UICONTROL Code incorporé]** qui est associé à la variable `Universal_HTML5_Video` visionneuse.

   * Sélectionner **[!UICONTROL Affichage de la grille]**, **[!UICONTROL Mode Liste]**, ou **[!UICONTROL Affichage des détails]**. Dans la même barre d’outils, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**.

     Dans la page Liste des visionneuses, sous la colonne Actions du tableau, sélectionnez **[!UICONTROL Code incorporé]**. Pour une bonne pratique, sélectionnez **[!UICONTROL Code incorporé]** qui est associé à la variable `Universal_HTML5_Video` visionneuse.

1. Dans la boîte de dialogue Code incorporé, sélectionnez **[!UICONTROL Copier dans le Presse-papiers]**.

   Vous ne pouvez pas modifier le code dans la boîte de dialogue Code incorporé.

1. select **[!UICONTROL Fermer]**.
1. Collez le code intégré dans vos pages Web.

### Mise en oeuvre du code intégré pour l’utilisation de la vidéo HTML5 avec des ressources vidéo MP4 {#implementing-embed-code-for-using-html-video-with-mp-video-assets}

Si vous n’utilisez pas le lecteur vidéo Adobe Dynamic Media Classic HTML5, mais que vous souhaitez utiliser le HTML natif5. `<video>` avec des ressources vidéo MP4, vous pouvez utiliser l’exemple de code intégré suivant :

```as3
<video poster="S7 video thumbnail URL" controls> 
        <source src="S7 OGG video asset URL (no player)" type='video/ogg; codecs="theora, vorbis"'/> 
        <source src="S7 MP4 mobile progressive video asset URL (no player)" type='video/mp4; codecs="avc1.4D401E, mp4a.40.2"'/> 
        <p>This is fallback content</p> 
</video>
```

* Remplacer `"S7 video thumbnail URL"` avec l’URL de miniature de la vidéo, qui est l’image miniature de la vidéo qu’un utilisateur voit avant de lire la vidéo.

  Voir [Obtention des URL des miniatures vidéo](deploying-video-websites-mobile-sites.md#obtaining_video_thumbnail_urls).

* Remplacer `"S7 OGG video asset URL (no player)"` avec l’URL progressive de la vidéo OGG.

  Voir [Liaison d’une URL de vidéo à un site mobile ou à un site web](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

* Remplacer `"S7 MP4 mobile progressive video asset URL (no player)"` avec l’URL progressive mobile de la vidéo.

  Voir [Liaison d’une URL de vidéo à un site mobile ou à un site web](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

## Déploiement d’une vidéo à l’aide d’un lecteur vidéo tiers {#deploying-video-using-a-third-party-video-player}

Si vous utilisez un lecteur vidéo tiers ou un lecteur vidéo personnalisé au lieu d’une visionneuse de vidéos Dynamic Media Classic, vous obtenez l’URL de vidéo directe qui fonctionne pour la diffusion en continu à débit multiple HLS ou le téléchargement progressif.

**Déploiement d’une vidéo à l’aide d’un lecteur vidéo tiers:**

1. Dans Adobe Dynamic Media Classic, dans la barre de navigation globale, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Paramètres généraux]**.
1. Selon le type d’URL à utiliser, effectuez l’une des opérations suivantes :

* Pour générer une URL de vidéo en flux continu HLS direct (à débit multiple)

  Sur le **[!UICONTROL Paramètres généraux de l’application]** , dans la variable **[!UICONTROL Serveurs]** , dans la variable **[!UICONTROL Nom du serveur publié]** champ de texte, construisez l’URL directe. Utilisez la syntaxe suivante : `server/is/content/company/folder/filename.m3u8`

  Supposons, par exemple, que le nom du serveur publié soit `https://s7d9.scene7.com/.` En utilisant la syntaxe de l’étape 2, l’URL directe peut se présenter comme suit :
  `https://s7d9.scene7.com/is/content/GeoRetail/AdobeRIA-AVS.m3u8`

* Pour générer une URL de vidéo en flux continu HLS direct (débit unique)

  Sur le **[!UICONTROL Paramètres généraux de l’application]** , dans la variable **[!UICONTROL Serveurs]** , dans la variable **[!UICONTROL Nom du serveur de diffusion HLS]** champ de texte, construisez l’URL directe à l’aide de la syntaxe suivante :

  `server/company/folder/filename.ext.m3u8`

  Supposons, par exemple, que le nom du serveur de diffusion HLS soit `https://s7mbrstream.scene7.com/hls-vod/`. En utilisant la syntaxe de l’étape 2, l’URL directe peut se présenter comme suit :
  `https://s7mbrstream.scene7.com/hls-vod/GeoRetail/MBR/ToyStory3\_Teaser1\_High\_iPad\_768x432\_1296K.mp4.m3u8`

* Génération d’une URL de vidéo progressive directe

  Sur la page **[!UICONTROL Paramètres généraux de l’application]**, dans le groupe **[!UICONTROL Serveurs]**, dans le champ **[!UICONTROL Nom du serveur de vidéo progressive]**, générez l’URL eVideo directe selon la syntaxe suivante :

  `server/company/folder/filename`

  Supposons, par exemple, que le nom du serveur de vidéo progressive soit `https://s7d9.scene7.com/is/content/`. En utilisant la syntaxe de l’étape 2, l’URL directe peut se présenter comme suit :
  `https://s7d9.scene7.com/e2/GeoRetail/SourceVideo/outdoors.mp4`

## Utilisation des miniatures vidéo {#working-with-video-thumbnails}

Adobe Dynamic Media Classic génère des miniatures pour les vidéos codées et les vidéos précodées. Vous pouvez utiliser des miniatures vidéo comme n’importe quelle autre image. De plus, vous pouvez obtenir des URL pour les miniatures vidéo générées par Adobe Dynamic Media Classic. Vous pouvez ensuite déployer ces URL en dehors d’Adobe Dynamic Media Classic. Vous pouvez, par exemple, déployer les miniatures dans des résultats de recherche, des listes de vidéos correspondantes et des listes de lecture vidéo sur un site Web.

Les miniatures sont générées en fonction de la première image hétérogène (pas une image toute noire, toute blanche, etc.) de la vidéo.

### Obtention des URL des miniatures vidéo {#obtaining-video-thumbnail-urls}

Adobe Dynamic Media Classic génère automatiquement des miniatures vidéo pendant le processus de téléchargement. Les miniatures s’affichent dans le panneau Parcourir en mode Liste et Grille.

Pour générer des URL de miniatures vidéo, effectuez une opération de publication.

Voir [Publier la vidéo](deploying-video-websites-mobile-sites.md#publishing_video).

Une fois la publication terminée, vous pouvez obtenir des URL de miniatures vidéo en mode Affichage des détails dans le panneau URL et Code intégré. Sélectionner **[!UICONTROL Copier l’URL]** à droite de la miniature vidéo afin que vous puissiez copier l’URL qui lui est associée.

### Modification des images d’affiche dans les visionneuses de vidéos {#modifying-poster-frames-in-video-viewers}

Le *cadre d’affiche* est la première image qui apparaît dans les visionneuses de vidéos avant que ne commence la lecture de la vidéo. Adobe Dynamic Media Classic utilise des miniatures vidéo comme images d’affiche.

Vous pouvez appliquer des modificateurs d’image au cadre d’affiche. Vous pouvez, par exemple, rogner le cadre d’affiche ou le rendre transparent. Pour modifier le cadre d’affiche, ouvrez l’écran de configuration de la visionneuse de vidéos et saisissez les modificateurs dans la section Poster Image Modifiers (Modificateurs de l’image d’affiche). 

Voir [Ajouter ou modifier un paramètre prédéfini de visionneuse de vidéos](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

Voir [Guide de diffusion d’images](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-is-home.html?lang=en#image-serving-api).

Vous pouvez également modifier des miniatures vidéo en ajoutant des modificateurs aux URL de miniature vidéo.

>[!MORELIKETHIS]
>
>* [Publication de fichiers](publishing-files.md#publishing_files)