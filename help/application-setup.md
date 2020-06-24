---
title: Configuration de l’application
seo-title: Configuration de l’application
description: Découvrez comment configurer la zone d’application de Dynamic Media Classic.
seo-description: Découvrez comment configurer la zone d’application de Dynamic Media Classic.
uuid: 3e2f1d30-8f33-4a9d-bbe4-e8c3dbc968f8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: ae2d1895-a437-4463-bfac-3960c8027551
translation-type: tm+mt
source-git-commit: 74238f90f45f0fb9a4566915a20a1d41dfb69fe1
workflow-type: tm+mt
source-wordcount: '11120'
ht-degree: 71%

---


# Configuration de l’application{#application-setup}

Vous pouvez utiliser les pages Configuration de l’application pour saisir des paramètres généraux, créer des paramètres d’image prédéfinis, des paramètres prédéfinis de codage vidéo, des paramètres prédéfinis de visionneuse ou définir des visionneuses par défaut et des métadonnées. Vous pouvez également configurer les paramètres prédéfinis d’ensemble par lot afin d’automatiser la génération de visionneuses à 360° 2D (par exemple), des paramètres de publication et des paramètres d’optimisation du référencement de la vidéo.

>[!NOTE]
>
>seuls les administrateurs Scene7 Publishing System sont habilités à modifier les paramètres des pages Configuration de l’application.

## Paramètres généraux {#general-settings}

Pour ouvrir la page Paramètres généraux de l’application, sur la barre de navigation globale, cliquez sur **[!UICONTROL Configuration > Configuration de l’application > Paramètres généraux]**.

### Serveurs

Lors de la création de compte, Dynamic Media Classic fournit automatiquement les serveurs affectés à votre société. Ces serveurs sont utilisés pour créer des chaînes URL pour votre site Web et vos applications. Ces appels d’URL sont spécifiques à votre compte.

