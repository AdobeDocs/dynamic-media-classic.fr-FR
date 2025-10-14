---
title: 'Démarrage rapide : vidéo dans Adobe Dynamic Media Classic'
description: Présentation et démarrage rapide d’Adobe Dynamic Media Classic Video pour vous aider à démarrer rapidement.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 1157400c-b33a-422e-848c-258660ddc748
topic: Content Management
level: Beginner
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '1441'
ht-degree: 24%

---

# Démarrage rapide : vidéo dans Adobe Dynamic Media Classic{#quick-start-video}

Adobe Dynamic Media Classic Video est une solution complète qui facilite la publication de vidéos adaptatives haute qualité pour la diffusion sur plusieurs écrans, notamment les postes de travail, iOS, Android™, BlackBerry® et les appareils mobiles Windows®. Une visionneuse de vidéos adaptative regroupe les versions d’une même vidéo codées dans des débits et des formats différents, par exemple 400 kbit/s, 800 kbit/s et 1 000 kbit/s. L’ordinateur de bureau ou le périphérique mobile détecte la bande passante disponible.

Par exemple, sur un périphérique mobile iOS, il détecte une bande passante telle que 3G, 4G ou une connexion Wi-Fi, puis sélectionne automatiquement la vidéo codée selon le débit correspondant parmi ceux disponibles dans la visionneuse de vidéos adaptative. La vidéo est diffusée en continu sur les ordinateurs, les appareils mobiles ou les tablettes.

En outre, la qualité de la vidéo est automatiquement adaptée en temps réel selon les conditions réseau sur le bureau ou l’appareil mobile. En outre, si un client ou une cliente passe en mode plein écran sur un bureau, la visionneuse de vidéos à débit adaptatif réagit en utilisant une meilleure résolution, améliorant l’expérience de visionnage du client ou de la cliente. L’utilisation des visionneuses de vidéos adaptatives offre une lecture optimale. Il est préférable que les clients lisent la vidéo Adobe Dynamic Media Classic sur plusieurs écrans et appareils.

La logique appliquée par un lecteur vidéo pour déterminer quelles sont les vidéos codées à lire ou à sélectionner en cours de lecture repose sur l’algorithme suivant :

1. Le lecteur vidéo charge le fragment vidéo initial en fonction du débit le plus proche de la valeur définie pour le « débit binaire initial » dans le lecteur lui-même.
1. Le lecteur vidéo change en fonction des modifications apportées à la vitesse de bande passante à l’aide des critères suivants :

   1. Le lecteur sélectionne la bande passante la plus élevée inférieure ou égale à la bande passante estimée.
   1. Le lecteur ne prend en compte que 80 % de la bande passante disponible. Cependant, si elle change, elle est plus prudente à seulement 70 % pour éviter la surestimation et revenir immédiatement en arrière.

Consultez la logique de l’algorithme à l’adresse [https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp) pour obtenir des informations techniques à son sujet.

Pour la gestion des vidéos uniques et des visionneuses de vidéos adaptatives, Adobe Dynamic Media Classic prend en charge les éléments suivants :

* Chargement de vidéos à partir de nombreux formats vidéo pris en charge. Vous pouvez également charger des formats audio et coder des vidéos au format MP4 H.264 pour les lire sur plusieurs écrans. Vous pouvez utiliser des paramètres prédéfinis de vidéo adaptative Adobe Dynamic Media Classic, des paramètres prédéfinis de codage vidéo unique ou personnaliser votre propre codage pour contrôler la qualité et la taille de la vidéo.

