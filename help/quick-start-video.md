---
title: '"Démarrage rapide : Vidéo"'
description: Introduction et démarrage rapide pour Adobe la vidéo Dynamic Media Classic afin de vous aider à démarrer rapidement.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Visionneuses,Vidéo
role: Business Practitioner
exl-id: 1157400c-b33a-422e-848c-258660ddc748
source-git-commit: 1beb30b9eda4487dcd549034906079dee0b3149a
workflow-type: tm+mt
source-wordcount: '1425'
ht-degree: 43%

---

# Démarrage rapide : Vidéo{#quick-start-video}

Adobe Dynamic Media Classic Video est une solution de bout en bout qui facilite la publication de vidéos adaptatives de haute qualité pour la diffusion en continu sur plusieurs écrans, y compris les appareils mobiles de bureau, iOS, Android™, BlackBerry® et Windows®. Une visionneuse de vidéos adaptative regroupe les versions d’une même vidéo codées dans des débits et des formats différents, par exemple 400 kbit/s, 800 kbit/s et 1 000 kbit/s. L’ordinateur de bureau ou le périphérique mobile détecte la bande passante disponible.

Par exemple, sur un périphérique mobile iOS, il détecte une bande passante telle que 3G, 4G ou une connexion Wi-Fi, puis sélectionne automatiquement la vidéo codée selon le débit correspondant parmi ceux disponibles dans la visionneuse de vidéos adaptative. La vidéo est diffusée en continu sur les ordinateurs, les appareils mobiles ou les tablettes.

En outre, la qualité de la vidéo est automatiquement adaptée en temps réel selon les conditions réseau sur le bureau ou l’appareil mobile. En outre, si un client passe en mode plein écran sur un bureau, la visionneuse de vidéos adaptative répond en utilisant une meilleure résolution, améliorant ainsi l’expérience de visionnage du client. L’utilisation de visionneuses de vidéos adaptatives vous permet de lire le mieux possible la vidéo Dynamic Media Classic sur plusieurs écrans et appareils.

La logique appliquée par un lecteur vidéo pour déterminer quelles sont les vidéos codées à lire ou à sélectionner en cours de lecture repose sur l’algorithme suivant :

1. Le lecteur vidéo charge le fragment vidéo initial en fonction du débit le plus proche de la valeur définie pour le &quot;débit initial&quot; dans le lecteur lui-même.
1. Le lecteur vidéo bascule sur les modifications apportées à la vitesse de bande passante à l’aide des critères suivants :

   1. Le lecteur sélectionne la bande passante la plus élevée en dessous ou égale à la bande passante estimée.
   1. Le lecteur ne prend en compte que 80 % de la bande passante disponible. Cependant, s’il change, il est plus prudent à seulement 70 % pour éviter de surestimer et de devoir immédiatement revenir en arrière.

Pour obtenir des informations techniques à ce sujet, voir la logique de l’algorithme à l’adresse [https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp) .

Pour la gestion des visionneuses de vidéos adaptatives et de vidéos uniques, Dynamic Media Classic prend en charge les éléments suivants :

* Téléchargement de vidéos en différents formats vidéo et audio pris en charge et codage vidéo au format MP4 H.264 pour la lecture sur plusieurs écrans. Vous pouvez utiliser des paramètres prédéfinis de vidéo adaptative Dynamic Media Classic prédéfinis, des paramètres prédéfinis de codage vidéo unique ou personnaliser votre propre codage pour contrôler la qualité et la taille de la vidéo.

   Lorsqu’une visionneuse de vidéos adaptative est générée, elle comprend des vidéos MP4.

   >[!NOTE]
   >
   >Les vidéos Principal/source et toute autre vidéo au format source ne sont *pas* ajoutées à une visionneuse de vidéos adaptative.

* Sous-titrage des vidéos dans les visionneuses Univeral_HTML5_Video, Universal_HTML5_MixedMedia_dark et Universal_HTML5_MixedMedia_light et navigation dans les chapitres vidéo dans les visionneuses Univeral_HTML5_Video, Universal_HTML5_MixedMedia_dark et Universal_HTML5_MixedMedia_light.

   Reportez-vous à [Ajout de sous-titres aux vidéos](adding-captions-video.md).

   Voir [Ajout de marques de chapitre à la vidéo](adding-chapter-markers-video.md).

