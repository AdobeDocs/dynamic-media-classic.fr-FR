---
title: Déploiement de vidéos sur vos sites Web et sites mobiles
seo-title: Déploiement de vidéos sur vos sites Web et sites mobiles
description: 'null'
seo-description: Découvrez comment déployer une vidéo sur vos sites Web et sites mobiles.
uuid: 22 bb 4402-c 0 ab -4 df 0-89 b 9-99707 d 111927
contentOwner: admin
content-type: référence
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/video
discoiquuid: 0 d 006314-c 4 cc -4 f 6 c-a 51 c -6075 bb 445 e 39
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Déploiement de vidéos sur vos sites Web et sites mobiles{#deploying-video-to-your-websites-and-mobile-sites}

Les sites Web, sites mobiles et applications de bureau accèdent au contenu du serveur Dynamic Media Classic, y compris aux vidéos, à l'aide de chaînes URL ou de code incorporé. Dynamic Media Classic active ces chaînes URL pendant le processus de publication. Pour placer la chaîne d’URL ou le code intégré de la vidéo dans vos pages Web, pages mobiles et applications de bureau, copiez-les depuis Scene7 Publishing System.

>[!NOTE]
>
>l’URL ou le code intégré n’est actif(ve) qu’une fois le fichier publié.

## Publication des vidéos {#publishing-video}

La publication d'une vidéo permet aux serveurs Dynamic Media Classic de diffuser des vidéos sur votre site Web, site mobile ou application.

Deux méthodes peuvent être utilisées pour publier la vidéo :

* **Publication de vidéos automatiquement et immédiatement lors du transfert**

   Dans le cadre du processus de téléchargement vidéo, Dynamic Media Classic peut publier automatiquement des vidéos lorsqu'elles sont téléchargées et codées. Cette capacité de publication instantanée signifie qu’il n’est pas nécessaire de publier les vidéos séparément après coup.

* **Publication d’une vidéo manuellement après le transfert**

   Si vous ne souhaitez pas publier les vidéos immédiatement, vous pouvez les publier manuellement à tout moment.

Une fois que vous avez publié des vidéos, Scene7 Publishing System active les chaînes URL du code HTML de vos pages ou de votre application.

**Publication d’une vidéo**

1. Effectuez l’une des opérations suivantes :

   * Pour publier des vidéos automatiquement et immédiatement lors du transfert, dans l’écran de téléchargement, cliquez sur **Publier après le téléchargement**. Vous avez terminé ; il ne reste plus aucune étape à exécuter.
   * Pour publier manuellement les vidéos après le téléchargement, dans le panneau de navigation, sélectionnez-les, puis sur la barre de navigation globale, cliquez sur **Publier**.

## Liaison d’une URL de vidéo à un site Web ou un site mobile {#linking-a-video-url-to-a-mobile-site-or-a-website}

Après avoir publié une vidéo, vous pouvez obtenir son URL en vue de l’utiliser sur un site Web, un site mobile ou dans une application de bureau. Utilisez l’URL de la vidéo lorsque vous souhaitez afficher la vidéo dans une fenêtre contextuelle ou modale au haut de la page Web.

Lorsqu’un utilisateur clique sur le lien, son périphérique, sa bande passante et la taille de son écran sont automatiquement détectés. S’il s’agit d’un ordinateur, la vidéo adéquate s’affiche dans une visionneuse prédéfinie ; dans le cas d’un smartphone ou d’une tablette, elle s’affiche dans le lecteur vidéo natif du périphérique en question.

Voir aussi [Incorporation de la visionneuse de vidéos sur une page Web](deploying-video-websites-mobile-sites.md#embedding_the_video_viewer_on_a_web_page).

**Liaison d’une URL de vidéo à un site Web ou à un site mobile**

1. Dans la liste déroulante Afficher du panneau de navigation des fichiers, cliquez sur **Vidéo** ou sur **Visionneuse de vidéos adaptative**.
1. Dans le panneau Bibliothèque de fichiers sur la gauche, accédez au dossier Fichiers qui contient la vidéo ou la vidéo adaptative que vous souhaitez lier.
1. Au-dessus du panneau de navigation dans les fichiers, à droite de la barre d’outils, effectuez l’une des opérations suivantes :

   * Cliquez sur **Affichage de la grille** ou **Affichage par liste**. Dans le panneau de navigation des fichiers, cliquez deux fois sur la miniature vidéo d’un fichier pour l’ouvrir en mode Affichage des détails. Dans le panneau des URL et du code intégré sur la droite, sous Diffusion en flux continu HTTP, cliquez sur **Copier l’URL** à droite de la visionneuse appropriée. As a best practice, copy the URL associated with the `Universal_HTML5_Video` viewer.
   * Cliquez sur **Affichage de la grille**. Dans le panneau de navigation dans les fichiers, sélectionnez un fichier, puis sous l’image miniature, cliquez sur **Prévisualiser** &gt; **Liste des visionneuses**.

      Dans la page Liste des visionneuses, dans la colonne Actions du tableau, cliquez sur **Copier l’URL**. As a best practice, copy the URL associated with the `Universal_HTML5_Video` viewer.

   * Cliquez sur **Affichage par liste**. Dans le panneau de navigation dans les fichiers, sélectionnez un fichier, puis à droite de l’image miniature, cliquez sur **Prévisualiser** &gt; **Liste des visionneuses**.

      Dans la page Liste des visionneuses, dans la colonne Actions du tableau, cliquez sur **Copier l’URL**. As a best practice, copy the URL associated with the `Universal_HTML5_Video` viewer.

   * Cliquez sur **Affichage de la grille**, **Affichage par liste** ou **Affichage des détails**. Dans la même barre d’outils, cliquez sur **Prévisualiser** &gt; **Liste des visionneuses**.

      Dans la page Liste des visionneuses, dans la colonne Actions du tableau, cliquez sur **Copier l’URL**. As a best practice, copy the URL associated with the `Universal_HTML5_Video` viewer.

1. Collez l’URL de vidéo HTML5 sur vos sites Web et mobile.

## Intégration de la visionneuse de vidéos sur une page Web {#embedding-the-video-viewer-on-a-web-page}

Utilisez la fonction Intégrer le code lorsque vous souhaitez lire la vidéo incorporée sur une page Web. Vous copiez le code intégré dans le Presse-papiers afin de pouvoir le coller dans vos pages Web. Vous ne pouvez pas modifier le code dans la boîte de dialogue Code intégré.

Voir aussi [Liaison d’une URL de vidéo à un site Web ou à un site mobile](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

**Incorporation de la visionneuse de vidéos sur une page Web**

1. Dans la liste déroulante Afficher du panneau de navigation des fichiers, cliquez sur **Vidéo** ou sur **Visionneuse de vidéos adaptative**.
1. Dans le panneau Bibliothèque de fichiers sur la gauche, accédez au dossier Fichiers qui contient la vidéo ou la visionneuse de vidéos adaptative dont vous voulez copier le code intégré.
1. Au-dessus du panneau de navigation dans les fichiers, à droite de la barre d’outils, effectuez l’une des opérations suivantes :

   * Cliquez sur **Affichage de la grille** ou **Affichage par liste**. Dans le panneau de navigation des fichiers, cliquez deux fois sur la miniature vidéo d’un fichier pour l’ouvrir en mode Affichage des détails. Dans le panneau des URL et du code intégré sur la droite, sous Diffusion en flux continu HTTP, cliquez sur **Intégrer le code** à droite de la visionneuse appropriée. As a best practice, click **Embed Code** that is associated with the `Universal_HTML5_Video` viewer.
   * Cliquez sur **Affichage de la grille**. Dans le panneau de navigation dans les fichiers, sélectionnez un fichier, puis sous l’image miniature de vidéo, cliquez sur **Prévisualiser** &gt; **Liste des visionneuses**.

      Dans la page Liste des visionneuses, dans la colonne Actions du tableau, cliquez sur **Code intégré**. As a best practice, click **Embed Code** that is associated with the `Universal_HTML5_Video` viewer.

   * Cliquez sur **Affichage par liste**. Dans le panneau de navigation dans les fichiers, sélectionnez un fichier, puis à droite de l’image miniature, cliquez sur **Prévisualiser** &gt; **Liste des visionneuses**.

      Dans la page Liste des visionneuses, dans la colonne Actions du tableau, cliquez sur **Code intégré**. As a best practice, click **Embed Code** that is associated with the `Universal_HTML5_Video` viewer.

   * Cliquez sur **Affichage de la grille**, **Affichage par liste** ou **Affichage des détails**. Dans la même barre d’outils, cliquez sur **Prévisualiser** &gt; **Liste des visionneuses**.

      Dans la page Liste des visionneuses, dans la colonne Actions du tableau, cliquez sur **Code intégré**. As a best practice, click **Embed Code** that is associated with the `Universal_HTML5_Video` viewer.

1. Dans la boîte de dialogue Code incorporé, cliquez sur **Copier dans le Presse-papiers**.

   Vous ne pouvez pas modifier le code dans la boîte de dialogue Code intégré.

1. Cliquez sur **Fermer**.
1. Collez le code intégré dans vos pages Web.

### Implementing embed code for using HTML5 video with MP4 video assets {#implementing-embed-code-for-using-html-video-with-mp-video-assets}

If you do not use the Dynamic Media Classic HTML5 video player, but instead want to use the native HTML5 `<video>` tag with MP4 video assets, you can use the following embed code sample:

```as3
<video poster="S7 video thumbnail URL" controls> 
        <source src="S7 OGG video asset URL (no player)" type='video/ogg; codecs="theora, vorbis"'/> 
        <source src="S7 MP4 mobile progressive video asset URL (no player)" type='video/mp4; codecs="avc1.4D401E, mp4a.40.2"'/> 
        <p>This is fallback content</p> 
</video>
```

* Replace `"S7 video thumbnail URL"` with the video’s thumbnail URL. Il s’agit de l’image miniature de la vidéo visible par l’utilisateur avant de lancer la vidéo.

   Voir [Obtention d’URL de miniatures vidéo](deploying-video-websites-mobile-sites.md#obtaining_video_thumbnail_urls).

* Replace `"S7 OGG video asset URL (no player)"` with the video’s progressive URL for OGG video.

   Voir [Liaison d’une URL de vidéo à un site Web ou un site mobile](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

* Remplacez `"S7 MP4 mobile progressive video asset URL (no player)"` cette option par l'URL progressive de la vidéo.

   Voir [Liaison d’une URL de vidéo à un site Web ou un site mobile](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

## Déploiement d’une vidéo à l’aide d’un lecteur vidéo tiers {#deploying-video-using-a-third-party-video-player}

Si vous utilisez un lecteur vidéo tiers ou un lecteur vidéo intégré personnalisé au lieu d'une visionneuse vidéo Classic Media Classic, vous pouvez obtenir l'URL directe de vidéo compatible avec le téléchargement progressif ou progressif de vidéo HLS.

**Déploiement d’une vidéo à l’aide d’un lecteur vidéo tiers**

1. Dans SPS (Scene7 Publishing System), sur la barre de navigation générale, cliquez sur **Configuration** &gt; **Configuration de l’application** &gt; **Paramètres généraux**.
1. Selon le type d’URL à utiliser, effectuez l’une des opérations suivantes :
* Génération d'une URL directe de vidéo en flux continu HLS (débit multiple)

   Sur **la page Paramètres** généraux de l'application, dans le groupe **Serveurs** , **dans le champ Nom** du serveur publié, générez l'URL directe selon la syntaxe suivante : `server/is/content/company/folder/filename.m3u8`
Supposons, par exemple, que le nom du serveur publié utilise `https://s7d9.scene7.com/.` la syntaxe de l'étape 2, l'URL directe ressemblerait à ce qui suit :
   `https://s7d9.scene7.com/is/content/GeoRetail/AdobeRIA-AVS.m3u8`

* Génération d'une URL directe de vidéo en flux continu HLS (débit unique)

   On the **Application General Settings** page, in the **Servers** group, in the **HLS Streaming Server Name** text field, construct the direct URL using the following syntax:
   `server/company/folder/filename.ext.m3u8`Supposons par exemple que le nom du serveur de flux continu HLS est `https://s7mbrstream.scene7.com/hls-vod/`. En utilisant la syntaxe de l’étape 2, l’URL directe ressemblerait à ce qui suit :
   `https://s7mbrstream.scene7.com/hls-vod/GeoRetail/MBR/ToyStory3\_Teaser1\_High\_iPad\_768x432\_1296K.mp4.m3u8`

* Génération d’une URL de vidéo progressive directe

   Sur la page **Paramètres généraux de l’application**, dans le groupe **Serveurs**, dans le champ **Nom du serveur de vidéo progressive**, générez l’URL eVideo directe selon la syntaxe suivante : `server/company/folder/filename`Supposons, par exemple, que le nom du serveur vidéo progressif soit `https://s7d9.scene7.com/is/content/`. En utilisant la syntaxe de l’étape 2, l’URL directe ressemblerait à ce qui suit :
   `https://s7d9.scene7.com/e2/GeoRetail/SourceVideo/outdoors.mp4`

## Utilisation de miniatures de vidéo {#working-with-video-thumbnails}

Dynamic Media Classic génère des miniatures pour les vidéos codées et les vidéos précodées. Vous pouvez utiliser des miniatures vidéo comme n’importe quelle autre image. De plus, vous pouvez obtenir des URL pour les miniatures vidéo générées par Dynamic Media Classic et les déployer en dehors de SPS. Vous pouvez, par exemple, déployer les miniatures dans des résultats de recherche, des listes de vidéos correspondantes et des listes de lecture vidéo sur un site Web.

Les miniatures sont générées en fonction de la première image hétérogène (pas une image toute noire, toute blanche, etc.) de la vidéo.

### Obtention d’URL de miniatures vidéo {#obtaining-video-thumbnail-urls}

Dynamic Media Classic génère automatiquement des miniatures vidéo au cours du processus de téléchargement. Ces miniatures apparaissent dans le panneau de navigation en mode Affichage de la liste et Affichage de la grille.

Pour générer des URL de miniatures vidéo, effectuez une opération de publication.

Voir [Publication de vidéos](deploying-video-websites-mobile-sites.md#publishing_video).

Une fois la publication terminée, vous pouvez obtenir des URL de miniatures vidéo en mode Affichage des détails dans le panneau URL et Code intégré. Cliquez sur **Copier l’URL** à droite de la miniature vidéo pour copier son URL.

### Modification de cadres d’affiche dans des visionneuses de vidéos {#modifying-poster-frames-in-video-viewers}

Le *cadre d’affiche* est la première image qui apparaît dans les visionneuses de vidéos avant que ne commence la lecture de la vidéo. Dynamic Media Classic utilise des miniatures vidéo comme cadres d'affiche.

Vous pouvez appliquer des modificateurs d’image au cadre d’affiche. Vous pouvez, par exemple, rogner le cadre d’affiche ou le rendre transparent. Pour modifier le cadre d’affiche, ouvrez l’écran de configuration de la visionneuse de vidéos et saisissez les modificateurs dans la section Poster Image Modifiers (Modificateurs de l’image d’affiche). 

Voir [Ajout ou modification d’un paramètre prédéfini de visionneuse de vidéos](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

Voir [www.adobe.com/go/learn_s7_image_server_guide_en](https://www.adobe.com/go/learn_s7_image_server_guide_en).

Vous pouvez également modifier des miniatures vidéo en ajoutant des modificateurs aux URL de miniature vidéo.

>[!MORELIKETHIS]
>
>* [Publication de fichiers](publishing-files.md#publishing_files)

