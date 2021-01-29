---
title: Déploiement de vidéos sur vos sites Web et sites mobiles
description: Découvrez comment déployer des vidéos sur vos sites Web et sites mobiles.
uuid: 22bb4402-c0ab-4df0-89b9-99707d111927
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 0d006314-c4cc-4f6c-a51c-6075bb445e39
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '1680'
ht-degree: 68%

---


# Déploiement de vidéos sur vos sites Web et sites mobiles{#deploying-video-to-your-websites-and-mobile-sites}

Les sites Web, sites mobiles et applications de bureau accèdent au contenu des serveurs Dynamic Media Classic, y compris aux vidéos, au moyen de chaînes URL ou de code incorporé. Dynamic Media Classic active ces chaînes URL lors du processus de publication. Pour placer la chaîne URL ou le code incorporé de la vidéo dans vos pages Web, pages mobiles et applications de bureau, copiez-la depuis Dynamic Media Classic.

>[!NOTE]
>
>l’URL ou le code intégré n’est actif(ve) qu’une fois le fichier publié.

## Publication des vidéos  {#publishing-video}

La publication d’une vidéo permet aux serveurs Dynamic Media Classic de diffuser de la vidéo sur votre site Web, site mobile ou application.

Deux méthodes peuvent être utilisées pour publier la vidéo :

* **Publication de vidéos automatiquement et immédiatement lors du transfert**

   Dans le cadre du processus de téléchargement de vidéo, Dynamic Media Classic peut automatiquement publier des vidéos lorsqu’elles sont téléchargées et codées. Cette capacité de publication instantanée signifie qu’il n’est pas nécessaire de publier les vidéos séparément après coup.

* **Publication d’une vidéo manuellement après le transfert**

   Si vous ne souhaitez pas publier les vidéos immédiatement, vous pouvez les publier manuellement à tout moment.

Après avoir publié des vidéos, Dynamic Media Classic active les chaînes URL de votre page HTML ou code d’application.

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

   * Cliquez sur **Affichage de la grille** ou **Affichage par liste**. Dans le panneau de navigation des fichiers, cliquez deux fois sur la miniature vidéo d’un fichier pour l’ouvrir en mode Affichage des détails. Dans le panneau des URL et du code intégré sur la droite, sous Diffusion en flux continu HTTP, cliquez sur **Copier l’URL** à droite de la visionneuse appropriée. Il est recommandé de copier l’URL associée à la visionneuse `Universal_HTML5_Video`.
   * Cliquez sur **Affichage de la grille**. Dans le panneau de navigation dans les fichiers, sélectionnez un fichier, puis sous l’image miniature, cliquez sur **Prévisualiser** > **Liste des visionneuses**.

      Dans la page Liste des visionneuses, dans la colonne Actions du tableau, cliquez sur **Copier l’URL**. Il est recommandé de copier l’URL associée à la visionneuse `Universal_HTML5_Video`.

   * Cliquez sur **Affichage par liste**. Dans le panneau de navigation dans les fichiers, sélectionnez un fichier, puis à droite de l’image miniature, cliquez sur **Prévisualiser** > **Liste des visionneuses**.

      Dans la page Liste des visionneuses, dans la colonne Actions du tableau, cliquez sur **Copier l’URL**. Il est recommandé de copier l’URL associée à la visionneuse `Universal_HTML5_Video`.

   * Cliquez sur **Affichage de la grille**, **Affichage par liste** ou **Affichage des détails**. Dans la même barre d’outils, cliquez sur **Prévisualiser** > **Liste des visionneuses**.

      Dans la page Liste des visionneuses, dans la colonne Actions du tableau, cliquez sur **Copier l’URL**. Il est recommandé de copier l’URL associée à la visionneuse `Universal_HTML5_Video`.

1. Collez l’URL de vidéo HTML5 sur vos sites Web et mobile.

## Intégration de la visionneuse de vidéos sur une page Web  {#embedding-the-video-viewer-on-a-web-page}

Utilisez la fonction Intégrer le code lorsque vous souhaitez lire la vidéo incorporée sur une page Web. Vous copiez le code intégré dans le presse-papiers pour pouvoir le coller dans vos pages web. Vous ne pouvez pas modifier le code dans la boîte de dialogue Intégrer le code.

