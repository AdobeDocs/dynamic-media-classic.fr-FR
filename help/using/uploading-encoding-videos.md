---
title: Chargement et codage de vidéos
description: Découvrez comment charger et coder des vidéos dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 93ad91d7-f3dd-484b-b62c-633fcb864bbf
topic: Content Management
level: Intermediate
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '3989'
ht-degree: 40%

---

# Chargement et codage de vidéos{#uploading-and-encoding-videos}

Pour créer des visionneuses de vidéos ou adaptatives uniques à diffuser sur le Web ou sur des appareils mobiles, vous devez d’abord charger vos fichiers vidéo principaux dans Adobe Dynamic Media Classic. Adobe Dynamic Media Classic code les vidéos au format MP4 et les publie dans les formats de fichiers suivants :

* **MP4** : Adobe Dynamic Media Classic recommande le format MP4 comme format de fichier vidéo préféré. Utilisez le format de fichiers MP4 pour effectuer les opérations suivantes :

   * Diffusion en flux continu dynamique HTTP sur les ordinateurs de bureau.
   * HTTP Live Streaming (protocole de diffusion en continu Apple).
   * Diffusion vidéo progressive sur des appareils mobiles Android™, BlackBerry® et Windows®

  Adobe Dynamic Media Classic propose deux processus pour charger des fichiers vidéo :

* **Vidéos pré-codées** : vous téléchargez des fichiers MP4 directement vers Adobe Dynamic Media Classic. En procédant ainsi, les fichiers ne sont pas codés au moment où vous les téléchargez. Les fichiers sont précodés en vue de la diffusion sur l’ordinateur de bureau et sur des périphériques mobiles.