* Organiser, parcourir et effectuer des recherches dans la vidéo avec une prise en charge complète des métadonnées pour une gestion efficace des fichiers vidéo.
* Diffusez des visionneuses de vidéos adaptatives sur le web et sur les ordinateurs de bureau et les appareils mobiles, y compris l’iPhone, l’iPad, Android™, BlackBerry® et le téléphone Windows®.

   La diffusion de vidéo adaptative en continu est prise en charge sur différentes plateformes iOS.

   Voir la dernière prise en charge dans le [Guide de référence des visionneuses d’Adobe](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources.html).

   Dynamic Media Classic prend en charge la lecture vidéo mobile pour la vidéo MP4 H.264. Vous trouverez les appareils BlackBerry® qui prennent en charge ce format vidéo sur le site web suivant :

   Voir [Formats vidéo pris en charge sur BlackBerry®](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482).

   Vous trouverez les périphériques Windows® qui prennent en charge ce format vidéo à l’adresse suivante :

   Voir [Formats vidéo pris en charge sur Windows® Phone](https://docs.microsoft.com/en-us/).

* Lecture de la vidéo à l’aide des paramètres prédéfinis de la visionneuse Dynamic Media Classic, notamment :

   * des visionneuses de vidéos uniques,
   * des visionneuses de supports mixtes combinant du contenu vidéo et des images.

* Configurer des lecteurs vidéo pour répondre à vos besoins de stratégie de marque.
* Intégrer la vidéo à votre site Web, site mobile ou application mobile grâce à une simple URL ou à un code intégré.

**Démarrage rapide**

La description suivante du workflow étape par étape est conçue pour vous aider à maîtriser rapidement les opérations liées aux visionneuses de vidéos adaptatives dans Dynamic Media Classic. Chaque étape se termine par un renvoi à une rubrique contenant de plus amples informations.

## 1. Chargement et codage des vidéos

Téléchargez et générez des visionneuses de vidéos adaptatives en suivant l’un des deux scénarios ci-après :

* **Télécharger des vidéos précodées**  : si vos vidéos ont déjà été codées en dehors de Dynamic Media Classic, dans la barre de navigation globale, cliquez sur  **** Télécharger pour parcourir et charger les fichiers vidéo MP4 directement dans Dynamic Media Classic. Cliquez ensuite sur **[!UICONTROL Créer]** > **[!UICONTROL Visionneuses de vidéos adaptatives]**. Accédez aux fichiers vidéo requis. Faites-les glisser et déposez-les dans le tableau Visionneuse de vidéos adaptative, puis enregistrez la visionneuse.
* **Télécharger les vidéos sources originales**  : si vos vidéos ne sont pas codées, dans la barre de navigation globale, cliquez sur  **** Télécharger pour charger les fichiers source de la vidéo originale (non MP4) et demandez à Dynamic Media Classic de les coder en fichiers MP4 pour vous. Dans la boîte de dialogue **[!UICONTROL Télécharger les options de la tâche]**, sous **[!UICONTROL Options eVideo]**, sélectionnez **[!UICONTROL Vidéo adaptative]**.

   Cette option conseillée permet de créer une visionneuse de vidéos adaptative qui applique automatiquement à la vidéo les paramètres de codage prédéfinis corrects, qu’il s’agisse d’un format 16:9 ou 4:3, en fonction des dimensions de la vidéo téléchargée. Lorsque vous procédez au transfert, une visionneuse de vidéos adaptative est automatiquement créée, avec trois codages vidéo aux proportions appropriées.

   Ou, dans la même boîte de dialogue **[!UICONTROL Options de tâche]**, sous **[!UICONTROL Options eVideo]**, développez **[!UICONTROL Paramètres prédéfinis de codage uniques]**. Sélectionnez les paramètres prédéfinis de codage vidéo individuels que vous souhaitez utiliser à partir de **Bureau**, **Mobile (iPhone, iPad, Android™)** et **Tablette (iPad, Android™)** pour créer les fichiers MP4.

* Vous pouvez également retraiter une vidéo originale à l’aide de la fonction **[!UICONTROL Retraiter]** . Les vidéos récemment codées sont ajoutées à la visionneuse de vidéos adaptative existante.

Voir [Chargement et codage de vidéos](uploading-encoding-videos.md#uploading_and_encoding_videos).

**Facultatif**

Dynamic Media Classic propose de nombreux paramètres prédéfinis de codage vidéo. Ces paramètres prédéfinis représentent les paramètres de codage vidéo les plus courants et sont optimisés pour la lecture sur les pages cibles.

Toutefois, si une personnalisation plus poussée est nécessaire, les administrateurs peuvent créer des paramètres vidéo prédéfinis pour personnaliser la taille et la lecture des vidéos pour les utilisateurs. Les administrateurs peuvent ajouter et gérer des paramètres vidéo prédéfinis à partir de la page Paramètres vidéo prédéfinis disponible sous **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Paramètres vidéo prédéfinis]** > **[!UICONTROL Paramètres prédéfinis de codage uniques]**. La page Paramètres vidéo prédéfinis propose des options permettant d’ajouter, de modifier, de supprimer et d’activer des paramètres vidéo prédéfinis.

Voir [Utilisation des paramètres prédéfinis de codage vidéo](uploading-encoding-videos.md#working_with_video_encoding_presets).

## 2. Prévisualisation de vidéos dans une visionneuse de vidéos

Pour découvrir comment un utilisateur final voit une vidéo sur un ordinateur, votre site Web ou un périphérique mobile, sélectionnez la vidéo dans le panneau de navigation, puis cliquez sur **[!UICONTROL Prévisualiser]**.

Voir [Prévisualisation de vidéos dans une visionneuse](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer).

Vous pouvez lire la vidéo sur la page Aperçu . Vous pouvez également choisir différentes visionneuses de vidéos pour découvrir comment votre vidéo apparaît dans différents lecteurs. En règle générale, utilisez le lecteur vidéo HTML5 pour une lecture sur plusieurs écrans sur ordinateur, tablette et appareil mobile.

**Facultatif**

Personnalisation des paramètres prédéfinis de la visionneuse : Dynamic Media Classic propose des paramètres prédéfinis de visionneuse pour la diffusion vidéo. Ces paramètres déterminent l’aspect de la visionneuse et le mode de fonctionnement des commandes de lecture. Pour personnaliser la visionneuse de vidéos, les administrateurs peuvent ajouter et gérer des paramètres prédéfinis de visionneuse à partir de la page Paramètres prédéfinis de la visionneuse. Pour ouvrir cette page, dans le coin supérieur droit de Dynamic Media Classic, cliquez sur **[!UICONTROL Configuration]** > **[!UICONTROL Paramètres prédéfinis de la visionneuse]**. La page Paramètres prédéfinis de la visionneuse propose des commandes permettant d’ajouter, de modifier, de supprimer et d’activer des paramètres prédéfinis de la visionneuse.

Voir [Utilisation des paramètres prédéfinis de visionneuse de vidéos](previewing-videos-video-viewer.md#working_with_video_viewer_presets).

## 3. Déploiement de vidéos sur vos sites web et vos sites mobiles

Pour intégrer la vidéo sur votre site Web, procédez de l’une des manières suivantes :

* Affichez la vidéo dans sa propre fenêtre contextuelle ou modale, auquel cas utilisez la fonction **[!UICONTROL Copier l’URL]**.

   Pour obtenir l’URL d’une vidéo, en mode Grille ou Liste, sélectionnez la vidéo dans le panneau de navigation. Cliquez sur **[!UICONTROL Aperçu]**, puis sur **[!UICONTROL Copier l’URL]** à droite de `Universal_HTML5_Viewer`.

   Lorsque vous cliquez sur **[!UICONTROL Copier l’URL]**, l’URL est copiée dans le Presse-papiers. Placez ce code dans le code HTML de votre site Web, site mobile ou application.

   >[!NOTE]
   >
   >les URL sont activées uniquement après que vous ayez publié la vidéo ou la visionneuse de vidéos adaptative.

* Affichez la vidéo incorporée dans la page web, auquel cas utilisez la fonction **[!UICONTROL Code incorporé]**.

   Pour obtenir le code intégré d’une vidéo, en mode Grille ou Liste, sélectionnez la vidéo dans le panneau de navigation. Cliquez sur **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**. Dans la colonne Actions du tableau, cliquez sur **[!UICONTROL Code incorporé]** à droite de `Universal_HTML5_Video`. Il n’est pas possible de modifier le code.

   Cliquez sur **[!UICONTROL Fermer]** et collez le code incorporé dans vos pages web.

   >[!NOTE]
   >
   >le code intégré est activé uniquement après que vous ayez publié la vidéo ou la visionneuse de vidéos adaptative.

Voir [Déploiement de vidéos sur vos sites Web et sites mobiles](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites).

>[!MORELIKETHIS]
>
>* [Meilleures pratiques en matière de codage de vidéo](uploading-encoding-videos.md#best_practices_for_video_encoding)