Voir aussi [Test du service Secure Testing](testing-assets-making-them-public.md#testing_the_secure_testing_service).

**Nom** du serveur publié Ce serveur est le serveur CDN actif utilisé dans tous les appels d’URL générés par le système et spécifiques à votre compte. Ne modifiez pas ce nom de serveur à moins que vous ne soyez invité à le faire par un technicien de l’assistance technique Dynamic Media Classic.

**Nom** du serveur d&#39;Origines Ce serveur est utilisé uniquement pour les tests d&#39;assurance qualité. Ne changez pas le nom de ce serveur, sauf si un technicien de l’assistance technique Dynamic Media Classic vous le demande.

**Nom** du serveur AGM Ce serveur est utilisé pour les modèles Web-to-Print. Ce serveur est défini à l’échelle de l’entreprise. Ne changez pas le nom de ce serveur, sauf si un technicien de l’assistance technique Dynamic Media Classic vous le demande.

**Test&amp;Cible Server attribue un nom** à votre URL Test&amp;Cible, jusqu’à .com compris. Pour plus d’informations sur l’obtention de cette URL, voir Intégration de Dynamic Media Classic à Cible Classic.

**Nom** du serveur de flux continu iOS URL de votre serveur de flux continu iOS Dynamic Media Classic. Ce serveur permet de proposer des vidéos en flux continu sur les périphériques iOS à l’aide du protocole HTTP.

**Nom** du serveur de vidéo progressive URL de votre serveur de vidéo progressive Dynamic Media Classic. Ce serveur permet de proposer des vidéos progressives à l’aide du protocole HTTP.

**Afficher l’URL des fichiers** non publiés Sélectionnez cette option si vous souhaitez que Dynamic Media Classic affiche une URL lors de la prévisualisation d’un fichier, qu’il soit publié ou non. Si le fichier n’est pas publié, l’URL ne fonctionne pas. Vous pouvez, cependant, utiliser l’URL à des fins de planification ou d’organisation.

**Autoriser l’installation** d’AIR Sélectionnez cette option pour permettre aux utilisateurs de télécharger la version de bureau de Scene7 Publishing System sur leur disque dur local. Les utilisateurs peuvent installer l’application à partir de la zone Version de bureau de l’écran Configuration personnelle.

Les utilisateurs d’AIR peuvent désinstaller manuellement leur application existante et effectuer une réinstallation à partir de la version en ligne de Scene7 Publishing System (sous Paramètres personnels). Après cette réinstallation unique, vous êtes invité à effectuer une mise à niveau lorsque le serveur dispose d’une version plus récente de Scene7 Publishing System AIR. Scene7 Publishing System est intégré dans Application Update Framework qui simplifie le processus de mise à niveau.

**Modèle** d’invalidation CDN Indique le modèle utilisé pour invalider le cache CDN (Content Diffusion Network).

For example, suppose you enter an image URL (including image presets or modifiers) referencing `<ID>`, instead of a specific image ID as in the following example:

`https://sample.scene7.com/is/image/Company/<ID>?$s7product$`

If the Template just contains `<ID>`, then SPS fills in the `https://<server>/is/image`, where `<server>` is the Publish Server Name that is defined in General Settings.

Si vous définissez le modèle CDN Invalidate, que vous sélectionnez une image nommée Backpack_B, puis que vous cliquez sur **Fichier** > **Invalider sur le réseau de diffusion de contenu**, l’URL suivante est générée dans l’interface de CDN Invalidate :

`https://sample.scene7.com/is/image/Company/Backpack_B?$s7product$`

Dans la zone de la liste des URL, cliquez sur **Continuer** pour effacer la mémoire cache de cet appel d’URL d’image spécifique. Notez que vous pouvez également ajouter des URL en les saisissant ou en les collant dans la zone de la liste des URL ; vous n’avez pas besoin de définir le modèle au préalable.

Une fois le modèle d’invalidation sur le réseau de diffusion de contenu sélectionné et une demande d’invalidation sur le réseau de diffusion de contenu effectuée, un indicateur s’affiche dans l’interface utilisateur et donne une évaluation du temps nécessaire pour effacer le cache.

De même, si plusieurs images sont sélectionnées dans SPS lorsque vous cliquez sur **Fichier** > **Invalider sur le réseau de diffusion de contenu**, chaque image est référencée dans l’URL modèle enregistrée. Par conséquent, vous pouvez définir un modèle CDN Invalidate référençant chaque URL référencée sur votre site Web (comme le détail d’un produit, les résultats de recherche, et ainsi de suite). Ensuite, lorsque vous sélectionnez une ou plusieurs images pour invalidation à partir du cache, les URL renseignent automatiquement l’interface.

Voir [Mise en cache du contenu](scene7-platform-overview.md#content_caching).

Voir [Fichiers republiés et délais CDN](publishing-files.md#republished_assets_and_cdn_delays).

**Parcourir**

**Afficher les projets** Détermine si des projets sont disponibles pour organiser vos ressources Dynamic Media Classic. (voir Organisation de votre travail avec des projets).

**Afficher l’exemple de contenu** eVideo Activez ou désactivez l’affichage de l’exemple de contenu eVideo.

**Afficher le contenu** généré Dans les dossiers, affiche le contenu généré à partir d’un fichier. Par exemple, lorsqu’un fichier PDF est pixellisé au moment du téléchargement, Dynamic Media Classic crée une image pour chaque page du fichier PDF d’origine. Si cette option est sélectionnée, chaque image générée au moment du téléchargement du fichier PDF original apparaît aux côtés du fichier PDF dans le dossier où il a été téléchargé.

**Afficher les vidéos** codées désélectionnées (désactivées) par défaut.

Pour rechercher rapidement des vidéos dans Scene7 Publishing System sans avoir à parcourir de nombreux dérivés codés de la même vidéo, ne désélectionnez pas cette option (par défaut). Seule la miniature de la vidéo originale, qui est la vidéo source que vous avez téléchargée et utilisée pour créer tous les dérivés, et seule la miniature de la visionneuse de vidéos adaptative « parent », qui contient tous les dérivés « enfants » de la visionneuse de vidéos codées, sont affichées dans l’interface utilisateur.

Il est toujours possible d’accéder à des vidéos codées individuelles à partir de la vidéo originale ou de la visionneuse de vidéos adaptatives. Pour ce faire, double-cliquez sur l’image miniature de la vidéo pour passer en mode Affichage des détails. Cliquez ensuite sur **Vidéos codées** dans le panneau droit pour accéder à l’intégralité des vidéos « enfants ».

Vous pouvez également utiliser la commande **Fichier > Retraiter** pour créer d’autres vidéos codées « enfants » directement depuis une visionneuse de vidéos adaptatives. Scene7 Publishing System recherche automatiquement la vidéo originale « parent » de la visionneuse de vidéos adaptatives et l’utilise comme source vidéo pour le transcodage. Cependant, lorsque vous enregistrez les nouvelles vidéos codées individuelles, elles ne sont pas visibles lors d’une recherche ou d’une navigation. Elles restent néanmoins accessibles à partir de l’onglet Vidéos codées dans la vue Affichage des détails.

Voir [Téléchargement et transcodage vidéo](uploading-encoding-videos.md#uploading_and_encoding_videos).

Pour continuer à accéder à toutes les vidéos codées dérivées lors d’une recherche ou d’une navigation, sélectionnez **Afficher les vidéos codées**.

Certaines actions du menu Créer ne fonctionnent qu’avec des vidéos individuelles. C’est la raison pour laquelle il est nécessaire d’afficher toutes les vidéos codées dérivées pouvant être sélectionnées, quelle que soit la façon dont vous définissez le paramètre **Afficher les vidéos codées**. The Build actions that over-ride the **Show Encoded Videos** setting include **Adaptive Video Sets**, and **eCatalogs**.

>[Note]
>
>Si vous n’avez pas utilisé Scene7 Publishing System pour télécharger et coder vos fichiers vidéo, Dynamic Media Classic affiche toutes vos vidéos codées individuelles, même si cette option est désélectionnée.

**Afficher le bouton** Actualiser les sous-dossiers Active ou désactive l&#39;affichage du bouton Actualiser des sous-dossiers.

**Compte FTP Dynamic Media Classic**

**Le serveur** Liste votre serveur de compte FTP.

**Nom** d’utilisateur Liste le nom d’utilisateur de votre compte FTP.

**Télécharger dans l’application**

**Ecraser les images** Dynamic Media Classic ne permet pas à deux fichiers d’avoir le même nom. L’identifiant Scene7 Publishing System de chaque élément (le nom de l’image sans l’extension de fichier) doit être unique. De par cette règle, la boîte de dialogue Télécharger contient une option Ecraser. L’effet précis de cette option dépend de l’option Ecraser les images spécifiée. Ces options spécifient la manière dont les images de remplacement sont téléchargées : elles peuvent remplacer les images d’origine ou devenir des doublons. Lorsqu’un doublon est créé, le suffixe « -1 » est ajouté au nom de l’image d’origine. Par exemple, le nom chaise.tif devient chaise-1.tif pour le doublon. Ces options affectent les images téléchargées dans un dossier autre que le dossier d’origine ou les images dont l’extension est différente de celle du fichier d’origine (telle que JPG, TIF ou encore PNG) (voir Utilisation de l’option Ecraser les images).

**Ecraser dans le dossier actuel, même nom/même extension d’image de base**

Cette règle de remplacement est la plus stricte. Elle nécessite que vous téléchargiez l’image de remplacement dans le même dossier que l’image d’origine, et qu’elle ait la même extension que le fichier d’origine. Si ces conditions ne sont pas remplies, un doublon est créé.

**Ecraser dans le dossier actuel, même nom de fichier de base sans tenir compte de l’extension**

Cette règle nécessite que vous téléchargiez l’image de remplacement dans le même dossier que l’image d’origine, mais l’extension peut être différente de celle du fichier d’origine. Par exemple, chaise.tif peut remplacer chaise.jpg.

**Ecraser dans n’importe quel dossier, même nom/extension de fichier de base**

Cette règle nécessite que l’image de remplacement ait la même extension que l’image d’origine (par exemple, chaise.jpg peut remplacer uniquement chaise.jpg et non chaise.tif). Vous pouvez toutefois télécharger l’image de remplacement dans un dossier différent de celui de l’image d’origine. L’image mise à jour se trouve dans le nouveau dossier, et le fichier d’origine n’est plus disponible à l’emplacement d’origine.

**Ecraser dans un dossier, même nom de fichier, extension indépendante**

Cette règle de remplacement est la plus permissive. Elle vous permet de télécharger une image de remplacement dans un dossier autre que celui de l’image d’origine, de télécharger un fichier dont l’extension est différente de celle du fichier d’origine et de remplacer le fichier d’origine. Si le fichier d’origine se trouve dans un dossier différent, l’image de remplacement est enregistrée dans le dossier où elle a été téléchargée.

**Conserver la publication** Indique si une image de remplacement téléchargée dans Dynamic Media Classic conserve le paramètre Prêt à publier de l’image qu’elle remplace ou si le paramètre est spécifié lors du téléchargement.

**Profils** de couleurs par défaut Indique les profils de couleurs appliqués dans le cadre des options de Profil de couleurs par défaut lors de l’ajout d’images CMJN.

**Options** de téléchargement par défaut Ouvre la boîte de dialogue Télécharger les options de la tâche, dans laquelle vous pouvez spécifier les options de téléchargement par défaut. Pour plus d’informations sur ces options, voir Options de téléchargement.

**Editeur de zone cliquable, vers l’application**

**HREF** de mappage d’images par défaut Définit l’URL par défaut utilisée pour la colonne HREF de mappage d’images. Il s’agit de l’URL par défaut qui apparaît lorsque vous créez des zones cliquables.

**Modèle** de mappage d’images par défaut Définit le script JavaScript par défaut pour le modèle HREF de mappage d’images. Vous pouvez également définir un code personnalisé à exécuter chaque fois que vous cliquez sur une zone cliquable.

**Autres paramètres, vers l’application**

**La corbeille peut nettoyer les avertissements** Les fichiers de la corbeille sont automatiquement supprimés dans les sept jours. Sélectionnez « Envoyer des e-mails avant la suppression automatique des éléments de la corbeille » si vous voulez que des notifications soient envoyées aux administrateurs des entreprises quatre jours avant la suppression définitive d’éléments situés dans la corbeille. (Voir Gestion du dossier Corbeille).

## Utilisation de l’option Écraser les images {#using-the-overwrite-images-option}

Dynamic Media Classic n’autorise pas deux fichiers portant le même nom. L’identifiant Scene7 Publishing System de chaque élément (le nom de l’image sans l’extension de fichier) doit être unique. De par cette règle, la boîte de dialogue Télécharger contient des options Ecraser les images. L’effet précis de cette option dépend de l’un des paramètres internes de Scene7 Publishing System pour chaque entreprise.

Si vous avez précédemment téléchargé des images, puis modifié les fichiers d’origine (ou les avez remplacés), l’option Ecraser sélectionnée indique comment Dynamic Media Classic remplace les images. Aucune donnée sur l’image ne change, mais la nouvelle image remplace l’ancienne. Si le dossier contient également des images qui ne se trouvent pas encore dans Dynamic Media Classic, ces images sont ajoutées.

Utilisez cette option si les images que vous avez téléchargées ont été modifiées d’une façon ou d’une autre (retouchées, par exemple), mais que la référence à l’image reste inchangée. L’écrasement se révèle particulièrement utile lorsque des fichiers Adobe® PDF sont téléchargés puis extraits. To fine-tune how Dynamic Media Classic *rips* the image, adjust the ICC color profile options in the Upload dialog box and re-upload using the Overwrite feature.

Les identifiants Dynamic Media Classic utilisés pour accéder aux images à partir des serveurs de production proviennent des noms de fichier des images. L’utilisation de caractères majuscules et minuscules dans le nom de fichier est importante, tant pour le remplacement de fichiers existants que pour les ID Dynamic Media Classic utilisés pour accéder à l’image. Assurez-vous que l’utilisation de caractères majuscules et minuscules dans les noms de fichier est correcte avant de procéder au téléchargement dans Dynamic Media Classic pour éviter que les ID Dynamic Media Classic ne diffèrent que par la casse de la même image.

Si vous désactivez cette option, toutes les images dont les noms sont identiques à des images existantes sont considérées comme des doublons et ne sont donc pas ajoutées.

## Paramètres d’image prédéfinis {#image-presets}

L’écran Paramètres d’image prédéfinis sert à créer et à modifier les paramètres d’image prédéfinis. Les paramètres d’image prédéfinis permettent à Dynamic Media Classic de diffuser des images de manière dynamique à des tailles différentes à partir de la même image originale. Chaque paramètre d’image prédéfini forme un ensemble prédéfini de commandes de dimensionnement et de formatage permettant d’afficher les images. Lorsque vous créez un paramètre d’image prédéfini, vous choisissez une taille pour la diffusion des images. Vous devez également sélectionner les commandes de formatage pour optimiser l’aspect de l’image lors de sa diffusion.

Les administrateurs peuvent créer des paramètres prédéfinis pour l’exportation de fichiers. Les utilisateurs peuvent choisir un paramètre prédéfini au moment de l’exportation des images, qui reformate également les images selon les spécifications définies par l’administrateur.

To open the Image Preset screen, on the Global Navigation bar, click **Setup** > **Image Presets**.

Voir Images [](https://helpx.adobe.com/experience-manager/6-3/assets/using/imaging-faq.html)intelligentes.

### Création et modification de paramètres d’image prédéfinis {#creating-and-editing-image-presets}

1. Cliquez sur **Configuration** > **Paramètres d’image prédéfinis**.
1. Créez un paramètre prédéfini à partir d’un paramètre existant :
   * **Création d’un paramètre** d’image prédéfini - Cliquez sur **Ajouter**.
   * **Création d’un paramètre d’image prédéfini à partir d’un paramètre** existant : sélectionnez le paramètre d’image prédéfini qui ressemble le plus à celui que vous souhaitez créer, puis cliquez sur Modifier.

1. Sur l’écran Ajouter un paramètre prédéfini ou Modifier le paramètre prédéfini, attribuez un nom au paramètre prédéfini.
1. Définissez les options de paramètres prédéfinis de votre choix. 

   Voir [Options des paramètres d’image prédéfinis](application-setup.md#image_preset_options).

1. Click **Save**, or if you started from an existing preset, click **Save As**.
1. To preview the preset with your own image, click **Browse** and then select an image. To preview with the default image, click **Reset**.

Pour modifier un paramètre d’image prédéfini, sélectionnez son nom dans l’écran Paramètres d’image prédéfinis, puis cliquez sur Modifier. Pour supprimer un paramètre d’image prédéfini, sélectionnez-le, puis cliquez sur Supprimer.

### Options des paramètres d’image prédéfinis {#image-preset-options}

Les écrans Ajouter un paramètre prédéfini et Modifier le paramètre prédéfini mettent à votre disposition les options suivantes pour créer et modifier les paramètres d’image prédéfinis :

**Nom** du paramètre prédéfini Saisissez un nom descriptif sans espaces. Ajoutez la spécification de taille de l’image dans le nom pour permettre aux utilisateurs d’identifier ce paramètre d’image prédéfini.

**Largeur et Hauteur** Saisissez en pixels la taille de diffusion de l’image.

**Format** Choisissez un format dans le menu. Le choix du format GIF, JPEG, PDF ou TIFF apporte des options supplémentaires :

* Options Quantification de couleurs GIF

   **Type**

   Choisissez Adaptatif (par défaut), Web ou Macintosh. Si vous choisissez GIF avec Alpha, l’option Macintosh® n’est pas disponible.

   **Juxtaposition**

   Sélectionnez Diffus ou Non.

   **Nombre de couleurs**

   Faites glisser le curseur pour entrer une valeur comprise entre 2 et 255.

   **Liste de couleurs**

   Entrez une liste séparée par des virgules. Par exemple, pour le blanc, le gris et le noir, entrez 000000,888888,ffffff.

* Options JPEG

   **Qualité**

   Contrôle le niveau de compression JPEG. Ce paramètre affecte à la fois la taille du fichier et la qualité de l’image. L’échelle de qualité JPEG est de 1 à 100.

   **Activer la réduction de la chrominance JPEG**

   Comme l’œil humain est moins sensible aux données chromatiques à fréquence élevée qu’à la luminance à fréquence élevée, les images JPEG divisent les informations graphiques en composantes de luminance et de couleur. Lorsqu’une image JPEG est compressée, la composante de luminance conserve sa pleine résolution, tandis que les composantes de couleur sont sous-échantillonnées par interpolation, c’est-à-dire le calcul de la moyenne de groupes de pixels. La réduction de résolution (sous-échantillonnage) réduit de moitié ou d’un tiers le volume de données, quasiment sans nuire à la qualité perceptible par l’œil humain. La réduction de résolution ne s’applique pas aux images en niveaux de gris. Cette technique réduit le niveau de compression nécessaire pour les images présentant un contraste élevé (par exemple, les images contenant du texte superposé).

* Options PDF et TIFF

   **Compression**

   Choisissez un algorithme de compression.

**Espace colorimétrique** Choisissez un espace colorimétrique.

**Accentuation** Sélectionnez l’option Activer l’accentuation simple pour appliquer un filtre d’accentuation de base à l’image après toute mise à l’échelle. L’accentuation peut compenser le flou produit lors de l’affichage d’une image à une taille différente. 

Pour plus de détails sur l’accentuation, les modes de ré-échantillonnage et le masquage flou, voir [Accentuation d’une image](sharpening-image.md#sharpening_an_image).

**Mode** de ré-échantillonnage Choisissez une option de mode de ré-échantillonnage. Les options suivantes permettent d’accentuer l’image lorsque sa résolution est réduite :

**B-Linéaire** La méthode de rééchantillonnage la plus rapide ; certains artefacts de crénelage sont visibles.

**Bi-Cubique** augmente l’utilisation du processeur sur le serveur Image Server, mais produit des images plus nettes avec des artefacts de crénelage moins visibles.

**Sharp2** peut produire des résultats légèrement plus nets que l’option Bi-Cubique, mais à un coût CPU encore plus élevé sur le serveur Image Server.

**Tri-linéaire** utilise des résolutions plus élevées et plus basses, le cas échéant ; recommandé uniquement lorsque le crénelage est un problème. Elle réduit la taille du fichier JPEG en raison des données à haute fréquence réduites.

**Masquage flou** Choisissez les options suivantes pour affiner l’accentuation :

**Montant** Contrôle le degré de contraste appliqué aux pixels de contour. La valeur par défaut est de 1. Pour des images à haute résolution, vous pouvez l’augmenter jusqu’à 5. Imaginez la quantité comme étant l’unité de mesure de l’intensité du filtre.

**Rayon** Détermine le nombre de pixels entourant les pixels de contour qui affectent l’accentuation. Pour les images à haute résolution, entrez une valeur comprise entre 1 et 2. Une valeur faible renforce uniquement les pixels de contour, tandis qu’une valeur élevée traite une plus large bande de pixels. La valeur appropriée dépend de la taille de l’image.

**Seuil** Détermine la plage de contraste à ignorer lorsque le filtre de masquage flou est appliqué. En d’autres termes, cette option définit l’écart recherché entre les pixels et la zone environnante avant qu’ils ne soient considérés comme des pixels de contour et ne soient accentués. Pour éviter d’introduire du bruit, jouez avec des valeurs comprises entre 0,02 et 0,2. La valeur par défaut de 6 permet d’accentuer tous les pixels de l’image.

**Espace** colorimétrique Détermine si l’image utilise l’espace dans lequel elle a été créée, généralement RVB (original) ou un espace de luminance (intensité).

**Couleur** Choisissez les options suivantes :

**Profil** de couleurs de sortie Sélectionnez Utiliser la couleur par défaut ou l’un des profils de couleurs ICC disponibles dans Scene7 Publishing System.

(voir aussi [Profils ICC](icc-profiles.md#icc_profiles)).

**Mode** de rendu Sélectionnez une option si vous souhaitez remplacer le mode de rendu par défaut du profil de couleurs. Utilisez cette option lorsqu’un des profils ICC par défaut est l’espace cible d’une conversion de couleurs, qu’un périphérique de sortie (imprimante ou moniteur) est caractérisé par ce profil et que le mode de rendu spécifié est valide pour ce profil.

**Incorporer le Profil** Sélectionnez cette option pour que, si vous ouvrez cette image dans Adobe® Photoshop®, elle utilise ce profil.

**Résolution** d&#39;impression Choisissez une résolution pour imprimer cette image ; 72 pixels est la valeur par défaut.

**Modificateurs** d’URL Si vous préférez spécifier les modificateurs d’URL qui définissent votre paramètre d’image prédéfini plutôt que les paramètres, entrez les modificateurs ici.

**L’exemple d’URL** d’image Liste la chaîne URL &quot;brute&quot; utilisée par le serveur Dynamic Media Image Server pour diffuser des images avec le paramètre d’image prédéfini que vous ajoutez ou modifiez. Cette chaîne URL code tous les paramètres de format que vous sélectionnez sur l’écran Ajouter un paramètre prédéfini ou Modifier le paramètre prédéfini.

### Modification, suppression ou désactivation d’un paramètre d’image prédéfini {#editing-removing-or-deactivating-an-image-preset}

1. Cliquez sur **Configuration** > **Paramètres d’image prédéfinis**.
1. Dans l’écran Paramètres d’image prédéfinis, sélectionnez un paramètre prédéfini dans le tableau, puis effectuez l’une des opérations suivantes :

   * Click **Edit** and then specify new options in the Edit Preset dialog box.
   * Click **Delete** to remove the preset from the list.
   * Décochez la case Actif située en regard du nom du paramètre prédéfini à supprimer de l’ensemble de l’interface utilisateur de Scene7 Publishing System pour les utilisateurs du portail multimédia.

## Activation ou désactivation des paramètres prédéfinis de vidéo adaptative {#activating-or-deactivating-adaptive-video-presets}

Dynamic Media Classic offres les paramètres prédéfinis de codage de vidéo adaptative. Il s’agit d’une liste type de paramètres prédéfinis qui associe dans un seul groupe les paramètres prédéfinis de vidéo adaptative 16:9 et les paramètres prédéfinis de vidéo adaptative 4:3. Ces paramètres prédéfinis représentent les paramètres de codage les plus courants et sont optimisés pour la lecture sur périphériques mobiles, tablettes cibles et ordinateurs.

Seuls les paramètres prédéfinis de codage de « vidéo adaptative » sont activés par défaut. Vous pouvez les désactiver, si vous le souhaitez. Les paramètres prédéfinis de vidéo adaptative inactifs n’apparaissent pas sous forme d’option sélectionnable dans la section eVideo de la boîte de dialogue Télécharger les options de la tâche.

Voir [Chargement et codage de vidéos](uploading-encoding-videos.md#uploading_and_encoding_videos).

**Activation ou désactivation des paramètres prédéfinis de vidéo adaptative**

1. Près du coin supérieur droit de Scene7 Publishing System, cliquez sur **Configuration** > **Configuration de l’application** > **Paramètres vidéo prédéfinis** > **Paramètres prédéfinis de vidéo adaptative**.
1. Sur la page Paramètres prédéfinis de vidéo adaptative, décochez la case située en regard du nom d’un paramètre prédéfini à supprimer de la liste Options eVideo figurant dans la boîte de dialogue Télécharger les options de la tâche.
1. Cliquez sur **Fermer**.

## Paramètres vidéo prédéfinis pour le codage des fichiers vidéo {#video-presets-for-encoding-video-files}

Pour choisir un paramètre de codage prédéfini, dans le coin inférieur droit de la page de chargement, cliquez sur Options de tâche. Ensuite, dans la boîte de dialogue Télécharger les options de la tâche, affichez les options eVideo et choisissez les paramètres prédéfinis de codage vidéo.

>[!NOTE]
>
>A l’exception de la « vidéo adaptative », qui est activée par défaut, il est possible que les autres paramètres prédéfinis de codage de vidéo adaptative ou de vidéo unique ne s’affichent pas tous dans la boîte de dialogue Télécharger les options de la tâche. Les administrateurs Dynamic Media Classic déterminent quels paramètres prédéfinis de codage vidéo sont visibles dans la boîte de dialogue Télécharger les options de la tâche.

* Choisissez l’un des paramètres prédéfinis de codage de vidéo adaptative ou de codage unique suivants :

   **Vidéo adaptative 16:9**

   Créez des vidéos 16:9 pour diffusion sur les ordinateurs de bureau, les appareils mobiles (iPhone, iPad, Android) et les tablettes (iPad, Android), avec la résolution et le débit qui correspondent le mieux à la vitesse de connexion du lecteur.

   **Vidéo adaptative 4:3**

   Créez des vidéos de rapport L/H 4:3 pour la diffusion sur les ordinateurs, les appareils mobiles (iPhone, iPad, Android) et les tablettes (iPad, Android), en optimisant la résolution et le débit qui correspondent le mieux à la vitesse de connexion du lecteur.

   **Vidéo adaptative**

   Un paramètre prédéfini de codage unique qui fonctionne avec n’importe quelle proportion pour créer des vidéos pour une diffusion sur téléphone, tablette et ordinateur de bureau. Les vidéos source transférées qui sont codées avec ce paramètre prédéfini sont définies avec une hauteur fixe. Toutefois, la largeur est automatiquement mise à l’échelle pour conserver les proportions de la vidéo.

   Cette souplesse que procure la fonctionnalité de « redimensionnement automatique » est également disponible par défaut lorsque vous créez votre propre paramètre prédéfini de codage de vidéo personnalisé.

   Voir [Ajout ou modification d’un paramètre prédéfini de codage vidéo](uploading-encoding-videos.md#adding_or_editing_a_video_encoding_preset).

   **Codage de vidéo adaptative (16:9 ou 4:3)**

   Créez des vidéos 16:9 et 4:3 pour la diffusion sur les ordinateurs de bureau, les appareils mobiles (iPhone, iPad, Android) et les tablettes (iPad, Android), avec la résolution et le débit qui correspondent le mieux à la vitesse de connexion du lecteur.

   Voir [Paramètres prédéfinis de codage de vidéo adaptative (16:9 ou 4:3)](application-setup.md#adaptive_video_encoding_16_9_or_4_3_video_presets).

   **Paramètres prédéfinis de codage uniques**

   >[REMARQUE]
   >
   >pour diffuser de la vidéo sur des iPads, vous pouvez choisir un paramètre de codage prédéfini Mobile ou Tablette. Les paramètres prédéfinis Tablette sont spécialement conçus pour l’iPad, généralement avec une meilleure résolution et une qualité supérieure pour tirer parti de l’écran plus large et de la connexion à bande passante plus puissante. Afin de diffuser des fichiers vidéo codés avec un paramètre prédéfini Tablette, vous devez inclure un code de détection de périphérique sur votre site ou application mobile. Ce code bascule entre une expérience vidéo iPhone ou iPad, selon le périphérique de lecture. Le choix d’un paramètre prédéfini Mobile pour la diffusion de fichiers vidéo sur l’iPad représente un flux de travail plus simple, car vous pouvez utiliser le même fichier vidéo pour les iPhones et les iPads. En revanche, la qualité est normalisée sur la résolution iPhone, qui est inférieure.

   * Sous le groupe Paramètres prédéfinis de codage, dans la liste déroulante Trier les paramètres prédéfinis de codage, sélectionnez Nom ou Taille pour trier les paramètres prédéfinis par nom ou taille de résolution.
   * Choisissez un paramètre de codage prédéfini en fonction de la taille de résolution et de la bande passante prévues pour lire la vidéo. 
   * Sélectionnez Codage de vidéo adaptative et un ou plusieurs paramètres prédéfinis de codage par vidéo. Par exemple, vous pouvez coder un fichier pour les ordinateurs de bureau et pour les périphériques mobiles dans le cadre d’une seule tâche de téléchargement.

Après avoir cliqué sur **Démarr. téléch.**, le fichier vidéo original est téléchargé et des fichiers codés sont générés à partir de celui-ci.

### A propos des options de codage prédéfinies {#about-encoding-preset-options}

Les paramètres des options de codage prédéfinies sont comme suit :

**Vitesse** de connexion à la Cible Vitesse de connexion à Internet de l&#39;utilisateur final ciblé.

**Suffixe** de fichier codé Suffixe joint au fichier vidéo codé à des fins d’identification.

**Débit vidéo (débit de données)** Quantité de données codées pour produire une seule seconde de lecture vidéo (en kilobits par seconde).

**Largeur/hauteur** en pixels La largeur de l’image à l’écran, en pixels ; la hauteur de l’image à l’écran (en pixels).

**Image par seconde (ips)** Nombre d’images, ou d’images fixes, pour chaque seconde de vidéo. Aux Etats-Unis et au Japon, la plupart des vidéos sont tournées à 29,97 ips ; en Europe et dans les autres pays d’Asie, la plupart des vidéos le sont à 25 ips. Un film est tourné à 24 ips.

**Débit** audio Quantité de données codées pour produire une seule seconde de lecture audio, en kilobits par seconde.

Le tableau suivant répertorie les meilleures pratiques recommandées pour la sélection de paramètres vidéo prédéfinis et les conventions de dénomination qui sont utilisées pour désigner les fichiers codés.

### Vidéo adaptative (par défaut) {#adaptive-video-default}

Un paramètre prédéfini de codage qui fonctionne avec n’importe quelle proportion pour permettre la création de vidéos pour une diffusion sur téléphone, tablette et ordinateur de bureau Les vidéos source transférées qui sont codées à l’aide de ce paramètre prédéfini (la valeur par défaut et recommandée) sont définies avec une hauteur fixe alors que la largeur est redimensionnée automatiquement pour conserver les proportions de la vidéo.

**Vidéo adaptative (valeur par défaut)**

|  | Nom du paramètre prédéfini de codage/Texte de l’info-bulle | Suffixe de fichier codé | Débit de données vidéo (Kb/s) | Largeur/hauteur (pixels) | Nombre d’images par seconde (i/s) | Débit audio (Kbit/s) | Recommandations |
|--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | Automatique x 360, 800 Kbits/s | _Mobile_Autox360p_800K | 800 | Autox360 | Identique à la source | 64 | Mobile (iPhone, iPad, Android) |
| 2 | Automatique x 480, 1 400 Kbits/s | _Tablet_Autox480p_1400K | 1400 | Autox480 | Identique à la source | 96 | Tablette (iPad, Android) |
| 3 | Automatique x 720, 2 600 Kbits/s | _Desktop_Autox720p_2600K | 2600 | Autox720 | Identique à la source | 128 | Pour bureau |

### Paramètres prédéfinis de codage de vidéo adaptative (16:9 ou 4:3){#adaptive-video-encoding-or-video-presets}

Ces paramètres prédéfinis de codage de vidéo adaptative combinent une série de paramètres prédéfinis de codage individuels qui sont automatiquement sélectionnés en fonction des proportions de la vidéo que vous transférez. Si, par exemple, vous téléchargez une vidéo 4:3, elle est automatiquement codée à l’aide des cinq paramètres prédéfinis 4:3 trouvés dans la liste des paramètres prédéfinis originaux dans l’option **Codage de vidéo adaptative (16:9 ou 4:3)**.

Pour plus d’informations sur les options de codage, voir [A propos des options de codage prédéfinies](application-setup.md#about_encoding_preset_options).

**Paramètres prédéfinis de codage de vidéo adaptative (16:9 ou 4:3)**

|  | Nom du paramètre prédéfini de codage/Texte de l’info-bulle | Vitesse de connexion cible (Kbit/s) | Suffixe de fichier codé | Débit de données vidéo (Kb/s) | Largeur/hauteur (pixels) | Nombre d’images par seconde (i/s) | Débit audio (Kbit/s) | Recommandations |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 512x288, mobile (iPhone, iPad, Android), (400 kbits/s) | 500 | _Mobile_512x288_400K | 400 | 512x288 | Identique à la source | 64 | Faible résolution, 3G |
| 2 | 4:3, 384x288, mobile (iPhone, iPad, Android), (400 kbits/s) | 500 | _Mobile_384x288_400K | 400 | 384 x 288 | Identique à la source | 64 | Faible résolution, 3G |
| 3 | 16:9, 512x288, mobile (iPhone, iPad, Android), (600 kbits/s) | 700 | _Mobile_512x288_600K | 600 | 512 x 288 | Identique à la source | 64 | Résolution moyenne, 3G |
| 4 | 4:3, 384x288, mobile (iPhone, iPad, Android), (600 kbits/s) | 700 | _Mobile_384x288 _600 | 600 | 384 x 288 | Identique à la source | 64 | Résolution moyenne, 3G |
| 5 | 16:9, 640x360, tablette (iPad, Android), (800 Kbits/s) | 900 | _iPad_640x360_800K | 800 | 640 x 360 | Identique à la source | 80 | Résolution moyenne, Wi-Fi |
| 6 | 4:3, 640x480, tablette (iPad, Android), (800 Kbits/s) | 900 | _iPad_640x480_800K | 800 | 640 x 480 | Identique à la source | 80 | Résolution moyenne, Wi-Fi |
| 7 | 16:9, 768x432, tablette (iPad, Android), (1 200 Kbits/s) | 1,5 Mbit/s | _iPad_768x432_1200K | 1 200 | 768 x 432 | Identique à la source | 96 | Haute résolution, Wi-Fi |
| 8 | 4:3, 768x576, tablette (iPad, Android), (1 200 Kbits/s) | 1,5 Mbit/s | _iPad_768x576_1200K | 1 200 | 768 x 576 | Identique à la source | 96 | Haute résolution, Wi-Fi |
| 9 | 16:9, 1280 x 720, bureau, (2 000 Kbits/s) | 3 Mbits/s | _1280X720_2000K | 2 000 | 1280 x 720 | Identique à la source | 128 | Haute définition, Grand écran |
| 10 | 4:3, 1 280 x 960, bureau, (2 000 Kbits/s) | 3 Mbits/s | _1280X 960_2000K | 2 000 Kbits/s | 1280x960 | Identique à la source | 128 | Haute définition |

### Paramètres prédéfinis de codage de vidéo pour ordinateur de bureau {#desktop-video-encoding-presets}

Il s’agit des paramètres prédéfinis de codage pour les formats vidéo MP4 et OGV sur les ordinateurs de bureau.

Pour plus d’informations sur les options de codage prédéfinies, voir [A propos des options de codage prédéfinies](application-setup.md#about_encoding_preset_options).

**H264 Main 3.2 - Audio AAC, Extension de fichier MP4**

|  | Nom du paramètre prédéfini de codage/Texte de l’info-bulle | Vitesse de connexion cible (Kbit/s) | Suffixe de fichier codé | Débit de données vidéo (Kb/s) | Largeur/hauteur (pixels) | Nombre d’images par seconde (i/s) | Débit audio (Kbit/s) | Recommandations |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 480 x 270 (400 Kbit/s) | 500 | _480X270_400K | 400 | 480 x 270 | Identique à la source | 64 | Résolution grand écran faible |
| 2 | 16:9, 640 x 360 (800 Kbits/s) | 900 | _640X360_800K | 800 | 640 x 360 | Identique à la source | 80 | Résolution grand écran moyenne |
| 3 | 16:9, 800 x 450 (1 200 Kbits/s) | 1,5 Mbit/s | _800X450_1200K | 1 200 | 800 x 450 | Identique à la source | 96 | Moyenne à haute résolution |
| 4 | 16:9, 1280 x 720 (2 000 Kbits/s) | 3 Mbits/s | _1280X720_2000K | 2 000 | 1280 x 720 | Identique à la source | 128 | Haute définition, Grand écran |
| 5 | 4:3, 320 x 240 (400 kb/s) | 500 | _320X240_400K | 400 | 320 x 240 | Identique à la source | 64 | Basse résolution |
| 6 | 4:3, 480 x 360 (800 Kbits/s) | 900 | _480X360_800K | 800 | 480 x 360 | Identique à la source | 80 | Résolution moyenne |
| 7 | 4:3, 640 x 480 (1 200 Kbits/s) | 1,5 Mbit/s | _640X480_1200K | 1 200 | 640 x 480 | Identique à la source | 96 | Moyenne à haute résolution |
| 8 | 4:3, 1 280 x 960 (2 000 Kbits/s) | 3 Mbits/s | _1280X960_2000K | 2 000 | 1280 x 960 | Identique à la source | 128 | Haute définition |

**OGG Theora Vorbis - extension de fichier OGV**

|  | Nom du paramètre prédéfini de codage/Texte de l’info-bulle | Vitesse de connexion cible (Kbit/s) | Suffixe de fichier codé | Débit de données vidéo (Kb/s) | Largeur/hauteur (pixels) | Nombre d’images par seconde (i/s) | Débit audio (Kbit/s) | Recommandations |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 480 x 270 (400 Kbits/s, OGG | 500 | _OGG_480x270_400K | 400 | 480 x 270 | Identique à la source | 64 | Résolution grand écran faible |
| 2 | 16:9, 640 x 360 (800 Kbits/s), OGG | 900 | _OGG_640x360_800K | 800 | 640 x 360 | Identique à la source | 80 | Résolution grand écran moyenne |
| 3 | 16:9, 800 x 450 (1 200 Kbits/s), OGG | 1,5 Mbit/s | _OGG_800x450_1200K | 1 200 | 800 x 450 | Identique à la source | 96 | Moyenne à haute résolution |
| 4 | 16:9, 1280 x 720 (2 000 Kbits/s), OGG | 3 Mbits/s | _OGG_1280x720_2000K | 2 000 | 1280 x 720 | Identique à la source | 128 | Haute définition, Grand écran |
| 5 | 4:3, 320 x 240 (400 kb/s), OGG | 500 | _OGG_320X240_400K | 400 | 320 x 240 | Identique à la source | 64 | Basse résolution |
| 6 | 4:3, 480 x 360 (800 Kbits/s), OGG | 900 | _OGG_480x360_800K | 800 | 480 x 360 | Identique à la source | 80 | Résolution moyenne |
| 7 | 4:3, 640 x 480 (1 200 Kbits/s), OGG | 1,5 Mbit/s | _OGG_640x480_1200K | 1 200 | 640 x 480 | Identique à la source | 96 | Moyenne à haute résolution |
| 8 | 4:3, 1 280 x 960 (2 000 Kbits/s), OGG | 3 Mbits/s | _OGG_1280x960_2000K | 2 000 | 1280 x 960 | Identique à la source | 128 | Haute définition |

### Paramètres prédéfinis de codage vidéo pour périphérique mobile {#mobile-video-encoding-presets}

Identique au débit source. Paramètres prédéfinis de codage de vidéo pour périphériques mobiles tels que l’iPhone, l’iPad et Android.

Pour plus d’informations sur les options de codage prédéfinies, voir [A propos des options de codage prédéfinies](application-setup.md#about_encoding_preset_options).

**H264 Baseline 2.1 - Audio AAC, Extension de fichier MP4**

|  | Nom du paramètre prédéfini de codage/Texte de l’info-bulle | Vitesse de connexion cible (Kbit/s) | Suffixe de fichier codé | Débit vidéo (Kbit/s) | Hauteur/largeur en pixels | Nombre d’images par seconde (i/s) | Débit audio (Kbit/s) | Recommandations |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 512 x 288, Mobile (400 Kbit/s) | 500 | _Mobile_512x288_400K | 400 | 512x288 | Identique à la source | 64 | Faible résolution, 3G |
| 2 | 16:9, 512 x 288, Mobile (600 Kbit/s) | 700 | _Mobile_512x288_600K | 600 | 512 x 288 | Identique à la source | 64 | Résolution moyenne, 3G |
| 3 | 16:9, 512 x 288, Mobile (800 Kbit/s) | 900 | _Mobile_512x288_800K | 800 | 512 x 288 | Identique à la source | 80 | Résolution moyenne, Wi-Fi |
| 4 | 16:9, 512 x 288, Mobile (1 000 Kbit/s) | 1,2 Mbit/s | _Mobile_512x288_1000K | 1 000 | 512 x 288 | Identique à la source | 80 | Haute résolution, Wi-Fi |
| 5 | 16:9, 512 x 288, Mobile (1 200 Kbit/s) | 1,5 Mbit/s | _Mobile_512x288_1200K | 1 200 | 512 x 288 | Identique à la source | 96 | Haute résolution, Wi-Fi |
| 6 | 4:3, 384 x 288, Mobile (400 Kbit/s) | 500 | _Mobile_384x288_400K | 400 | 384 x 288 | Identique à la source | 64 | Faible résolution, 3G |
| 7 | 4:3, 384 x 288, Mobile (600 Kbit/s) | 700 | _Mobile_384x288_600K | 600 | 384 x 288 | Identique à la source | 64 | Résolution moyenne, 3G |
| 8 | 4:3, 448 x 336, Mobile (800 Kbit/s) | 900 | _Mobile_448x336_800K | 800 | 448 x 336 | Identique à la source | 80 | Résolution moyenne, Wi-Fi |
| 9 | 4:3, 448 x 336, Mobile (1 000 Kbit/s) | 1,2 Mbit/s | _Mobile_448x336_1000K | 1 000 | 448 x 336 | Identique à la source | 80 | Haute résolution, Wi-Fi |
| 10 | 4:3, 448 x 336, Mobile (1 200 Kbit/s) | 1,5 Mbit/s | _Mobile_448x336_1200K | 1 200 | 448 x 336 | Identique à la source | 96 | Haute résolution, Wi-Fi |

## Paramètres prédéfinis de la visionneuse {#viewer-presets}

>[!NOTE]
>
>**Avis** de fin de vie des visionneuses Flash - Depuis le 31 janvier 2017, Adobe Scene7 Publishing System a officiellement mis fin à la prise en charge de la plate-forme de la visionneuse Flash. Pour plus d&#39;informations sur cette modification importante, consultez le site Web de la FAQ suivante : [https://docs.adobe.com/content/docs/en/aem/6-1/administer/integration/marketing-cloud/scene7/flash-eol.html](https://docs.adobe.com/content/docs/en/aem/6-1/administer/integration/marketing-cloud/scene7/flash-eol.html).

Un *paramètre prédéfini de visionneuse* est un ensemble de paramètres qui déterminent comment les utilisateurs voient les fichiers de média enrichi sur leur écran d’ordinateur et périphériques mobiles. En tant qu’administrateur, vous pouvez créer des paramètres de visionneuse prédéfinis. Des paramètres sont disponibles pour un ensemble d’options de configuration de la visionneuse. Vous pouvez, par exemple, modifier la taille d’affichage de la visionneuse, le comportement du zoom, les modes de couleurs, les bordures et les polices.

Il est recommandé d’utiliser les visionneuses de vidéos HTML5 Dynamic Media Classic. Les paramètres prédéfinis utilisés dans des visionneuses de vidéos HTML5 sont des lecteurs vidéo fiables. En combinant dans un seul lecteur la capacité de concevoir les composants de lecture à l’aide de code HTML5 et CSS, d’avoir accès à la lecture incorporée et d’utiliser les flux continus adaptatifs et progressifs selon la capacité du navigateur, vous pouvez étendre la portée de votre contenu multimédia aux utilisateurs d’appareils mobiles, de tablettes et d’ordinateurs et garantir ainsi une expérience vidéo rationalisée.

Voir [A propos des visionneuses](hhttps://docs.adobe.com/content/help/en/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers.html) HTML5 dans le Guide de référence des visionneuses Adobe.

Voir Matrice [de compatibilité des paramètres prédéfinis de la visionneuse](application-setup.md#scene7_viewer_preset_compatibility_matrix)Dynamic Media Classic.

Reportez-vous à la section [Meilleure pratique : Utilisation de la visionneuse de vidéos HTML5](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer).

Selon la visionneuse, vous pouvez ajouter des fonctions communautaires. Ces fonctions comprennent des boutons d’incorporation, d’e-mail, de lien et de visite de site. Ces boutons permettent aux utilisateurs de partager le lecteur avec d’autres personnes ou d’ouvrir le site Web Dynamic Media Classic.

Voir aussi Exemples [de bibliothèques de référence des visionneuses](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html)Adobe.

### Prise en charge des visionneuses pour les pages Web adaptées {#viewer-support-for-responsive-designed-web-pages}

Différentes pages Web ont différents besoins. Vous pouvez souhaiter qu’une page Web fournisse un lien qui ouvre la visionneuse HTML5 dans une fenêtre distincte du navigateur. Dans d’autres cas, il peut être nécessaire d’incorporer la visionneuse HTML5 directement sur la page d’hébergement. Dans ce dernier cas, la page Web peut avoir une disposition statique. Sinon, elle peut être « adaptée » et s’afficher différemment en fonction du périphérique ou de la taille du navigateur. Pour répondre à ces besoins, les visionneuses HTML5 fournies avec Dynamic Media Classic prennent en charge les pages Web statiques et les pages Web adaptées.

Voir [Bibliothèque d’images statiques](https://marketing.adobe.com.com/resources/help/en_US/s7/is_ir_api/is_api/c_about_responsive_static_image_library.html)réactives dans l’aide *de l’API* Adobe Image Serving pour en savoir plus sur la manière d’incorporer des visionneuses adaptées à vos pages Web.

### Types de paramètres prédéfinis de visionneuse {#viewer-preset-types}

Les administrateurs peuvent créer et personnaliser les types de paramètres prédéfinis suivants :

**Visionneuse** de catalogue électronique Simule l’expérience de lecture d’un catalogue imprimé. Vous pouvez passer d’une page à l’autre, effectuer un zoom avant ou arrière sur les éléments d’une page, utiliser des zones cliquables pour afficher davantage d’informations sur les éléments de la page ou effectuer des recherches dans le catalogue. Vous pouvez également inclure un panneau d’informations afin d’afficher des informations détaillées et un objet créé à partir d’une image si la zone cliquable contient un attribut rollover_key valide. Pour ce faire, indiquez l’URL du serveur d’informations dans le volet Paramètres du panneau d’informations de la fenêtre des paramètres par défaut de la visionneuse de catalogue électronique.

**Visionneuse** d’échantillons Affiche une image dans une couleur, un matériau, une texture, un fini ou un tissu différent. Les utilisateurs cliquent sur une miniature pour voir les variations de l’image.

**Visionneuse** de supports variés : affiche différents types de supports dans une seule visionneuse. Vous pouvez y inclure des séries d’échantillons, des visionneuses à 360°, des images et des vidéos. Vous pouvez également configurer des onglets pour stocker différents types de contenu (par exemple, un pour les visionneuses d’images et un autre pour les vidéos). Les vidéos lues grâce à une visionneuse de supports variés utilisent une visionneuse de vidéos standard comportant un plan de montage chronologique et des commandes vidéo comme Arrêt, Pause, Rembobinage et Lecture. Lorsque vous configurez un paramètre prédéfini de visionneuse de supports variés, vous indiquez les visionneuses à utiliser pour les différents types de fichiers qu’elle contient. Vous pouvez également utiliser la visionneuse de grille ou de carrousel pour visualiser les fichiers d’une visionneuse de supports variés.

**Visionneuse à 360°** Fournit plusieurs vues d’une image afin que les utilisateurs puissent tourner l’objet pour examiner les différents côtés et angles.

**Visionneuse** de vidéos Affiche les vidéos en utilisant les dimensions de résolution du fichier source ou une taille personnalisée. Dynamic Media Classic est fourni avec de nombreux paramètres prédéfinis de visionneuse pour la lecture vidéo. En outre, si vous êtes un administrateur, vous pouvez créer des paramètres prédéfinis personnalisés pour la visionneuse de vidéos. Il existe plus d’une douzaine de paramètres distincts pour la configuration de la visionneuse de vidéos. Vous pouvez configurer la taille, la couleur de premier plan et d’arrière-plan, les commandes vidéo et audio, la barre de progression, l’habillage de l’interface utilisateur, les fonctions sociales et l’aide.

**Les visionneuses** de zoom Offre trois types de visionneuses de zoom :

**Visionneuse** de zoom Permet aux utilisateurs d’effectuer un zoom sur la zone en cliquant dessus. Ils peuvent cliquer sur les commandes pour effectuer un zoom avant ou arrière et rétablir la taille par défaut de l’image.

**Visionneuse de zoom : Fenêtre déroulante** Affiche une seconde image de la zone agrandie en regard de l’image d’origine. Aucune commande n’est disponible. Il suffit de déplacer la sélection sur la zone à visualiser.

Pour déterminer la quantité totale de bande passante allouée à la visionneuse, n’oubliez pas que l’image principale et celle de la fenêtre déroulante sont toutes deux diffusées par la visionneuse. La taille de l’image principale (largeur et hauteur d’affichage) et le facteur de zoom déterminent la taille de la fenêtre déroulante. Pour que la fenêtre déroulante ne devienne pas trop volumineuse, équilibrez ces deux valeurs : si la taille de l’image principale est importante, réduisez la valeur du facteur de zoom. (La Largeur de la fenêtre déroulante et la Hauteur de la fenêtre déroulante déterminent la taille de la fenêtre déroulante, mais pas la taille de l’image diffusée par la visionneuse.)

Par exemple, si la taille de l’image principale est de 350 x 350 pixels et que le facteur de zoom est de 3, la taille d’image de la fenêtre déroulante sera de 1 050 x 1 050 pixels. Si la taille de l’image principale est de 300 x 300 pixels et que le facteur de zoom est de 4, la taille d’image de la fenêtre déroulante sera de 1 200 x 1 200 pixels. Selon la valeur de qualité JPEG sélectionnée (une valeur comprise entre 80 et 90 est recommandée), il est possible de réduire sensiblement la taille du fichier. Selon la taille de l’image principale, un facteur de zoom de 2,5 à 4 est recommandé.

### Matrice de compatibilité des paramètres prédéfinis de la visionneuse Dynamic Media Classic {#scene-viewer-preset-compatibility-matrix}

**Avis** de fin de vie des visionneuses Flash : Depuis le 31 janvier 2017, Adobe Scene7 Publishing System a officiellement mis fin à la prise en charge de la plate-forme de la visionneuse Flash.

Pour plus d&#39;informations sur cette modification importante, consultez le site Web de la FAQ suivante : [https://docs.adobe.com/content/docs/en/aem/6-1/administer/integration/marketing-cloud/scene7/flash-eol.html](https://docs.adobe.com/content/docs/en/aem/6-1/administer/integration/marketing-cloud/scene7/flash-eol.html).

Le tableau suivant identifie les paramètres prédéfinis actuellement disponibles pour la visionneuse Dynamic Media Classic. Ce tableau indique également la compatibilité de la visionneuse avec les périphériques mobiles et fixes, et la technologie utilisée pour chacune des visionneuses données.

Voir aussi Exemples [de bibliothèques de référence des visionneuses](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html)Adobe.

Pour en savoir plus sur les versions de navigateur Web et de système d’exploitation prises en charge pour les visionneuses, consultez les notes de mise à jour des visionneuses.

Voir Notes [de mise à jour des références des visionneuses](https://docs.adobe.com/content/help/en/dynamic-media-developer-resources/library/home.html)Adobe.

|  | Technologie de la visionneuse | Bureau | Apple iPhone | Apple iPad | Smartphone Android | Tablette Android |
|--- |--- |--- |--- |--- |--- |--- |
| Visionneuses de zoom |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_inline | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_light | HTML5 | X | X | X | X | X |


|  | Technologie de la visionneuse | Bureau | Apple iPhone | Apple iPad | Smartphone Android | Tablette Android |
|--- |--- |--- |--- |--- |--- |--- |
| Visionneuses d’images |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

|  | Technologie de la visionneuse | Bureau | Apple iPhone | Apple iPad | Smartphone Android | Tablette Android |
|--- |--- |--- |--- |--- |--- |--- |
| Visionneuses d’échantillons |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_light | HTML5 | X | X | X | X | X |

|  | Technologie de la visionneuse | Bureau | Apple iPhone | Apple iPad | Smartphone Android | Tablette Android |
|--- |--- |--- |--- |--- |--- |--- |
| Visionneuses de catalogue électronique |  |  |  |  |  |  |
| Universal_HTML5_eCatalog_Adv(Inclut la prise en charge de la recherche dans les médias sociaux et les catalogues.) | HTML5 | X | X | X | X | X |
| Universal_HTML5_eCatalog (Inclut la prise en charge de la recherche dans les médias sociaux et les catalogues.) | HTML5 | X | X | X | X | X |

|  | Technologie de la visionneuse | Bureau | Apple iPhone | Apple iPad | Smartphone Android | Tablette Android |
|--- |--- |--- |--- |--- |--- |--- |
| Visionneuses à 360° |  |  |  |  |  |  |
| Universal_HTML5_SpinSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SpinSet_light | HTML5 | X | X | X | X | X |

**Visionneuses d’eVideo**

Dynamic Media Classic prend en charge la lecture vidéo mobile pour la vidéo MP4 H.264.

* Vous trouverez les périphériques Blackberry qui prennent en charge ce format vidéo à l’adresse suivante : [Formats vidéo pris en charge sur Blackberry](https://developer.blackberry.com/devzone/develop/supported_media/bb10_media_support.html)
* Vous pouvez également trouver les périphériques Windows qui prennent en charge ce format vidéo à l’adresse suivante :Formats vidéo[pris en charge sur Windows Phone](https://docs.microsoft.com/en-us/previous-versions/windows/apps/ff462087(v=vs.105)?redirectedfrom=MSDN)

|  | Technologie de la visionneuse | Bureau | Apple iPhone | Apple iPad | Smartphone Android | Tablette Android | Smartphone Blackberry | Windows Phone |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| Universal_HTML5_Video (inclut la prise en charge du sous-titrage.) Reportez-vous à la section [Meilleure pratique : Utilisation de la visionneuse de vidéos HTML5 universelle.](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer) | HTML5 | X | X | X | X | X | X | X |
| Universal_HTML5_Video_social(Inclut la prise en charge du sous-titrage et des médias sociaux.) | HTML5 | X | X | X | X | X | X | X |

|  | Technologie de la visionneuse | Bureau | Apple iPhone | Apple iPad | Smartphone Android | Tablette Android |
|--- |--- |--- |--- |--- |--- |--- |
| Visionneuses de supports variés |  |  |  |  |  |  |
| Universal_HTML5_MixedMedia_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_MixedMedia_light | HTML5 | X | X | X | X | X |

### Matrice des mouvements des visionneuses mobiles pris en charge {#supported-mobile-viewers-gestures-matrix}

Le tableau suivant identifie les mouvements des visionneuses mobiles qui sont pris en charge sur les périphériques iOS, Android 2.x et Android 3.x.

|  | Technologie de la visionneuse | Bureau | Apple iPhone | Apple iPad | Smartphone Android | Tablette Android |
|--- |--- |--- |--- |--- |--- |--- |
| Visionneuses d’images |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

### À propos de l’écran Paramètres prédéfinis de la visionneuse {#about-the-viewer-preset-screen}

Créez et gérez des paramètres prédéfinis de la visionneuse sur l’écran Paramètres prédéfinis de la visionneuse. Pour ouvrir cet écran, cliquez sur **Configuration** > **Paramètres prédéfinis de la visionneuse**.

L’écran Paramètres prédéfinis de la visionneuse propose des outils permettant d’effectuer les tâches suivantes :

**Ajouter un paramètre prédéfini** Cliquez sur Ajouter et faites vos choix dans la boîte de dialogue Ajouter un paramètre prédéfini de visionneuse.

Voir [Ajout et modification des paramètres prédéfinis de visionneuse](application-setup.md#adding_and_editing_viewer_presets).

**Modification d’un paramètre prédéfini** Sélectionnez un paramètre prédéfini, puis cliquez sur **Modifier**.

Voir [Ajout et modification des paramètres prédéfinis de visionneuse](application-setup.md#adding_and_editing_viewer_presets).

**Suppression d’un paramètre prédéfini** Sélectionnez un paramètre prédéfini, puis cliquez sur **Supprimer**.

**Exportation d’un paramètre prédéfini** Sélectionnez un paramètre prédéfini de visionneuse HTML5, puis cliquez sur Exporter pour télécharger l’habillage de la visionneuse afin que vous puissiez l’utiliser comme base pour créer et ajouter un nouveau paramètre prédéfini de visionneuse.

Voir [Exportation d’un paramètre prédéfini](application-setup.md#exporting_an_html5_viewer_preset)de visionneuse HTML5.

**Filtrage de la liste** de paramètres prédéfinis de la visionneuse Utilisez les outils suivants pour filtrer la liste :

* Dans la liste déroulante **Actifs/Inactifs**, choisissez une option pour afficher les paramètres prédéfinis actifs, les paramètres prédéfinis inactifs ou tous les paramètres prédéfinis.
* Dans la liste déroulante **Visionneuse**, choisissez une option pour afficher uniquement les visionneuses d’un certain type. Sélectionnez **Toutes les visionneuses** pour les voir toutes.

**Tri des paramètres prédéfinis** Cliquez sur un en-tête de colonne (Actif, Type, Paramètre prédéfini ou Platform) pour trier la liste sur une colonne. Cliquez à nouveau sur un en-tête de colonne pour trier la liste dans l’ordre décroissant (ou croissant).

**Activation et désactivation des paramètres prédéfinis** Sélectionnez un paramètre prédéfini et cliquez sur son option Actif pour l’activer ou le désactiver.

Voir [Activation ou désactivation des paramètres prédéfinis de la visionneuse](application-setup.md#activating_or_deactivating_viewer_presets).

>[!NOTE]
>
>Cliquez sur Prévisualiser sur le côté droit de l’écran Paramètres prédéfinis de la visionneuse pour avoir une idée du rendu d’un fichier avec le paramètre de visionneuse prédéfini sélectionné. Pour voir un autre fichier, vous pouvez cliquer sur le bouton Parcourir de l’écran Paramètres prédéfinis de la visionneuse et sélectionner un autre fichier dans la boîte de dialogue Choisir fich. à prévisualiser.

### Ajout et modification de paramètres prédéfinis de la visionneuse {#adding-and-editing-viewer-presets}

Outre l’option Ajouter de l’interface utilisateur, vous pouvez également utiliser l’option Exporter pour ajouter un paramètre prédéfini de visionneuse. Il vous suffit d’exporter un paramètre prédéfini de visionneuse HTML5 existant, puis de l’utiliser comme base du nouveau paramètre prédéfini.

Voir [Exportation d’un paramètre prédéfini](application-setup.md#exporting_an_html5_viewer_preset)de visionneuse HTML5.

**Ajout et modification de paramètres prédéfinis de visionneuse**

1. Près de l’angle supérieur droit de Scene7 Publishing System, cliquez sur **Configuration** > **Paramètres prédéfinis de la visionneuse**.

   Vous pouvez filtrer la liste des paramètres prédéfinis. Par exemple, pour afficher uniquement les paramètres prédéfinis pour les visionneuses de vidéos, sélectionnez Visionneuse de vidéos dans le menu déroulant des visionneuses sur la barre d’outils qui se trouve directement au-dessus du tableau.

1. Dans l’écran Paramètres prédéfinis de la visionneuse, ajoutez ou modifiez le paramètre prédéfini de visionneuse.

   **Ajouter** Cliquez sur Ajouter dans la barre d’outils. Dans la boîte de dialogue Ajouter un paramètre prédéfini de visionneuse, choisissez une plate-forme et un type de fichier de média enrichi. 

   Cliquez sur **Enregistrer en tant que** lorsque vous avez terminé de créer le paramètre prédéfini de la visionneuse.

   **Ajouté à partir d’un paramètre prédéfini** de visionneuse existant Dans le tableau, sélectionnez un paramètre prédéfini de visionneuse de vidéos, puis cliquez sur Modifier dans la barre d’outils.

   Après avoir reconfiguré la visionneuse de vidéos, cliquez sur **Enregistrer en tant que** pour enregistrer le paramètre prédéfini sous un autre nom dans le champ Nom du paramètre prédéfini.

   **Modification** Sélectionnez un paramètre prédéfini de visionneuse existant, puis cliquez sur **Modifier**.

1. Dans l’écran Configurer la visionneuse, dans le champ Nom du paramètre prédéfini, saisissez ou modifiez le nom du paramètre prédéfini.
1. Définissez les options restantes si vous le souhaitez.

   >[REMARQUE]
   >
   >choisissez Identique à la source pour dimensionner automatiquement la visionneuse de vidéos selon la taille de résolution de la vidéo codée. Si vous sélectionnez cette option, vous ne pouvez pas saisir la largeur d’affichage et la hauteur d’affichage. Ces valeurs proviennent directement de la vidéo elle-même. Si vous choisissez Identique à la source, définissez l’option Taille de marge, de sorte qu’elle reflète les dimensions d’habillage en dehors de la zone de lecture vidéo. Cette taille de marge correspond à la hauteur et à la largeur, en pixels, des commandes vidéo. Vous pouvez utiliser l’illustration suivante pour vous aider à déterminer les tailles des marges à utiliser.*

   ![](assets/vs_video_viewer_configure_margin.png)

1. Effectuez l’une des opérations suivantes :

   * Cliquez sur **Enregistrer en tant que** si vous avez ajouté un paramètre prédéfini de visionneuse à partir d’un paramètre prédéfini existant.
   * Cliquez sur **Enregistrer** si vous avez ajouté ou modifié un paramètre prédéfini de visionneuse.

### Exportation d’un paramètre prédéfini de visionneuse HTML5 {#exporting-an-html-viewer-preset}

Vous pouvez exporter un paramètre prédéfini de visionneuse HTML5 existant afin de l’utiliser comme base pour créer un nouveau paramètre prédéfini de visionneuse HTML5. Cette méthode est pratique car elle vous évite d’avoir à créer une visionneuse depuis le début. En effet, il vous suffit d’exporter un paramètre prédéfini présentant des caractéristiques et un comportement semblables à ce que vous recherchez, puis de l’utiliser comme point de départ pour vos modifications.

Notez que tous les fichiers CSS prédéfinis de visionneuse prêts à l’emploi par défaut dans SPS utilisent des chemins de diffusion d’images relatifs pointant vers des fichiers situés sur `Scene7SharedAssets`. Par exemple, voici un chemin relatif vers un fichier d’image dans un fichier CSS de paramètre prédéfini de visionneuse situé sur `Scene7SharedAsset`: `.s7videoviewer .s7fullscreenbutton[state][selected] { background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }`Cependant, si vous hébergez des fichiers CSS de visionneuse sur votre propre site, vous devez résoudre ce chemin relatif d’image en utilisant un chemin explicite vers le serveur d’images dans votre propre environnement. À des fins d’illustration, si vous deviez mettre à jour le chemin relatif au-dessus d’un chemin explicite, il peut ressembler à ce qui suit, où `https://s7d1.scene7.com` est le chemin direct vers votre serveur d’images : `https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha`

**Pour exporter un paramètre prédéfini de visionneuse HTML5**

```as3
.s7videoviewer .s7fullscreenbutton[state][selected] 
{ background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }
```

```as3
https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha
```

1. Cliquez sur **Configuration** > **Paramètres prédéfinis de la visionneuse**.
1. On the Viewer Presets toolbar, in the second drop-down list from the left, select **HTML5**.
1. Dans la troisième liste déroulante en partant de la gauche, sélectionnez **Toutes les visionneuses**.
1. Sélectionnez le paramètre prédéfini de visionneuse à utiliser comme base pour un nouveau paramètre prédéfini de visionneuse HTML5.
1. Dans la barre d’outils, cliquez sur **Exporter**.
1. Dans la boîte de dialogue Exporter les fichiers sélectionnés, cliquez sur **Lancer l’exportation**.

   Après l’exportation, vous obtenez un fichier CSS. Téléchargez et décompressez l’archive.

1. Ouvrez le fichier CSS dans un éditeur CSS, effectuez vos modifications, puis enregistrez le fichier.
1. Téléchargez le fichier CSS vers Scene7 Publishing System.

   Voir [Transfert de fichiers](uploading-files.md#uploading_files).

1. Publiez le fichier CSS sur le serveur Dynamic Media Image Server.

   Voir [Publication de fichiers](publishing-files.md#publishing_files).

1. Ajoutez le nouveau paramètre prédéfini de visionneuse comme vous le faites habituellement. Sélectionnez le fichier CSS de la visionneuse que vous avez téléchargé.

   Voir [Ajout et modification des paramètres prédéfinis de visionneuse](application-setup.md#adding_and_editing_viewer_presets).

### Activation ou désactivation des paramètres prédéfinis de la visionneuse {#activating-or-deactivating-viewer-presets}

Pour créer une URL afin d’afficher des fichiers, les utilisateurs ouvrent la liste déroulante Paramètres prédéfinis de la boîte de dialogue de prévisualisation, sélectionnent un paramètre prédéfini de visionneuse et cliquent sur Copier l’URL (voir [Copie de l’URL d’un paramètre prédéfini de visionneuse](application-setup.md#copying_the_url_of_a_viewer_preset)). Cette liste de paramètres prédéfinis présente les paramètres prédéfinis de la visionneuse que les administrateurs ajoutent et gèrent sur l’écran Paramètres prédéfinis de la visionneuse. Par exemple, tous les paramètres prédéfinis actifs de la Visionneuse de catalogue électronique apparaissent dans la liste déroulante Paramètres prédéfinis de la boîte de dialogue Prévisualisation lorsqu’un utilisateur prévisualise un catalogue électronique.

A moins que vous ne désactiviez les Paramètres prédéfinis de la visionneuse sur l’écran Paramètres prédéfinis de la visionneuse, la liste déroulante Paramètres prédéfinis de la boîte de dialogue Prévisualisation peut très vite être remplie. 

**Activation ou désactivation des paramètres prédéfinis de visionneuse**

1. Choose **Setup** > **Viewer Presets** to open the Viewer Presets screen.
1. Sélectionnez ou désélectionnez les options Actif pour activer ou désactiver les Paramètres prédéfinis de la visionneuse.

### Copie de l’URL d’un paramètre prédéfini de visionneuse {#copying-the-url-of-a-viewer-preset}

Après avoir publié un fichier, vous pouvez copier une URL pour afficher le fichier avec les valeurs d’un paramètre prédéfini de visionneuse.

L’URL est copiée dans le Presse-papiers. Vous pouvez l’utiliser, selon vos besoins, dans le code HTML de votre page Web, de votre périphérique mobile ou de votre application.

**Copie de l’URL d’un paramètre prédéfini de visionneuse**

1. Sélectionnez le fichier dans le panneau de navigation.
1. Au-dessus du panneau de navigation des fichiers, sur le côté droit de la barre d’outils, exécutez l’une des opérations suivantes :

   * Cliquez sur **Affichage de la grille**. Dans le panneau de navigation des fichiers, cliquez deux fois sur un fichier pour l’ouvrir dans le mode Affichage des détails. Dans le panneau des URL et d’intégration du code, sur la droite, cliquez sur **Copier l’URL** à droite de la visionneuse appropriée.
   * Cliquez sur **Affichage de la grille**. Dans le panneau de navigation des fichiers, sélectionnez un fichier, puis sous l’image miniature, cliquez sur **Prévisualiser** > **Liste des visionneuses**.

   Dans la page Liste des visionneuses, dans la colonne Actions du tableau, cliquez sur **Copier l’URL**.

   * Cliquez sur **Affichage par liste**. Dans le panneau de navigation des fichiers, sélectionnez un fichier, puis à droite de l’image miniature, cliquez sur **Prévisualiser** > **Liste des visionneuses**.

   Dans la page Liste des visionneuses, dans la colonne Actions du tableau, cliquez sur **Copier l’URL**.

   * Cliquez sur **Affichage de la grille**, **Affichage par liste** ou **Affichage des détails**. Dans la même barre d’outils, cliquez sur **Prévisualiser** > **Liste des visionneuses**.

   Dans la page Liste des visionneuses, dans la colonne Actions du tableau, cliquez sur **Copier l’URL**.

### Copie du code intégré d’un paramètre prédéfini de visionneuse {#copying-the-embed-code-of-a-viewer-preset}

La fonction Code incorporé permet de vérifier le code du paramètre prédéfini de la visionneuse sélectionnée. Vous pouvez aussi copier le code dans le Presse-papiers afin de le coller dans vos pages Web pour le déploiement de la visionneuse.

Vous ne pouvez pas modifier le code dans la boîte de dialogue Intégrer le code.

**Copie du code intégré d’un paramètre prédéfini de visionneuse**

1. Sélectionnez le fichier dans le panneau de navigation des fichiers.
1. Au-dessus du panneau de navigation des fichiers, sur le côté droit de la barre d’outils, exécutez l’une des opérations suivantes :

   * Cliquez sur **Affichage de la grille**. Dans le panneau de navigation des fichiers, cliquez deux fois sur un fichier pour l’ouvrir dans le mode Affichage des détails. Dans le panneau des URL sur la droite, cliquez sur **Code incorporé**.
   * Cliquez sur **Affichage de la grille**. Dans le panneau de navigation des fichiers, sélectionnez un fichier, puis sous l’image miniature, cliquez sur **Prévisualiser** > **Liste des visionneuses**.

   Dans la page Liste des visionneuses, dans la colonne Actions du tableau, cliquez sur **Code incorporé**.

   * Cliquez sur **Affichage par liste**. Dans le panneau de navigation des fichiers, sélectionnez un fichier, puis à droite de l’image miniature, cliquez sur **Prévisualiser** > **Liste des visionneuses**.

   Dans la page Liste des visionneuses, dans la colonne Actions du tableau, cliquez sur **Code incorporé**.

   * Cliquez sur **Affichage de la grille**, **Affichage par liste** ou **Affichage des détails**. Dans la même barre d’outils, cliquez sur **Prévisualiser** > **Liste des visionneuses**.

   Dans la page Liste des visionneuses, dans la colonne Actions du tableau, cliquez sur **Code incorporé**.

1. Dans la boîte de dialogue Code incorporé, cliquez sur **Copier dans le Presse-papiers**.
1. Cliquez sur **Fermer**.

## Configuration des visionneuses par défaut {#configuring-default-viewers}

Vous pouvez utiliser les visionneuses par défaut pour configurer la visionneuse par défaut qui est associée au fichier lorsque vous utilisez l’option Prévisualiser dans Scene7 Publishing System. Vous pouvez configurer l’expérience de prévisualisation par défaut pour les types de fichier suivants :

* Image
* Vidéo
* Visionneuse à 360°
* Catalogue
* ImageSet
* SwatchSet
* Visionneuse de supports

**Pour configurer les visionneuses par défaut**

1. In the Setup drop-down list, click **Application Setup**.
1. In the Setup window, in the left pane, expand **Application Setup** > **Viewers**
1. Click **Default Viewers**.
1. Sur la fenêtre Visionneuses par défaut, dans la liste déroulante de chaque type de fichier, sélectionnez la visionneuse que vous souhaitez associer à l’aperçu du fichier.
1. In the lower-right corner of the Default Viewers window, click **Save Settings**.
1. In the lower-right corner of the Setup window, click **Close** to return to the Asset window.

## Vues des métadonnées {#metadata-views}

Les *métadonnées* sont des informations normalisées concernant un fichier. Vous pouvez utiliser les métadonnées pour rationaliser votre flux de travail, organiser vos fichiers et améliorer les performances de recherche. Dynamic Media Classic prend en charge les normes IPTC (International Press Telecommunications Council) et XMP (extensible metadata platform). Avant d’afficher ou de saisir des métadonnées pour un fichier en mode Affichage des détails, les utilisateurs peuvent ouvrir le menu Vues des métadonnées et choisir le jeu de champs de métadonnées à afficher ou utiliser pour décrire le fichier. 

Dynamic Media Classic est fourni avec des Vues de métadonnées prédéfinies et les administrateurs peuvent créer leurs propres Vues de métadonnées pour que les utilisateurs puissent choisir lorsqu’ils saisissent des métadonnées.

### Création d’une vue de métadonnées {#creating-a-metadata-view}

1. Click **Setup** > **Application Setup** > **Metadata** > **Metadata Views**.
1. Cliquez sur **Ajouter**.
1. Dans le champ de texte Nom du paramètre prédéfini, saisissez le nom de la vue.
1. (Optional) Check **Make Default** to make this view the one that users see when they open the Metadata panel in Detail View.
1. (Optional) Select **Include UDF** to include user-defined fields in the view. Les champs définis par les utilisateurs apparaissent en haut du panneau Métadonnées en mode Affichage des détails.
1. Select the fields you want for the view (click **Select All** to select all the fields).
1. Cliquez sur **Enregistrer**.

   Les catégories et les champs sélectionnés pour la vue apparaissent dans le panneau de prévisualisation.

### Gestion des vues de métadonnées {#managing-metadata-views}

1. Click **Setup** > **Application Setup** > **Metadata** > **Metadata Views**.
1. Utilisez l’une des méthodes suivantes :

   * Pour prévisualiser une vue, sélectionnez-la. Les champs de la vue apparaissent dans le panneau de prévisualisation.
   * To edit a view, select it and then click **Edit**. Then select or deselect field names on the Preview panel, and select or deselect the **Include UDF** option.
   * To delete a view, select it and then click **Delete**.
   * To make a view the default, select it and then click **Make Default**. La vue par défaut est celle qui s’affiche automatiquement lorsque les utilisateurs ouvrent un fichier en mode Affichage des détails, puis accèdent au panneau Métadonnées.

## Paramètres prédéfinis des métadonnées {#metadata-presets}

Les paramètres prédéfinis des métadonnées permettent aux administrateurs de contrôler et de réguler les métadonnées attribuées aux fichiers. En mode Affichage des détails, un utilisateur peut entrer des métadonnées concernant un fichier dans les champs fournis à cet effet. Par exemple, un utilisateur peut entrer un nom de propriétaire, une description de copyright et une adresse. Pour vous assurer que les utilisateurs entrent correctement ces informations, vous pouvez créer des paramètres prédéfinis de métadonnées. Le fait de choisir un paramètre prédéfini de métadonnées en mode Affichage des détails remplit les champs des métadonnées à l’aide de valeurs prédéfinies. Par exemple, un nom de propriétaire, une description de copyright et une adresse sont entrés de façon automatique.

Créez un paramètre prédéfini de métadonnées pour chaque ensemble de valeurs de métadonnées que vous souhaitez que les utilisateurs puissent entrer automatiquement en mode Affichage des détails pour décrire un fichier.

### Création ou modification d’un paramètre prédéfini de métadonnées {#creating-or-editing-a-metadata-preset}

1. Click **Setup** > **Application Setup** > **Metadata** > **Metadata Presets** .
1. Dans l’écran Paramètres prédéfinis de métadonnées, utilisez l’une des méthodes suivantes :

   * To create a preset, click **Add**. Dans le champ de texte Nom du modèle de métadonnées, saisissez le nom du paramètre prédéfini, puis cliquez sur Vues **de** métadonnées et choisissez une vue dans la liste déroulante (voir Vues [](application-setup.md#metadata_views)de métadonnées).
   * To edit an existing preset, select the preset from the Metadata Presets list and then click **Edit**.

1. Développez les en-têtes que vous souhaitez inclure dans le paramètre prédéfini et entrez les valeurs dans les différents champs que vous souhaitez inclure dans le paramètre prédéfini.
1. Cliquez sur **Enregistrer**.

   Les catégories et les champs sélectionnés pour le paramètre prédéfini sont visibles dans le panneau de prévisualisation.

### Gestion des paramètres prédéfinis des métadonnées {#managing-metadata-presets}

1. Click **Setup** > **Application Setup** > **Metadata** > **Metadata Presets**.
1. Utilisez l’une des méthodes suivantes :

   * Pour prévisualiser un paramètre prédéfini, sélectionnez ce dernier. Les informations correspondantes (catégories et champs) s’affichent dans l’écran de prévisualisation.
   * To delete a preset, select the preset, and then click **Delete**.

## Champs personnalisés {#user-defined-fields}

Un administrateur de portail multimédia ou un administrateur d’entreprise peut créer des champs de métadonnées définis par l’utilisateur personnalisés. Les champs personnalisés peuvent vous aider à organiser les fichiers dans Scene7 Publishing System. Si nécessaire, vous pouvez marquer les champs comme Actifs. Quand ils sont activés, les noms de ces champs de métadonnées personnalisés s’affichent dans le panneau Métadonnées de la vue de détails. Les utilisateurs peuvent renseigner les champs de métadonnées définies par les utilisateurs pour décrire les fichiers. Ils peuvent également définir un champ de métadonnées utilisateur comme critère de recherche.

Pour utiliser efficacement les champs de métadonnées définis par l’utilisateur, retardez l’heure d’activation d’un fichier pour un lancement ou une vente spécifique. Vous définissez un champ &quot;activation&quot;, en fonction du type *Date*. Then, using the **Metadata** panel in **Detail** view or **File** > **Edit Info**, you can specify when the asset is activated. Scene7 Publishing System vérifie l’état de publication d’un fichier, ainsi que l’historique de publication. S’il n’est pas dans le délai d’activation, l’état de publication s’affiche comme &quot;Non publié&quot;.

>[!NOTE]
>
>pour afficher les champs définis par les utilisateurs dans le panneau Métadonnées en mode Affichage des détails, incluez ces types de champs dans les vues des métadonnées. Dans l’écran Vues des métadonnées, sélectionnez l’option Include UDF (Inclure les champs définis par les utilisateurs). Pour plus d’informations, voir [Vues des métadonnées](application-setup.md#metadata_views).

>[!NOTE]
>
>Pour rechercher des fichiers en utilisant les champs personnalisés définis par les utilisateurs, cliquez sur **Configuration** > **Configuration personnelle**, puis sélectionnez **Inclure les champs définis par les utilisateurs dans la recherche**. Voir [Configuration personnelle](personal-setup.md#personal_setup).

### Création d’un champ de métadonnées défini par l’utilisateur {#creating-a-user-defined-metadata-field}

1. Cliquez sur **Configuration** > **Configuration de l’application** > **Métadonnées** > **Champs définis par l’utilisateur**.
1. Cliquez sur **Ajouter**.
1. Dans la boîte de dialogue Champ personnalisé, définissez les options de votre choix.

   **Nom** Entrez le nom du champ de métadonnées.

   **Type** Choisissez une option qui définit le type d’informations que les utilisateurs peuvent entrer dans le champ de métadonnées :

   **Chaîne** Chaîne de texte.

   **Int** An integer.

   **Flottant** Nombre à virgule flottante.

   **Oui/Non** Valeur booléenne oui/non.

   **Date** A date. Le format de date MM/JJ/AAAA est accepté.

   **Nom** de fichier Nom d’un fichier.

   **Couleur** Nom d’une couleur.

   **Dimension** Largeur et hauteur du fichier.

   **Non saisi** Pour une compatibilité ascendante. Ne sélectionnez pas cette option.

   **Valeur** par défaut (facultatif), entrez la valeur que les utilisateurs sont le plus susceptibles d’entrer dans le champ. La valeur que vous entrez devient la valeur par défaut du champ que vous créez.

   **S’applique** éventuellement, choisissez un type de fichier si vous souhaitez que le champ de métadonnées s’applique uniquement à un type de fichier spécifique.

   ***Note**: Choose an **Applies To** option carefully because you cannot change the **Applies To** option after you create a user-defined field. Dynamic Media Classic lets you edit the name, type, and default value of a user-defined field, but not the **Applies To** setting. *

1. Cliquez sur **Enregistrer** lorsque vous avez terminé de créer le champ de métadonnées.

### Gestion de champs définis par les utilisateurs {#manage-user-defined-fields}

L’écran Champs définis par l’utilisateur comporte des commandes qui permettent de gérer des champs de métadonnées personnalisés définis par les utilisateurs. 

Seul un administrateur du portail multimédia ou un administrateur d’entreprise peut gérer les champs définis par l’utilisateur.

Pour ouvrir cet écran, choisissez **Configuration** > **Configuration de l’application** > **Métadonnées** > **Champs définis par l’utilisateur**.

**Modification d’un champ** Sélectionnez le champ, puis cliquez sur **Modifier**.

**Suppression d’un champ** Sélectionnez le champ, puis cliquez sur **Supprimer**.

**Activer le champ** Cliquez pour sélectionner ou désélectionner l’option Actif en regard du nom d’un champ. Si vous êtes un administrateur dans la société, cette option peut ne pas s’afficher. Cette option étant liée à MediaPortal, vous devez sélectionner (activer) Afficher les fonctionnalités MediaPortal dans la configuration personnelle pour afficher les champs activés.

## Optimisation des fichiers {#optimize-files}

A mesure que vous téléchargez des fichiers dans Scene7 Publishing System, ils y sont optimisés pour leur stockage et leur publication. Toutefois, en cas d’interruption du processus de téléchargement, certaines images ne pourront pas être optimisées. Dans ce cas, le message « Image non optimisée » s’affiche. Vous pouvez cependant optimiser ces fichiers si vous êtes un administrateur.

Scene7 Publishing System lance une recherche sur vos fichiers pour n’optimiser que les images qui n’ont pas été entièrement optimisées auparavant.

1. Choisissez **Configuration** > Configuration **de l’** application, puis sélectionnez **Optimiser les fichiers**.
1. Enter information for the optimization job and click **Submit**.

   Si vous travaillez pour plusieurs sociétés, optimisez les fichiers des différentes entreprises séparément.

## Paramètres prédéfinis d’ensemble par lot {#batch-set-presets}

Utilisez les paramètres prédéfinis d’ensemble par lot pour créer automatiquement des visionneuses d’images ou des visionneuses à 360° pendant l’exécution d’une tâche de téléchargement de fichiers dans Scene7 Publishing System.

Les administrateurs d’entreprise définissent d’abord des conventions d’affectation de nom pour les fichiers qu’ils souhaitent regrouper dans un ensemble. Vous pouvez ensuite créer un paramètre prédéfini d’ensemble par lot pour référencer ces images. Chaque paramètre prédéfini correspond à un ensemble d’instructions indépendant à nom unique qui définit comment créer la visionneuse en utilisant des images correspondant aux conventions d’affectation de nom définies dans la recette de paramètres prédéfinis.

Tous les paramètres prédéfinis d’ensemble par lot actifs d’une entreprise sont répertoriés dans la boîte de dialogue Télécharger les options de la tâche. Ainsi, vous pouvez indiquer le paramètre prédéfini qui sera appliqué lors de chaque téléchargement. Les administrateurs d’entreprise verront tous les paramètres prédéfinis d’ensemble par lot actifs et inactifs. Lorsque vous téléchargez des fichiers, Dynamic Media Classic crée automatiquement une visionneuse contenant tous les fichiers qui correspondent à la convention d’affectation de nom définie dans les paramètres prédéfinis actifs.

### Affectation de nom par défaut {#default-naming}

L’administrateur d’entreprise crée une convention d’affectation de nom par défaut, qui est utilisée dans n’importe quelle recette de paramètres prédéfinis d’ensemble par lot. La convention d’affectation de nom par défaut sélectionnée dans la définition des paramètres prédéfinis d’ensemble par lot peut être la seule convention dont votre entreprise a besoin pour générer des visionneuses par lot pour tous les sites Web. Vous devez créer un paramètre prédéfini d’ensemble par lot pour utiliser la convention d’affectation de nom par défaut définie. Vous pouvez créer autant de paramètres prédéfinis d’ensemble par lot que nécessaire avec des conventions d’affectation de nom différentes et personnalisées pour une visionneuse de contenu spécifique au cas où il existe une exception dans l’affectation de nom par défaut définie par l’entreprise. 

Bien que la définition d’une convention d’affectation de nom par défaut ne soit pas nécessaire pour utiliser les paramètres prédéfinis d’ensemble par lot, il est recommandé d’utiliser la convention d’affectation de nom par défaut pour définir les éléments de votre convention d’affectation de nom que vous souhaitez regrouper dans une visionneuse afin de rationaliser la création d’ensembles par lot.

1. Cliquez sur **Configuration** > **Configuration de l’application** > **Paramètres prédéfinis d’ensemble par lot** > **Affectation de nom par défaut**.
1. Sélectionnez **Afficher le formulaire** ou **Afficher le code** pour indiquer comment afficher et saisir des informations sur chaque élément.

   Vous pouvez cocher la case Afficher le code pour afficher la valeur d’expression régulière à côté de vos sélections dans le formulaire. Vous pouvez saisir ou modifier ces valeurs pour définir les éléments de la convention d’affectation de nom si l’affichage sous forme de formulaire vous bloque pour quelque raison que ce soit. Si vos valeurs ne peuvent pas être analysées dans l’affichage sous forme de formulaire, les champs de formulaire seront inactifs.

   >[!NOTE]
   les champs de formulaire désactivés n’indiquent pas que l’expression régulière n’est pas valide. Aucune validation ne vous permet de confirmer que vos expressions régulières sont correctes. Vous verrez les résultats de l’expression régulière que vous créez pour chaque élément après la ligne Résultat. L’expression régulière est visible en entier en bas de la page.

1. Développez chaque élément selon vos besoins et indiquez les conventions d’affectation de nom que vous voulez utiliser.
1. Si nécessaire, cliquez sur **Ajouter** pour ajouter une autre convention d’appellation à un élément. Pour supprimer la convention d’appellation d’un élément, cliquez sur **Supprimer**.
1. Cliquez sur **Enregistrer sous** et saisissez un nom pour le paramètre prédéfini. Si vous modifiez un paramètre prédéfini existant, cliquez sur **Enregistrer**.

Vous pouvez également utiliser l’affichage du code sans champ de formulaire. Cet affichage vous permet de définir vos conventions d’affectation de nom en utilisant uniquement des expressions régulières.

Deux éléments sont disponibles pour la définition : Correspondance et Nom de base. Ces champs vous permettent de définir tous les éléments de la convention d’affectation de nom et d’identifier la partie de la convention utilisée pour nommer la visionneuse dans laquelle ils se trouvent. La convention d’affectation de nom individuelle d’une entreprise est susceptible d’utiliser une ou plusieurs lignes de définition pour chacun de ces éléments. Vous pouvez utiliser autant de lignes que vous le souhaitez pour votre définition unique et les regrouper dans des éléments distincts, par exemple pour l’image principale, l’élément Couleur, l’élément d’affichage secondaire et l’élément Echantillon.

### Création d’un paramètre prédéfini d’ensemble par lot {#creating-a-batch-set-preset}

Dynamic Media Classic utilise des paramètres prédéfinis d’ensemble par lot pour organiser les fichiers qui partagent des informations ou du contenu communs dans des visionneuses d’images en vue de les afficher dans les visionneuses. Les recettes de paramètres prédéfinis d’ensemble par lot s’exécutent automatiquement en même temps que les tâches d’importation de ressources planifiées dans Dynamic Media Classic.

Utilisez Paramètre prédéfini d’ensemble par lot pour créer, modifier et gérer vos paramètres prédéfinis d’ensemble par lot. Vous pouvez créer autant de paramètres prédéfinis d’ensemble par lot que vous le souhaitez pour couvrir l’ensemble des tâches d’assimilation des fichiers. Il existe deux formes de définition de paramètre prédéfini d’ensemble par lot : une pour la convention d’affectation de nom par défaut que vous avez définie et une pour les conventions d’affectation de nom personnalisées que vous créez en cas de besoin.

Pour définir un paramètre prédéfini d’ensemble par lot, utilisez la méthode de champ de formulaire ou la méthode de code, qui vous permet d’utiliser les expressions régulières. Tout comme pour l’affectation de nom par défaut, vous pouvez choisir d’afficher le code lorsque vous créez des définitions sous forme de formulaire et utiliser des expressions régulières pour créer vos définitions. Vous pouvez également désélectionner l’un des deux affichages pour utiliser uniquement l’un ou l’autre.

Voir également [Création d’un paramètre prédéfini d’ensemble par lot pour la génération automatique d’une visionneuse à 360° 2D](application-setup.md#creating_a_batch_set_preset_for_the_auto_generation_of_a_2d_spin_set).

**Création d’un paramètre prédéfini d’ensemble par lot**

1. Cliquez sur **Configuration** > **Configuration de l’application** > **Paramètres prédéfinis d’ensemble par lot** > **Paramètre prédéfini d’ensemble par lot**. La vue par défaut est la vue **Afficher le formulaire**, comme défini dans le coin supérieur droit de la page Détails.
1. Dans le panneau Liste des paramètres prédéfinis, cliquez sur **Ajouter** pour activer les champs de définition dans le panneau Détails situé sur la droite de l’écran.
1. Dans le panneau Détails, dans le champ Nom du paramètre prédéfini, nommez le paramètre prédéfini.
1. Dans le menu déroulant Type d’ensemble par lot, sélectionnez un type de paramètre prédéfini.

   Pour générer automatiquement une visionneuse à 360° 2D, sélectionnez **Visionneuse à 360° multi-axe** dans la liste déroulante Type d’ensemble par lot.

1. Effectuez l’une des opérations suivantes :

   * Si vous appliquez une convention d’affectation de nom par défaut que vous avez précédemment définie sous Configuration de l’application > Paramètres prédéfinis d’ensemble par lot > Affectation de nom par défaut, développez **Conventions d’affectation de nom** puis, dans la liste déroulante Affectation de nom de fichier, cliquez sur **Par défaut**.
   * Pour définir une convention d’affectation de nom quand vous configurez le paramètre prédéfini, développez **Conventions d’affectation de nom** puis, dans la liste déroulante Affectation de nom de fichier, cliquez sur **Personnalisé**.

1. Pour l’ordre des séquences, définissez l’ordre des images une fois que la visionneuse est regroupée dans Dynamic Media Classic. Par défaut, les fichiers seront classés par ordre alphanumérique. Cependant, vous pouvez utiliser une liste d’expressions courantes de format CSV (valeurs séparées par des virgules) pour définir l’ordre.
1. Dans Options de création et d’affectation de nom de l’ensemble, indiquez le suffixe ou le préfixe du nom de base que vous avez défini dans la convention d’affectation de nom. Définissez également l’emplacement de création de la visionneuse d’images dans la structure de dossiers Dynamic Media Classic.

   Si vous définissez un grand nombre de visionneuses d’images, vous préférerez sans doute les conserver séparément des dossiers contenant les fichiers. De nombreux utilisateurs créent un dossier Visionneuses d’images et configurent l’application de façon à ce qu’elle importe les visionneuses générées par lot à cet emplacement.

1. Cliquez sur **Enregistrer** dans le panneau Détails.

### Création d’un paramètre prédéfini d’ensemble par lot pour la génération automatique d’une visionneuse à 360° 2D {#creating-a-batch-set-preset-for-the-auto-generation-of-a-d-spin-set}

Utilisez le type d’ensemble par lot **Visionneuse à 360° multi-axe** pour créer une « recette » qui automatise la génération des visionneuses à 360° 2D. Le regroupement des images utilise les expressions régulières Ligne et Colonne afin que les fichiers d’image soient correctement alignés à l’emplacement correspondant dans le tableau multidimensionnel.

Voir également [Création d’un paramètre prédéfini d’ensemble par lot](application-setup.md#creating_a_batch_set_preset).

Il n’existe aucune limite minimale ou maximale quant au nombre de lignes ou de colonnes nécessaires dans la visionneuse à 360° multi-axe.

Par exemple, supposons que vous souhaitiez créer une visionneuse à 360° multi-axe nommée *spin-2dspin*. Vous disposez d’un ensemble d’images de la visionneuse à 360° qui contient trois lignes, avec 12 images par ligne. Les images sont nommées comme suit :

```as3
spin-01-01
spin-01-02
… 
spin-01-12
spin-02-01
… 
spin-03-12
```

Avec ces informations, vous pouvez créer votre recette de type d’ensemble par lot comme suit :

![](assets/se_batch_set_recipe.png)

Le regroupement de la partie du nom de ressource partagé de la visionneuse à 360° est ajouté au champ **Correspondance** (éléments en surbrillance). La partie variable du nom de ressource contenant la ligne et la colonne est ajoutée respectivement aux champs **Ligne** et **Colonne**.

Lorsque la visionneuse à 360° est téléchargée et publiée, vous activez le nom de la recette de visionneuse à 360° répertoriée sous **Paramètres prédéfinis d’ensemble par lot** dans la boîte de dialogue **Télécharger les options de la tâche**.

**Création d’un paramètre prédéfini d’ensemble par lot pour la génération automatique d’une visionneuse à 360° 2D.**

1. Sélectionnez **Configuration** > **Configuration de l’application** > **Paramètres prédéfinis d’ensemble par lot** > **Paramètre prédéfini d’ensemble par lot**. La vue par défaut est la vue **Afficher le formulaire**, comme défini dans le coin supérieur droit de la page Détails.
1. Dans le panneau Liste des paramètres prédéfinis, cliquez sur **Ajouter** pour activer les champs de définition dans le panneau Détails situé sur la droite de l’écran.
1. Dans le panneau Détails, dans le champ Nom du paramètre prédéfini, nommez le paramètre prédéfini.
1. Dans le menu déroulant Type d’ensemble par lot, sélectionnez **Visionneuse de ressources**.
1. Dans la liste déroulante Sous-type, sélectionnez **Visionneuse à 360° multi-axe**.
1. Développez les **Conventions d’affectation de nom** puis, dans la liste déroulante Affectation de nom de fichier, cliquez sur **Personnalisé**.
1. Utilisez les attributs **Correspondance** et, éventuellement, **Nom de base** pour définir une expression régulière pour nommer les fichiers d’image qui constituent le regroupement.

   Par exemple, votre expression régulière Correspondance littérale peut se présenter comme suit :

   `(\w+)-\w+-\w+`

1. Développez **Position des colonnes/lignes**, puis définissez le format de nom de la position du fichier d’image dans le tableau de la visionneuse à 360° 2D.

   Placez la position de ligne ou de colonne entre parenthèses dans le nom de fichier.

   Par exemple, l’expression régulière de ligne peut se présenter comme suit :

   `\w+-R([0-9]+)-\w+`

   ou

   `\w+-(\d+)-\w+`

   L’expression régulière de colonne peut se présenter comme suit :

   `\w+-\w+-C([0-9]+)`

   ou

   `\w+-\w+-C(\d+)`

   N’oubliez pas qu’il s’agit uniquement d’exemples. Vous pouvez créer votre expression régulière comme bon vous semble, en fonction de vos besoins.

   >[!NOTE]
   si la combinaison des expressions régulières de ligne et de colonne ne parvient pas à déterminer la position du fichier dans le tableau de visionneuse à 360° multidimensionnel, ce fichier n’est pas ajouté à la visionneuse et une erreur est enregistrée.

1. Dans Options de création et d’affectation de nom de l’ensemble, indiquez le suffixe ou le préfixe du nom de base que vous avez défini dans la convention d’affectation de nom. Définissez également l’emplacement de création de la visionneuse d’images dans la structure de dossiers Dynamic Media Classic.

   Si vous définissez un grand nombre de visionneuses d’images, vous préférerez sans doute les conserver séparément des dossiers contenant les fichiers. De nombreux utilisateurs créent un dossier Visionneuses d’images et configurent l’application de façon à ce qu’elle importe les visionneuses générées par lot à cet emplacement.

1. Cliquez sur **Enregistrer** dans le panneau Détails.
1. Téléchargez et publiez la visionneuse à 360° comme vous le faites habituellement, en veillant à activer le nom de la visionneuse à 360° 2D dans la boîte de dialogue Options de téléchargement de tâche, sous Paramètres prédéfinis d’ensemble par lot.

>[!MORELIKETHIS]
* [Prévisualisation d’un fichier](previewing-asset.md#previewing_an_asset)
* [Configuration des paramètres d’image prédéfinis](setting-image-presets.md#setting_up_image_presets)
* [Affichage, ajout et exportation de métadonnées](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
* [Vérification de fichiers de tâche](checking-job-files.md#checking_job_files)

