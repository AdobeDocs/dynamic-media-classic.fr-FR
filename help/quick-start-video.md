---
title: '"Démarrage rapide : Vidéo"'
seo-title: '"Démarrage rapide : Vidéo"'
description: 'null'
seo-description: Présentation et démarrage rapide de la vidéo pour vous aider à maîtriser rapidement les opérations.
uuid: bf 0 ecf 87-a 1 f 2-4 e 83-8041-df 5192 dd 26 a 1
contentOwner: admin
content-type: référence
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/video
discoiquuid: 6 cef 541 b-e 9 df -48 eb -9 a 16-ca 3 e 1 f 07238 e
translation-type: tm+mt
source-git-commit: de7d2608f94935f238a11d8310b97dddc5476f57

---


# Démarrage rapide : Vidéo{#quick-start-video}

Adobe Dynamic Media Classic Video est une solution de bout en bout qui facilite la publication de vidéos adaptatives haute qualité pour la diffusion en continu sur plusieurs écrans, notamment les périphériques mobiles, ios, Android, Blackberry et Windows. Une visionneuse de vidéos adaptative regroupe les versions d’une même vidéo codées dans des débits et des formats différents, par exemple 400 kbit/s, 800 kbit/s et 1 000 kbit/s. L’ordinateur de bureau ou le périphérique mobile détecte la bande passante disponible.

Par exemple, sur un périphérique mobile iOS, il détecte une bande passante telle que 3G, 4G ou une connexion Wi-Fi, puis sélectionne automatiquement la vidéo codée selon le débit correspondant parmi ceux disponibles dans la visionneuse de vidéos adaptative. La vidéo est diffusée en continu sur les ordinateurs, les appareils mobiles ou les tablettes.

En outre, la qualité de la vidéo est automatiquement adaptée en temps réel selon les conditions réseau sur le bureau ou l’appareil mobile. De même, si un client passe en mode plein écran sur un bureau, la visionneuse de vidéos adaptative réagit en utilisant une meilleure résolution, améliorant ainsi l’expérience de visionnage du client. L'utilisation de visionneuses de vidéos adaptatives offre une lecture optimale aux utilisateurs lisant la vidéo Dynamic Media Classic sur plusieurs écrans et périphériques.

La logique appliquée par un lecteur vidéo pour déterminer quelles sont les vidéos codées à lire ou à sélectionner en cours de lecture repose sur l’algorithme suivant :

1. Le lecteur vidéo charge le fragment vidéo initial en fonction du débit binaire le plus proche de la valeur définie pour le débit initial dans le lecteur lui-même.
1. Le lecteur vidéo bascule en fonction des modifications apportées à la vitesse de bande passante en utilisant les critères suivants :

   1. Le lecteur sélectionne le flux de bande passante le plus élevé au-dessous ou égal à la bande passante estimée.
   1. Player considère seulement 80 % de la bande passante disponible. Toutefois, s'il change de compte, il est plus conversatif à 70 % pour éviter la surestimation et avoir à revenir immédiatement.

Pour obtenir des informations techniques sur celle-ci, reportez-vous à la logique de l'algorithme [https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp) .

Pour la gestion des visionneuses de vidéos adaptatives et vidéo unique, Dynamic Media Classic prend en charge les éléments suivants :

* Téléchargement de vidéos en différents formats vidéo et audio pris en charge et codage vidéo au format MP4 H.264 pour la lecture sur plusieurs écrans. Vous pouvez utiliser des paramètres prédéfinis de vidéo adaptative Classic Media Classic, des paramètres prédéfinis de codage vidéo uniques ou personnaliser votre propre codage pour contrôler la qualité et la taille de la vidéo.

   Lorsqu'une visionneuse de vidéos adaptative est générée, elle inclut les vidéos MP 4.

   `**Note:**` Les vidéos originales/sources et les vidéos de format source ne sont *pas ajoutées* à une visionneuse de vidéos adaptative.

* Sous-titrage vidéo dans les visionneuses Univeral_ HTML 5_ Video, Universal_ HTML 5_ mixedmedia_ dark et Universal_ HTML 5_ mixedmedia_ light et la navigation des chapitres vidéo dans les visionneuses Univeral_ HTML 5_ Video, Universal_ HTML 5_ mixedmedia_ dark et Universal_ HTML 5_ mixedmedia_ light.

   Reportez-vous à [Ajout de sous-titres aux vidéos](adding-captions-video.md).

   Voir [Ajout de marques de chapitre à la vidéo](adding-chapter-markers-video.md).