Voir aussi [Liaison d’une URL de vidéo à un site Web ou à un site mobile](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

**Incorporation de la visionneuse de vidéos sur une page Web**

1. Dans la liste déroulante Afficher du panneau de navigation des fichiers, cliquez sur **Vidéo** ou sur **Visionneuse de vidéos adaptative**.
1. Dans le panneau Bibliothèque de fichiers sur la gauche, accédez au dossier Fichiers qui contient la vidéo ou la visionneuse de vidéos adaptative dont vous voulez copier le code intégré.
1. Au-dessus du panneau de navigation dans les fichiers, à droite de la barre d’outils, effectuez l’une des opérations suivantes :

   * Cliquez sur **Affichage de la grille** ou **Affichage par liste**. Dans le panneau de navigation des fichiers, cliquez deux fois sur la miniature vidéo d’un fichier pour l’ouvrir en mode Affichage des détails. Dans le panneau des URL et du code intégré sur la droite, sous Diffusion en flux continu HTTP, cliquez sur **Intégrer le code** à droite de la visionneuse appropriée. Il est recommandé de cliquer sur **Code incorporé** associé à la visionneuse `Universal_HTML5_Video`.
   * Cliquez sur **Affichage de la grille**. Dans le panneau de navigation dans les fichiers, sélectionnez un fichier, puis sous l’image miniature de vidéo, cliquez sur **Prévisualiser** > **Liste des visionneuses**.

      Dans la page Liste des visionneuses, dans la colonne Actions du tableau, cliquez sur **Code intégré**. Il est recommandé de cliquer sur **Code incorporé** associé à la visionneuse `Universal_HTML5_Video`.

   * Cliquez sur **Affichage par liste**. Dans le panneau de navigation dans les fichiers, sélectionnez un fichier, puis à droite de l’image miniature, cliquez sur **Prévisualiser** > **Liste des visionneuses**.

      Dans la page Liste des visionneuses, dans la colonne Actions du tableau, cliquez sur **Code intégré**. Il est recommandé de cliquer sur **Code incorporé** associé à la visionneuse `Universal_HTML5_Video`.

   * Cliquez sur **Affichage de la grille**, **Affichage par liste** ou **Affichage des détails**. Dans la même barre d’outils, cliquez sur **Prévisualiser** > **Liste des visionneuses**.

      Dans la page Liste des visionneuses, dans la colonne Actions du tableau, cliquez sur **Code intégré**. Il est recommandé de cliquer sur **Code incorporé** associé à la visionneuse `Universal_HTML5_Video`.

1. Dans la boîte de dialogue Code incorporé, cliquez sur **Copier dans le Presse-papiers**.

   Vous ne pouvez pas modifier le code dans la boîte de dialogue Code intégré.

1. Cliquez sur **Fermer**.
1. Collez le code intégré dans vos pages Web.

### Mise en oeuvre du code intégré pour l’utilisation de vidéos HTML5 avec des ressources vidéo MP4 {#implementing-embed-code-for-using-html-video-with-mp-video-assets}

Si vous n’utilisez pas le lecteur vidéo HTML5 Dynamic Media Classic, mais souhaitez plutôt utiliser la balise HTML5 `<video>` native avec les ressources vidéo MP4, vous pouvez utiliser l’exemple de code intégré suivant :

```as3
<video poster="S7 video thumbnail URL" controls> 
        <source src="S7 OGG video asset URL (no player)" type='video/ogg; codecs="theora, vorbis"'/> 
        <source src="S7 MP4 mobile progressive video asset URL (no player)" type='video/mp4; codecs="avc1.4D401E, mp4a.40.2"'/> 
        <p>This is fallback content</p> 
</video>
```

* Remplacez `"S7 video thumbnail URL"` par l’URL de miniature de la vidéo. Il s’agit de l’image miniature de la vidéo visible par l’utilisateur avant de lancer la vidéo.

   Voir [Obtention d’URL de miniatures vidéo](deploying-video-websites-mobile-sites.md#obtaining_video_thumbnail_urls).

* Remplacez `"S7 OGG video asset URL (no player)"` par l’URL progressive de la vidéo pour la vidéo OGG.

   Voir [Liaison d’une URL de vidéo à un site Web ou un site mobile](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

* Remplacez `"S7 MP4 mobile progressive video asset URL (no player)"` par l’URL progressive mobile de la vidéo.

   Voir [Liaison d’une URL de vidéo à un site Web ou un site mobile](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

## Déploiement d’une vidéo à l’aide d’un lecteur vidéo tiers  {#deploying-video-using-a-third-party-video-player}

Si vous utilisez un lecteur vidéo tiers ou un lecteur vidéo intégré personnalisé au lieu d’une visionneuse de vidéos Dynamic Media Classic, vous pouvez obtenir l’URL de vidéo directe qui fonctionne pour la diffusion en flux continu à débit multiple HLS ou le téléchargement progressif.

**Déploiement d’une vidéo à l’aide d’un lecteur vidéo tiers**

1. Dans Dynamic Media Classic, sur la barre de navigation globale, cliquez sur **Configuration** > **Configuration de l’application** > **Paramètres généraux**.
1. Selon le type d’URL à utiliser, effectuez l’une des opérations suivantes :
* Génération d’une URL directe de vidéo en flux continu HLS (débit multiple)

   Sur la page **Paramètres généraux de l’application**, dans le groupe **Servers**, dans le champ **Nom du serveur publié**, générez l’URL directe en utilisant la syntaxe suivante : `server/is/content/company/folder/filename.m3u8`
Par exemple, supposons que le nom du serveur publié soit `https://s7d9.scene7.com/.` En utilisant la syntaxe de l’étape 2, l’URL directe peut ressembler à ce qui suit :
   `https://s7d9.scene7.com/is/content/GeoRetail/AdobeRIA-AVS.m3u8`

* Pour générer une URL directe de vidéo en flux continu HLS (débit unique)

   Sur la page **Paramètres généraux de l&#39;application**, dans le groupe **Servers**, dans le champ **Nom du serveur de diffusion en continu HLS**, générez l&#39;URL directe en utilisant la syntaxe suivante :
   `server/company/folder/filename.ext.m3u8`
Par exemple, supposons que le nom du serveur de flux continu HLS soit  `https://s7mbrstream.scene7.com/hls-vod/`. En utilisant la syntaxe de l’étape 2, l’URL directe ressemblerait à ce qui suit :
   `https://s7mbrstream.scene7.com/hls-vod/GeoRetail/MBR/ToyStory3\_Teaser1\_High\_iPad\_768x432\_1296K.mp4.m3u8`

* Génération d’une URL de vidéo progressive directe

   Sur la page **Paramètres généraux de l’application**, dans le groupe **Serveurs**, dans le champ **Nom du serveur de vidéo progressive**, générez l’URL eVideo directe selon la syntaxe suivante :  `server/company/folder/filename`
Supposons, par exemple, que le nom du serveur de vidéo progressive soit  `https://s7d9.scene7.com/is/content/`identique. En utilisant la syntaxe de l’étape 2, l’URL directe ressemblerait à ce qui suit :
   `https://s7d9.scene7.com/e2/GeoRetail/SourceVideo/outdoors.mp4`

## Utilisation de miniatures de vidéo {#working-with-video-thumbnails}

Dynamic Media Classic génère des miniatures pour les vidéos codées et les vidéos précodées. Vous pouvez utiliser des miniatures vidéo comme n’importe quelle autre image. En outre, vous pouvez obtenir des URL pour les miniatures vidéo que Dynamic Media Classic génère et déployer ces URL en dehors de Dynamic Media Classic. Vous pouvez, par exemple, déployer les miniatures dans des résultats de recherche, des listes de vidéos correspondantes et des listes de lecture vidéo sur un site Web.

Les miniatures sont générées en fonction de la première image hétérogène (pas une image toute noire, toute blanche, etc.) de la vidéo.

### Obtention d’URL de miniatures vidéo {#obtaining-video-thumbnail-urls}

Dynamic Media Classic génère automatiquement des miniatures vidéo pendant le processus de téléchargement. Ces miniatures apparaissent dans le panneau de navigation en mode Affichage de la liste et Affichage de la grille.

Pour générer des URL de miniatures vidéo, effectuez une opération de publication.

Voir [Publication de vidéos](deploying-video-websites-mobile-sites.md#publishing_video).

Une fois la publication terminée, vous pouvez obtenir des URL de miniatures vidéo en mode Affichage des détails dans le panneau URL et Code intégré. Cliquez sur **Copier l’URL** à droite de la miniature vidéo pour copier son URL.

### Modification de cadres d’affiche dans des visionneuses de vidéos  {#modifying-poster-frames-in-video-viewers}

Le *cadre d’affiche* est la première image qui apparaît dans les visionneuses de vidéos avant que ne commence la lecture de la vidéo. Dynamic Media Classic utilise des miniatures vidéo comme cadres d’affiche.

Vous pouvez appliquer des modificateurs d’image au cadre d’affiche. Vous pouvez, par exemple, rogner le cadre d’affiche ou le rendre transparent. Pour modifier le cadre d’affiche, ouvrez l’écran de configuration de la visionneuse de vidéos et saisissez les modificateurs dans la section Poster Image Modifiers (Modificateurs de l’image d’affiche). 

Voir [Ajout ou modification d’un paramètre prédéfini de visionneuse de vidéos](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

Voir [www.adobe.com/go/learn_s7_image_server_guide_en](https://www.adobe.com/go/learn_s7_image_server_guide_en).

Vous pouvez également modifier des miniatures vidéo en ajoutant des modificateurs aux URL de miniature vidéo.

>[!MORELIKETHIS]
>
>* [Publication de fichiers ](publishing-files.md#publishing_files)

