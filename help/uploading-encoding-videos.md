---
title: Chargement et codage de vidéos
seo-title: Chargement et codage de vidéos
description: Découvrez comment télécharger et coder des vidéos.
seo-description: Découvrez comment télécharger et coder des vidéos.
uuid: 9a7d6513-b10c-40b0-aebb-18a795c2b8d1
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: a0941823-850c-4373-9e37-f32032de3805
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '3938'
ht-degree: 81%

---


# Chargement et codage de vidéos{#uploading-and-encoding-videos}

Pour créer des visionneuses de vidéos adaptatives ou uniques pour une diffusion sur le Web ou sur des périphériques mobiles, vous devez d’abord télécharger vos fichiers vidéo originaux dans Dynamic Media Classic. Dynamic Media Classic code les vidéos au format MP4 et les publie dans les formats de fichier suivants :

**MP4** Dynamic Media Classic recommande le format MP4 comme format de fichier vidéo préféré. Utilisez le format de fichiers MP4 pour effectuer les opérations suivantes :

* Diffusion en flux continu dynamique HTTP sur les ordinateurs de bureau.
* Diffusion en continu HTTP (protocole de diffusion d’Apple).
* Diffusion vidéo progressive sur appareils mobiles Android, Blackberry et Windows

Dynamic Media Classic offre deux workflows pour télécharger des fichiers vidéo :

**Vidéos** précodées Vous téléchargez directement des fichiers MP4 vers Dynamic Media Classic. En procédant ainsi, les fichiers ne sont pas codés au moment où vous les téléchargez. Les fichiers sont précodés en vue de la diffusion sur l’ordinateur de bureau et sur des périphériques mobiles.

**Vidéos** source du Maître Téléchargez des fichiers vidéo source originaux et, au moment du téléchargement, codez ces fichiers au format MP4. Les vidéos codées sont intitulées « Vidéos » dans le panneau de navigation. Dynamic Media Classic prend en charge le codage de fichiers vidéo dans de nombreux formats.