Voir [Activation ou désactivation des paramètres prédéfinis de vidéo adaptative](/help/using/application-setup.md#activating-or-deactivating-adaptive-video-presets)

Voir aussi [Paramètres vidéo prédéfinis](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) vidéo de formation.

Lorsqu’une visionneuse de vidéos adaptative est générée, elle inclut des vidéos MP4.

>[!NOTE]
>
>Les vidéos Principal/source et toute autre vidéo au format source ne sont *pas* ajoutées à une visionneuse de vidéos à débit adaptatif.

* Sous-titrage vidéo dans les visionneuses Univeral_HTML5_Video, Universal_HTML5_MixedMedia_dark et Universal_HTML5_MixedMedia_light et navigation par chapitre vidéo dans les visionneuses Univeral_HTML5_Video, Universal_HTML5_MixedMedia_dark et Universal_HTML5_MixedMedia_light.

  Voir [Ajout de sous-titres à une vidéo](adding-captions-video.md).

  Voir [Ajout de marqueurs de chapitre à une vidéo](adding-chapter-markers-video.md).

* Organiser, parcourir et effectuer des recherches dans la vidéo avec une prise en charge complète des métadonnées pour une gestion efficace des fichiers vidéo.
* Diffusez des visionneuses de vidéos adaptatives sur le Web et sur les postes de travail et les appareils mobiles, y compris iPhone, iPad, Android™, BlackBerry® et Windows® Phone.

  La diffusion en continu de vidéo adaptative est prise en charge sur diverses plateformes iOS.

  Consultez la dernière prise en charge dans le [Guide de référence des visionneuses Adobe](https://experienceleague.adobe.com/fr/docs/dynamic-media-developer-resources).

  Adobe Dynamic Media Classic prend en charge la lecture vidéo pour mobiles au format vidéo MP4 H.264. <!-- LINK IS 404; NO SUITABLE REPLACEMENT WAS FOUND You can find BlackBerry&reg; devices that support this video format at the following website: -->

  <!-- See [Supported video formats on BlackBerry&reg;](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482). -->

  Les appareils Windows® qui prennent en charge ce format vidéo sont répertoriés dans la liste :

  [Formats vidéo pris en charge sur Windows® Phone](https://learn.microsoft.com/en-us/windows/uwp/audio-video-camera/supported-codecs).

* Lisez la vidéo à l’aide des paramètres prédéfinis de la visionneuse Adobe Dynamic Media Classic, notamment les éléments suivants :

   * Visionneuses vidéo uniques.
   * des visionneuses de supports mixtes combinant du contenu vidéo et des images.

* Configurer des lecteurs vidéo pour répondre à vos besoins de stratégie de marque.
* Intégrez la vidéo à votre site web, site mobile ou application mobile à l’aide d’une simple URL ou d’un code intégré.

Regardez les vidéos de formation suivantes :
* Présentation vidéo de [MP4](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/563_MP4%20Video%20Overview_converted%20renamed_eVideos-AVS)

* Prévisualisation vidéo [MP4](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/564_MP4%20Video%20Preview_converted%20renamed_eVideos-AVS)

* Chargement vidéo [MP4](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/565_MP4%20Video%20Upload_converted%20renamed_eVideos-AVS)

* [Présentation de la diffusion en continu](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/567_Streaming%20Overview_master_eVideos_converted%20renamed_eVideos-AVS)

**Démarrage rapide**

Le processus détaillé décrit ci-après vise à vous aider à maîtriser rapidement les opérations liées aux visionneuses de vidéos adaptatives dans Adobe Dynamic Media Classic. Après chaque étape, il existe une référence croisée à un en-tête de rubrique dans laquelle vous pouvez trouver plus d’informations.

## &#x200B;1. Charger et coder des vidéos

Téléchargez et générez des visionneuses de vidéos adaptatives en suivant l’un des deux scénarios ci-après :

* **Charger des vidéos précodées** : si vos vidéos ont déjà été codées en externe à partir d’Adobe Dynamic Media Classic, sur la barre de navigation globale, sélectionnez **[!UICONTROL Charger]**. Parcourez et chargez des fichiers vidéo MP4 directement dans Adobe Dynamic Media Classic. Accédez ensuite à **[!UICONTROL Créer]** > **[!UICONTROL Visionneuses de vidéos adaptatives]**. Accédez aux fichiers vidéo requis. Faites glisser et déposez les fichiers vidéo de votre choix dans le tableau Visionneuse de vidéos adaptative, puis enregistrez la visionneuse.
* **Charger des vidéos issues de sources originales** : si vos vidéos ne sont pas codées, sur la barre de navigation générale, sélectionnez **[!UICONTROL Charger]** pour charger les fichiers issus de sources originales (non MP4). Adobe Dynamic Media Classic les encode en fichiers MP4 pour vous. Dans la boîte de dialogue **[!UICONTROL Charger les options de la tâche]**, sous **[!UICONTROL Options EVideo]**, sélectionnez **[!UICONTROL Vidéo adaptative]**.

  Avec cette option préférée, vous pouvez créer des visionneuses de vidéos adaptatives. Le paramètre prédéfini de codage correct est automatiquement appliqué à la vidéo, qu’elle soit de 16 :9 ou de 4 :3, pour correspondre aux dimensions de la vidéo que vous avez chargée. Lorsque vous envoyez votre tâche de chargement, une visionneuse de vidéos adaptative est automatiquement créée pour vous, qui inclut trois paramètres de vidéo de codage dans les proportions correctes.

  Ou, dans la même boîte de dialogue **[!UICONTROL Options de tâche]**, sous **[!UICONTROL Options EVideo]**, développez **[!UICONTROL Paramètres prédéfinis de codage unique]**. Sélectionnez les paramètres prédéfinis de codage vidéo de votre choix. Vous pouvez sélectionner **Bureau**, **Mobile (iPhone, iPad, Android™)** et **Tablette (iPad, Android™)** pour créer les fichiers MP4.

* Vous pouvez également retraiter une vidéo principale à l’aide de la fonction **[!UICONTROL Retraitement]**. Les vidéos récemment codées sont ajoutées à la visionneuse de vidéos adaptative existante.

Voir [Chargement et codage de vidéos](uploading-encoding-videos.md#uploading_and_encoding_videos).

**Facultatif**

Adobe Dynamic Media Classic propose de nombreux paramètres prédéfinis de codage vidéo. Ces paramètres prédéfinis reflètent les paramètres de codage vidéo les plus courants utilisés aujourd’hui et sont optimisés pour la lecture sur les pages cibles.

Toutefois, si une personnalisation plus poussée est nécessaire, les administrateurs peuvent créer des paramètres vidéo prédéfinis pour personnaliser la taille et la lecture des vidéos pour les utilisateurs. Les administrateurs peuvent ajouter et gérer des paramètres vidéo prédéfinis à partir de la page Paramètres vidéo prédéfinis disponible sous **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Paramètres vidéo prédéfinis]** > **[!UICONTROL Paramètres prédéfinis de codage unique]**. La page Paramètres vidéo prédéfinis propose des options permettant d’ajouter, de modifier, de supprimer et d’activer des paramètres vidéo prédéfinis.

Voir [&#x200B; Utilisation de paramètres prédéfinis de codage vidéo](uploading-encoding-videos.md#working_with_video_encoding_presets).

## &#x200B;2. Prévisualisation de vidéos dans une visionneuse de vidéos

Pour voir comment une vidéo est lue pour les utilisateurs finaux sur un bureau, votre site web ou un appareil mobile, sélectionnez-la dans le panneau de navigation. Sélectionnez ensuite **[!UICONTROL Aperçu]**.

Voir [Prévisualisation de vidéos dans une visionneuse de vidéos](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer).

Vous pouvez lire la vidéo dans la page Aperçu . Vous pouvez également choisir différentes visionneuses de vidéos pour découvrir comment votre vidéo apparaît dans différents lecteurs. En règle générale, utilisez le lecteur vidéo HTML5 pour une lecture sur plusieurs écrans sur ordinateur, tablette et appareil mobile.

**Facultatif**

Personnalisation des paramètres prédéfinis de la visionneuse : Adobe Dynamic Media Classic propose des paramètres prédéfinis de visionneuse pour la diffusion de vidéos. Ces paramètres déterminent l’aspect de la visionneuse et le mode de fonctionnement des commandes de lecture. Pour personnaliser la visionneuse de vidéos, les administrateurs peuvent ajouter et gérer des paramètres prédéfinis de visionneuse à partir de la page Paramètres prédéfinis de la visionneuse. Pour ouvrir cette page, dans le coin supérieur droit d’Adobe Dynamic Media Classic, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Paramètres prédéfinis de la visionneuse]**. La page Paramètres prédéfinis de la visionneuse propose des commandes permettant d’ajouter, de modifier, de supprimer et d’activer des paramètres prédéfinis de la visionneuse.

Voir [&#x200B; Utilisation des paramètres prédéfinis de visionneuse vidéo &#x200B;](previewing-videos-video-viewer.md#working_with_video_viewer_presets).

Voir aussi [Paramètres vidéo prédéfinis](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) vidéo de formation.

## &#x200B;3. Déploiement de vidéos sur vos sites web et sites mobiles

Pour intégrer la vidéo sur votre site Web, procédez de l’une des manières suivantes :

* Affichez la vidéo dans sa propre fenêtre pop-up ou modale, auquel cas utilisez la fonction **[!UICONTROL Copier l’URL]**.

  Pour obtenir l’URL d’une vidéo, dans la vue Grille ou Liste, sélectionnez-la dans le panneau Parcourir . Sélectionnez **[!UICONTROL Aperçu]**, puis sélectionnez **[!UICONTROL Copier l’URL]** à droite de `Universal_HTML5_Viewer`.

  Lorsque vous sélectionnez **[!UICONTROL Copier l’URL]**, l’URL est copiée dans le Presse-papiers. Placez ce code dans le code HTML de votre site Web, site mobile ou application.

  >[!NOTE]
  >
  >les URL sont activées uniquement après que vous ayez publié la vidéo ou la visionneuse de vidéos adaptative.

* Affichez la vidéo incorporée dans la page web, auquel cas utilisez la fonction **[!UICONTROL Code incorporé]**.

  Pour obtenir le code intégré d’une vidéo, dans la vue Grille ou Liste, sélectionnez la vidéo dans le panneau Parcourir . Accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**. Dans la colonne Actions du tableau, sélectionnez **[!UICONTROL Code incorporé]** à droite de `Universal_HTML5_Video`. Il n’est pas possible de modifier le code.

  Sélectionnez **[!UICONTROL Fermer]** et collez le code incorporé dans une ou plusieurs de vos pages web.

  >[!NOTE]
  >
  >Le code incorporé n’est activé qu’après la publication de la vidéo ou de la visionneuse de vidéos adaptative.

Voir [Déploiement de vidéos sur vos sites web et sites mobiles](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites).

>[!MORELIKETHIS]
>
>* [Meilleures pratiques en matière de codage de vidéo](uploading-encoding-videos.md#best_practices_for_video_encoding)
