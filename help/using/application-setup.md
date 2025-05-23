---
title: Configuration de l’application
description: Découvrez comment configurer la zone Application d’Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
feature: Dynamic Media Classic
role: Admin
exl-id: 3f96606e-ef5c-4c01-aa0f-3148f14e28be
topic: Administration
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '10945'
ht-degree: 29%

---

# Configuration de l’application{#application-setup}

Vous pouvez utiliser les pages Configuration de l’application pour saisir des paramètres généraux, créer des paramètres d’image prédéfinis, des paramètres de codage vidéo prédéfinis, des paramètres de visionneuse prédéfinis ou définir des visionneuses par défaut et des métadonnées. Vous pouvez configurer des paramètres prédéfinis d’ensemble par lot afin qu’ils automatisent la génération de visionneuses à 360° en 2D (par exemple), de paramètres de publication et de paramètres d’optimisation pour les moteurs de recherche vidéo.

>[!NOTE]
>
>Seuls les administrateurs Adobe Dynamic Media Classic peuvent modifier les paramètres dans la configuration de l’application.

## Paramètres généraux {#general-settings}

Pour ouvrir la page Paramètres généraux de l’application, dans la barre de navigation globale, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Paramètres généraux]**.

### Serveurs

Lors de la création du compte, Adobe Dynamic Media Classic fournit automatiquement les serveurs attribués à votre entreprise. Ces serveurs sont utilisés pour créer des chaînes URL pour votre site Web et vos applications. Ces appels d’URL sont spécifiques à votre compte.