* Vérifiez que les fichiers vidéo sources originaux que vous souhaitez coder sont pris en charge. 

   Voir [Types de fichiers vidéo pris en charge pour le codage](uploading-encoding-videos.md#supported-video-file-types-for-encoding).

* Choisissez un paramètre prédéfini de codage vidéo.

   Voir [Paramètres vidéo prédéfinis pour le codage des fichiers vidéo](application-setup.md#video-presets-for-encoding-video-files).

   Voir [Meilleures pratiques en matière de codage vidéo](uploading-encoding-videos.md#best-practices-for-video-encoding).

Dynamic Media Classic génère également des miniatures vidéo. Vous pouvez en savoir plus sur les miniatures de vidéos, l’obtention de leurs URL et la modification des images de l’affiche.

Voir [Utilisation de miniatures de vidéo](deploying-video-websites-mobile-sites.md#working-with-video-thumbnails).

**Pour télécharger et coder des vidéos**

Effectuez l’une des opérations suivantes :

*Si les vidéos sont déjà codées*

1. Sur la barre de navigation globale, cliquez sur **Télécharger**.
1. Dans l’écran Télécharger, cliquez sur l’onglet **A partir du bureau**.
1. On the Upload page, in the Select Files for Upload panel, click **Browse**, navigate to an MP4 video file, and then click **Open**.
1. Dans le panneau Choisir le dossier de destination, sélectionnez le dossier dans lequel placer le fichier téléchargé.
1. Sur la page de téléchargement, assurez-vous que l’option **Publier après le téléchargement** est cochée.
1. Cliquez sur **Lancer le téléchargement**.

*Si vous souhaitez coder vos vidéos à l’aide de Dynamic Media Classic*

1. Sur la barre de navigation globale, cliquez sur **Télécharger**.
1. Dans l’écran Télécharger, cliquez sur l’onglet **A partir du bureau**.
1. Dans le panneau Sélectionner les fichiers à télécharger, cliquez sur **Parcourir**, accédez à un fichier vidéo source original, puis cliquez sur **Ouvrir**.
1. Dans le panneau Choisir le dossier de destination, sélectionnez le dossier dans lequel placer le fichier téléchargé.
1. Dans le coin inférieur droit de la page, cliquez sur **Options tâche**.
1. Dans la boîte de dialogue Télécharger les options de la tâche, choisissez Options eVideo.
   * Effectuez l’une des opérations suivantes :
      * Il est conseillé d’utiliser la méthode suivante.
Sélectionnez **Codage de vidéo adaptative**.
Voir [Vidéo adaptative (par défaut)](application-setup.md#adaptive-video-default).
   * Facultatif : si vous souhaitez utiliser des paramètres de codage individuels, procédez comme suit.
Développez la liste **Paramètres prédéfinis de codage uniques**, puis sélectionnez des options de codage pour le Bureau, les mobiles et les tablettes.
Voir [Paramètres prédéfinis de codage de vidéo pour ordinateur de bureau](application-setup.md#desktop-video-encoding-presets), [Paramètres prédéfinis de codage vidéo pour périphérique mobile](application-setup.md#mobile-video-encoding-presets), [Paramètres prédéfinis de codage vidéo pour tablette](application-setup.md#tablet-video-encoding-presets).
1. Dans la boîte de dialogue Télécharger les options de la tâche, cliquez sur **Enregistrer**.
1. Sur la page de téléchargement, assurez-vous que l’option **Publier après le téléchargement** est cochée.
1. Sur la page de téléchargement, dans le coin inférieur droit, cliquez sur **Lancer le téléchargement**.

Si vous souhaitez coder à nouveau un fichier vidéo que vous avez précédemment téléchargé

1. Dans Dynamic Media Classic, dans le panneau de navigation, accédez à la vidéo et sélectionnez-la.
1. Cliquez sur **Fichier** > **Retraiter**.
1. Dans la boîte de dialogue Retraitement des fichiers de la tâche, choisissez Options eVideo.
1. Effectuez l’une des opérations suivantes :
   * Il est conseillé d’utiliser la méthode suivante.
Sélectionnez **Vidéo adaptative**.
Voir [Vidéo adaptative (par défaut)](application-setup.md#adaptive-video-default).
   * Facultatif : si vous souhaitez utiliser des paramètres de codage individuels, procédez comme suit.
Développez la liste **Paramètres prédéfinis de codage uniques**, puis sélectionnez des options de codage pour le Bureau, les mobiles et les tablettes.
Voir [Paramètres prédéfinis de codage de vidéo pour ordinateur de bureau](application-setup.md#desktop-video-encoding-presets), [Paramètres prédéfinis de codage vidéo pour périphérique mobile](application-setup.md#mobile-video-encoding-presets), [Paramètres prédéfinis de codage vidéo pour tablette](application-setup.md#tablet-video-encoding-presets).
1. Dans la boîte de dialogue Retraitement des fichiers, cliquez sur **Envoyer**.

Lorsque vous utilisez un paramètre prédéfini de codage de vidéo adaptative ou si vous utilisez plusieurs paramètres prédéfinis de codage uniques, une visionneuse de vidéos adaptative est automatiquement créée avec plusieurs codages vidéo. Vous pouvez également créer manuellement une visionneuse de vidéos adaptative en choisissant des vidéos individuelles.

Seuls les fichiers de type MP4 et M4V sont créés lorsque vous générez une visionneuse de vidéos adaptative automatiquement ou manuellement.

## Types de fichiers vidéo pris en charge pour le codage {#supported-video-file-types-for-encoding}

Le tableau suivant répertorie les types de fichiers vidéo (avec les codecs vidéo autorisés) que vous pouvez coder au format MP4 ou OGV lorsque vous transférez des fichiers. Le tableau répertorie les formats de fichiers et les codecs :

**Formats** de fichiers vidéo Tout comme un fichier ZIP, un format de fichier vidéo détermine comment les fichiers sont contenus dans le fichier vidéo. Un fichier vidéo contient généralement plusieurs pistes : une piste vidéo (sans audio) et une ou plusieurs pistes audio (sans vidéo), qui sont étroitement liées et synchronisées. Le format de fichier vidéo détermine comment ces différentes pistes de données et métadonnées sont organisées.

**Codecs** vidéo Un codec vidéo décrit l’algorithme par lequel une vidéo est codée. Un lecteur vidéo décode la vidéo en fonction de son codec, puis affiche une série d’images, ou cadres, à l’écran. Les codecs limitent la quantité d’informations que les fichiers vidéo ont besoin de stocker pour lire la vidéo. Les fichiers vidéo n’ont ainsi pas besoin de stocker les informations de chaque cadre, mais seulement les différences entre un cadre et le suivant. Comme la plupart des vidéos changent peu d’un cadre au suivant, les codecs permettent d’obtenir des taux de compression élevés et donc, des tailles de fichiers plus petites.

| Format de fichier vidéo | Codecs vidéo |
|:--- |:--- |
| 3GP | H.263, H.264 |
| Audio Video Interleave (AVI) | DivX, DV |
| M2P | MPEG-2 PS |
| M2T | MPEG-2 TS |
| M2TS | MPEG-2 TS |
| M2V | MPEG-2 ES |
| M4V | H.264 |
| MOV | DV, DVCPro 50, H.261, H.263, H.264, Sorenson Video 1 |
| MP4 | H.264/MPEG-4 AVC |
| MPEG | MPEG-2 SS |
| MPG | MPEG-2 SS |
| MTS | MPEG-2 |
| ProRes | APCN, APCS, APCO, APCH, AP4H |
| TS | DVCPro 50 |
| VOB | MPEG-2 |
| WMV/ASF | VC-1, Windows Media Video 7, Windows Media Video 8 |

>[!NOTE]
>
>l’écran Tâches vous alerte si vous téléchargez et tentez de coder un fichier vidéo, mais que celui-ci est rejeté car il contient un codec ou un conteneur de fichiers incompatible. Pour plus d’informations, voir [Vérification de fichiers de tâche](checking-job-files.md).

## Meilleures pratiques en matière de codage de vidéo {#best-practices-for-video-encoding}

Vous trouverez ci-dessous des conseils sur les meilleures pratiques pour le codage des fichiers vidéo source dans Dynamic Media Classic.

Pour plus de conseils sur le codage vidéo, voir :

* Article: *Streaming 101: The Basics — Codecs, Bandwidth, Data Rate, and Resolution: * [www.adobe.com/go/learn_s7_streaming101_en](https://www.adobe.com/go/learn_s7_streaming101_en).
* Video: *Video Encoding Basics: * [www.adobe.com/go/learn_s7_encoding_en](https://www.adobe.com/go/learn_s7_encoding_en).

### Fichiers vidéo source {#source-video-files}

Lorsque vous codez un fichier vidéo, utilisez un fichier vidéo source ayant la plus haute qualité possible. Evitez d’utiliser des fichiers vidéo précédemment codés, car ces fichiers sont déjà compressés, et un codage supplémentaire crée une vidéo de qualité inférieure.

Le tableau ci-dessous décrit la taille recommandée, le format et le débit minimal requis pour vos fichiers vidéo sources au moment de leur codage :

| Taille | Format | Débit minimum |
|--- |--- |--- |
| 1024 x 768 | 4:3 | 4 500 Kbits/s pour la plupart des vidéos. |
| 1280 x 720 | 16:9 | 3 000 à 6 000 Kbits/s, selon la quantité de mouvement dans la vidéo. |
| 1920 x 1080 | 16:9 | 6 000 à 8 000 Kbits/s, selon la quantité de mouvement dans la vidéo. |

### Obtention des métadonnées d’un fichier {#obtaining-a-file-s-metadata}

Vous pouvez obtenir les métadonnées d’un fichier en visualisant ses métadonnées dans Dynamic Media Classic, à l’aide d’un outil d’édition vidéo ou d’une application conçue pour l’obtention de métadonnées. Voici les instructions d’utilisation de MediaInfo, une application tierce permettant d’extraire les métadonnées d’un fichier vidéo :

1. Accédez à cette page Web : [https://mediainfo.sourceforge.net/en/Download](https://mediainfo.sourceforge.net/en/Download).
1. Sélectionnez et téléchargez le programme d’installation pour la version interface graphique utilisateur, puis suivez les instructions d’installation.
1. Après l’installation, cliquez avec le bouton droit sur le fichier vidéo (dans Windows seulement) et sélectionnez MediaInfo, ou bien ouvrez MediaInfo et faites glisser votre fichier vidéo dans l’application. Toutes les métadonnées de votre fichier vidéo, telles que sa largeur, sa hauteur et le nombre d’images par seconde, sont alors visibles à l’écran. 

### Format {#aspect-ratio}

Lorsque vous choisissez ou créez un paramètre prédéfini de codage vidéo pour votre fichier vidéo original, assurez-vous que le paramètre prédéfini indique le même format que le fichier vidéo original. Le *format* fait référence au rapport largeur/hauteur de la vidéo.

Pour déterminer le format d’un fichier vidéo, récupérez les métadonnées de ce fichier et notez les valeurs de largeur et de hauteur (voir [Obtention des métadonnées d’un fichier](uploading-encoding-videos.md#obtaining_a_file_s_metadata)). Utilisez ensuite cette formule pour déterminer le format :

largeur/hauteur = format

Ce tableau décrit la façon dont les résultats de la formule se traduisent en choix de formats :

| Résultat de la formule | Format |
|--- |--- |
| 1.33 | 4:3 |
| 0.75 | 3:4 |
| 1.78 | 16:9 |
| 0.56 | 9:16 |

Par exemple, une vidéo qui a une largeur de 1 440 pour une hauteur de 1 080 a un format de 1 440/1 080, soit 1,33. Dans ce cas, vous choisissez un paramètre prédéfini de codage vidéo avec un format de 4:3 pour le codage du fichier vidéo.

### Débit {#data-rate}

The *data rate* (also called the* bit rate*) is the amount of data that is encoded to make up a single second of video playback. Le débit de données est mesuré en kilobits par seconde (Kbits/s).

>[!NOTE]
>
>du fait que tous les codecs utilisent la compression avec perte, le débit de données est le facteur le plus important de la qualité vidéo. Quand vous utilisez la compression avec perte, plus vous compressez la vidéo, plus la qualité de l’image se dégrade. Toutes les autres caractéristiques étant égales (résolution, taux de rafraîchissement et codec), plus le débit de données est faible, moins la qualité du fichier compressé est bonne.

Lorsque vous choisissez un paramètre prédéfini de codage vidéo, tenez compte de la vitesse de connexion de l’utilisateur final auquel la vidéo est destinée. Choisissez un paramètre prédéfini avec un débit de données correspondant à 80 pour cent de cette vitesse. Par exemple, si la vitesse de connexion de l’utilisateur final est de 1 000 Kb/s, le meilleur paramètre prédéfini est celui qui comprend un débit vidéo de 800 Kb/s.

Ce tableau décrit le débit de données de vitesses de connexion courantes.

| Vitesse (Kb/s) | Type de connexion |
|--- |--- |
| 256 | Connexion commutée. |
| 800 | Connexion mobile standard. Pour cette connexion, visez un débit de données de l’ordre de 400 Kb/s, jusqu’à 800 Kb/s pour les expériences 3G. |
| 2 000 | Connexion haut débit standard de bureau. Pour cette connexion, cible un débit de données dans la plage de 800 à 2 000 Kbits/s, la plupart des cibles atteignant en moyenne 1 200 à 1 500 Kbits/s. |
| 5000 | Connexion haut débit standard. Il est déconseillé de coder dans cette fourchette supérieure, car la diffusion de la vidéo à cette vitesse n’est pas possible pour la plupart des consommateurs. |

### Résolution {#resolution}

La *résolution* décrit la hauteur et la largeur d’un fichier vidéo, exprimée en pixels. La plupart des vidéos sources sont stockées à une résolution élevée (par exemple, 1 920 x 1 080). A des fins de diffusion en flux continu, la vidéo source est compressée à une résolution inférieure (640 x 480, voire moins).

La résolution et le débit de données sont deux facteurs étroitement liés qui déterminent la qualité de la vidéo. Pour maintenir la même qualité vidéo, plus le nombre de pixels (c’est-à-dire la résolution) est élevé dans un fichier vidéo, plus le débit de données doit l’être également. Par exemple, considérez le nombre de pixels par image dans un fichier vidéo d’une résolution de 320 x 240 pixels et dans un fichier vidéo d’une résolution de 640 x 480 pixels :

| Résolution | Pixels par image |
|--- |--- |
| 320 x 240 | 76 800 |
| 640 x 480 | 307 200 |

Le fichier de 640 x 480 possède quatre fois plus de pixels par image. Pour atteindre le même débit de données avec ces deux résolutions, vous appliquez une compression de 4 au fichier d’une résolution de 640 x 480 pixels, ce qui peut réduire la qualité de la vidéo. Par conséquent, un débit de données vidéo de 250 Kb/s produit un affichage de haute qualité à une résolution de 320 x 240 pixels, mais pas à une résolution de 640 x 480 pixels.

>[!NOTE]
>
>En général, plus le débit de données que vous utilisez est élevé, meilleure est la qualité de la vidéo, et plus la résolution que vous utilisez est élevée, plus le débit de données doit l’être également pour que la qualité de visionnage soit préservée (par rapport aux résolutions inférieures).

Du fait que la résolution et le débit de données sont liés, vous avez le choix entre deux options lors du codage vidéo :

* Choisir un débit de données puis, en fonction de ce paramètre, coder à la résolution la plus haute pour obtenir une vidéo de bonne qualité.
* Choisir une résolution, puis coder au débit de données nécessaire pour que la qualité vidéo soit optimale à la résolution choisie.

Lorsque vous choisissez (ou créez) un paramètre prédéfini de codage vidéo pour votre fichier vidéo original, utilisez ce tableau pour choisir la résolution cible appropriée.

| Résolution | Hauteur (pixels) | Taille d’écran |
|--- |--- |--- |
| 240p | 240 | Ecran de très petite taille |
| 300p | 300 | Petit écran équipant généralement les appareils mobiles |
| 360p | 360 | Petit écran |
| 480p | 480 | Ecran de taille moyenne |
| 720p | 720 | Grand écran |
| 1080p | 1 080 | Grand écran haute définition |

### Images par seconde {#fps-frames-per-second}

Aux Etats-Unis et au Japon, la plupart des vidéos sont tournées à 29,97 ips ; en Europe, la plupart des vidéos le sont à 25 ips. Un film est tourné à 24 ips.

Choisissez un paramètre prédéfini de codage vidéo correspondant au nombre d’ips de votre vidéo originale. Par exemple, si le débit est de 25 ips pour la vidéo originale, choisissez un paramètre prédéfini de 25 ips pour le codage. Par défaut, tous les codages personnalisés utilisent le nombre d’images par seconde de la vidéo originale. C’est pourquoi il est inutile d’indiquer le nombre d’images par seconde lorsque vous créez un paramètre prédéfini de codage vidéo.

### Dimensions du codage vidéo {#video-encoding-dimensions}

Pour obtenir des résultats optimaux, sélectionnez les dimensions de codage de façon à ce que la vidéo source corresponde à un multiple entier de toutes vos vidéos codées.

Pour ce faire, il suffit de diviser la largeur de la source par la largeur codée pour obtenir le rapport de largeur, puis de diviser la hauteur de la source par la hauteur codée pour obtenir le rapport de hauteur.

Si le résultat est un nombre entier, cela signifie que la mise à l’échelle de la vidéo est parfaite. Si le résultat n’est pas un nombre entier, la qualité vidéo s’en ressentira en raison de la présence d’artefacts vidéo (pixels résiduels). Cet effet est plus visible lorsque la vidéo contient du texte.

Supposons, par exemple, que la résolution de votre vidéo source soit équivalente à 1920 x 1080 pixels. Dans le tableau ci-après, les trois vidéos codées indiquent les paramètres de codage optimaux à appliquer.

| Type de vidéo | Largeur x Hauteur | Rapport de largeur | Rapport de hauteur |
|--- |--- |--- |--- |
| Source | 1 920 x 1 080 | 1 | 1 |
| Codée | 960 x 540 | 2 | 2 |
| Codée | 640 x 360 | 3 | 3 |
| Codée | 480 x 270 | 4 | 4 |

### Format de fichier vidéo codé {#encoded-video-file-format}

Adobe Dynamic Media Classic recommande l’utilisation des paramètres prédéfinis de codage vidéo MP4 H.264. Comme les fichiers MP4 utilisent le codec vidéo H.264, la vidéo est de haute qualité mais dans un fichier au volume compressé.

## Utilisation des paramètres prédéfinis de codage vidéo {#working-with-video-encoding-presets}

Les fichiers vidéo originaux créés à partir d’équipement de production vidéo et de logiciels d’édition vidéo sont souvent trop volumineux et dans un format inapproprié à la diffusion vers des destinations en ligne. Pour convertir de la vidéo numérique afin qu’elle présente le format et les spécifications appropriés pour être lue sur divers écrans, vous pouvez *transcoder* les fichiers vidéo (processus également appelé « *codage* »). Durant le processus de codage, la vidéo est compressée pour atteindre une taille de fichier inférieure optimale pour la distribution sur le Web et sur des périphériques mobiles.

Voir [Chargement et codage de vidéos](uploading-encoding-videos.md#uploading-and-encoding-videos).

Dynamic Media Classic vous offre une bibliothèque de paramètres prédéfinis de codage vidéo qui reflètent les paramètres de codage les plus courants. Ces paramètres ont été optimisés pour la lecture sur les écrans cibles. De plus, les administrateurs peuvent créer leurs propres paramètres prédéfinis de codage vidéo pour personnaliser la taille et la qualité de lecture des vidéos pour les utilisateurs. Tous les paramètres prédéfinis de codage vidéo, prêts à l’emploi de Dynamic Media Classic ou personnalisés, permettent de produire de la vidéo au format MP4.

Sur l’écran Paramètres vidéo prédéfinis, les administrateurs peuvent configurer et gérer le codage vidéo. Ils peuvent effectuer les opérations suivantes :

* activer et désactiver les paramètres vidéo prédéfinis ;
* créer un paramètre prédéfini de codage vidéo ;
* modifier les paramètres prédéfinis de codage vidéo ;
* supprimer des paramètres vidéo prédéfinis.

Toute vidéo que vous téléchargez vers Dynamic Media Classic ou que vous codez dans Dynamic Media Classic est traitée comme une &quot;vidéo&quot;. En d’autres termes, ce mode de classification des fichiers signifie que vous pouvez diffuser la vidéo à des fins de lecture sur des ordinateurs de bureau, des appareils mobiles, ou les deux. Par exemple, vous pouvez prévisualisation ces types de vidéos dans Dynamic Media Classic. Vous pouvez également générer des URL (à l’aide de la fonction Copier l’URL) et du code que vous pouvez incorporer (à l’aide de la fonction Intégrer le code) pour l’utiliser avec les lecteurs vidéo, sur les sites web, etc.

Voir [Prévisualisation de vidéos dans une visionneuse](previewing-videos-video-viewer.md#previewing-videos-in-a-video-viewer).

Voir [Liaison d’une URL de vidéo à un site Web ou un site mobile](deploying-video-websites-mobile-sites.md#linking-a-video-url-to-a-mobile-site-or-a-website).

Voir [Incorporation de la visionneuse de vidéos sur une page Web](deploying-video-websites-mobile-sites.md#embedding-the-video-viewer-on-a-web-page).

Pour les fichiers vidéo que vous téléchargez et codez dans Dynamic Media Classic, la vidéo est diffusée au format de fichier suivant :

**MP4 H.264** Utilisez des fichiers MP4 pour les opérations suivantes :

* Diffusion en flux continu dynamique HTTP sur les ordinateurs de bureau.
* HLS (HTTP Live Streaming, protocole de diffusion en continu d’Apple).
* Diffusion vidéo progressive sur appareils mobiles Android, Blackberry et Windows.

Tout autre format vidéo et codec est traité comme une &quot;vidéo Maîtresse&quot;. Ce mode de classification des fichiers signifie que la vidéo est un fichier vidéo source non prévu pour la lecture vidéo sur des périphériques de bureau ou des périphériques mobiles. Par exemple, vous ne pouvez pas prévisualisation ces types de vidéos dans Dynamic Media Classic. Vous ne pouvez pas non plus copier des URL et du code intégré destinés aux lecteurs vidéo, aux sites web, et ainsi de suite.

### Filtrage de la liste des paramètres prédéfinis de codage vidéo {#filtering-the-list-of-video-encoding-presets}

Les pages Paramètres vidéo prédéfinis et Paramètres prédéfinis de vidéo adaptative se composent d’un tableau qui répertorie l’état actif, le nom du paramètre prédéfini, le périphérique de lecture prévu, la dimension de la vidéo et le débit cible des données de chaque paramètre vidéo prédéfini.

Vous pouvez affiner la liste en choisissant le filtrage Les deux, Actif ou Inactif, pour afficher tous les paramètres vidéo prédéfinis ou restreindre la liste aux paramètres actifs ou inactifs.

Vous pouvez également les filtrer en fonction d’une option de périphérique de lecture afin de restreindre la liste aux paramètres vidéo prédéfinis conçus pour la lecture de vidéos sur tous les appareils, sur les ordinateurs de bureau, les appareils mobiles ou les tablettes.

**Filtrage de la liste des paramètres prédéfinis de codage vidéo**

1. In Dynamic Media Classic, click **Setup** > **Application Setup** > **Video Presets** > **Adaptive Video Presets** or **Single Encoding Presets**.

   Les pages Paramètres prédéfinis de vidéo adaptative et Paramètres prédéfinis de codage uniques se composent d’un tableau qui répertorie l’état actif, le nom du paramètre prédéfini, le périphérique de lecture prévu, la dimension de la vidéo et le débit cible des données de chaque paramètre vidéo prédéfini.

1. Sur la page Paramètres prédéfinis de codage uniques intitulée Paramètres vidéo prédéfinis, sur la barre d’outils Paramètres vidéo prédéfinis, utilisez les deux listes déroulantes pour affiner la liste des paramètres prédéfinis dans le tableau en fonction de l’état Actif et du périphérique de lecture.

   * Dans la première, une liste déroulante restreinte, sélectionnez **Les deux** pour afficher tous les paramètres vidéo prédéfinis ou choisissez **Actif** ou **Inactif** pour restreindre la liste aux paramètres actifs ou inactifs.
   * Dans la deuxième, une liste déroulante plus étendue, sélectionnez une option de périphérique de lecture pour restreindre la liste aux paramètres vidéo prédéfinis destinés à lire des vidéos sur les ordinateurs de bureau, sur les appareils mobiles ou sur les tablettes.

### Activation ou désactivation des paramètres prédéfinis de codage vidéo {#activating-or-deactivating-video-encoding-presets}

Les paramètres vidéo prédéfinis activés sont répertoriés dans la boîte de dialogue Télécharger les options de la tâche. Cette boîte de dialogue s’ouvre lorsqu’un utilisateur transfère les fichiers vidéo pendant le processus de téléchargement. Ils peuvent choisir parmi une liste de tous les paramètres prédéfinis de codage activés.

**Activation ou désactivation des paramètres prédéfinis de codage vidéo**

1. Dans Dynamic Media Classic, cliquez sur **Configuration** > Configuration **de l’** application > Paramètres prédéfinis **** vidéo.
1. Effectuez l’une des opérations suivantes :

   * Cliquez sur **Paramètres prédéfinis de vidéo adaptative**.
   * Cliquez sur **Paramètres prédéfinis de codage uniques**.

1. Effectuez l’une des opérations suivantes :

   * Pour activer un paramètre vidéo prédéfini, sur la page Paramètres prédéfinis, sous la colonne Actif, cochez la case en regard du nom du paramètre prédéfini.
   * Pour désactiver un paramètre vidéo prédéfini, décochez la case en regard des paramètres vidéo prédéfinis que vous souhaitez rendre inactifs.

      ***note**: Inactive Video Presets do not appear in the Upload Job Options dialog box. *

1. Dans le coin inférieur droit de la page, cliquez sur **Fermer**.

### Ajout ou modification d’un paramètre prédéfini de codage vidéo {#adding-or-editing-a-video-encoding-preset}

Vous pouvez créer vos propres paramètres prédéfinis de codage unique et les ajouter au tableau Paramètres vidéo prédéfinis. Vous pouvez également apporter des modifications à tous les paramètres vidéo prédéfinis de codage unique fournis avec Dynamic Media Classic, à condition d’enregistrer le paramètre prédéfini modifié sous un nouveau nom.

Dynamic Media Classic a défini des limites maximales sur le débit de données de la cible, la hauteur de résolution et la largeur de résolution afin de garantir une expérience de lecture appropriée. Les messages d’avertissement s’affichent si vous dépassez les limites suivantes :

* Pour une lecture vidéo sur ordinateur, les limites sont : (Largeur/16) * (Hauteur/16) &lt; 8192. 
* Pour une lecture vidéo sur périphérique mobile, les limites sont : (Largeur/16) * (Hauteur/16) &lt; 660 ; débit de données cible &lt; 4000. 
* Pour une lecture vidéo sur tablette, les limites sont : (Largeur/16) * (Hauteur/16) &lt; 3600.

**Ajout ou modification d’un paramètre prédéfini de codage vidéo**

1. Dans Dynamic Media Classic, cliquez sur **Configuration** > Configuration **de l’** application > Paramètres prédéfinis **** vidéo.
1. Cliquez sur **Paramètres prédéfinis de codage uniques** pour ouvrir la page Paramètres vidéo prédéfinis.
1. Sur la page Paramètres vidéo prédéfinis, procédez de l’une des manières suivantes :

   * Sur la barre d’outils Paramètres vidéo prédéfinis, cliquez sur **Ajouter** pour ajouter un nouveau paramètre vidéo prédéfini.
   * Sélectionnez un paramètre vidéo prédéfini. Dans la barre d’outils, cliquez sur **Modifier**.

      You cannot edit Dynamic Media Classic predefined presets; you can only create a preset from an existing one by choosing **Save As**.

1. Dans la page Ajout d’un paramètre vidéo prédéfini ou Modification d’un paramètre vidéo prédéfini, définissez les options Paramètres vidéo prédéfinis dont vous avez besoin.

   Voir [Meilleures pratiques en matière de codage de vidéo](uploading-encoding-videos.md#best-practices-for-video-encoding) pour connaître les paramètres recommandés.

   | Option de paramètres vidéo prédéfinis | Description |
   |--- |--- |
   | Nom du paramètre prédéfini | Entrez un nom descriptif pour le paramètre vidéo prédéfini. Le nom que vous indiquez est visible dans la boîte de dialogue Télécharger les options de la tâche, où les utilisateurs choisissent les options de transcodage. |
   | Description | Décrivez le paramètre vidéo prédéfini. La description que vous fournissez apparaît sous forme d’info-bulle lorsque vous déplacez le pointeur sur le nom du paramètre prédéfini dans la boîte de dialogue Télécharger les options de la tâche, où les utilisateurs choisissent les options de transcodage. |
   | Périphérique de lecture | Choisissez le périphérique sur lequel il est prévu que la vidéo soit lue. Les options sont Ordinateur (ordinateurs de bureau), Mobile (iPhone, iPad, Android); ou Tablette (iPad uniquement). Ce paramètre détermine automatiquement le codec audio et vidéo approprié utilisé pendant le codage. |
   | Débit de la cible | Entrez la vitesse de connexion Internet moyenne (en kilobits par seconde) de l’utilisateur final cible. Vous pouvez saisir le débit ou faire glisser le curseur pour le saisir. Le spectre de vitesse de connexion de l’utilisateur répertorie les vitesses attendues pour les connexions haut débit, DSL, mobiles et à ligne commutée. Ce paramètre détermine automatiquement le débit combiné de données audio et vidéo, autrement dit, la quantité de données qu’il est nécessaire de coder pour produire une seule seconde de lecture vidéo. Plus le débit binaire est élevé, meilleure est la qualité de la vidéo produite. Cependant, un débit de données trop élevé se traduit par des fichiers de taille très importante, ce qui peut altérer l’expérience de visionnage pour les utilisateurs qui ne disposent pas d’une connexion avec une bande passante aussi large. Il est préférable d’essayer d’équilibrer ces deux facteurs afin d’offrir une expérience de lecture vidéo de qualité, qui convienne également aux utilisateurs qui ne disposent pas d’une bande passante aussi large. |
   | Format | Le format fait référence au rapport de la largeur de la vidéo à sa hauteur. Les deux premières proportions répertoriées ci-dessous sont souvent utilisées pour afficher la vidéo horizontalement :<ul><li> 4:3, utilisé pour la diffusion de la quasi-totalité des contenus télévisés de définition standard.</li><li>16:9, utilisé pour la diffusion sur grand écran de la quasi-totalité des contenus télévisés haute définition (HDTV) et des films.</li><li>Auto-scale (« Redimensionnement automatique ») : (valeur par défaut) un paramètre prédéfini de codage unique qui fonctionne avec n’importe quelle proportion pour créer des vidéos pour une diffusion sur téléphone, tablette et ordinateur de bureau. Les vidéos source transférées qui sont codées à l’aide de ce paramètre prédéfini sont définies avec une hauteur fixe. Toutefois, la largeur est automatiquement mise à l’échelle pour conserver les proportions de la vidéo (rapport largeur/hauteur).</li><li>Custom (« Personnaliser ») : option utilisée lorsque vous souhaitez définir une taille de vidéo non standard.</li><li>La sélection du format permet de contrôler la taille de la résolution en largeur et en hauteur, de sorte que chaque valeur soit automatiquement mise à l’échelle avec le format adéquat.</li></ul> |
   | Taille de résolution | La taille de résolution fait référence aux dimensions de la vidéo, en termes de rapport du nombre de pixels en largeur sur le nombre de pixels en hauteur. Saisissez une valeur de largeur et de hauteur en pixels ou faites glisser le curseur pour saisir ces valeurs. Le spectre des résolutions répertorie les tailles de résolution les plus utilisées. Les valeurs de largeur et de hauteur s’adapteront automatiquement au format que vous avez sélectionné. Par exemple, si vous sélectionnez le format 4:3 et saisissez 400 pour la largeur, 300 est automatiquement entré pour la hauteur.Si vous avez sélectionné Mise à l&#39;échelle automatique pour le paramètre Format, la valeur Largeur de la taille de résolution est automatiquement définie sur Auto.Cliquez sur Prévisualisation pour ouvrir une fenêtre de navigateur et voir vos choix de résolution. |
   | Encoder un suffixe de fichier | Entrez un suffixe. Ce suffixe est ajouté au fichier vidéo encodé résultant. Vous pouvez entrer un trait d’union et un trait de soulignement dans le nom, mais les espaces et les caractères spéciaux ne sont pas autorisés. |
   | Autres paramètres | Dynamic Media Classic détermine automatiquement tous les autres paramètres de codage en fonction des recommandations de codage. |

1. Effectuez l’une des opérations suivantes :

   * Cliquez sur **Enregistrer** si vous avez ajouté ou modifié un paramètre vidéo prédéfini.
   * Cliquez sur **Enregistrer en tant que** si vous avez ajouté un paramètre vidéo prédéfini à partir d’un paramètre prédéfini existant.

### Suppression d’un paramètre prédéfini de codage vidéo {#deleting-a-video-encoding-preset}

Les administrateurs peuvent supprimer des paramètres vidéo prédéfinis personnalisés. Les paramètres vidéo prédéfinis fournis avec Dynamic Media Classic ne peuvent pas être supprimés.

**Suppression d’un paramètre prédéfini de codage vidéo**

1. Dans Dynamic Media Classic, cliquez sur **Configuration** > Configuration **de l’** application > Paramètres prédéfinis **** vidéo.
1. Cliquez sur **Paramètres prédéfinis de codage uniques** pour ouvrir la page Paramètres vidéo prédéfinis.
1. Sur la page Paramètres vidéo prédéfinis, sélectionnez dans le tableau un paramètre vidéo prédéfini dont vous n’avez plus besoin.
1. Sur la barre d’outils Paramètres vidéo prédéfinis, cliquez sur **Supprimer**.
1. Dans la boîte de dialogue Supprimer le paramètre prédéfini, cliquez sur **Supprimer**.

>[!MORELIKETHIS]
>
>* [Démarrage rapide : Vidéo](quick-start-video.md#quick-start-video)
>* [Chargement et codage de vidéos](uploading-encoding-videos.md#uploading-and-encoding-videos)
>* [Utilisation des paramètres prédéfinis de visionneuse de vidéos](previewing-videos-video-viewer.md#working-with-video-viewer-presets)