* Organiser, parcourir et effectuer des recherches dans la vidéo avec une prise en charge complète des métadonnées pour une gestion efficace des fichiers vidéo.
* Proposer des visionneuses de vidéos adaptatives en ligne ainsi que sur des ordinateurs et des appareils mobiles (iPhone, iPad, Android™, Blackberry et Windows Phone notamment).

   La diffusion de vidéo adaptative en flux continu est prise en charge sur diverses plateformes iOS.

   Consultez la dernière prise en charge du guide de référence des visionneuses [Adobe](https://marketing.adobe.com/resources/help/en_US/s7/viewers_ref/).

   Dynamic Media Classic prend en charge la lecture vidéo mobile pour la vidéo MP 4 H .264. Le document suivant recense les périphériques BlackBerry prenant en charge ce format vidéo sur le site Web suivant :

   Voir [Formats vidéo pris en charge sur Blackberry](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482).

   La liste des périphériques Windows compatibles avec ce format vidéo figure dans le document suivant :

   Voir [Formats vidéo pris en charge sous Windows Phone](https://msdn.microsoft.com/en-us/library/ff462087(v=vs.92).aspx).

* Lisez la vidéo à l'aide des paramètres prédéfinis de visionneuse multimédia Classic, notamment :

   * des visionneuses de vidéos uniques,
   * des visionneuses de supports mixtes combinant du contenu vidéo et des images.

* Configurer des lecteurs vidéo pour répondre à vos besoins de stratégie de marque.
* Intégrer la vidéo à votre site Web, site mobile ou application mobile grâce à une simple URL ou à un code intégré.

**Démarrage rapide**

La description de flux de travaux détaillée suivante est conçue pour vous aider à maîtriser rapidement les opérations liées aux visionneuses de vidéos adaptatives dans Dynamic Media Classic. Chaque étape se termine par un renvoi à une rubrique contenant de plus amples informations.

**Cookie. Chargement et codage de vidéos**

Téléchargez et générez des visionneuses de vidéos adaptatives en suivant l’un des deux scénarios ci-après :

* **Télécharger des vidéos précodées** : si vos vidéos étaient déjà codées en dehors de Dynamic Media Classic, cliquez **sur Télécharger** sur la barre de navigation globale pour rechercher et télécharger des fichiers vidéo MP 4 directement dans Scene 7 Publishing System. Cliquez ensuite sur **Créer** &gt; **Visionneuses de vidéos adaptatives**. Accédez aux fichiers vidéo requis. Faites-les glisser et déposez-les dans le tableau Visionneuse de vidéos adaptative, puis enregistrez la visionneuse.
* **Télécharger des vidéos sources originales** : si vos vidéos ne sont pas codées, cliquez **sur Télécharger** sur la barre de navigation globale pour télécharger des fichiers source vidéo originaux (non-MP 4) et codez Scene 7 Publishing System en tant que fichiers MP 4 pour vous. Dans la boîte de dialogue Télécharger les options de la tâche, sous Options eVideo, sélectionnez **Vidéo adaptative**.

   Cette option conseillée permet de créer une visionneuse de vidéos adaptative qui applique automatiquement à la vidéo les paramètres de codage prédéfinis corrects, qu’il s’agisse d’un format 16:9 ou 4:3, en fonction des dimensions de la vidéo téléchargée. Lorsque vous procédez au transfert, une visionneuse de vidéos adaptative est automatiquement créée, avec trois codages vidéo aux proportions appropriées.

   Ou, dans la boîte de dialogue Options de tâche, sous Options eVideo, développez la liste **Paramètres prédéfinis de codage uniques** et sélectionnez des options de codage vidéo individuels parmi **Bureau**, **Mobile (iPhone, iPad, Android)** et **Tablette (iPad, Android)** afin de créer les fichiers MP4.

* Vous pouvez aussi retraiter une vidéo originale avec la fonction Retraiter. Les vidéos récemment codées sont ajoutées à la visionneuse de vidéos adaptative existante.

Voir [Chargement et codage de vidéos](uploading-encoding-videos.md#uploading_and_encoding_videos).

**Facultatif**

Dynamic Media Classic propose de nombreux paramètres prédéfinis de codage vidéo. Ces paramètres prédéfinis représentent les paramètres de codage vidéo les plus courants et ont été optimisés pour la lecture sur les écrans cibles.

Toutefois, si une personnalisation plus poussée est nécessaire, les administrateurs peuvent créer des paramètres vidéo prédéfinis pour personnaliser la taille et la lecture des vidéos pour les utilisateurs. Les administrateurs peuvent ajouter et gérer des paramètres vidéo prédéfinis sur la page Paramètres vidéo prédéfinis, sous Configuration &gt; Configuration de l’application &gt; Paramètres vidéo prédéfinis &gt; Paramètres prédéfinis de codage uniques. La page Paramètres vidéo prédéfinis propose des options permettant d’ajouter, de modifier, de supprimer et d’activer des paramètres vidéo prédéfinis.

Voir [Utilisation des paramètres prédéfinis de codage vidéo](uploading-encoding-videos.md#working_with_video_encoding_presets).

**2. Prévisualisation de vidéos dans une visionneuse**

Pour découvrir comment un utilisateur final voit une vidéo sur un ordinateur, votre site Web ou un périphérique mobile, sélectionnez la vidéo dans le panneau de navigation, puis cliquez sur **Prévisualiser**.

Voir [Prévisualisation de vidéos dans une visionneuse](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer).

Vous pouvez visionner la vidéo sur l’écran de prévisualisation. Vous pouvez également choisir d’autres visionneuses de vidéo pour vérifier l’aspect de la vidéo dans d’autres lecteurs. En règle générale, utilisez le lecteur vidéo HTML5 pour une lecture sur plusieurs écrans sur ordinateur, tablette et appareil mobile.

**Facultatif**

Personnalisation des paramètres prédéfinis de visionneuse - Dynamic Media Classic propose des paramètres prédéfinis de visionneuse pour la diffusion vidéo. Ces paramètres déterminent l’aspect de la visionneuse et le mode de fonctionnement des commandes de lecture. Pour personnaliser la visionneuse de vidéos, les administrateurs peuvent ajouter et gérer des paramètres prédéfinis de visionneuse à partir de la page Paramètres prédéfinis de la visionneuse. Pour ouvrir cette page, dans le coin supérieur droit de Scene7 Publishing System, cliquez sur Configuration &gt; Paramètres prédéfinis de la visionneuse. La page Paramètres prédéfinis de la visionneuse propose des commandes permettant d’ajouter, de modifier, de supprimer et d’activer des paramètres prédéfinis de la visionneuse.

Voir [Utilisation des paramètres prédéfinis de visionneuse de vidéos](previewing-videos-video-viewer.md#working_with_video_viewer_presets).

**Cookie. Déploiement de vidéos sur vos sites Web et sites mobiles**

Pour intégrer la vidéo sur votre site Web, procédez de l’une des manières suivantes :

* Affichez la vidéo dans sa propre fenêtre contextuelle ou modale, auquel cas vous devez utiliser la fonctionnalité Copier l’URL.

   Pour obtenir l’URL d’une vidéo, en mode Grille ou Liste, sélectionnez la vidéo dans le panneau de navigation. Click Preview, and then click Copy URL to the right of `Universal_HTML5_Viewer`.

   Lorsque vous cliquez sur Copier l’URL, l’URL est copiée dans le Presse-papiers. Placez ce code dans le code HTML de votre site Web, site mobile ou application.

   ***remarque**: Les URL sont activées uniquement après la publication de la vidéo ou de la visionneuse de vidéos adaptative.*

* Affichez la vidéo incorporée dans la page Web, auquel cas vous devez utiliser la fonction Intégrer le code.

   Pour obtenir le code intégré d’une vidéo, en mode Grille ou Liste, sélectionnez la vidéo dans le panneau de navigation. Cliquez sur Prévisualisation &gt; Liste des visionneuses. Sous la colonne Actions du tableau, cliquez sur Intégrer le code à droite de `Universal_HTML5_Video`. Il n’est pas possible de modifier le code.

   Cliquez sur Fermer et collez le code intégré dans vos pages Web.

   ***remarque**: Le code incorporé n'est activé que lorsque vous publiez la vidéo ou la visionneuse de vidéos adaptative.*

Voir [Déploiement de vidéos sur vos sites Web et sites mobiles](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites).

>[!MORELIKETHIS]
>
>* [Meilleures pratiques en matière de codage de vidéo](uploading-encoding-videos.md#best_practices_for_video_encoding)