Voir aussi [Test du service Secure Testing](testing-assets-making-them-public.md#testing_the_secure_testing_service).

* **[!UICONTROL Nom du serveur publié]** : ce serveur est le serveur CDN actif (réseau de diffusion de contenu) utilisé dans tous les appels d’URL générés par le système et spécifiques à votre compte. Modifiez ce nom de serveur uniquement si un technicien de l’assistance Adobe Dynamic Media Classic vous demande de le faire.

* **[!UICONTROL Nom du serveur d’origine]** : ce serveur est utilisé uniquement pour les tests d’assurance qualité. Modifiez ce nom de serveur uniquement si un technicien de l’assistance Adobe Dynamic Media Classic vous demande de le faire.

<!-- **AGM Server Name** This server is used for Web-to-Print templates. This server is set on a company-wide basis. Do not change this server name unless instructed to do so by an Adobe DynamicMedia Classic support technician. -->

* **[!UICONTROL Nom du serveur Test&amp;Target]** : URL Test&amp;Target, y compris `.com`. Pour plus d&#39;informations sur l&#39;obtention de cette URL, voir Intégration de [!DNL Adobe Dynamic Media Classic] à [!DNL Adobe Target Standard/Premium].

<!-- **Test Publish Context Server Name** -->

* **[!UICONTROL Nom du serveur de diffusion en continu iOS]** : URL de votre serveur de diffusion en continu iOS [!DNL Adobe Dynamic Media Classic]. Ce serveur diffuse des vidéos en continu vers les appareils iOS à l’aide du protocole HTTP.

* **[!UICONTROL Nom du serveur de vidéo progressive]** : URL de votre serveur de vidéo progressive [!DNL Adobe Dynamic Media Classic]. Ce serveur fournit une vidéo progressive à l’aide du protocole HTTP.

* **[!UICONTROL Afficher l’URL des ressources non publiées]** : sélectionnez cette option si vous souhaitez que [!DNL Adobe Dynamic Media Classic] affiche une URL lorsque vous prévisualisez une ressource, publiée ou non. Si le fichier n’est pas publié, l’URL ne fonctionne pas. Vous pouvez, cependant, utiliser l’URL à des fins de planification ou d’organisation.

<!-- **Allow AIR install** Select this option to allow users to download Adobe Dynamic Media Classic desktop version to their local hard drives. Users install the application from the Desktop Version area of the Personal Setup screen. -->

<!-- AIR users must manually uninstall their existing app and reinstall from the Web version of Adobe Dynamic Media Classic (in Personal Settings). After this one-time reinstallation, you are prompted to upgrade whenever the server has a newer version of Adobe Dynamic Media Classic AIR. Adobe Dynamic Media Classic is integrated with the Application Update Framework which streamlines the upgrade process. -->

* **[!UICONTROL Modèle d’invalidation du réseau de diffusion de contenu]** : spécifie le modèle utilisé pour invalider le cache du réseau de diffusion de contenu.

  Par exemple, supposons que vous saisissiez une URL d’image (y compris des paramètres d’image prédéfinis ou des modificateurs) faisant référence à `<ID>`, au lieu d’un ID d’image spécifique, comme dans l’exemple suivant :

  `https://sample.scene7.com/is/image/Company/<ID>?$s7product$`

  Si le modèle contient uniquement `<ID>`, Adobe Dynamic Media Classic renseigne `https://<server>/is/image`, où `<server>` est le nom du serveur de publication défini dans les paramètres généraux.

  Si vous définissez le modèle d’invalidation du réseau CDN, sélectionnez une image nommée Backpack_B, puis accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Invalider sur le réseau de diffusion de contenu]** , l’URL générée suivante s’affiche dans l’interface d’invalidation du réseau CDN :

  `https://sample.scene7.com/is/image/Company/Backpack_B?$s7product$`

  Dans la zone de liste URL, sélectionnez **[!UICONTROL Continuer]** pour effacer le cache de cet appel d’URL d’image spécifique. Vous pouvez également ajouter des URL en les saisissant ou en les collant dans la zone de liste URL ; il n’est pas nécessaire de définir le modèle au préalable.

  Après avoir sélectionné votre modèle d’invalidation du réseau de diffusion de contenu et effectué une requête d’invalidation du réseau de diffusion de contenu, un indicateur s’affiche dans l’interface utilisateur. Vous obtenez une estimation du temps nécessaire pour effacer le cache.

  Lorsque vous cliquez sur **[!UICONTROL Fichier]** > **[!UICONTROL Invalider le CDN]**, chaque image est référencée dans l’URL du modèle enregistrée si plusieurs images sont sélectionnées dans Dynamic Media Classic. Par conséquent, vous pouvez définir un modèle d’invalidation CDN référençant chaque URL référencée sur votre site Web (comme les détails du produit et les résultats de recherche). Ensuite, lorsque vous sélectionnez une ou plusieurs images à invalider dans le cache, les URL renseignent automatiquement l’interface.

  Voir [Mise en cache du contenu](dmc-platform-overview.md#content_caching).

  Voir [Fichiers republiés et délais CDN](publishing-files.md#republished_assets_and_cdn_delays).

### Parcourir

* **[!UICONTROL Afficher les projets]** : détermine si des projets sont disponibles pour organiser vos ressources Adobe Dynamic Media Classic. Voir [Organiser votre travail avec les projets](/help/using/organizing-projects.md).

* **[!UICONTROL Afficher l’exemple de contenu eVideo]** : activez ou désactivez l’affichage de l’exemple de contenu eVideo.

* **[!UICONTROL Afficher le contenu généré]** : dans les dossiers, il affiche le contenu généré à partir d’une ressource. Par exemple, lorsqu’un fichier de PDF est pixellisé au fur et à mesure de son chargement, Adobe Dynamic Media Classic crée une image pour chaque page du PDF d’origine. Si l’option Afficher le contenu généré est sélectionnée, chaque image générée lorsque le PDF d’origine est téléchargé s’affiche. Il apparaît avec le PDF dans le dossier dans lequel le PDF a été chargé.

* **[!UICONTROL Afficher les vidéos codées]** : désélectionnée par défaut.

  Vous pouvez rechercher et parcourir rapidement des vidéos dans Adobe Dynamic Media Classic sans avoir à parcourir de nombreux dérivés codés de la même vidéo. Laissez cette option désélectionnée (par défaut). Seule la miniature de la vidéo Principal (la vidéo source que vous avez téléchargée et utilisée pour créer les dérivés) et la miniature de la visionneuse de vidéos adaptative &quot;parente&quot; (qui contient les dérivés &quot;enfants&quot; de la visionneuse de vidéos codées) s’affichent.

  Vous pouvez toutefois accéder à des vidéos codées individuelles à partir de la vidéo par Principal ou de la visionneuse de vidéos adaptative. Pour ce faire, double-cliquez sur l’image miniature de la vidéo pour passer en mode Affichage des détails. Sélectionnez ensuite **[!UICONTROL Vidéos codées]** dans le panneau de droite pour accéder à toutes les vidéos &quot;enfants&quot;.

  Vous pouvez également accéder à **[!UICONTROL Fichier]** > **[!UICONTROL Retraiter]** pour créer d’autres vidéos &quot;enfants&quot; codées directement à partir d’une visionneuse de vidéos adaptative. Adobe Dynamic Media Classic recherche automatiquement la vidéo de Principal &quot;parent&quot; de la visionneuse de vidéos adaptative et l’utilise comme vidéo source pour le transcodage. Cependant, lorsque vous enregistrez les nouvelles vidéos codées individuelles, elles ne sont pas visibles lors d’une recherche ou d’une navigation. Elles restent néanmoins accessibles à partir de l’onglet Vidéos codées dans la vue Affichage des détails.

  Voir [Téléchargement et transcodage de vidéos](uploading-encoding-videos.md#uploading_and_encoding_videos).

  Pour continuer à accéder à toutes les vidéos codées dérivées lors d’une recherche ou d’une navigation, sélectionnez **[!UICONTROL Afficher les vidéos codées]**.

  Certaines actions du menu Créer ne fonctionnent qu’avec des vidéos individuelles. C’est la raison pour laquelle il est nécessaire d’afficher toutes les vidéos codées dérivées pouvant être sélectionnées, quelle que soit la façon dont vous définissez le paramètre **[!UICONTROL Afficher les vidéos codées]**. Les actions de création qui remplacent le paramètre **[!UICONTROL Afficher les vidéos codées]** incluent **[!UICONTROL visionneuses de vidéos adaptatives]** et **[!UICONTROL catalogues électroniques]**.

  >[!NOTE]
  >
  >Si vous n’avez pas utilisé Adobe Dynamic Media Classic pour charger et coder vos ressources vidéo, Adobe Dynamic Media Classic affiche toutes vos vidéos codées individuelles, même si cette option est désélectionnée.

* **[!UICONTROL Afficher le bouton d’actualisation des sous-dossiers]** : activez ou désactivez l’affichage du bouton d’actualisation des sous-dossiers.

### Compte FTP Adobe Dynamic Media Classic

* **[!UICONTROL Serveur]** : répertorie votre serveur de compte FTP.

* **[!UICONTROL Nom d’utilisateur]** : répertorie le nom d’utilisateur de votre compte FTP.

### Télécharger dans l’application

Voir aussi la vidéo de formation [Options pour les tâches de chargement](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/569_Default%20Job%20Options_converted%20renamed_Getting%20Started-AVS).

* **[!UICONTROL Remplacer les images]** : Adobe Dynamic Media Classic ne permet pas que deux fichiers portent le même nom. L’Adobe Dynamic Media Classic ID de chaque élément (le nom de l’image sans l’extension de nom de fichier) doit être unique. De par cette règle, la boîte de dialogue Télécharger contient une option Ecraser. L’effet précis de cette option dépend de l’option Ecraser les images spécifiée. Ces options spécifient la manière dont les images de remplacement sont téléchargées : elles peuvent remplacer les images d’origine ou devenir des doublons. Les images en double sont renommées par &quot;-1&quot; (par exemple, chaise.tif est renommé chaise-1.tif). Ces options affectent les images téléchargées dans un dossier autre que le dossier d’origine ou les images dont l’extension est différente de celle du fichier d’origine (telle que JPG, TIF ou encore PNG) Voir [Utiliser l’option Remplacer les images](#using-the-overwrite-images-option).

   * **[!UICONTROL Écraser dans dossier actuel, même nom ou même extension de fichier de base]** : cette option est la règle la plus stricte pour le remplacement. Elle nécessite que vous téléchargiez l’image de remplacement dans le même dossier que l’image d’origine, et qu’elle ait la même extension que le fichier d’origine. Si ces conditions ne sont pas remplies, un doublon est créé.

   * **[!UICONTROL Écraser dans le dossier actuel, même nom de fichier, extension indépendante]** : nécessite que vous téléchargiez l’image de remplacement dans le même dossier que l’original, mais l’extension du nom de fichier peut être différente de celle de l’original. Par exemple, chaise.tif peut remplacer chaise.jpg.

   * **[!UICONTROL Écraser dans un dossier, même nom ou même extension de fichier]** : nécessite que l’image de remplacement ait la même extension que l’image d’origine. Par exemple, chaise.jpg doit remplacer chaise.jpg, et non chaise.tif). Vous pouvez toutefois télécharger l’image de remplacement dans un dossier différent de celui de l’image d’origine. L’image mise à jour se trouve dans le nouveau dossier, et le fichier d’origine n’est plus disponible à l’emplacement d’origine.

   * **[!UICONTROL Écraser dans un dossier, même nom de fichier, extension indépendante]** : cette option est la règle de remplacement la plus inclusive. Elle vous permet de télécharger une image de remplacement dans un dossier autre que celui de l’image d’origine, de télécharger un fichier dont l’extension est différente de celle du fichier d’origine et de remplacer le fichier d’origine. Si le fichier d’origine se trouve dans un dossier différent, l’image de remplacement est enregistrée dans le dossier où elle a été téléchargée.

* **[!UICONTROL Retain Publish]** : indique si une image de remplacement chargée dans Adobe Dynamic Media Classic conserve le paramètre Ready to Publish de l’image qu’elle remplace. Ou, le paramètre est spécifié lors du téléchargement.

* **[!UICONTROL Profils de couleurs par défaut]** : spécifie les profils de couleurs appliqués dans le cadre des options de profil de couleurs par défaut lors de l’ajout d’images CMJN.

* **[!UICONTROL Options de téléchargement par défaut]** : ouvre la boîte de dialogue Télécharger les options de la tâche, dans laquelle vous pouvez spécifier les options de téléchargement par défaut. Pour plus d’informations sur ces options, voir [Options de téléchargement](/help/using/uploading-files.md#upload_options).

### Éditeur de zone cliquable (vers application)

* **[!UICONTROL Mappage d’images par défaut HREF]** : définit l’URL par défaut utilisée pour la colonne HREF dans le mappage d’images. Cette URL est l’URL par défaut qui s’affiche lors de la création de zones cliquables.

* **[!UICONTROL Modèle de mappage d’images par défaut]** : définit le JavaScript par défaut du modèle HREF dans le mappage d’images. Vous pouvez définir ici un code personnalisé à exécuter chaque fois que vous sélectionnez une zone cliquable.

### Autres paramètres (vers application)

* **[!UICONTROL La corbeille peut nettoyer les avertissements]** : Assets dans la corbeille est automatiquement supprimé dans les sept jours. Sélectionnez &quot;Envoyer des emails avant que les éléments de la corbeille ne soient automatiquement supprimés&quot; pour que les notifications soient envoyées aux administrateurs de l’entreprise lorsque les ressources qui se trouvent dans la corbeille sont à quatre jours de la suppression définitive. Voir [Gestion du dossier Corbeille](/help/using/trash-folder.md).

## Utilisation de l’option Remplacer les images {#using-the-overwrite-images-option}

Adobe Dynamic Media Classic ne permet pas que deux fichiers portent le même nom. L’Adobe Dynamic Media Classic ID de chaque élément (le nom de l’image sans l’extension de nom de fichier) doit être unique. De par cette règle, la boîte de dialogue Télécharger contient des options Ecraser les images. L’effet exact de cette option dépend d’un paramètre pour les paramètres internes Adobe Dynamic Media Classic de chaque entreprise.

Si vous avez précédemment téléchargé des images, puis modifié les fichiers d’origine (ou les avez remplacés), l’option Écraser sélectionnée indique comment Adobe Dynamic Media Classic remplace les images. Aucune donnée sur l’image ne change, mais la nouvelle image remplace l’ancienne. Si le dossier contient également des images qui ne se trouvent pas déjà dans Adobe Dynamic Media Classic, ces images sont ajoutées.

Utilisez cette option si les images téléchargées ont changé d’une manière ou d’une autre (l’image a été modifiée), mais que la référence à l’image reste la même. Le remplacement s’avère également utile lors du chargement et de l’extraction de PDF d’Adobe®. Vous pouvez affiner la façon dont Adobe Dynamic Media Classic *déchire* l’image. Vous pouvez également ajuster les options de profil de couleur ICC dans la boîte de dialogue Télécharger et effectuer un nouveau chargement à l’aide de la fonction de remplacement.

Les Adobe Dynamic Media Classic ID utilisés pour accéder aux images à partir des serveurs de production sont dérivés des noms de fichier image. L’utilisation de caractères majuscules et minuscules dans le nom de fichier est importante, tant pour le remplacement de fichiers existants que pour les Adobe Dynamic Media Classic ID utilisés pour accéder à l’image. L’utilisation de noms de fichier avec des caractères majuscules et minuscules est correcte avant le chargement dans Adobe Dynamic Media Classic afin d’éviter que les Adobe Dynamic Media Classic ID ne diffèrent que par le cas d’une même image.

Si vous désactivez cette option, toutes les images dont les noms sont identiques à des images existantes sont considérées comme des doublons et ne sont donc pas ajoutées.

## Paramètres d’image prédéfinis {#image-presets}

L’écran Paramètres d’image prédéfinis sert à créer et à modifier les paramètres d’image prédéfinis. Les paramètres d’image prédéfinis permettent à Adobe Dynamic Media Classic de diffuser des images dynamiquement à des tailles différentes à partir d’une même image principale. Chaque paramètre d’image prédéfini forme un ensemble prédéfini de commandes de dimensionnement et de formatage permettant d’afficher les images. Lorsque vous créez un paramètre d’image prédéfini, vous sélectionnez une taille pour la diffusion de l’image. Vous pouvez également sélectionner des commandes de formatage afin d’optimiser l’aspect de l’image lors de sa diffusion.

Les administrateurs peuvent créer des paramètres prédéfinis pour l’exportation de fichiers. Les utilisateurs peuvent choisir un paramètre prédéfini lorsqu’ils exportent des images, qui reformate également les images selon les spécifications définies par l’administrateur.

Pour ouvrir l’écran Paramètre d’image prédéfini, dans la barre de navigation globale, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Paramètres d’image prédéfinis]**.

Voir [Imagerie dynamique](https://experienceleague.adobe.com/fr/docs/experience-manager-65/content/assets/dynamic/imaging-faq).

### Création et modification des paramètres d’image prédéfinis {#creating-and-editing-image-presets}

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Paramètres d’image prédéfinis]**.
1. Créez un paramètre prédéfini ou démarrez à partir d’un paramètre existant :

   * **Créer un paramètre d’image prédéfini** : sélectionnez **[!UICONTROL Ajouter]**.
   * **Créer un paramètre d’image prédéfini à partir d’un paramètre prédéfini existant** : sélectionnez le paramètre d’image prédéfini qui ressemble le plus à celui que vous souhaitez créer, puis sélectionnez **[!UICONTROL Modifier]**.

1. Sur la page Ajouter (ou Modifier) un paramètre prédéfini , saisissez le nom du paramètre prédéfini.
1. Définissez les options de paramètres prédéfinis de votre choix. 

   Voir [Options des paramètres d’image prédéfinis](application-setup.md#image_preset_options).

1. Sélectionnez **[!UICONTROL Enregistrer]** ou, si vous avez commencé à partir d’un paramètre prédéfini existant, sélectionnez **[!UICONTROL Enregistrer sous]**.
1. Pour prévisualiser le paramètre prédéfini avec votre propre image, sélectionnez **[!UICONTROL Parcourir]**, puis sélectionnez une image. Pour prévisualiser avec l’image par défaut, sélectionnez **[!UICONTROL Réinitialiser]**.

Vous pouvez modifier un paramètre d’image prédéfini en sélectionnant son nom dans l’écran Paramètres d’image prédéfinis, puis en sélectionnant **[!UICONTROL Modifier]**. Pour supprimer un paramètre d’image prédéfini, sélectionnez-le, puis sélectionnez **[!UICONTROL Supprimer]**.

### Options des paramètres d’image prédéfinis {#image-preset-options}

Les écrans Ajouter un paramètre prédéfini et Modifier le paramètre prédéfini mettent à votre disposition les options suivantes pour créer et modifier les paramètres d’image prédéfinis :

* **[!UICONTROL Nom du paramètre prédéfini]** : saisissez un nom descriptif sans espaces vides. Pour aider les utilisateurs à identifier ce paramètre d’image prédéfini, incluez la spécification de taille de l’image dans le nom.

* **[!UICONTROL Largeur et hauteur]** : saisissez en pixels la taille à laquelle l’image est diffusée.

* **[!UICONTROL Format]** : sélectionnez un format dans le menu. Le choix du format GIF, JPEG, PDF ou TIFF offre d’autres options :

   * Options Quantification de couleurs GIF

      * **[!UICONTROL Type]** : sélectionnez Adaptatif (valeur par défaut), Web ou Mac. Si vous sélectionnez **[!UICONTROL GIF avec Alpha]**, l’option Mac n’est pas disponible.

      * **[!UICONTROL Dither]** : sélectionnez Diffus ou Désactivé.

      * **[!UICONTROL Nombre de couleurs]** : faites glisser le curseur pour entrer entre 2 et 255.

      * **[!UICONTROL Liste de couleurs]** : entrez une liste séparée par des virgules. Par exemple, pour le blanc, le gris et le noir, saisissez `000000,888888,ffffff`.

   * Options JPEG

      * **[!UICONTROL Qualité]** : contrôle le niveau de compression du JPEG. Ce paramètre affecte à la fois la taille du fichier et la qualité de l’image. L’échelle de qualité JPEG s’étend de 1 à 100.

      * **[!UICONTROL Activer le sous-échantillonnage de la chrominance JPG]** : comme l’oeil est moins sensible aux informations colorimétriques à haute fréquence qu’à la luminance à haute fréquence, les images de JPEG divisent les informations d’image en composantes de luminance et de couleur. Lorsqu’une image JPEG est compressée, la composante de luminance conserve sa pleine résolution, tandis que les composantes de couleur sont sous-échantillonnées par interpolation, c’est-à-dire le calcul de la moyenne de groupes de pixels. Le sous-échantillonnage réduit le volume des données d’un demi-tiers ou d’un tiers, sans pratiquement avoir d’incidence sur la qualité perçue. La réduction de résolution ne s’applique pas aux images en niveaux de gris. Cette technique réduit le niveau de compression nécessaire pour les images présentant un contraste élevé (par exemple, les images contenant du texte superposé).

   * Options PDF et TIFF

      * **[!UICONTROL Compression]** : sélectionnez un algorithme de compression.

* **[!UICONTROL Colorspace]** : sélectionnez un espace colorimétrique.

* **[!UICONTROL Accentuation]** : sélectionnez l’option Activer l’accentuation simple pour appliquer un filtre d’accentuation de base à l’image à l’issue des opérations de mise à l’échelle. L’accentuation peut compenser le flou produit lors de l’affichage d’une image à une taille différente. 

  Pour plus d’informations sur l’accentuation, les modes de rééchantillonnage et le masquage flou, voir [Accentuer une image](sharpening-image.md#sharpening_an_image). Voir aussi la vidéo de formation [Accentuation](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/547_sharpening1_converted%20renamed_Done-AVS).

* **[!UICONTROL Mode Rééchantillonnage]** : sélectionnez une option Mode Rééchantillonnage. Les options suivantes permettent d’accentuer l’image lorsque sa résolution est réduite :

* **[!UICONTROL B-Linear]** : méthode de rééchantillonnage la plus rapide ; certains artefacts de crénelage sont visibles.

* **[!UICONTROL Bicubique]** : accroît l’utilisation du processeur sur le serveur d’images, mais produit des images plus nettes avec des artefacts de crénelage plus discrets.

* **[!UICONTROL `Sharp 2`]** : peut produire des résultats légèrement plus nets que l’option Bicubique, mais avec un coût processeur encore plus élevé sur le serveur d’images.

* **[!UICONTROL Tri-Linear]** : utilise des résolutions supérieure et inférieure, si elles sont disponibles ; recommandé uniquement lorsque le crénelage est un problème. Elle réduit la taille du fichier JPEG en raison des données à haute fréquence réduites.

* **[!UICONTROL Masquage flou]** : sélectionnez ces options pour affiner l’accentuation :

* **[!UICONTROL Quantité]** : contrôle le degré de contraste appliqué aux pixels de contour. La valeur par défaut est de 1. Pour des images à haute résolution, vous pouvez l’augmenter jusqu’à 5. Imaginez la quantité comme étant l’unité de mesure de l’intensité du filtre.

* **[!UICONTROL Rayon]** : détermine le nombre de pixels entourant les pixels de contour qui affectent l’accentuation. Pour les images à haute résolution, entrez une valeur comprise entre 1 et 2. Une valeur faible renforce uniquement les pixels de contour, tandis qu’une valeur élevée traite une plus large bande de pixels. La valeur appropriée dépend de la taille de l’image.

* **[!UICONTROL Seuil]** : détermine la plage de contraste à ignorer lorsque le filtre de masquage flou est appliqué. En d’autres termes, cela peut aider à résoudre l’écart recherché entre les pixels accentués et la zone environnante avant qu’ils ne soient considérés comme des pixels de contour et accentués. Pour éviter d’introduire du bruit, essayez des valeurs comprises entre `.02` et `0.2`. La valeur par défaut de 6 accentue tous les pixels de l’image.

* **[!UICONTROL Espace colorimétrique]** : détermine si l’image utilise l’espace dans lequel l’image a été créée, généralement RGB (original) ou un espace de luminance (intensité).

* **[!UICONTROL Color]** Choisissez les options suivantes :

* **[!UICONTROL Profil de couleurs de sortie]** : sélectionnez **[!UICONTROL Utiliser la valeur par défaut]** ou l’un des profils de couleurs ICC disponibles dans Adobe Dynamic Media Classic.

  (voir aussi [Profils ICC](icc-profiles.md#icc_profiles)).

* **[!UICONTROL Intention de rendu]** : sélectionnez une option si vous souhaitez remplacer l’intention de rendu par défaut du profil de couleur. Utilisez cette option lorsque l’un des profils ICC par défaut est l’espace colorimétrique cible d’une conversion de couleurs. Ou, ce profil caractérise le périphérique de sortie (imprimante ou moniteur), et l’intention de rendu spécifiée est valide pour ce profil.

* **[!UICONTROL Intégrer le profil]** : sélectionnez cette option de sorte que, si vous ouvrez cette image dans Adobe® Photoshop®, elle utilise ce profil.

* **[!UICONTROL Résolution d’impression]** : sélectionnez une résolution pour l’impression de cette image ; 72 pixels est la résolution par défaut.

* **[!UICONTROL Modificateurs d’URL]** : si vous préférez spécifier les modificateurs d’URL qui définissent votre paramètre d’image prédéfini, plutôt que les paramètres, saisissez les modificateurs ici.

* **[!UICONTROL Exemple d’URL d’image]** : répertorie la chaîne d’URL &quot;brute&quot; utilisée par le serveur d’images Dynamic Media pour diffuser des images avec le paramètre d’image prédéfini que vous ajoutez ou modifiez. Cette chaîne URL code tous les paramètres de format que vous sélectionnez dans l’écran Ajouter un paramètre prédéfini ou Modifier le paramètre prédéfini .

### Modifier, supprimer ou désactiver un paramètre d’image prédéfini {#editing-removing-or-deactivating-an-image-preset}

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Paramètres d’image prédéfinis]**.
1. Dans l’écran Paramètres d’image prédéfinis, sélectionnez un paramètre prédéfini dans le tableau, puis effectuez l’une des opérations suivantes :

   * Sélectionnez **[!UICONTROL Modifier]**, puis spécifiez de nouvelles options dans la boîte de dialogue Modifier le paramètre prédéfini.
   * Sélectionnez **[!UICONTROL Supprimer]** pour supprimer le paramètre prédéfini de la liste.
   * Décochez la case **[!UICONTROL Actif]** en regard d’un nom de paramètre prédéfini si vous souhaitez le supprimer de l’interface utilisateur complète d’Adobe Dynamic Media Classic pour les utilisateurs de MediaPortal.

## Activation ou désactivation des paramètres prédéfinis de vidéo adaptative {#activating-or-deactivating-adaptive-video-presets}

Adobe Dynamic Media Classic propose des paramètres prédéfinis de codage vidéo adaptatif. Il s’agit d’une liste principale de paramètres prédéfinis qui combine en un seul groupe les paramètres prédéfinis de vidéo adaptative 16:9 et les paramètres prédéfinis de vidéo adaptative 4:3. Ces paramètres prédéfinis représentent les paramètres de codage les plus courants et sont optimisés pour la lecture sur périphériques mobiles, tablettes cibles et ordinateurs.

Seuls les paramètres prédéfinis de codage &quot;Vidéo adaptative&quot; sont activés par défaut. Vous pouvez les désactiver, si vous le souhaitez. Les paramètres prédéfinis de vidéo adaptative inactifs n’apparaissent pas sous forme d’option sélectionnable dans la section eVideo de la boîte de dialogue Télécharger les options de la tâche.

Voir [Téléchargement et codage de vidéos](uploading-encoding-videos.md#uploading_and_encoding_videos).

Voir aussi la vidéo de formation [Paramètres vidéo prédéfinis](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS).

**Pour activer ou désactiver les paramètres prédéfinis de vidéo adaptative :**

1. Près du coin supérieur droit d’Adobe Dynamic Media Classic, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Paramètres vidéo prédéfinis]** > **[!UICONTROL Paramètres vidéo prédéfinis adaptatifs]**.
1. Sur la page Paramètres prédéfinis de vidéo adaptative, décochez la case située en regard du nom d’un paramètre prédéfini à supprimer de la liste Options eVideo figurant dans la boîte de dialogue Télécharger les options de la tâche.
1. Sélectionnez **[!UICONTROL Fermer]**.

## Paramètres vidéo prédéfinis pour le codage des fichiers vidéo {#video-presets-for-encoding-video-files}

Pour sélectionner un paramètre prédéfini de codage, dans le coin inférieur droit de la page Télécharger, sélectionnez **[!UICONTROL Options de tâche]**. Dans la boîte de dialogue Télécharger les options de la tâche, développez Options eVideo et sélectionnez les paramètres prédéfinis de codage vidéo de votre choix.

>[!NOTE]
>
>À l’exception de &quot;Vidéo adaptative&quot;, qui est activée par défaut, vous ne pouvez pas voir tous les autres paramètres prédéfinis de codage vidéo ou adaptatif dans la boîte de dialogue Télécharger les options de la tâche. Les administrateurs Adobe Dynamic Media Classic déterminent quels paramètres prédéfinis de codage vidéo sont visibles dans la boîte de dialogue Télécharger les options de la tâche .

* Sélectionnez l’un des paramètres prédéfinis de codage de vidéo adaptative ou de codage unique suivants :

   * **[!UICONTROL Vidéo adaptative 16:9]** : créez des vidéos de format 16:9 pour une diffusion sur les ordinateurs de bureau, les appareils mobiles (iPhone, iPad, Android™) et les tablettes (iPad, Android™), optimisées avec la résolution et le débit qui correspondent le mieux à la vitesse de connexion de la visionneuse.

   * **[!UICONTROL Vidéo adaptative 4:3]** : créez des vidéos 4:3 de rapport largeur/hauteur pour une diffusion sur les ordinateurs de bureau, les appareils mobiles (iPhone, iPad, Android™) et les tablettes (iPad, Android™), optimisées avec la résolution et le débit qui correspondent le mieux à la vitesse de connexion de la visionneuse.

   * **[!UICONTROL Vidéo adaptative]** : paramètre prédéfini à codage unique qui fonctionne avec n’importe quel rapport d’aspect pour créer des vidéos à diffuser sur mobile, tablette et ordinateur de bureau. Les vidéos source transférées qui sont codées à l’aide de ce paramètre prédéfini sont définies avec une hauteur fixe. Toutefois, la largeur est automatiquement mise à l’échelle afin de préserver les proportions de la vidéo.

     Cette flexibilité d’une &quot;mise à l’échelle automatique&quot; est également disponible par défaut lorsque vous créez votre propre paramètre prédéfini de codage vidéo personnalisé.

     Voir [Ajout ou modification d’un paramètre prédéfini de codage vidéo](uploading-encoding-videos.md#adding_or_editing_a_video_encoding_preset).

   * **[!UICONTROL Codage vidéo adaptatif (16:9 ou 4:3)]** : créez des vidéos aux proportions 16:9 et 4:3 pour une diffusion sur les ordinateurs de bureau, les appareils mobiles (iPhone, iPad, Android™) et les tablettes (iPad, Android™). Toutes optimisées avec la résolution et le débit qui correspondent le mieux à la vitesse de connexion de la visionneuse.

     Voir [Paramètres prédéfinis de codage de vidéo adaptative (16:9 ou 4:3)](application-setup.md#adaptive_video_encoding_16_9_or_4_3_video_presets).

   * **[!UICONTROL Paramètres prédéfinis de codage uniques]**

     >[!NOTE]
     >
     >Pour diffuser une vidéo sur iPad, vous pouvez sélectionner un paramètre prédéfini de codage mobile ou un paramètre prédéfini de codage tablette. Les paramètres prédéfinis Tablette sont spécialement conçus pour l’iPad, généralement avec une meilleure résolution et une qualité supérieure pour tirer parti de l’écran plus large et de la connexion à bande passante plus puissante. Afin de diffuser des fichiers vidéo codés avec un paramètre prédéfini Tablette, vous devez inclure un code de détection de périphérique sur votre site ou application mobile. Ce code bascule entre une expérience vidéo iPhone ou iPad, selon le périphérique de lecture. Le choix d’un paramètre prédéfini Mobile pour la diffusion de fichiers vidéo sur l’iPad représente un flux de travail plus simple, car vous pouvez utiliser le même fichier vidéo pour les iPhones et les iPads. En revanche, la qualité est normalisée sur la résolution iPhone, qui est inférieure.

      * Sous le groupe Paramètres prédéfinis de codage , dans la liste déroulante Trier les paramètres prédéfinis de codage, sélectionnez Nom ou Taille pour trier les paramètres prédéfinis par nom ou taille de résolution.
      * Sélectionnez un paramètre prédéfini de codage en fonction de la taille de résolution et de la bande passante avec lesquelles vous prévoyez de lire la vidéo.
      * Vous pouvez sélectionner Codage vidéo adaptatif et un ou plusieurs paramètres prédéfinis de codage par vidéo. Par exemple, vous pouvez coder un fichier pour les ordinateurs de bureau et pour les périphériques mobiles dans le cadre d’une seule tâche de téléchargement.

Une fois que vous avez sélectionné **[!UICONTROL Démarrer le téléchargement]**, le fichier vidéo de Principal d’origine est téléchargé et les fichiers codés sont générés à partir du fichier principal.

### A propos des options de codage prédéfinies {#about-encoding-preset-options}

Les paramètres des options de codage prédéfinies sont comme suit :

* **[!UICONTROL Vitesse de connexion cible]** : vitesse de connexion Internet de l’utilisateur final ciblé.

* **[!UICONTROL Suffixe de fichier codé]** : suffixe joint au fichier vidéo codé à des fins d’identification.

* **[!UICONTROL Débit vidéo (débit de données)]** : quantité de données codées pour constituer une seconde de lecture vidéo (en kilobits par seconde).

* **[!UICONTROL Largeur/hauteur en pixels]** : dimension de largeur de l’image écran, en pixels ; dimension de hauteur de l’image écran (en pixels).

* **[!UICONTROL Image par seconde (ips)]** : nombre d’images, ou images fixes, pour chaque seconde de vidéo. Aux Etats-Unis et au Japon, la plupart des vidéos sont tournées à 29,97 ips ; en Europe et dans les autres pays d’Asie, la plupart des vidéos le sont à 25 ips. Le film est tourné à 24 ips.

* **[!UICONTROL Débit audio]** : quantité de données codées pour constituer une seconde de lecture audio, en kilobits par seconde.

Le tableau suivant répertorie les meilleures pratiques recommandées pour la sélection de paramètres vidéo prédéfinis et les conventions de dénomination qui sont utilisées pour désigner les fichiers codés.

### Vidéo adaptative (par défaut) {#adaptive-video-default}

Un paramètre prédéfini de codage qui fonctionne avec n’importe quelle proportion pour permettre la création de vidéos pour une diffusion sur téléphone, tablette et ordinateur de bureau Les vidéos source téléchargées codées avec ce paramètre prédéfini (valeur par défaut et recommandée) sont définies sur une hauteur fixe, tandis que la largeur est automatiquement mise à l’échelle pour préserver les proportions de la vidéo.

**Vidéo adaptative (par défaut)**

|  | Nom du paramètre prédéfini de codage/Texte de l’info-bulle | Suffixe de fichier codé | Débit de données vidéo (Kb/s) | Largeur/hauteur (pixels) | Image par seconde | Débit audio (Kbit/s) | Recommandations |
|--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | Auto × 360, 800 Kbit/s | _Mobile_Auto×360p_800K | 800 | Auto×360 | Identique à la source | 64 | Pour mobile (iPhone, iPad, Android™) |
| 2 | Auto × 480, 1 400 Kbit/s | _Tablet_Auto×480p_1400K | 1400 | Auto×480 | Identique à la source | 96 | Pour les tablettes (iPad, Android™) |
| 3 | Auto × 720, 2 600 Kbit/s | _Desktop_Auto×720p_2600K | 2600 | Auto×720 | Identique à la source | 128 | Pour ordinateur de bureau |

### Paramètres prédéfinis de codage vidéo adaptatif (16:9 ou 4:3) {#adaptive-video-encoding-or-video-presets}

Ces paramètres prédéfinis de codage vidéo adaptatif combinent une série de paramètres prédéfinis de codage individuels qui sont automatiquement sélectionnés en fonction des proportions de la vidéo que vous avez téléchargée. Par exemple, si vous téléchargez une vidéo 4:3, elle est automatiquement codée à l’aide des cinq paramètres prédéfinis 4:3 figurant dans la liste des paramètres prédéfinis principaux de l’option **Codage vidéo adaptatif (16:9 ou 4:3)** .

Pour plus d’informations sur les options de codage, voir [A propos des options de codage prédéfinies](application-setup.md#about_encoding_preset_options).

**Paramètres prédéfinis de codage vidéo adaptatif (16:9 ou 4:3)**

|  | Nom du paramètre prédéfini de codage/Texte de l’info-bulle | Vitesse de connexion cible (Kbit/s) | Suffixe de fichier codé | Débit de données vidéo (Kb/s) | Largeur/hauteur (pixels) | Image par seconde | Débit audio (Kbit/s) | Recommandations |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | `16:9, 512x288, Mobile (iPhone, iPad, Android&trade;), (400 Kbps)` | 500 | _Mobile_512x288_400K | 400 | 512x288 | Identique à la source | 64 | Faible résolution, 3G |
| 2 | `4:3, 384x288px, Mobile (iPhone, iPad, Android&trade;), (400 Kbps)` | 500 | _Mobile_384x288_400K | 400 | 384 x 288 | Identique à la source | 64 | Faible résolution, 3G |
| 3 | `16:9, 512x288, Mobile (iPhone, iPad, Android&trade;), (600 Kbps)` | 700 | _Mobile_512x288_600K | 600 | 512 x 288 | Identique à la source | 64 | Résolution Medium, 3G |
| 4 | `4:3, 384x288, Mobile (iPhone, iPad, Android&trade;), (600 Kbps)` | 700 | _Mobile_384x288 _600 | 600 | 384 x 288 | Identique à la source | 64 | Résolution Medium, 3G |
| 5 | `16:9, 640x360, Tablet (iPad, Android&trade;), (800 Kbps)` | 900 | _iPad_640x360_800K | 800 | 640 x 360 | Identique à la source | 80 | Résolution Medium, WiFi |
| 6 | `4:3, 640x480, Tablet (iPad, Android&trade;), (800 Kbps)` | 900 | _iPad_640x480_800K | 800 | 640 x 480 | Identique à la source | 80 | Résolution Medium, WiFi |
| 7 | `16:9, 768x432, Tablet (iPad, Android&trade;), (1200 Kbps)` | 1,5 Mbit/s | _iPad_768x432_1200K | 1 200 | 768 x 432 | Identique à la source | 96 | Haute résolution, WiFi |
| 8 | `4:3, 768x576, Tablet (iPad, Android&trade;), (1200 Kbps)` | 1,5 Mbit/s | _iPad_768x576_1200K | 1 200 | 768 x 576 | Identique à la source | 96 | Haute résolution, WiFi |
| 9 | `16:9, 1280x720, Desktop, (2000 Kbps)` | 3 Mbits/s | _1280X720_2000K | 2 000 | 1280 x 720 | Identique à la source | 128 | Haute définition, Grand écran |
| 10 | `4:3, 1280x960, Desktop, (2000 Kbps)` | 3 Mbits/s | _1280X 960_2000K | 2 000 Kbits/s | 1280x960 | Identique à la source | 128 | Haute définition |

### Paramètres prédéfinis de codage de vidéo pour ordinateur de bureau {#desktop-video-encoding-presets}

Il s’agit des paramètres prédéfinis de codage pour les formats vidéo MP4 et OGV sur les ordinateurs de bureau.

Pour plus d’informations sur les options de codage prédéfinies, voir [A propos des options de codage prédéfinies](application-setup.md#about_encoding_preset_options).

**H264 Main 3.2 : Audio AAC, extension de fichier MP4**

|  | Nom du paramètre prédéfini de codage/Texte de l’info-bulle | Vitesse de connexion cible (Kbit/s) | Suffixe de fichier codé | Débit de données vidéo (Kb/s) | Largeur/hauteur (pixels) | Image par seconde | Débit audio (Kbit/s) | Recommandations |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 480 x 270 (400 Kbit/s) | 500 | _480X270_400K | 400 | 480 x 270 | Identique à la source | 64 | Résolution grand écran faible |
| 2 | 16:9, 640 x 360 (800 Kbits/s) | 900 | _640X360_800K | 800 | 640 x 360 | Identique à la source | 80 | Résolution grand écran moyenne |
| 3 | 16:9, 800 x 450 (1 200 Kbits/s) | 1,5 Mbit/s | _800X450_1200K | 1 200 | 800 x 450 | Identique à la source | 96 | Moyenne à haute résolution |
| 4 | 16:9, 1280 x 720 (2 000 Kbits/s) | 3 Mbits/s | _1280X720_2000K | 2 000 | 1280 x 720 | Identique à la source | 128 | Haute définition, Grand écran |
| 5 | 4:3, 320 x 240 (400 kb/s) | 500 | _320X240_400K | 400 | 320 x 240 | Identique à la source | 64 | Basse résolution |
| 6 | 4:3, 480 x 360 (800 Kbits/s) | 900 | _480X360_800K | 800 | 480 x 360 | Identique à la source | 80 | Résolution moyenne |
| 7 | 4:3, 640 x 480 (1 200 Kbits/s) | 1,5 Mbit/s | _640X480_1200K | 1 200 | 640 x 480 | Identique à la source | 96 | Moyenne à haute résolution |
| 8 | 4:3, 1 280 x 960 (2 000 Kbits/s) | 3 Mbits/s | _1280X960_2000K | 2 000 | 1280 x 960 | Identique à la source | 128 | Haute définition |

**OGG Theora Vorbis : extension de fichier OGV**

|  | Nom du paramètre prédéfini de codage/Texte de l’info-bulle | Vitesse de connexion cible (Kbit/s) | Suffixe de fichier codé | Débit de données vidéo (Kb/s) | Largeur/hauteur (pixels) | Image par seconde | Débit audio (Kbit/s) | Recommandations |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 480 x 270 (400 Kbits/s, OGG | 500 | _OGG_480x270_400K | 400 | 480 x 270 | Identique à la source | 64 | Résolution grand écran faible |
| 2 | 16:9, 640 x 360 (800 Kbits/s), OGG | 900 | _OGG_640x360_800K | 800 | 640 x 360 | Identique à la source | 80 | Résolution grand écran moyenne |
| 3 | 16:9, 800 x 450 (1 200 Kbits/s), OGG | 1,5 Mbit/s | _OGG_800x450_1200K | 1 200 | 800 x 450 | Identique à la source | 96 | Moyenne à haute résolution |
| 4 | 16:9, 1 280 x 720 (2 000 Kbit/s), OGG | 3 Mbits/s | _OGG_1280x720_2000K | 2 000 | 1280 x 720 | Identique à la source | 128 | Haute définition, Grand écran |
| 5 | 4:3, 320 x 240 (400 Kbits/s), OGG | 500 | _OGG_320X240_400K | 400 | 320 x 240 | Identique à la source | 64 | Basse résolution |
| 6 | 4:3, 480 x 360 (800 Kbits/s), OGG | 900 | _OGG_480x360_800K | 800 | 480 x 360 | Identique à la source | 80 | Résolution moyenne |
| 7 | 4:3, 640 x 480 (1 200 Kbits/s), OGG | 1,5 Mbit/s | _OGG_640x480_1200K | 1 200 | 640 x 480 | Identique à la source | 96 | Moyenne à haute résolution |
| 8 | 4:3, 1 280 x 960 (2 000 Kbits/s), OGG | 3 Mbits/s | _OGG_1280x960_2000K | 2 000 | 1280 x 960 | Identique à la source | 128 | Haute définition |

### Paramètres prédéfinis de codage vidéo pour périphérique mobile {#mobile-video-encoding-presets}

Identique au débit source. Paramètres prédéfinis de codage vidéo pour les appareils mobiles iPhone, iPad et Android™.

Pour plus d’informations sur les options de codage prédéfinies, voir [A propos des options de codage prédéfinies](application-setup.md#about_encoding_preset_options).

**H264 Baseline 2.1 : Audio AAC, extension de fichier MP4**

|  | Nom du paramètre prédéfini de codage/Texte de l’info-bulle | Vitesse de connexion cible (Kbit/s) | Suffixe de fichier codé | Débit vidéo (Kbit/s) | Hauteur/largeur en pixels | Image par seconde | Débit audio (Kbit/s) | Recommandations |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 512 x 288, Mobile (400 Kbit/s) | 500 | _Mobile_512x288_400K | 400 | 512x288 | Identique à la source | 64 | Faible résolution, 3G |
| 2 | 16:9, 512 x 288, Mobile (600 Kbit/s) | 700 | _Mobile_512x288_600K | 600 | 512 x 288 | Identique à la source | 64 | Résolution Medium, 3G |
| 3 | 16:9, 512 x 288, Mobile (800 Kbit/s) | 900 | _Mobile_512x288_800K | 800 | 512 x 288 | Identique à la source | 80 | Résolution Medium, Wi-Fi |
| 4 | 16:9, 512 x 288, Mobile (1 000 Kbit/s) | 1,2 Mbit/s | _Mobile_512x288_1000K | 1 000 | 512 x 288 | Identique à la source | 80 | Haute résolution, Wi-Fi |
| 5 | 16:9, 512 x 288, Mobile (1 200 Kbit/s) | 1,5 Mbit/s | _Mobile_512x288_1200K | 1 200 | 512 x 288 | Identique à la source | 96 | Haute résolution, Wi-Fi |
| 6 | 4:3, 384 x 288, Mobile (400 Kbit/s) | 500 | _Mobile_384x288_400K | 400 | 384 x 288 | Identique à la source | 64 | Faible résolution, 3G |
| 7 | 4:3, 384 x 288, Mobile (600 Kbit/s) | 700 | _Mobile_384x288_600K | 600 | 384 x 288 | Identique à la source | 64 | Résolution Medium, 3G |
| 8 | 4:3, 448 x 336, Mobile (800 Kbit/s) | 900 | _Mobile_448x336_800K | 800 | 448 x 336 | Identique à la source | 80 | Résolution Medium, Wi-Fi |
| 9 | 4:3, 448 x 336, Mobile (1 000 Kbit/s) | 1,2 Mbit/s | _Mobile_448x336_1000K | 1 000 | 448 x 336 | Identique à la source | 80 | Haute résolution, Wi-Fi |
| 10 | 4:3, 448 x 336, Mobile (1 200 Kbit/s) | 1,5 Mbit/s | _Mobile_448x336_1200K | 1 200 | 448 x 336 | Identique à la source | 96 | Haute résolution, Wi-Fi |

## Paramètres prédéfinis de la visionneuse {#viewer-presets}

>[!NOTE]
>
>**Notification de fin de vie des visionneuses par Flash** : à compter du 31 janvier 2017, Adobe Dynamic Media Classic a officiellement arrêté la prise en charge de la plate-forme de la visionneuse de Flashs.

Un *paramètre prédéfini de visionneuse* est un ensemble de paramètres qui déterminent comment les utilisateurs voient les fichiers de média enrichi sur leur écran d’ordinateur et périphériques mobiles. En tant qu’administrateur, vous pouvez créer des paramètres de visionneuse prédéfinis. Des paramètres sont disponibles pour un ensemble d’options de configuration de la visionneuse. Vous pouvez, par exemple, modifier la taille d’affichage de la visionneuse, le comportement du zoom, les modes de couleurs, les bordures et les polices.

Pour respecter les bonnes pratiques, utilisez les visionneuses de vidéos Adobe Dynamic Media Classic HTML5. Les paramètres prédéfinis utilisés dans les visionneuses vidéo HTML5 sont des lecteurs vidéo fiables.

En combinant dans un seul lecteur les éléments suivants :

* La possibilité de concevoir les composants de lecture à l’aide d’HTML5 et de CSS.
* Lecture incorporée.
* Utilisez la diffusion en continu adaptative et progressive selon les fonctionnalités du navigateur.

Vous étendez la portée de votre contenu multimédia aux utilisateurs de bureau, de tablette et de mobile, et garantissez une expérience vidéo rationalisée.

Voir [À propos des visionneuses HTML5](https://experienceleague.adobe.com/fr/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers#viewers-for-aem-assets-only) dans le Guide de référence des visionneuses d’Adobe.

Voir la [matrice de compatibilité des paramètres prédéfinis de la visionneuse Adobe Dynamic Media Classic](application-setup.md#scene7_viewer_preset_compatibility_matrix).

Reportez-vous à la section [Meilleure pratique : Utilisation de la visionneuse de vidéos HTML5](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer).

Selon la visionneuse, vous pouvez ajouter des fonctions communautaires. Ces fonctions comprennent des boutons d’incorporation, d’e-mail, de lien et de visite de site. Ces boutons permettent aux utilisateurs de partager la visionneuse avec d’autres personnes ou d’ouvrir le site Web Adobe Dynamic Media Classic.

Voir aussi [Exemples de bibliothèques de références de visionneuses d’Adobe](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

### Prise en charge des visionneuses pour les pages web réactives {#viewer-support-for-responsive-designed-web-pages}

Différentes pages Web ont des besoins différents. Il arrive que vous souhaitiez une page Web qui fournit un lien qui ouvre la visionneuse HTML5 dans une fenêtre de navigateur distincte. Dans d’autres cas, il est nécessaire d’incorporer la visionneuse HTML5 directement sur la page d’hébergement. Dans ce dernier cas, la page Web a probablement une disposition statique. Il est également &quot;réactif&quot; et s’affiche différemment sur différents appareils ou pour différentes tailles de fenêtre de navigateur. Pour répondre à ces besoins, les visionneuses HTML5 fournies avec Adobe Dynamic Media Classic prennent en charge les pages web statiques et les pages web adaptées.

Pour plus d’informations sur la manière d’incorporer des visionneuses réactives dans vos pages web, voir [À propos de la bibliothèque d’images réactives](https://experienceleague.adobe.com/fr/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/c-about-responsive-static-image-library#image-serving-api), [Utiliser la bibliothèque d’images réactives](https://experienceleague.adobe.com/fr/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library#image-serving-api) et [Référence de commande : attributs de commande](https://experienceleague.adobe.com/fr/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library#responsive-static-image-library).

### Types de paramètres prédéfinis de visionneuse {#viewer-preset-types}

Les administrateurs peuvent créer et personnaliser les types de paramètres prédéfinis suivants :

* **[!UICONTROL Visionneuse de catalogue électronique]** : simule l’expérience de lecture d’un catalogue imprimé. Vous pouvez passer d’une page à l’autre, effectuer un zoom avant ou arrière sur les éléments d’une page, utiliser les zones cliquables pour afficher plus d’informations sur les éléments de la page ou effectuer des recherches dans le catalogue. Vous pouvez également inclure un panneau Informations pour afficher des informations détaillées et un élément mappé sur une image si la zone de carte possède un attribut rollover_key valide. Pour inclure un panneau Informations, spécifiez une URL de serveur d’informations dans le panneau Paramètres du panneau Informations de la fenêtre Paramètre prédéfini de la visionneuse de catalogue électronique.

* **[!UICONTROL Visionneuse d’échantillons]** : affiche une image dans une couleur, un matériau, une texture, une finition ou un tissu différents. Les utilisateurs sélectionnent une miniature pour afficher les variations de l’image.

* **[!UICONTROL Visionneuse de supports variés]** : affiche différents types de médias dans une seule visionneuse. Vous pouvez y inclure des séries d’échantillons, des visionneuses à 360°, des images et des vidéos. Vous pouvez configurer des onglets pour contenir différents types de contenu, tels qu’un onglet pour les visionneuses d’images et un onglet pour les vidéos. Les vidéos lues à partir d’une visionneuse de médias mixtes utilisent une visionneuse de vidéos standard avec une chronologie et des commandes vidéo, telles que Arrêter, Mettre en pause, Revenir en arrière et Lire. Lorsque vous configurez un paramètre prédéfini de visionneuse de médias mixtes, vous spécifiez les visionneuses à utiliser pour les différents types de ressources de la visionneuse. Vous pouvez également utiliser la visionneuse de grille ou de carrousel pour visualiser les fichiers d’une visionneuse de supports variés.

* **[!UICONTROL Visionneuse à 360°]** : fournit plusieurs vues d’une image afin que les utilisateurs puissent faire pivoter l’objet pour l’examiner sous différents angles.

* **Visionneuse de vidéos** : affiche les vidéos à l’aide des dimensions de résolution du fichier source ou d’une taille personnalisée. Adobe Dynamic Media Classic est fourni avec de nombreux paramètres prédéfinis de visionneuse pour la lecture de vidéos. Si vous êtes administrateur, vous pouvez créer des paramètres prédéfinis de visionneuse vidéo personnalisés. Il existe plus de 12 paramètres différents pour la configuration de la visionneuse vidéo. Vous pouvez configurer les options suivantes :

   * taille
   * Couleur de premier plan et d’arrière-plan
   * Contrôles vidéo et audio
   * barre de progression
   * habillage de l’interface utilisateur
   * fonctions sociales
   * et aide

* **[!UICONTROL Visionneuses de zoom]** : offre le choix de trois types de visionneuses de zoom :

* **[!UICONTROL Visionneuse de zoom]** : permet aux utilisateurs d’effectuer un zoom sur la zone en la sélectionnant. Ils peuvent sélectionner des commandes pour effectuer un zoom avant, un zoom arrière et rétablir la taille par défaut de l’image.

* **[!UICONTROL Visionneuse de zoom : fenêtre déroulante]** : affiche une seconde image de la zone agrandie en regard de l’image d’origine. Aucune commande n’est disponible. Il suffit de déplacer la sélection sur la zone à visualiser.

Pour déterminer la quantité totale de bande passante allouée à la visionneuse, n’oubliez pas que l’image principale et celle de la fenêtre déroulante sont toutes deux diffusées par la visionneuse. La taille de l’image principale (largeur et hauteur d’affichage) et le facteur de zoom déterminent la taille de la fenêtre déroulante. Pour que la fenêtre déroulante ne devienne pas trop volumineuse, équilibrez ces deux valeurs : si la taille de l’image principale est importante, réduisez la valeur du facteur de zoom. (La Largeur de la fenêtre déroulante et la Hauteur de la fenêtre déroulante déterminent la taille de la fenêtre déroulante, mais pas la taille de l’image diffusée par la visionneuse.)

Par exemple, si la taille de l’image principale est de 350 x 350 pixels et que le facteur de zoom est de 3, la taille d’image de la fenêtre déroulante sera de 1 050 x 1 050 pixels. Si la taille de l’image principale est de 300 x 300 pixels et que le facteur de zoom est de 4, la taille d’image de la fenêtre déroulante sera de 1 200 x 1 200 pixels. Selon la valeur de qualité JPEG sélectionnée (une valeur comprise entre 80 et 90 est recommandée), il est possible de réduire sensiblement la taille du fichier. Selon la taille de l’image principale, un facteur de zoom de 2,5 à 4 est recommandé.

### Matrice de compatibilité des paramètres prédéfinis de la visionneuse Adobe Dynamic Media Classic {#scene-viewer-preset-compatibility-matrix}

**Notification de fin de vie des visionneuses par Flash** : à compter du 31 janvier 2017, Adobe Dynamic Media Classic a officiellement arrêté la prise en charge de la plate-forme de la visionneuse de Flashs.

Le tableau suivant identifie les paramètres prédéfinis de la visionneuse Adobe Dynamic Media Classic actuellement disponibles. Le tableau indique également la compatibilité de la visionneuse avec les appareils mobiles et de bureau, ainsi que la technologie utilisée pour chaque visionneuse donnée.

Voir aussi [Exemples de bibliothèques de références de visionneuses d’Adobe](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

Pour plus d’informations sur les versions de navigateur Web et de système d’exploitation prises en charge pour les visionneuses, vous pouvez consulter les notes de mise à jour des visionneuses.

Voir [Notes de mise à jour de référence des visionneuses Adobe](https://experienceleague.adobe.com/fr/docs/dynamic-media-developer-resources).

|  | Technologie de la visionneuse | Bureau | Apple iPhone | Apple iPad | Smartphone Android™ | Tablette Android™ |
|--- |--- |--- |--- |--- |--- |--- |
| Visionneuses de zoom |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_inline | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_light | HTML5 | X | X | X | X | X |


|  | Technologie de la visionneuse | Bureau | Apple iPhone | Apple iPad | Smartphone Android™ | Tablette Android™ |
|--- |--- |--- |--- |--- |--- |--- |
| Visionneuses de visionneuses d’images |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

|  | Technologie de la visionneuse | Bureau | Apple iPhone | Apple iPad | Smartphone Android™ | Tablette Android™ |
|--- |--- |--- |--- |--- |--- |--- |
| Visionneuses de séries d’échantillons |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_light | HTML5 | X | X | X | X | X |

|  | Technologie de la visionneuse | Bureau | Apple iPhone | Apple iPad | Smartphone Android™ | Tablette Android™ |
|--- |--- |--- |--- |--- |--- |--- |
| Visionneuses de catalogue électronique |  |  |  |  |  |  |
| Universal_HTML5_eCatalog_Adv(comprend la prise en charge de la recherche dans les médias sociaux et les catalogues.) | HTML5 | X | X | X | X | X |
| Universal_HTML5_eCatalog (comprend la prise en charge de la recherche catalogue et des médias sociaux.) | HTML5 | X | X | X | X | X |

|  | Technologie de la visionneuse | Bureau | Apple iPhone | Apple iPad | Smartphone Android™ | Tablette Android™ |
|--- |--- |--- |--- |--- |--- |--- |
| Visionneuses à 360° |  |  |  |  |  |  |
| Universal_HTML5_SpinSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SpinSet_light | HTML5 | X | X | X | X | X |

**Visionneuses d’eVideo**

Adobe Dynamic Media Classic prend en charge la lecture vidéo mobile pour la vidéo MP4 H.264.

* Vous trouverez les appareils BlackBerry® qui prennent en charge ce format vidéo à l’adresse suivante : [Formats vidéo pris en charge sur BlackBerry®](https://developers.blackberry.com/us/en)
* Vous pouvez également trouver les appareils Windows® qui prennent en charge ce format vidéo à l’adresse suivante : [Formats vidéo pris en charge sur Windows® Phone](https://learn.microsoft.com/en-us/windows/uwp/audio-video-camera/supported-codecs)

|  | Technologie de la visionneuse | Bureau | Apple iPhone | Apple iPad | Smartphone Android™ | Tablette Android™ | Smartphone BlackBerry® | Windows® Phone |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| Universal_HTML5_Video (comprend la prise en charge du sous-titrage codé.) Voir [Bonne pratique : Utilisation de la visionneuse de vidéos Universal HTML5.](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer) | HTML5 | X | X | X | X | X | X | X |
| Universal_HTML5_Video_social(comprend la prise en charge du sous-titrage et des médias sociaux fermés.) | HTML5 | X | X | X | X | X | X | X |

|  | Technologie de la visionneuse | Bureau | Apple iPhone | Apple iPad | Smartphone Android™ | Tablette Android™ |
|--- |--- |--- |--- |--- |--- |--- |
| Visionneuses de supports variés |  |  |  |  |  |  |
| Universal_HTML5_MixedMedia_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_MixedMedia_light | HTML5 | X | X | X | X | X |

### Matrice des mouvements des visionneuses mobiles pris en charge {#supported-mobile-viewers-gestures-matrix}

Le tableau suivant identifie les mouvements des visionneuses mobiles pris en charge sur les appareils iOS, Android™ 2.x et Android™ 3.x.

|  | Technologie de la visionneuse | Bureau | Apple iPhone | Apple iPad | Smartphone Android™ | Tablette Android™ |
|--- |--- |--- |--- |--- |--- |--- |
| Visionneuses de visionneuses d’images |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

### A propos de l’écran Paramètres prédéfinis de la visionneuse {#about-the-viewer-preset-screen}

Créez et gérez des paramètres prédéfinis de la visionneuse sur l’écran Paramètres prédéfinis de la visionneuse. Pour ouvrir cet écran, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Paramètres prédéfinis de la visionneuse]**.

L’écran Paramètres prédéfinis de la visionneuse propose des outils permettant d’effectuer les tâches suivantes :

* **Ajouter un paramètre prédéfini** : sélectionnez **[!UICONTROL Ajouter]** et faites des choix dans la boîte de dialogue Ajouter un paramètre prédéfini de visionneuse.

       Voir [Ajout et modification de paramètres de visionneuse prédéfinis](application-setup.md#adding_and_editing_viewer_presets).
  
* **Modifier un paramètre prédéfini** : sélectionnez un paramètre prédéfini, puis sélectionnez **[!UICONTROL Modifier]**.

       Voir [Ajout et modification de paramètres de visionneuse prédéfinis](application-setup.md#adding_and_editing_viewer_presets).
  
* **Supprimer un paramètre prédéfini** : sélectionnez un paramètre prédéfini, puis sélectionnez **[!UICONTROL Supprimer]**.

* **Exporter un paramètre prédéfini** : sélectionnez un paramètre prédéfini de visionneuse HTML5. Cliquez ensuite sur **[!UICONTROL Exporter]** pour télécharger l’habillage de la visionneuse afin que vous puissiez l’utiliser comme base pour créer et ajouter un autre paramètre prédéfini de visionneuse.

      Voir [Exportation d’un paramètre prédéfini de visionneuse HTML5](application-setup.md#export_an_html5_viewer_preset).
  
* **Filtrer la liste des paramètres prédéfinis de la visionneuse** : utilisez ces outils pour filtrer la liste :

      * Ouvrez la liste déroulante **Actif/Inactif** et sélectionnez une option pour afficher les paramètres prédéfinis actifs, inactifs ou tous les paramètres prédéfinis.
     * Ouvrez la liste déroulante **Visionneuse** et sélectionnez une option pour afficher uniquement les visionneuses d’un certain type. Sélectionnez **[!UICONTROL Toutes les visionneuses]** pour afficher toutes les visionneuses.
  
* **Trier les paramètres prédéfinis** : sélectionnez un en-tête de colonne (**[!UICONTROL Actif]**, **[!UICONTROL Type]**, **[!UICONTROL Paramètre prédéfini]** ou **[!UICONTROL Plateforme]**) pour trier la liste sur une colonne. Sélectionnez un en-tête de colonne une seconde fois pour trier la liste par ordre décroissant (ou croissant).

* **Activer et désactiver des paramètres prédéfinis** : sélectionnez un paramètre prédéfini, puis sélectionnez son option Actif afin de pouvoir l’activer ou le désactiver.

      Voir [Activation ou désactivation des paramètres prédéfinis de la visionneuse](application-setup.md#activating_or_deactivating_viewer_presets).
  
>[!NOTE]
>
>Sélectionnez **[!UICONTROL Aperçu]** sur le côté droit de la page Paramètres prédéfinis de la visionneuse afin que vous puissiez voir à quoi ressemble une ressource dans le paramètre prédéfini de la visionneuse que vous avez sélectionné. Pour afficher une autre ressource, sélectionnez **[!UICONTROL Parcourir]** sur la page Paramètres visionneuse et sélectionnez une autre ressource dans la boîte de dialogue Sélectionner l’aperçu de la ressource.

### Ajout et modification de paramètres prédéfinis de visionneuse {#adding-and-editing-viewer-presets}

Outre l’ajout de paramètres de visionneuse prédéfinis à l’aide de l’option **[!UICONTROL Ajouter]** dans l’interface utilisateur, vous pouvez également utiliser l’option **[!UICONTROL Exporter]** pour ajouter un paramètre de visionneuse prédéfini. Vous pouvez simplement exporter un paramètre prédéfini de visionneuse HTML5 existant, puis l’utiliser comme base du nouveau paramètre prédéfini.

Voir [Exportation des paramètres prédéfinis de la visionneuse HTML5](application-setup.md#exporting_an_html5_viewer_preset).

Voir aussi la vidéo de formation [Paramètres visionneuse prédéfinis](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS).

**Pour ajouter et modifier des paramètres prédéfinis de visionneuse :**

1. Près du coin supérieur droit d’Adobe Dynamic Media Classic, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Paramètres prédéfinis de la visionneuse]**.

   Vous pouvez filtrer la liste des paramètres prédéfinis. Par exemple, pour afficher uniquement les paramètres prédéfinis pour les visionneuses de vidéos, sélectionnez Visionneuse de vidéos dans le menu déroulant des visionneuses sur la barre d’outils qui se trouve directement au-dessus du tableau.

1. Sur la page Paramètres visionneuse, ajoutez ou modifiez le paramètre prédéfini de la visionneuse sur l’écran Paramètres prédéfinis de la visionneuse.

   * **Ajouter** : dans la barre d’outils, sélectionnez **[!UICONTROL Ajouter]**. Dans la boîte de dialogue Ajouter un paramètre prédéfini de visionneuse, sélectionnez une plateforme, puis un type de ressource de média enrichi.

         Sélectionnez **[!UICONTROL Enregistrer sous]** lorsque vous avez terminé de créer le paramètre prédéfini de la visionneuse.
     
   * **Ajouter à partir d’un paramètre prédéfini de visionneuse existant** : dans le tableau, sélectionnez un paramètre prédéfini de visionneuse de vidéos, puis sélectionnez **[!UICONTROL Modifier]** dans la barre d’outils.

         Après avoir reconfiguré la visionneuse de vidéos, sélectionnez **[!UICONTROL Enregistrer sous]** pour enregistrer le paramètre prédéfini à l’aide d’un autre nom dans le champ de texte Nom du paramètre prédéfini.
     
   * **Modifier** : sélectionnez un paramètre prédéfini de visionneuse existant, puis sélectionnez **[!UICONTROL Modifier]**.

1. Dans la page Configuration de la visionneuse, dans le champ Nom du paramètre prédéfini, saisissez ou modifiez le nom du paramètre prédéfini.
1. Définissez les options restantes si vous le souhaitez.

   >[!NOTE]
   >
   >Sélectionnez **[!UICONTROL Identique à Source]** afin de dimensionner automatiquement la visionneuse de vidéos en fonction de la taille de résolution de la vidéo codée elle-même. Si vous sélectionnez cette option, vous ne pouvez pas saisir la largeur d’affichage et la hauteur d’affichage. Ces valeurs proviennent directement de la vidéo elle-même. Si vous sélectionnez **[!UICONTROL Identique à Source]**, définissez l’option Taille de marge pour qu’elle reflète les dimensions de l’habillage en dehors de la zone de lecture vidéo. Cette taille de marge correspond à la hauteur et à la largeur, en pixels, des commandes vidéo. Vous pouvez utiliser l’image suivante pour vous aider à déterminer la taille des marges à utiliser.*

   ![Configuration de marge de la visionneuse de vidéos](assets/vs_video_viewer_configure_margin.png)

1. Effectuez l’une des opérations suivantes :

   * Sélectionnez **[!UICONTROL Enregistrer sous]** si vous avez ajouté un paramètre prédéfini de visionneuse à partir d’un paramètre prédéfini existant.
   * Sélectionnez **[!UICONTROL Enregistrer]** si vous avez ajouté ou modifié un paramètre de visionneuse prédéfini.

### Exportation d’un paramètre prédéfini de visionneuse HTML5 {#exporting-an-html-viewer-preset}

Vous pouvez exporter un paramètre prédéfini de visionneuse HTML5 existant à utiliser comme base pour créer un paramètre prédéfini de visionneuse HTML5. Cette méthode est pratique car elle vous évite d’avoir à créer une visionneuse depuis le début. En effet, il vous suffit d’exporter un paramètre prédéfini présentant des caractéristiques et un comportement semblables à ce que vous recherchez, puis de l’utiliser comme point de départ pour vos modifications.

Tous les fichiers CSS de paramètre prédéfini de visionneuse par défaut dans Adobe Dynamic Media Classic utilisent des chemins de service d’images relatifs qui pointent vers des ressources sur `Scene7SharedAssets`. Par exemple, voici un chemin relatif à une ressource image dans un fichier CSS de paramètre prédéfini de visionneuse sur

`Scene7SharedAsset` : `.s7videoviewer .s7fullscreenbutton[state][selected] { background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }`

Cependant, si vous hébergez des fichiers CSS de visionneuse sur votre propre site, vous devez résoudre ces chemins d’image relatifs en utilisant un chemin d’accès explicite au serveur d’images dans votre propre environnement. Par exemple, si vous avez mis à jour le chemin relatif ci-dessus vers un chemin explicite, il peut se présenter comme suit, où `https://s7d1.scene7.com` est le chemin direct vers votre serveur d’images : `https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha`

**Pour exporter un paramètre prédéfini de visionneuse HTML5 :**

```as3
.s7videoviewer .s7fullscreenbutton[state][selected] 
{ background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }
```

```as3
https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha
```

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Paramètres visionneuse prédéfinis]**.
1. Dans la barre d’outils Paramètres prédéfinis de la visionneuse, dans la deuxième liste déroulante de gauche, sélectionnez **[!UICONTROL HTML5]**.
1. Dans la troisième liste déroulante en partant de la gauche, sélectionnez **[!UICONTROL Toutes les visionneuses]**.
1. Sélectionnez le paramètre prédéfini de visionneuse que vous souhaitez utiliser comme base d’un nouveau paramètre prédéfini de visionneuse HTML5.
1. Dans la barre d’outils, sélectionnez **[!UICONTROL Export]**.
1. Dans la boîte de dialogue Exporter l’Assets sélectionnée, sélectionnez **[!UICONTROL Submit Export]**.

   Après l’exportation, vous obtenez un fichier CSS. Téléchargez et décompressez l’archive.

1. Ouvrez le fichier CSS dans un éditeur CSS, effectuez vos modifications, puis enregistrez le fichier.
1. Téléchargez le fichier CSS vers Adobe Dynamic Media Classic.

   Voir [Téléchargement de fichiers](uploading-files.md#uploading_files).

1. Publish du fichier CSS sur le serveur d’images Dynamic Media.

   Voir [Fichiers Publish](publishing-files.md#publishing_files).

1. Ajoutez le nouveau paramètre prédéfini de visionneuse comme vous le faites habituellement. Sélectionnez le fichier CSS de visionneuse que vous avez chargé.

   Voir [Ajout et modification de paramètres de visionneuse prédéfinis](application-setup.md#adding_and_editing_viewer_presets).

### Activation ou désactivation des paramètres prédéfinis de visionneuse {#activating-or-deactivating-viewer-presets}

Pour créer une URL permettant d’afficher les ressources, les utilisateurs ouvrent la liste déroulante Paramètres prédéfinis dans la boîte de dialogue Aperçu, sélectionnent un paramètre prédéfini de visionneuse, puis sélectionnez **[!UICONTROL Copier l’URL]** (voir [Copier l’URL d’un paramètre prédéfini de visionneuse](application-setup.md#copying_the_url_of_a_viewer_preset)). Cette liste de paramètres prédéfinis présente les paramètres prédéfinis de la visionneuse que les administrateurs ajoutent et gèrent sur l’écran Paramètres prédéfinis de la visionneuse. Par exemple, tous les paramètres prédéfinis de visionneuse de catalogue électronique actifs apparaissent dans la liste déroulante Paramètres prédéfinis de la boîte de dialogue Aperçu lorsqu’un utilisateur prévisualise un catalogue électronique.

A moins que vous ne désactiviez les Paramètres prédéfinis de la visionneuse sur l’écran Paramètres prédéfinis de la visionneuse, la liste déroulante Paramètres prédéfinis de la boîte de dialogue Prévisualisation peut très vite être remplie. 

**Pour activer ou désactiver les paramètres de visionneuse prédéfinis :**

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Paramètres visionneuse prédéfinis]**.
1. Sur la page Paramètres visionneuse, sélectionnez ou désélectionnez les options **[!UICONTROL Actif]** pour activer ou désactiver les paramètres prédéfinis de visionneuse.

### Copie de l’URL d’un paramètre prédéfini de visionneuse {#copying-the-url-of-a-viewer-preset}

Après avoir publié un fichier, vous pouvez copier une URL pour afficher le fichier avec les valeurs d’un paramètre prédéfini de visionneuse.

L’URL est copiée dans le Presse-papiers. Vous pouvez l’utiliser selon vos besoins dans le code d’HTML de votre page Web, de votre périphérique mobile ou de votre application.

**Pour copier l’URL d’un paramètre prédéfini de visionneuse :**

1. Sélectionnez la ressource dans le panneau Parcourir .
1. Au-dessus de panneau de navigation des fichiers, sur le côté droit de la barre d’outils, exécutez l’une des opérations suivantes :

   * Sélectionnez **[!UICONTROL Affichage de la grille]**. Dans le panneau de navigation des fichiers, cliquez deux fois sur un fichier pour l’ouvrir dans le mode Affichage des détails. Dans le panneau URL et code intégré à droite, sélectionnez **[!UICONTROL Copier l’URL]** à droite de la visionneuse de votre choix.
   * Sélectionnez **[!UICONTROL Affichage de la grille]**. Dans le panneau de navigation des ressources, sélectionnez une seule ressource, puis sous l’image miniature, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**.

   Dans la page Liste des visionneuses, sous la colonne Actions du tableau, sélectionnez **[!UICONTROL Copier l’URL]**.

   * Sélectionnez **[!UICONTROL Mode Liste]**. Dans le panneau de navigation des ressources, sélectionnez une seule ressource, puis, à droite de l’image miniature, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**.

   Dans la page Liste des visionneuses, sous la colonne Actions du tableau, sélectionnez **[!UICONTROL Copier l’URL]**.

   * Sélectionnez **[!UICONTROL Affichage de la grille]**, **&#x200B;**&#x200B;ou **[!UICONTROL Affichage des détails]**. Dans la même barre d’outils, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**.

   Dans la page Liste des visionneuses, sous la colonne Actions du tableau, sélectionnez **[!UICONTROL Copier l’URL]**.

### Copie du code incorporé d’un paramètre prédéfini de visionneuse {#copying-the-embed-code-of-a-viewer-preset}

La fonction Code incorporé permet de vérifier le code du paramètre prédéfini de la visionneuse sélectionnée. Vous pouvez également copier le code dans le Presse-papiers afin de le coller dans vos pages web pour le déploiement de la visionneuse.

Vous ne pouvez pas modifier le code dans la boîte de dialogue Code incorporé.

**Pour copier le code incorporé d’un paramètre prédéfini de visionneuse :**

1. Sélectionnez la ressource dans le panneau de navigation des ressources.
1. Au-dessus de panneau de navigation des fichiers, sur le côté droit de la barre d’outils, exécutez l’une des opérations suivantes :

   * Sélectionnez **[!UICONTROL Affichage de la grille]**. Dans le panneau de navigation des fichiers, cliquez deux fois sur un fichier pour l’ouvrir dans le mode Affichage des détails. Dans le panneau des URL à droite, sélectionnez **[!UICONTROL Code incorporé]**.
   * Sélectionnez **[!UICONTROL Affichage de la grille]**. Dans le panneau de navigation des ressources, sélectionnez une seule ressource, puis sous l’image miniature, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**.

   Dans la page Liste des visionneuses, dans la colonne Actions du tableau, sélectionnez **[!UICONTROL Code incorporé]**.

   * Sélectionnez **[!UICONTROL Mode Liste]**. Dans le panneau de navigation des ressources, sélectionnez une seule ressource, puis, à droite de l’image miniature, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**.

   Dans la page Liste des visionneuses, dans la colonne Actions du tableau, sélectionnez **[!UICONTROL Code incorporé]**.

   * Sélectionnez **[!UICONTROL Affichage de la grille]**, **&#x200B;**&#x200B;ou **[!UICONTROL Affichage des détails]**. Dans la même barre d’outils, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**.

   Dans la page Liste des visionneuses, dans la colonne Actions du tableau, sélectionnez **[!UICONTROL Code incorporé]**.

1. Dans la boîte de dialogue Code incorporé, sélectionnez **[!UICONTROL Copier dans le Presse-papiers]**.
1. Sélectionnez **[!UICONTROL Fermer]**.

## Configuration des visionneuses par défaut {#configure-default-viewers}

Vous pouvez utiliser les visionneuses par défaut pour configurer la visionneuse par défaut associée à une ressource lorsque vous utilisez l’aperçu dans Adobe Dynamic Media Classic. Vous pouvez configurer l’expérience de prévisualisation par défaut pour les types de fichier suivants :

* Image
* Vidéo
* Visionneuse à 360°
* Catalogue
* ImageSet
* SwatchSet
* Visionneuse de supports

**Pour configurer les visionneuses par défaut :**

1. Dans la liste déroulante Configuration, sélectionnez **[!UICONTROL Configuration de l’application]**.
1. Dans la fenêtre Configuration, dans le volet de gauche, accédez à **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Visionneuses]**
1. Sélectionnez **[!UICONTROL Visionneuses par défaut]**.
1. Dans la fenêtre Visionneuses par défaut, dans la liste déroulante de chaque type de ressource, sélectionnez la visionneuse à associer à l’aperçu de la ressource.
1. Dans le coin inférieur droit de la fenêtre Visionneuses par défaut, sélectionnez **[!UICONTROL Enregistrer les paramètres]**.
1. Dans le coin inférieur droit de la fenêtre Configuration, sélectionnez **[!UICONTROL Fermer]** pour revenir à la fenêtre Ressource.

## Vues des métadonnées {#metadata-views}

Les *métadonnées* sont des informations normalisées concernant un fichier. Vous pouvez utiliser les métadonnées pour rationaliser votre flux de travail, organiser vos fichiers et améliorer les performances de recherche. Adobe Dynamic Media Classic prend en charge la norme IPTC (Conseil international des télécommunications de la presse) et la norme XMP (plateforme de métadonnées extensible). Avant d’afficher ou de saisir des métadonnées sur une ressource en mode Affichage des détails, les utilisateurs peuvent ouvrir le menu Vues des métadonnées . À partir de là, ils peuvent sélectionner l’ensemble des champs de métadonnées qu’ils souhaitent afficher ou utiliser pour décrire la ressource.

Adobe Dynamic Media Classic est fourni avec des vues de métadonnées prédéfinies, et les administrateurs peuvent créer leurs propres vues de métadonnées pour que les utilisateurs puissent choisir lorsqu’ils saisissent des métadonnées.

### Création d’une vue de métadonnées {#creating-a-metadata-view}

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Métadonnées]** > **[!UICONTROL Vues des métadonnées]**.
1. Sélectionnez **[!UICONTROL Ajouter]**.
1. Dans le champ de texte Nom du paramètre prédéfini , saisissez un nom pour la vue.
1. (Facultatif) Cochez la case **[!UICONTROL Définir la valeur par défaut]** pour que cette vue soit celle que voient les utilisateurs lorsqu’ils ouvrent le panneau Métadonnées dans la vue Détails.
1. (Facultatif) Sélectionnez **[!UICONTROL Inclure les champs définis par l’utilisateur]** pour inclure les champs définis par l’utilisateur dans la vue. Les champs définis par les utilisateurs apparaissent en haut du panneau Métadonnées en mode Affichage des détails.
1. Sélectionnez les champs que vous souhaitez pour la vue (sélectionnez **[!UICONTROL Sélectionner tout]** pour sélectionner tous les champs).
1. Sélectionnez **[!UICONTROL Enregistrer]**.

   Les catégories et les champs sélectionnés pour la vue apparaissent dans le panneau de prévisualisation.

### Gestion des vues des métadonnées {#managing-metadata-views}

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Métadonnées]** > **[!UICONTROL Vues des métadonnées]**.
1. Utilisez l’une des méthodes suivantes :

   * Pour prévisualiser une vue, sélectionnez-la. Les champs de la vue apparaissent dans le panneau de prévisualisation.
   * Pour modifier une vue, sélectionnez-la, puis sélectionnez **[!UICONTROL Modifier]**. Sélectionnez ou désélectionnez ensuite les noms des champs dans le panneau Aperçu, puis sélectionnez ou désélectionnez l’option **[!UICONTROL Inclure les champs définis par l’utilisateur]** .
   * Pour supprimer une vue, sélectionnez-la, puis sélectionnez **[!UICONTROL Supprimer]**.
   * Pour créer une vue par défaut, sélectionnez-la, puis sélectionnez **[!UICONTROL Définir comme valeur par défaut]**. La vue par défaut est celle que les utilisateurs voient lorsqu’ils ouvrent une ressource dans la vue Détails et accèdent au panneau Métadonnées.

## Paramètres prédéfinis des métadonnées {#metadata-presets}

Les paramètres prédéfinis de métadonnées permettent aux administrateurs de contrôler et de réglementer les métadonnées affectées aux ressources. En mode Affichage des détails, un utilisateur peut saisir des métadonnées sur une ressource dans les champs fournis à cet effet. Par exemple, un utilisateur peut entrer un nom de propriétaire, une description de copyright et une adresse. Pour vous assurer que les utilisateurs saisissent ces informations de manière précise et complète, vous pouvez créer des paramètres prédéfinis de métadonnées. Le choix d’un paramètre prédéfini de métadonnées dans la vue Détails renseigne les champs de métadonnées avec des valeurs prédéfinies. Par exemple, un nom de propriétaire, une description de copyright et une adresse sont entrés de façon automatique.

Créez un paramètre prédéfini de métadonnées pour chaque ensemble de valeurs de métadonnées que les utilisateurs doivent pouvoir entrer automatiquement dans le mode Affichage des détails pour décrire une ressource.

### Création ou modification d’un paramètre prédéfini de métadonnées {#creating-or-editing-a-metadata-preset}

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Métadonnées]** > **[!UICONTROL Paramètres prédéfinis de métadonnées]**.
1. Dans l’écran Paramètres prédéfinis de métadonnées, utilisez l’une des méthodes suivantes :

   * Pour créer un paramètre prédéfini, sélectionnez **[!UICONTROL Ajouter]**. Dans le champ de texte Nom du modèle de métadonnées , saisissez le nom du paramètre prédéfini. Sélectionnez **[!UICONTROL Vues des métadonnées]**, puis une vue dans la liste déroulante (voir [Vues des métadonnées](application-setup.md#metadata_views)).
   * Pour modifier un paramètre prédéfini existant, sélectionnez le paramètre prédéfini dans la liste Paramètres prédéfinis des métadonnées, puis sélectionnez **[!UICONTROL Modifier]**.

1. Développez les en-têtes que vous souhaitez inclure dans le paramètre prédéfini et saisissez des valeurs dans les différents champs que vous souhaitez inclure dans le paramètre prédéfini.
1. Sélectionnez **[!UICONTROL Enregistrer]**.

   Les catégories et les champs sélectionnés pour le paramètre prédéfini sont visibles dans le panneau de prévisualisation.

### Gestion des paramètres prédéfinis des métadonnées {#managing-metadata-presets}

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Métadonnées]** > **[!UICONTROL Paramètres prédéfinis de métadonnées]**.
1. Utilisez l’une des méthodes suivantes :

   * Pour prévisualiser un paramètre prédéfini, sélectionnez ce dernier. Les informations correspondantes (catégories et champs) s’affichent dans l’écran de prévisualisation.
   * Pour supprimer un paramètre prédéfini, sélectionnez-le, puis sélectionnez **[!UICONTROL Supprimer]**.

## Champs définis par l’utilisateur {#user-defined-fields}

Un administrateur de portail multimédia ou un administrateur d’entreprise peut créer des champs de métadonnées définis par l’utilisateur personnalisés. Les champs personnalisés peuvent vous aider à organiser les ressources dans Adobe Dynamic Media Classic. Vous pouvez marquer les champs comme étant actifs, si nécessaire. Lorsqu’ils sont activés, les noms de ces champs de métadonnées personnalisés s’affichent dans le panneau Métadonnées de la vue Détails. Les utilisateurs peuvent renseigner les champs de métadonnées définies par les utilisateurs pour décrire les fichiers. Ils peuvent également définir un champ de métadonnées utilisateur comme critère de recherche.

Pour utiliser efficacement les champs de métadonnées définis par l’utilisateur, retardez l’heure d’activation d’un fichier pour un lancement ou une vente spécifique. Vous définissez un champ &quot;activation&quot;, en fonction du type *Date*. Ensuite, à l’aide du panneau **[!UICONTROL Métadonnées]** dans la vue Détails ou **[!UICONTROL Fichier]** > **[!UICONTROL Modifier les infos]**, vous pouvez spécifier le moment où la ressource est activée. Adobe Dynamic Media Classic vérifie l’état publié d’une ressource et l’historique de publication. S’il ne se trouve pas dans l’heure d’activation, l’état de publication s’affiche comme &quot;Non publié&quot;.

>[!NOTE]
>
>Pour que les champs définis par l’utilisateur apparaissent dans le panneau Métadonnées en mode Affichage des détails, incluez des champs définis par l’utilisateur dans les vues de métadonnées. Dans l’écran Vues des métadonnées, sélectionnez l’option Include UDF (Inclure les champs définis par les utilisateurs). Pour plus d’informations, voir [Vues des métadonnées](application-setup.md#metadata_views).

>[!NOTE]
>
>Pour rechercher des ressources à l’aide de champs personnalisés définis par l’utilisateur, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration personnelle]**, puis sélectionnez **[!UICONTROL Inclure les champs définis par l’utilisateur dans la recherche]**. Voir [Configuration personnelle](personal-setup.md#personal_setup).

### Créer un champ de métadonnées défini par l’utilisateur {#creating-a-user-defined-metadata-field}

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Métadonnées]** > **[!UICONTROL Champs définis par l’utilisateur]**.
1. Sélectionnez **[!UICONTROL Ajouter]**
1. Dans la boîte de dialogue Champ personnalisé, définissez les options de votre choix.

   * **[!UICONTROL Nom]** : saisissez un nom pour le champ de métadonnées.

   * **[!UICONTROL Type]** : sélectionnez une option qui définit le type d’informations que les utilisateurs peuvent saisir dans le champ de métadonnées :

   * **[!UICONTROL String]** : chaîne de texte.

   * **[!UICONTROL Int]** : Entier.

   * **[!UICONTROL Float]** : nombre à virgule flottante.

   * **[!UICONTROL Yes/No]** : une valeur booléenne oui/non.

   * **[!UICONTROL Date]** : une date. Le format de date MM/JJ/AAAA est accepté.

   * **[!UICONTROL Nom de fichier]** : nom d’un fichier.

   * **[!UICONTROL Color]** : nom d’une couleur.

   * **[!UICONTROL Dimension]** : largeur et hauteur de la ressource.

   * **[!UICONTROL Untyped]** : pour la rétrocompatibilité. Ne sélectionnez pas cette option.

   * **[!UICONTROL Valeur par défaut]** : facultatif. Saisissez la valeur que les utilisateurs sont les plus susceptibles de saisir dans le champ. La valeur que vous entrez devient la valeur par défaut du champ que vous créez.

   * **[!UICONTROL S’Applique À]** : Facultatif. Sélectionnez un type de ressource si vous souhaitez que le champ de métadonnées s’applique uniquement à un type spécifique de ressource.

     >[!NOTE]
     >
     >Sélectionnez soigneusement une option **[!UICONTROL S’applique à]** car vous ne pouvez pas modifier l’option **[!UICONTROL S’applique à]** après avoir créé un champ défini par l’utilisateur. Adobe Dynamic Media Classic vous permet de modifier le nom, le type et la valeur par défaut d’un champ défini par l’utilisateur, mais pas le paramètre **[!UICONTROL S’applique à]**. *

1. Sélectionnez **[!UICONTROL Enregistrer]** une fois la création du champ de métadonnées terminée.

### Gestion de champs définis par les utilisateurs {#manage-user-defined-fields}

L’écran Champs définis par l’utilisateur comporte des commandes qui permettent de gérer des champs de métadonnées personnalisés définis par les utilisateurs. 

Seul un administrateur du portail multimédia ou un administrateur d’entreprise peut gérer les champs définis par l’utilisateur.

Pour ouvrir cet écran, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Métadonnées]** > **[!UICONTROL Champs définis par l’utilisateur]**.

* **Modifier un champ** : sélectionnez le champ, puis **[!UICONTROL Modifier]**.

* **Supprimer un champ** : sélectionnez le champ, puis **[!UICONTROL Supprimer]**.

* **Activer le champ** : sélectionnez ou désélectionnez l’option **[!UICONTROL Active]** en regard du nom d’un champ. Si vous êtes administrateur d’entreprise, cette option n’est pas affichée. Comme cette option est liée à MediaPortal, vous devez sélectionner (activer) Afficher les fonctionnalités MediaPortal dans la configuration personnelle pour afficher les champs activés.

## Optimisation des fichiers {#optimize-files}

Lorsque vous chargez des fichiers dans Adobe Dynamic Media Classic, le système les optimise pour leur stockage et leur publication. Toutefois, en cas d’interruption du processus de téléchargement, certaines images ne pourront pas être optimisées. Dans ce cas, le message &quot;Image non encore optimisée&quot; s’affiche. Vous pouvez cependant optimiser ces fichiers si vous êtes un administrateur.

Adobe Dynamic Media Classic effectue des recherches dans vos fichiers et optimise uniquement les images qui n’ont pas été entièrement optimisées auparavant.

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]**, puis sélectionnez **[!UICONTROL Optimiser les fichiers]**.
1. Renseignez les informations de la tâche d&#39;optimisation et sélectionnez **[!UICONTROL Submit]**.

   Si vous travaillez pour plusieurs sociétés, optimisez les fichiers des différentes entreprises séparément.

## Paramètres prédéfinis d’ensemble par lot {#batch-set-presets}

Utilisez les paramètres prédéfinis d’ensemble par lot afin de pouvoir créer automatiquement des visionneuses d’images ou des visionneuses à 360° lorsqu’une tâche est en cours d’exécution pour charger des ressources dans Adobe Dynamic Media Classic.

Les administrateurs d’entreprise commencent par définir des conventions d’affectation de nom pour les ressources qu’ils souhaitent regrouper dans un ensemble. Vous pouvez ensuite créer un paramètre prédéfini d’ensemble par lot pour référencer ces images. Chaque paramètre prédéfini correspond à un ensemble d’instructions indépendant à nom unique qui définit comment créer la visionneuse en utilisant des images correspondant aux conventions d’affectation de nom définies dans la recette de paramètres prédéfinis.

Tous les paramètres prédéfinis d’ensemble par lot actifs pour une entreprise sont répertoriés dans la boîte de dialogue Télécharger l’option de tâche. Vous pouvez ainsi spécifier le paramètre prédéfini à appliquer au cours de chaque session de téléchargement. Les administrateurs d’entreprise voient tous les paramètres prédéfinis d’ensemble par lot actifs et inactifs. Lorsque vous chargez des fichiers, Adobe Dynamic Media Classic crée automatiquement un ensemble avec tous les fichiers correspondant à la convention d’affectation de nom définie dans les paramètres prédéfinis actifs.

### Affectation de nom par défaut {#default-naming}

L’administrateur d’entreprise crée une convention d’affectation des noms par défaut qui est utilisée dans n’importe quelle recette de paramètre prédéfini d’ensemble par lot. La convention d’affectation de nom par défaut sélectionnée dans la définition de paramètre prédéfini d’ensemble par lot peut être tout ce dont votre entreprise a besoin pour générer des visionneuses par lot pour tous les sites web. Un paramètre prédéfini d’ensemble par lot est créé pour utiliser la convention d’affectation de nom par défaut que vous définissez. Vous pouvez créer autant de paramètres prédéfinis d’ensemble par lot que nécessaire avec d’autres conventions d’affectation de nom personnalisées pour un ensemble de contenu spécifique lorsqu’il existe une exception à l’attribution de nom par défaut définie par l’entreprise.

La configuration d’une convention d’affectation de nom par défaut n’est pas nécessaire pour utiliser la fonctionnalité Paramètre prédéfini d’ensemble par lot. Toutefois, la bonne pratique d’Adobe recommande d’utiliser une convention d’affectation de nom par défaut pour définir autant d’éléments de votre convention d’affectation de nom que vous souhaitez regrouper dans un ensemble. Cela permet de rationaliser la création d’un ensemble de lots.

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Paramètres prédéfinis d’ensemble par lot]** > **[!UICONTROL Affectation de nom par défaut]**.
1. Sélectionnez **[!UICONTROL Afficher le formulaire]** ou **[!UICONTROL Afficher le code]** pour indiquer le mode de visualisation et de saisie des informations sur chaque élément.

   Vous pouvez cocher la case **[!UICONTROL Afficher le code]** pour afficher la valeur d’expression régulière qui se crée à côté de vos sélections de formulaire. Vous pouvez saisir ou modifier ces valeurs pour définir les éléments de la convention d’affectation des noms, si l’affichage du formulaire vous limite pour une raison quelconque. Si vos valeurs ne peuvent pas être analysées dans la vue de formulaire, les champs de formulaire deviennent inactifs.

   >[!NOTE]
   >
   >les champs de formulaire désactivés n’indiquent pas que l’expression régulière n’est pas valide. Aucune validation ne vous permet de confirmer que vos expressions régulières sont correctes. Vous verrez les résultats de l’expression régulière que vous créez pour chaque élément après la ligne Résultat. L’expression régulière est visible en entier en bas de la page.

1. Développez chaque élément selon vos besoins et indiquez les conventions d’affectation de nom que vous voulez utiliser.
1. Si nécessaire, sélectionnez **[!UICONTROL Ajouter]** pour ajouter une autre convention d’affectation des noms pour un élément. Ou, sélectionnez **[!UICONTROL Supprimer]** pour supprimer une convention d’affectation de nom pour un élément.
1. Sélectionnez **[!UICONTROL Enregistrer sous]** et saisissez le nom du paramètre prédéfini. Ou, sélectionnez **[!UICONTROL Enregistrer]** si vous modifiez un paramètre prédéfini existant.

Vous pouvez également utiliser l’affichage du code sans champ de formulaire. Dans cet affichage, vous créez vos définitions de convention d’affectation de nom entièrement à l’aide d’expressions régulières.

Deux éléments sont disponibles pour la définition : Correspondance et Nom de base. Ces champs sont tous les éléments que vous avez définis pour une convention d’affectation de nom. Ils peuvent aider à identifier la partie de la convention utilisée pour nommer l’ensemble dans lequel ils sont contenus. La convention de dénomination individuelle d’une entreprise peut utiliser une ou plusieurs lignes de définition pour chacun de ces éléments. Vous pouvez utiliser autant de lignes que vous le souhaitez pour votre définition unique et les regrouper en éléments distincts, comme pour l’image principale, l’élément de couleur, l’élément d’affichage secondaire et l’élément d’échantillon.

### Création d’un paramètre prédéfini d’ensemble par lot {#creating-a-batch-set-preset}

Adobe Dynamic Media Classic utilise des paramètres prédéfinis d’ensemble par lot pour organiser les ressources qui partagent des informations ou du contenu communs dans des ensembles d’images à afficher dans les visionneuses. Les recettes de paramètres prédéfinis d’ensemble par lot s’exécutent automatiquement avec les tâches d’importation de ressources planifiées dans Adobe Dynamic Media Classic.

Utilisez Paramètre prédéfini d’ensemble par lot pour créer, modifier et gérer vos paramètres prédéfinis d’ensemble par lot. Vous pouvez créer autant de paramètres prédéfinis que nécessaire pour couvrir toutes les tâches d’assimilation de ressources dont vous avez besoin. Il existe deux formes de définitions de paramètres prédéfinis d’ensemble par lot : une pour une convention d’affectation de nom par défaut que vous avez configurée, et une pour les conventions d’affectation de nom personnalisées que vous créez à la volée.

Vous pouvez utiliser la méthode de champ de formulaire pour définir un paramètre prédéfini d’ensemble par lot ou la méthode de code, qui vous permet d’utiliser des expressions régulières. Comme dans **[!UICONTROL Affectation de nom par défaut]**, vous pouvez sélectionner **[!UICONTROL Affichage de code]** au même moment que vous définissez dans la vue de formulaire et utiliser des expressions régulières pour créer vos définitions. Vous pouvez également désélectionner l’un des deux affichages pour utiliser uniquement l’un ou l’autre.

Voir aussi [Création d’un paramètre prédéfini d’ensemble par lot pour la génération automatique d’une visionneuse à 360° 2D](application-setup.md#creating_a_batch_set_preset_for_the_auto_generation_of_a_2d_spin_set).

Voir aussi la vidéo de formation [Visionneuse à 360° 2D](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/537_2d-spin_converted%20renamed_Done-AVS).

**Pour créer un paramètre prédéfini d’ensemble par lot :**

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Paramètres prédéfinis d’ensemble par lot]** > **[!UICONTROL Paramètre prédéfini d’ensemble par lot]**. La vue par défaut est la vue **[!UICONTROL Afficher le formulaire]**, comme défini dans le coin supérieur droit de la page Détails.
1. Dans le panneau Liste des paramètres prédéfinis, sélectionnez **[!UICONTROL Ajouter]** pour activer les champs de définition dans le panneau Détails situé dans la partie droite de la page.
1. Dans le panneau Détails, dans le champ Nom du paramètre prédéfini, nommez le paramètre prédéfini.
1. Dans le menu déroulant Type d’ensemble par lot, sélectionnez un type de paramètre prédéfini.

   Pour générer automatiquement une visionneuse à 360° 2D, sélectionnez **[!UICONTROL Visionneuse à 360° multi-axe]** dans la liste déroulante Type d’ensemble par lot.

1. Effectuez l’une des opérations suivantes :

   * Si vous utilisez une convention d’affectation de nom par défaut que vous avez précédemment définie sous **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Paramètres prédéfinis d’ensemble par lot]** > **[!UICONTROL Affectation de nom par défaut]**, développez **[!UICONTROL Conventions d’affectation de nom]**, puis dans la liste déroulante Affectation de nom de fichier, sélectionnez **[!UICONTROL Par défaut]**.
   * Pour définir une convention d’affectation de nom lors de la configuration du paramètre prédéfini, développez **[!UICONTROL Conventions d’affectation de nom]**, puis, dans la liste déroulante Affectation de nom de fichier, sélectionnez **[!UICONTROL Personnalisé]**.

1. Pour l’ordre des séquences, définissez l’ordre des images une fois la visionneuse regroupée dans Adobe Dynamic Media Classic. Par défaut, les fichiers seront classés par ordre alphanumérique. Cependant, vous pouvez utiliser une liste d’expressions courantes de format CSV (valeurs séparées par des virgules) pour définir l’ordre.
1. Pour la convention de création et d’affectation de nom de l’ensemble, spécifiez le suffixe ou le préfixe du nom de base que vous avez défini dans la convention d’affectation de nom. Définissez également l’emplacement de création de la visionneuse d’images dans la structure de dossiers Adobe Dynamic Media Classic.

   Si vous définissez un grand nombre de visionneuses d’images, séparez ces visionneuses des dossiers contenant les ressources elles-mêmes. De nombreux clients créent un dossier Visionneuses d’images et redirigent l’application pour y placer les visionneuses générées par une visionneuse par lot.

1. Sélectionnez **[!UICONTROL Enregistrer]** dans le panneau Détails.

### Création d’un paramètre prédéfini d’ensemble par lot pour la génération automatique d’une visionneuse à 360° en 2D {#creating-a-batch-set-preset-for-the-auto-generation-of-a-d-spin-set}

Vous pouvez utiliser le type d’ensemble par lot **Visionneuse à 360° multi-axe** pour créer une &quot;recette&quot; qui automatise la génération des visionneuses à 360° 2D. Le regroupement des images utilise les expressions régulières Ligne et Colonne afin que les fichiers d’image soient correctement alignés à l’emplacement correspondant dans le tableau multidimensionnel.

Voir aussi [Création d’un paramètre prédéfini d’ensemble par lot](application-setup.md#creating_a_batch_set_preset).

Il n’existe pas de nombre maximal ou minimal de lignes ou de colonnes dans une visionneuse à 360° multi-axe.

Par exemple, supposons que vous souhaitiez créer une visionneuse à 360° multi-axe nommée *spin-2dspin*. Vous disposez d’un ensemble d’images de visionneuse à 360° qui contiennent trois lignes, avec 12 images par ligne. Les images sont nommées comme suit :

```as3
spin-01-01
spin-01-02
… 
spin-01-12
spin-02-01
… 
spin-03-12
```

Avec ces informations, votre recette de type d’ensemble par lot peut être créée comme suit :

![Image de recette d’ensemble par lot](assets/se_batch_set_recipe.png)

Le regroupement de la partie du nom de ressource partagée de la visionneuse à 360° est ajouté au champ Correspondance (comme mis en surbrillance). La partie variable du nom de ressource contenant la ligne et la colonne est ajoutée respectivement aux champs Ligne et Colonne .

Lorsque la visionneuse à 360° est téléchargée et publiée, vous activez le nom de la recette de la visionneuse à 360° en 2D répertoriée sous **[!UICONTROL Paramètres prédéfinis d’ensemble par lot]** dans la boîte de dialogue Télécharger les options de la tâche.

**Pour créer un paramètre prédéfini d’ensemble par lot pour la génération automatique d’une visionneuse à 360° en 2D :**

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Paramètres prédéfinis d’ensemble par lot]** > **[!UICONTROL Paramètre prédéfini d’ensemble par lot]**. La vue par défaut est la vue **[!UICONTROL Afficher le formulaire]**, comme défini dans le coin supérieur droit de la page Détails.
1. Dans le panneau Liste des paramètres prédéfinis, sélectionnez **[!UICONTROL Ajouter]** pour activer les champs de définition dans le panneau Détails situé à droite de la page.
1. Dans le panneau Détails, dans le champ Nom du paramètre prédéfini, nommez le paramètre prédéfini.
1. Dans le menu déroulant Type d’ensemble par lot, sélectionnez **[!UICONTROL Visionneuse de fichiers]**.
1. Dans la liste déroulante Sous-type , sélectionnez **[!UICONTROL Visionneuse à 360° multi-axe]**.
1. Développez **[!UICONTROL Conventions d’affectation de nom]**, puis, dans la liste déroulante Affectation de nom de fichier, sélectionnez **[!UICONTROL Personnalisé]**.
1. Utilisez les attributs **[!UICONTROL Correspondance]** et, éventuellement, **[!UICONTROL Nom de base]** pour définir une expression régulière pour l’appellation des fichiers d’image du regroupement.

   Par exemple, votre expression régulière Correspondance littérale peut se présenter comme suit :

   `(\w+)-\w+-\w+`

1. Développez **[!UICONTROL Position des colonnes/lignes]**, puis définissez le format de nom de la position du fichier d’image dans le tableau de la visionneuse à 360° 2D.

   Placez la position de ligne ou de colonne entre parenthèses dans le nom de fichier.

   Par exemple, pour l’expression régulière de votre ligne, elle peut se présenter comme suit :

   `\w+-R([0-9]+)-\w+`

   ou

   `\w+-(\d+)-\w+`

   Pour l’expression régulière de colonne, elle peut se présenter comme suit :

   `\w+-\w+-C([0-9]+)`

   ou

   `\w+-\w+-C(\d+)`

   N’oubliez pas que ces expressions ne sont que des exemples. Vous pouvez créer votre expression régulière comme bon vous semble, en fonction de vos besoins.

   >[!NOTE]
   >
   >Si la combinaison d’expressions régulières dans les lignes et les colonnes ne peut pas déterminer la position de la ressource dans le tableau de la visionneuse à 360° multidimensionnelle, cette ressource n’est pas ajoutée à la visionneuse. Une erreur est consignée.

1. Pour la convention de création et d’affectation de nom de l’ensemble, spécifiez le suffixe ou le préfixe du nom de base que vous avez défini dans la convention d’affectation de nom. Définissez également l’emplacement de création de la visionneuse d’images dans la structure de dossiers Adobe Dynamic Media Classic.

   Si vous définissez un grand nombre de visionneuses d’images, séparez ces visionneuses des dossiers contenant les ressources elles-mêmes. De nombreux clients créent un dossier Visionneuses d’images et redirigent l’application pour y placer les visionneuses générées par une visionneuse par lot.

1. Sélectionnez **[!UICONTROL Enregistrer]** dans le panneau Détails.
1. Téléchargez et publiez votre visionneuse à 360° comme vous le faites habituellement, en veillant à activer le nom de la visionneuse à 360° 2D dans la boîte de dialogue Options de chargement de tâche, sous Paramètres prédéfinis d’ensemble par lot.

>[!MORELIKETHIS]
>
>* [Aperçu d’une ressource](previewing-asset.md#previewing_an_asset)
>* [Configuration de paramètres d’image prédéfinis](setting-image-presets.md#setting_up_image_presets)
>* [Affichage, ajout et exportation de métadonnées](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
>* [Vérifier les fichiers de tâche](checking-job-files.md#checking_job_files)