* **Principal des vidéos source** : téléchargez des fichiers vidéo sources originales et, lors du téléchargement, codez ces fichiers dans des fichiers MP4. Les vidéos codées sont intitulées &quot;Vidéo&quot; dans le panneau Parcourir . Adobe Dynamic Media Classic prend en charge le codage de fichiers vidéo dans de nombreux formats.

   * Assurez-vous que les fichiers vidéo sources originales à coder sont pris en charge.

     Voir [Types de fichiers vidéo pris en charge pour le codage](uploading-encoding-videos.md#supported-video-file-types-for-encoding).

   * Choisissez un paramètre prédéfini de codage vidéo.

     Voir [Paramètres vidéo prédéfinis pour le codage des fichiers vidéo](application-setup.md#video-presets-for-encoding-video-files).

     Voir [Meilleures pratiques en matière de codage vidéo](uploading-encoding-videos.md#best-practices-for-video-encoding).

Adobe Dynamic Media Classic génère également des miniatures vidéo. Vous pouvez en savoir plus sur les miniatures de vidéos, l’obtention de leurs URL et la modification des images de l’affiche.

Voir [Utilisation de miniatures vidéo](deploying-video-websites-mobile-sites.md#working-with-video-thumbnails).

**Pour télécharger et coder des vidéos :**

Effectuez l’une des opérations suivantes.

*Si vos vidéos sont déjà codées*

1. Dans la barre de navigation globale, sélectionnez **[!UICONTROL Télécharger]**.
1. Sur la page Télécharger, sélectionnez l’onglet **[!UICONTROL Depuis le bureau]** .
1. Sur la page Télécharger, dans le panneau **[!UICONTROL Sélectionner les fichiers à télécharger]**, sélectionnez **[!UICONTROL Parcourir]**, accédez à un fichier vidéo MP4, puis sélectionnez **[!UICONTROL Ouvrir]**.
1. Dans le panneau **[!UICONTROL Destination du dossier]** sélectionné, sélectionnez un dossier pour le fichier chargé.
1. Sur la page Télécharger , assurez-vous que l’option **[!UICONTROL Publish After Uploading]** est cochée.
1. Sélectionnez **[!UICONTROL Submit Upload]**.

*Si vous souhaitez coder vos vidéos à l’aide d’Adobe Dynamic Media Classic*

1. Dans la barre de navigation globale, sélectionnez **[!UICONTROL Télécharger]**.
1. Sur la page Télécharger, sélectionnez l’onglet **[!UICONTROL Depuis le bureau]** .
1. Dans le panneau **[!UICONTROL Select Files to Upload]**, sélectionnez **[!UICONTROL Browse]**, accédez à un fichier vidéo source principal, puis sélectionnez **[!UICONTROL Open]**.
1. Dans le panneau **[!UICONTROL Destination du dossier]** sélectionné, sélectionnez un dossier pour le fichier chargé.
1. Dans le coin inférieur droit de la page, sélectionnez **[!UICONTROL Options de tâche]**,
1. Dans la boîte de dialogue Télécharger les options de la tâche, développez **[!UICONTROL Options eVideo]**, puis effectuez l’une des opérations suivantes :

   * La bonne pratique consiste à sélectionner **[!UICONTROL Codage vidéo adaptatif]**. Voir [Vidéo adaptative (par défaut)](application-setup.md#adaptive-video-default).
   * Facultatif. Si vous souhaitez utiliser des paramètres de codage individuels, développez **[!UICONTROL Paramètres prédéfinis de codage uniques]**, puis sélectionnez les options de codage souhaitées pour Bureau, Mobile et Tablette.
Voir [Paramètres prédéfinis de codage de vidéo pour ordinateur de bureau](application-setup.md#desktop-video-encoding-presets), [Paramètres prédéfinis de codage vidéo pour périphérique mobile](application-setup.md#mobile-video-encoding-presets), [Paramètres prédéfinis de codage vidéo pour tablette](application-setup.md#tablet-video-encoding-presets).
1. Dans la boîte de dialogue Télécharger les options de la tâche, sélectionnez **[!UICONTROL Enregistrer]**.
1. Sur la page Télécharger , assurez-vous que l’option **[!UICONTROL Publish After Uploading]** est cochée.
1. Sur la page Télécharger, dans le coin inférieur droit, sélectionnez **[!UICONTROL Submit Upload]**.

*Si vous souhaitez réencoder un fichier vidéo que vous avez précédemment téléchargé*

1. Dans Adobe Dynamic Media Classic, dans le panneau Parcourir , accédez à la vidéo et sélectionnez-la.
1. Accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Retraiter]**.
1. Dans la boîte de dialogue Retraiter Assets, développez **[!UICONTROL Options eVideo]**, puis effectuez l’une des opérations suivantes :
   * La bonne pratique consiste à utiliser la méthode suivante. Sélectionnez **Vidéo adaptative**.
Voir [Vidéo adaptative (par défaut)](application-setup.md#adaptive-video-default).
   * Facultatif. Si vous souhaitez utiliser des paramètres de codage individuels, développez **[!UICONTROL Paramètres prédéfinis de codage uniques]**, puis sélectionnez les options de codage souhaitées pour Bureau, Mobile et Tablette.
Voir [Paramètres prédéfinis de codage de vidéo pour ordinateur de bureau](application-setup.md#desktop-video-encoding-presets), [Paramètres prédéfinis de codage vidéo pour périphérique mobile](application-setup.md#mobile-video-encoding-presets), [Paramètres prédéfinis de codage vidéo pour tablette](application-setup.md#tablet-video-encoding-presets).
1. Dans la boîte de dialogue Retraiter Assets, sélectionnez **[!UICONTROL Submit]**.

Lorsque vous utilisez un ou plusieurs paramètres prédéfinis de codage de vidéo adaptative, vous obtenez une visionneuse de vidéos adaptative automatiquement créée avec plusieurs codages vidéo. Vous pouvez également créer manuellement une visionneuse de vidéos adaptative en choisissant des vidéos individuelles.

Seuls les fichiers de type MP4 et M4V sont créés lorsque vous générez une visionneuse de vidéos adaptative automatiquement ou manuellement.

## Types de fichiers vidéo pris en charge pour le codage {#supported-video-file-types-for-encoding}

Le tableau suivant répertorie les types de fichiers vidéo (avec les codecs vidéo autorisés) que vous pouvez coder au format MP4 ou OGV lorsque vous transférez des fichiers. Le tableau répertorie les formats de fichiers et les codecs :

* **Formats de fichiers vidéo** : tout comme un fichier ZIP, un format de fichier vidéo détermine la manière dont les fichiers sont contenus dans le fichier vidéo. Un fichier vidéo contient généralement plusieurs pistes : une piste vidéo (sans audio) et une ou plusieurs pistes audio (sans vidéo), qui sont étroitement liées et synchronisées. Le format de fichier vidéo détermine comment ces différentes pistes de données et métadonnées sont organisées.

* **Codecs vidéo** : un codec vidéo décrit l’algorithme par lequel une vidéo est codée. Un lecteur vidéo décode la vidéo en fonction de son codec, puis affiche une série d’images, ou cadres, à l’écran. Les codecs limitent la quantité d’informations que les fichiers vidéo ont besoin de stocker pour lire la vidéo. Au lieu d’informations sur chaque image, seules les informations sur les différences entre une image et la suivante sont stockées. Comme la plupart des vidéos changent peu d’une image à l’autre, les codecs permettent des taux de compression élevés, ce qui se traduit par des tailles de fichiers plus petites.

  | Format de fichier vidéo | Codecs vidéo |
  | --- | --- |
  | 3GP | H.263, H.264 |
  | Audio Video Interleave (AVI) | DivX, DV |
  | M2P | MPEG-2 PS |
  | M2T | MPEG-2 TS |
  | M2TS | MPEG-2 TS |
  | M2V | MPEG-2 ES |
  | M4V | H.264 |
  | MOV | DV, DVCPro 50, H.261, H.263, H.264, Sorenson Video 1 |
  | MP4 | `H.264/MPEG-4` AVC |
  | MPEG | MPEG-2 SS |
  | MPG | MPEG-2 SS |
  | MTS | MPEG-2 |
  | ProRes | APCN, APCS, APCO, APCH, AP4H |
  | TS | DVCPro 50 |
  | VOB | MPEG-2 |
  | WMV/ASF | VC-1, Windows® Media Video 7, Windows® Media Video 8 |

  >[!NOTE]
  >
  >l’écran Tâches vous alerte si vous téléchargez et tentez de coder un fichier vidéo, mais que celui-ci est rejeté car il contient un codec ou un conteneur de fichiers incompatible. Pour plus d’informations, voir [Vérification des fichiers de tâche](checking-job-files.md).

## Meilleures pratiques en matière de codage de vidéo {#best-practices-for-video-encoding}

Vous trouverez ci-dessous des conseils sur les bonnes pratiques relatives au codage des fichiers vidéo sources dans Adobe Dynamic Media Classic.

<!-- THE FOLLOWINGS LINKS APPEAR TO BE DEAD AND THE CONTENT COMPLETELY LOST. THE GO URL DOESN'T EVEN WORK ANYMORE.
For advice about video encoding, see the following:

* Article: [Streaming 101: The Basics — Codecs, Bandwidth, Data Rate, and Resolution][www.adobe.com/go/learn_s7_streaming101_en](https://www.adobe.com/go/learn_s7_streaming101_en). THIS MATERIAL WAS FOUND ON A THIRD PARTY WEBSITE HERE: https://streaminglearningcenter.com/articles/streaming-101-the-basics-codecs-bandwidth-data-rate-and-resolution.html MATERIAL IS GOOD BUT DO NOT LINK TO IT
* Video: [Video Encoding Basics][www.adobe.com/go/learn_s7_encoding_en](https://www.adobe.com/go/learn_s7_encoding_en). -->

### Fichiers vidéo source {#source-video-files}

Lorsque vous codez un fichier vidéo, utilisez un fichier vidéo source ayant la plus haute qualité possible. Evitez d’utiliser des fichiers vidéo précédemment codés, car ces fichiers sont déjà compressés, et un codage supplémentaire crée une vidéo de qualité inférieure.

Le tableau suivant décrit la taille recommandée, les proportions et le débit minimal requis par vos fichiers vidéo sources lorsque vous les codez :

| Taille | Format | Débit minimum |
| --- | --- | --- |
| 1024 x 768 | 4:3 | 4 500 Kbits/s pour la plupart des vidéos. |
| 1280 x 720 | 16:9 | 3 000 : 6 000 Kbit/s, selon la quantité de mouvement dans la vidéo. |
| 1920 x 1080 | 16:9 | 6 000 : 8 000 Kbit/s, selon la quantité de mouvement dans la vidéo. |

### Obtention des métadonnées d’un fichier {#obtaining-a-file-s-metadata}

Vous pouvez obtenir les métadonnées d’un fichier en affichant ses métadonnées dans Adobe Dynamic Media Classic, à l’aide d’un outil de modification vidéo ou d’une application conçue pour obtenir des métadonnées. Vous trouverez ci-dessous des instructions sur l’utilisation de MediaInfo, une application tierce, pour obtenir les métadonnées d’un fichier vidéo :

1. Accédez à cette page Web : [https://mediaarea.net/en/MediaInfo](https://mediaarea.net/en/MediaInfo).
1. Sélectionnez et téléchargez le programme d’installation pour la version interface graphique utilisateur, puis suivez les instructions d’installation.
1. Après l’installation, cliquez avec le bouton droit sur le fichier vidéo (Windows® uniquement) et sélectionnez MediaInfo, ou ouvrez MediaInfo et faites glisser votre fichier vidéo dans l’application. Toutes les métadonnées de votre fichier vidéo, telles que sa largeur, sa hauteur et le nombre d’images par seconde, sont alors visibles à l’écran. 

### Format {#aspect-ratio}

Lorsque vous choisissez ou créez un paramètre prédéfini de codage vidéo pour votre fichier vidéo principal, assurez-vous que le paramètre prédéfini a le même format que le fichier vidéo principal. Le *format* fait référence au rapport largeur/hauteur de la vidéo.

Pour déterminer les proportions d’un fichier vidéo, obtenez les métadonnées du fichier et notez la largeur et la hauteur du fichier (voir [Obtention des métadonnées d’un fichier](uploading-encoding-videos.md#obtaining_a_file_s_metadata)). Utilisez ensuite cette formule pour déterminer le format :

Largeur / Hauteur = Rapport L/H

Ce tableau décrit la façon dont les résultats de la formule se traduisent en choix de formats :

| Résultat de la formule | Format |
| --- | --- |
| 1.33 | 4:3 |
| 0.75 | 3:4 |
| 1.78 | 16:9 |
| 0.56 | 9:16 |

Par exemple, une vidéo dont la largeur est de 1 440 × hauteur de 1 080 a un rapport d’aspect de 1440/1080, soit 1,33. Dans ce cas, vous choisissez un paramètre prédéfini de codage vidéo avec un format 4:3 pour coder le fichier vidéo.

### Débit {#data-rate}

Le *débit de données* (également appelé *débit binaire*) est la quantité de données qui est codée pour constituer une seconde de lecture vidéo. Le débit de données est mesuré en kilobits par seconde (Kbits/s).

>[!NOTE]
>
>du fait que tous les codecs utilisent la compression avec perte, le débit de données est le facteur le plus important de la qualité vidéo. Quand vous utilisez la compression avec perte, plus vous compressez la vidéo, plus la qualité de l’image se dégrade. Toutes les autres caractéristiques étant égales (résolution, taux de rafraîchissement et codec), plus le débit de données est faible, moins la qualité du fichier compressé est bonne.

Lorsque vous choisissez un paramètre prédéfini de codage vidéo, pensez à tenir compte de la vitesse de connexion de l’utilisateur final cible. Choisissez un paramètre prédéfini avec un débit de données correspondant à 80 % de cette vitesse. Par exemple, si la vitesse de connexion de l’utilisateur final est de 1 000 Kbit/s, le meilleur paramètre prédéfini est celui avec un débit de données vidéo de 800 Kbit/s.

Ce tableau décrit le débit de données de vitesses de connexion courantes.

| Vitesse (Kb/s) | Type de connexion |
| --- | --- |
| 256 | Connexion commutée. |
| 800 | Connexion mobile standard. Pour cette connexion, visez un débit de données de l’ordre de 400 Kb/s, jusqu’à 800 Kb/s pour les expériences 3G. |
| 2 000 | Connexion haut débit standard de bureau. Pour cette connexion, visez un débit de données de l’ordre de 800 à 2 000 Kb/s, bien qu’un débit de 1 200 à 1 500 Kb/s convienne à la plupart des cibles. |
| 5000 | Connexion haut débit standard. Il est déconseillé de coder dans cette fourchette supérieure, car la diffusion de la vidéo à cette vitesse n’est pas possible pour la plupart des consommateurs. |

### Résolution {#resolution}

*Resolution* décrit la hauteur et la largeur d’un fichier vidéo en pixels. La plupart des vidéos sources sont stockées à une résolution élevée (par exemple, 1920 × 1080). Pour la diffusion en continu, la vidéo source est compressée à une résolution inférieure (640 × 480 ou moins).

La résolution et le débit de données sont deux facteurs étroitement liés qui déterminent la qualité de la vidéo. Pour maintenir la même qualité vidéo, plus le nombre de pixels (c’est-à-dire la résolution) est élevé dans un fichier vidéo, plus le débit de données doit l’être également. Prenons l’exemple du nombre de pixels par image dans un fichier vidéo de résolution de 320 × 240 et d’une résolution de 640 × 480 :

| Résolution | Pixels par image |
| --- | --- |
| 320 × 240 | 76 800 |
| 640 × 480 | 307 200 |

Le fichier 640 × 480 a quatre fois plus de pixels par image. Pour obtenir le même débit de données pour ces deux exemples de résolution, vous appliquez quatre fois la compression au fichier 640 × 480, ce qui peut réduire la qualité de la vidéo. Par conséquent, un débit de données vidéo de 250 Kbit/s produit un affichage de haute qualité à une résolution de 320 × 240, mais pas à une résolution de 640 × 480.

>[!NOTE]
>
>En règle générale, plus le débit de données que vous utilisez est élevé, plus la vidéo s’affiche et plus la résolution que vous utilisez est élevée, plus le débit de données que vous devez conserver est élevé (par rapport à des résolutions plus basses).

Du fait que la résolution et le débit de données sont liés, vous avez le choix entre deux options lors du codage vidéo :

* Choisissez un débit de données, puis codez-le à la résolution la plus élevée qui s’affiche le mieux au débit de données que vous choisissez.
* Choisir une résolution, puis coder au débit de données nécessaire pour que la qualité vidéo soit optimale à la résolution choisie.

Lorsque vous choisissez (ou créez) un paramètre prédéfini de codage vidéo pour votre fichier vidéo principal, utilisez ce tableau pour cibler la résolution appropriée :

| Résolution | Hauteur (pixels) | Taille d’écran |
| --- | --- | --- |
| 240p | 240 | Ecran de très petite taille |
| 300p | 300 | Petits écrans généralement destinés aux appareils mobiles |
| 360p | 360 | Petit écran |
| 480p | 480 | Ecran de taille moyenne |
| 720p | 720 | Grand écran |
| 1080p | 1 080 | Grand écran haute définition |

### Images par seconde {#fps-frames-per-second}

Aux États-Unis et au Japon, la plupart des vidéos sont tournées à 29,97 images par seconde (i/s) ; en Europe, la plupart des vidéos sont tournées à 25 i/s. Le film est tourné à 24 FPS.

Choisissez un paramètre prédéfini de codage vidéo correspondant au débit d’images par seconde de votre fichier vidéo principal. Par exemple, si votre vidéo principale est de 25 i/s, choisissez un paramètre prédéfini de codage de 25 i/s. Par défaut, tous les encodages personnalisés utilisent le FPS du fichier vidéo principal. Pour cette raison, la spécification du paramètre FPS lors de la création d’un paramètre prédéfini de codage vidéo n’est pas nécessaire.

### Dimensions du codage vidéo {#video-encoding-dimensions}

Pour obtenir des résultats optimaux, sélectionnez les dimensions de codage de façon à ce que la vidéo source corresponde à un multiple entier de toutes vos vidéos codées.

Pour ce faire, il suffit de diviser la largeur de la source par la largeur codée pour obtenir le rapport de largeur, puis de diviser la hauteur de la source par la hauteur codée pour obtenir le rapport de hauteur.

Si le résultat est un nombre entier, cela signifie que la mise à l’échelle de la vidéo est parfaite. Si le résultat n’est pas un nombre entier, la qualité vidéo s’en ressentira en raison de la présence d’artefacts vidéo (pixels résiduels). Cet effet est plus visible lorsque la vidéo contient du texte.

Par exemple, supposons que la vidéo source soit 1 920 × 1 080. Dans le tableau ci-après, les trois vidéos codées indiquent les paramètres de codage optimaux à appliquer.

| Type de vidéo | Largeur × Hauteur | Rapport de largeur | Rapport de hauteur |
| --- | --- | --- | --- |
| Source | 1920 × 1080 | 1 | 1 |
| Codée | 960 × 540 | 2 | 2 |
| Codée | 640 × 360 | 3 | 3 |
| Codée | 480 × 270 | 4 | 4 |

### Format de fichier vidéo codé {#encoded-video-file-format}

Adobe Dynamic Media Classic recommande d’utiliser les paramètres prédéfinis de codage vidéo MP4 H.264. Comme les fichiers MP4 utilisent le codec vidéo H.264, la vidéo est de haute qualité mais dans un fichier au volume compressé.

## Utilisation des paramètres prédéfinis de codage vidéo {#working-with-video-encoding-presets}

Les fichiers vidéo Principal créés avec des équipements de production vidéo et des logiciels de montage vidéo sont souvent trop volumineux et ne sont pas dans le format approprié pour une diffusion vers des destinations en ligne. Pour convertir de la vidéo numérique afin qu’elle présente le format et les spécifications appropriés pour être lue sur divers écrans, vous pouvez *transcoder* les fichiers vidéo (processus également appelé « *codage* »). Au cours du processus de codage, la vidéo est compressée pour obtenir une taille de fichier plus petite et plus efficace. Il le fait pour une diffusion optimale sur le Web et sur les appareils mobiles.

Voir [Téléchargement et codage de vidéos](uploading-encoding-videos.md#uploading-and-encoding-videos).

Adobe Dynamic Media Classic fournit une bibliothèque de paramètres prédéfinis de codage vidéo qui reflètent les paramètres de codage les plus courants utilisés aujourd’hui. Ces paramètres ont été optimisés pour la lecture sur les écrans cibles. De plus, les administrateurs peuvent créer leurs propres paramètres prédéfinis de codage vidéo pour personnaliser la taille et la qualité de lecture des vidéos pour les utilisateurs. Tous les paramètres prédéfinis de codage vidéo, qu’ils soient prêts à l’emploi d’Adobe Dynamic Media Classic ou personnalisés, génèrent une vidéo au format de fichier MP4.

Sur l’écran Paramètres vidéo prédéfinis, les administrateurs peuvent configurer et gérer le codage vidéo. Ils peuvent effectuer les opérations suivantes :

* activer et désactiver les paramètres vidéo prédéfinis ;
* créer un paramètre prédéfini de codage vidéo ;
* modifier les paramètres prédéfinis de codage vidéo ;
* Suppression de paramètres vidéo prédéfinis.

Toute vidéo que vous chargez vers Adobe Dynamic Media Classic ou que vous codez dans Adobe Dynamic Media Classic est traitée comme une &quot;vidéo&quot;. En d’autres termes, ce mode de classification des fichiers signifie que vous pouvez diffuser la vidéo à des fins de lecture sur des ordinateurs de bureau, des appareils mobiles, ou les deux. Vous pouvez, par exemple, prévisualiser ces types de vidéos dans Adobe Dynamic Media Classic. Vous pouvez également générer des URL (à l’aide de la fonction Copier l’URL) et du code que vous pouvez incorporer (à l’aide de la fonction Intégrer le code) pour l’utiliser avec les lecteurs vidéo, sur les sites web, etc.

Voir [Prévisualisation de vidéos dans une visionneuse de vidéos](previewing-videos-video-viewer.md#previewing-videos-in-a-video-viewer).

Voir [Lier une URL de vidéo à un site mobile ou à un site web](deploying-video-websites-mobile-sites.md#linking-a-video-url-to-a-mobile-site-or-a-website).

Voir [Incorporation de la visionneuse de vidéos dans une page web](deploying-video-websites-mobile-sites.md#embedding-the-video-viewer-on-a-web-page).

Pour les ressources vidéo que vous chargez et codez dans Adobe Dynamic Media Classic, la vidéo est diffusée au format de fichier suivant :

**MP4 H.264** Utilisez des fichiers MP4 pour les opérations suivantes :

* Diffusion en flux continu dynamique HTTP sur les ordinateurs de bureau.
* HLS (HTTP Live Streaming, protocole de diffusion en continu Apple).
* Diffusion vidéo progressive sur des appareils mobiles Android™, BlackBerry® et Windows®.

Tout autre format vidéo et codec est traité comme une &quot;vidéo de Principal&quot;. Ce mode de classification des fichiers signifie que la vidéo est un fichier vidéo source non prévu pour la lecture vidéo sur des périphériques de bureau ou des périphériques mobiles. Par exemple, vous ne pouvez pas prévisualiser ces types de vidéos dans Adobe Dynamic Media Classic. Vous ne pouvez pas générer d’URL de copie ou de code intégré à utiliser dans des lecteurs vidéo, sur des sites web, etc.

### Filtrage de la liste des paramètres prédéfinis de codage vidéo {#filtering-the-list-of-video-encoding-presets}

La page Paramètres vidéo prédéfinis et la page Paramètres vidéo prédéfinis adaptatifs se composent d’un tableau répertoriant l’état actif, le nom du paramètre prédéfini, le périphérique de lecture prévu, la taille de la vidéo et le débit de données de chaque paramètre vidéo prédéfini.

Vous pouvez affiner la liste en choisissant le filtrage Les deux, Actif ou Inactif, pour afficher tous les paramètres vidéo prédéfinis ou restreindre la liste aux paramètres actifs ou inactifs.

Vous pouvez également les filtrer en fonction d’une option de périphérique de lecture afin de restreindre la liste aux paramètres vidéo prédéfinis conçus pour la lecture de vidéos sur tous les appareils, sur les ordinateurs de bureau, les appareils mobiles ou les tablettes.

**Pour filtrer la liste des paramètres prédéfinis de codage vidéo :**

1. Dans Adobe Dynamic Media Classic, sur la barre de navigation globale, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Paramètres vidéo prédéfinis]** > **[!UICONTROL Paramètres vidéo prédéfinis adaptatifs]** ou **[!UICONTROL Paramètres prédéfinis de codage uniques]**.

   Les pages des paramètres prédéfinis de vidéo adaptative et de codage unique incluent un tableau qui répertorie l’état actif, le nom du paramètre prédéfini, le périphérique de lecture prévu, les dimensions vidéo et le débit de données de chaque paramètre prédéfini vidéo.

1. Sur la page Paramètres prédéfinis de codage uniques intitulée Paramètres vidéo prédéfinis, sur la barre d’outils Paramètres vidéo prédéfinis, utilisez les deux listes déroulantes pour affiner la liste des paramètres prédéfinis dans le tableau en fonction de l’état Actif et du périphérique de lecture.

   * Dans la première, une liste déroulante restreinte, sélectionnez **[!UICONTROL Les deux]** pour afficher tous les paramètres vidéo prédéfinis ou choisissez **[!UICONTROL Actif]** ou **[!UICONTROL Inactif]** pour restreindre la liste aux paramètres actifs ou inactifs.
   * Dans la deuxième, une liste déroulante plus étendue, sélectionnez une option de périphérique de lecture pour restreindre la liste aux paramètres vidéo prédéfinis destinés à lire des vidéos sur les ordinateurs de bureau, sur les appareils mobiles ou sur les tablettes.

### Activation ou désactivation des paramètres prédéfinis de codage vidéo {#activating-or-deactivating-video-encoding-presets}

Les paramètres vidéo prédéfinis activés sont répertoriés dans la boîte de dialogue Télécharger les options de la tâche. La boîte de dialogue s’affiche lorsqu’un utilisateur charge des fichiers vidéo au cours du processus de chargement. Ils peuvent choisir parmi une liste de tous les paramètres prédéfinis de codage activés.

1. Dans Adobe Dynamic Media Classic, sur la barre de navigation globale, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Paramètres vidéo prédéfinis]**.
1. Effectuez l’une des opérations suivantes :

   * Sélectionnez **[!UICONTROL Paramètres prédéfinis de vidéo adaptative]**.
   * Sélectionnez **[!UICONTROL Paramètres prédéfinis de codage uniques]**.

1. Effectuez l’une des opérations suivantes :

   * Pour activer un paramètre vidéo prédéfini, dans la page des paramètres prédéfinis, sous la colonne Actif, cochez la case en regard d’un nom de paramètre prédéfini.
   * Pour désactiver un paramètre vidéo prédéfini, désélectionnez la case en regard du paramètre vidéo prédéfini que vous souhaitez rendre inactif.

     >[!NOTE]
     >
     >Les paramètres vidéo prédéfinis inactifs ne sont pas répertoriés dans la boîte de dialogue Télécharger les options de la tâche.

1. Dans le coin inférieur droit de la page, sélectionnez **[!UICONTROL Fermer]**.

### Ajout ou modification d’un paramètre prédéfini de codage vidéo {#adding-or-editing-a-video-encoding-preset}

Vous pouvez créer vos propres paramètres vidéo prédéfinis personnalisés à codage unique et les ajouter au tableau Paramètres vidéo prédéfinis. Vous pouvez également modifier les paramètres vidéo prédéfinis de codage unique fournis avec Adobe Dynamic Media Classic, à condition que vous ayez enregistré le paramètre prédéfini modifié sous un nouveau nom.

Adobe Dynamic Media Classic a défini des limites maximales sur le débit de données cible, la hauteur de résolution et la largeur de résolution afin de garantir une expérience de lecture correcte. Des messages d’avertissement s’affichent si vous dépassez ces limites, qui sont les suivantes :

* Pour la lecture sur ordinateur, les limites sont : (Largeur/16) &#42; (Hauteur/16) &lt; 8192.
* Pour la lecture sur appareil mobile, les limites sont : (Largeur/16) &#42; (Hauteur/16) &lt; 660 ; débit cible &lt; 4 000.
* Pour la lecture sur tablette, les limites sont : (Largeur/16) &#42; (Hauteur/16) &lt; 3 600.

**Pour ajouter ou modifier un paramètre prédéfini de codage vidéo :**

1. Dans Adobe Dynamic Media Classic, sur la barre de navigation globale, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Paramètres vidéo prédéfinis]**.
1. Sélectionnez **[!UICONTROL Paramètres prédéfinis de codage uniques]**.
1. Sur la page Paramètres vidéo prédéfinis, procédez de l’une des manières suivantes :

   * Dans la barre d’outils Paramètres vidéo prédéfinis, sélectionnez **[!UICONTROL Ajouter]** pour pouvoir ajouter un paramètre vidéo prédéfini.
   * Sélectionnez un paramètre vidéo prédéfini. Dans la barre d’outils, sélectionnez **[!UICONTROL Modifier]**.

     Vous ne pouvez pas modifier les paramètres prédéfinis Adobe Dynamic Media Classic ; vous pouvez uniquement créer un paramètre prédéfini à partir d’un paramètre existant en choisissant **[!UICONTROL Enregistrer sous]**.

1. Dans la page Ajout d’un paramètre vidéo prédéfini ou Modification d’un paramètre vidéo prédéfini, définissez les options Paramètres vidéo prédéfinis dont vous avez besoin.

   Voir [Meilleures pratiques en matière de codage de vidéo](uploading-encoding-videos.md#best-practices-for-video-encoding) pour connaître les paramètres recommandés.

   | Option de paramètres vidéo prédéfinis | Description |
   | --- | --- |
   | Nom du paramètre prédéfini | Entrez un nom descriptif pour le paramètre vidéo prédéfini. Le nom que vous indiquez est visible dans la boîte de dialogue Télécharger les options de la tâche, où les utilisateurs choisissent les options de transcodage. |
   | Description | Décrivez le paramètre vidéo prédéfini. Ce que vous saisissez apparaît sous forme d’info-bulle. Lorsque les utilisateurs choisissent des options de transcodage, l’info-bulle s’affiche lorsqu’ils déplacent le pointeur sur le nom du paramètre prédéfini dans la boîte de dialogue Télécharger les options de la tâche. |
   | Périphérique de lecture | Choisissez le périphérique sur lequel il est prévu que la vidéo soit lue. Les options disponibles sont Ordinateur (ordinateurs de bureau), Mobile (iPhone, iPad, Android™) ou Tablette (iPad uniquement). Ce paramètre détermine automatiquement le codec vidéo et audio approprié utilisé lors du codage. |
   | Débit de la cible | Entrez la vitesse de connexion Internet moyenne (en kilobits par seconde) de l’utilisateur final cible. Vous pouvez saisir le débit ou faire glisser le curseur pour le saisir. Le spectre de vitesse de connexion de l’utilisateur répertorie les vitesses attendues pour les connexions haut débit, DSL, mobiles et à ligne commutée. Ce paramètre détermine automatiquement le débit combiné de données audio et vidéo, autrement dit, la quantité de données qu’il est nécessaire de coder pour produire une seule seconde de lecture vidéo. Plus le débit binaire est élevé, meilleure est la qualité de la vidéo produite. Cependant, un débit de données trop élevé se traduit par des fichiers de taille très importante, ce qui peut altérer l’expérience de visionnage pour les utilisateurs qui ne disposent pas d’une connexion avec une bande passante aussi large. Il est préférable d’essayer d’équilibrer ces deux facteurs Essayez de créer une expérience de lecture de qualité adéquate sans aliéner les utilisateurs ayant des largeurs de bande limitées. |
   | Format | Le format est le rapport largeur/hauteur de la vidéo. Les deux premières proportions répertoriées ci-dessous sont souvent utilisées pour afficher la vidéo horizontalement :<ul><li> 4:3: Utilisé pour presque tous les contenus de diffusion TV à définition standard.</li><li>16:9: Utilisé pour presque tout le contenu et les films grand écran sur la télévision haute définition (HDTV).</li><li>Mise à l’échelle automatique : (valeur par défaut) paramètre prédéfini de codage unique qui fonctionne avec n’importe quel format pour créer des vidéos à diffuser sur mobile, tablette et ordinateur de bureau. Les vidéos source transférées qui sont codées à l’aide de ce paramètre prédéfini sont définies avec une hauteur fixe. Toutefois, la largeur est automatiquement mise à l’échelle afin de préserver les proportions de la vidéo (rapport largeur/hauteur).</li><li>Personnalisé : utilisé lorsque vous souhaitez définir une taille de vidéo non standard.</li><li>Les proportions que vous choisissez déterminent les paramètres de largeur et de hauteur pour la taille de résolution ; la largeur et la hauteur sont automatiquement mises à l’échelle selon les proportions appropriées.</li></ul> |
   | Taille de résolution | La taille de résolution, exprimée en nombre de pixels de large par le nombre de pixels de haut, détermine la taille. Saisissez une largeur et une hauteur en pixels ou faites glisser le curseur pour entrer ces valeurs. Le spectre des résolutions répertorie les tailles de résolution les plus utilisées. La valeur de largeur et la valeur de hauteur correspondent automatiquement aux proportions que vous avez sélectionnées. Par exemple, si vous sélectionnez 4:3 comme format et saisissez 400 pour la largeur, 300 est automatiquement renseigné pour la hauteur. Si vous avez sélectionné Mise à l’échelle automatique pour le paramètre Format, la valeur Largeur de la résolution est automatiquement définie sur Auto. Sélectionnez **[!UICONTROL Aperçu]** afin que vous puissiez ouvrir une fenêtre de navigateur et y voir vos choix de résolution. |
   | Encoder un suffixe de fichier | Entrez un suffixe. Ce suffixe est ajouté au fichier vidéo encodé résultant. Vous pouvez entrer un trait d’union et un trait de soulignement dans le nom, mais les espaces et les caractères spéciaux ne sont pas autorisés. |
   | Autres paramètres | Adobe Dynamic Media Classic détermine automatiquement tous les autres paramètres de codage, conformément aux bonnes pratiques en matière de codage. |

1. Effectuez l’une des opérations suivantes :

   * Sélectionnez **[!UICONTROL Enregistrer]** si vous avez ajouté ou modifié un paramètre vidéo prédéfini.
   * Sélectionnez **[!UICONTROL Enregistrer sous]** si vous avez ajouté un paramètre vidéo prédéfini à partir d’un paramètre prédéfini existant.

### Suppression d’un paramètre prédéfini de codage vidéo {#delete-a-video-encoding-preset}

Les administrateurs peuvent supprimer des paramètres vidéo prédéfinis personnalisés. Les paramètres vidéo prédéfinis fournis avec Adobe Dynamic Media Classic ne peuvent pas être supprimés.

1. Dans Adobe Dynamic Media Classic, sur la barre de navigation globale, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Paramètres vidéo prédéfinis]**.
1. Sélectionnez **[!UICONTROL Paramètres prédéfinis de codage uniques]**.
1. Sur la page Paramètres vidéo prédéfinis, sélectionnez dans le tableau un paramètre vidéo prédéfini dont vous n’avez plus besoin.
1. Dans la barre d’outils Paramètres vidéo prédéfinis, sélectionnez **[!UICONTROL Supprimer]**.
1. Dans la boîte de dialogue Supprimer le paramètre prédéfini, sélectionnez **[!UICONTROL Supprimer]**.

>[!MORELIKETHIS]
>
>* [Démarrage rapide : vidéo dans Adobe Dynamic Media Classic](quick-start-video.md#quick-start-video)
>* [Télécharger et coder des vidéos](uploading-encoding-videos.md#uploading-and-encoding-videos)
>* [Utilisation de paramètres prédéfinis de visionneuse vidéo](previewing-videos-video-viewer.md#working-with-video-viewer-presets)
>* Vidéo de formation [Paramètres vidéo prédéfinis](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS)
