---
title: Configuration de la publication
seo-title: Configuration de la publication
description: 'null'
seo-description: Les paramètres de l'écran Configuration de la publication déterminent la manière dont les fichiers sont diffusés par défaut à partir des serveurs Dynamic Media Classic vers les sites Web ou les applications.
uuid: 196 f 25 c 8-abf 5-4 c 5 d -8 f 6 f-bc 70007 a 0301
contentOwner: admin
content-type: référence
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
discoiquuid: cba 59093-28 b 6-4490-b 838-d 942 b 72 ad 1 ec
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Configuration de la publication {#publish-setup}

Les paramètres de l'écran Configuration de la publication déterminent la manière dont les fichiers sont diffusés par défaut à partir des serveurs Dynamic Media Classic vers les sites Web ou les applications. Si aucun paramètre n'est spécifié, le serveur Dynamic Media Classic fournit un fichier en fonction d'un paramètre par défaut sur l'écran Configuration de la publication. Par exemple, une requête de diffusion d’une image qui ne contient pas d’attribut de résolution renvoie une image avec le paramètre Résolution d’objet par défaut de l’écran Image Server.

Les administrateurs peuvent modifier les paramètres par défaut sur les écrans Image Server, Image Renderer et Vignette pour définir les paramètres par défaut utilisés pour diffuser des fichiers à partir des serveurs.

Pour ouvrir les écrans Configuration de la publication, cliquez sur Configuration &gt;Configuration de l’application &gt; Configuration de la publication.

>[!NOTE]
>
>les écrans Configuration de la publication s’adressent aux développeurs et programmeurs chevronnés de sites Web. Dynamic Media Classic suppose que les utilisateurs qui modifient les paramètres de ces écrans sont familiarisés avec Scene 7 Publishing System, les normes et les conventions de protocole HTTP et la technologie de base de l'image.

## Image Server {#image-server}

L’écran Image Server définit les paramètres par défaut permettant de diffuser les images à partir des serveurs d’images. Les paramètres sont disponibles dans cinq catégories (voir l’écran Image Server pour obtenir une description détaillée des paramètres).

Modifiez ces paramètres uniquement avec l'assistance d'une personne prise en charge de Media Classic Classic.

**Gestion des catalogues** Ces paramètres déterminent la manière dont Scene 7 Publishing System et le catalogue interagissent. Contrairement à la plupart des serveurs Web, les appels d'URL de serveur multimédia dynamique sont dirigés vers un fichier de manifeste ou de catalogue plutôt qu'un fichier image. Le fichier catalogue (à ne pas confondre avec un catalogue électronique) contient une liste de tous les contenus publiés sur le serveur d’images avec le chemin d’accès à chaque image. Si vous disposez d’un ID Digimarc, entrez vos informations d’utilisateur dans la section Informations d’utilisateur Digimarc.

**Attributs de requête** Ces paramètres imposent des limites aux images pouvant être diffusées à partir du serveur.

**Attributs de requête par défaut** Ces paramètres concernent l'aspect par défaut des images.

**Attributs de miniature courants** Ces paramètres concernent l'aspect par défaut et l'alignement des images miniatures.

**Valeurs par défaut des champs** de catalogue Ces paramètres concernent la résolution et le type de miniature par défaut des images.

**Attributs de gestion des couleurs** Ces paramètres déterminent les profils de couleurs ICC utilisés.

**Attributs de compatibilité** Ce paramètre permet aux paragraphes de début et de fin des calques de texte d'être traités comme dans la version 3.6 pour une compatibilité ascendante.

**Prise en charge de la localisation** Ces paramètres permettent de gérer plusieurs attributs de paramètres régionaux. Il permet également de définir une chaîne de carte de paramètres régionaux pour définir les langues à prendre en charge pour les info-bulles dans les visionneuses.

Par exemple, si votre entreprise est une société multinationale qui vend dans différents pays, chaque pays peut avoir sa propre visionneuse correspondant aux paramètres régionaux. Pour accomplir cette fonctionnalité, vous spécifiez une chaîne de carte de paramètres régionaux. Vous pouvez ensuite modifier le texte d’info-bulle dans un paramètre prédéfini de la visionneuse en ajoutant les chaînes de texte traduites de la langue appropriée.

>[!NOTE]
> Pour configurer les options d'aide à la localisation, contactez l'assistance technique d'Adobe Dynamic Media Classic ou envoyez un courrier électronique à s7support@adobe.com pour demander l'aide de configuration.

Pour plus d’informations sur la configuration de l’**Aide à la localisation**, voir [Considérations à prendre en compte lors de la configuration de la localisation des fichiers](publish-setup.md#considerations_when_setting_up_localization_of_assets).

### Considérations à prendre en compte lors de la configuration de la localisation des fichiers {#considerations-when-setting-up-localization-of-assets}

>[!NOTE]
>
>Si vous souhaitez configurer les options d'aide à la localisation dans Scene 7 Publishing System, comme le champ Carte de paramètres régionaux, contactez l'assistance technique d'Adobe Dynamic Media Classic. Ou envoyez un courrier électronique à s7support@adobe.com pour demander de l’aide au sujet de la configuration.

L’une des façons courantes d’utiliser Scene7 Publishing System (SPS) consiste à gérer les images de produit sur les sites Web de commerce électronique. Les sociétés internationales doivent gérer le fait que l’aspect des fichiers pour des produits similaires diffère d’un pays à l’autre. En général, ces différences concernent une petite partie seulement de l’ensemble des médias. Le fait de gérer de telles différences en copiant tous les fichiers pour chacun des pays et en remplaçant uniquement les différences représente un effort considérable et contredit la métaphore du fichier original unique. De telles différences de fichiers peuvent impliquer, en raison des vidéos spécifiques aux pays avec différentes pistes audio, des différences importantes bien que très subtiles des câbles d’alimentation utilisés avec le produit. Dynamic Media Classic utilise un mécanisme de recherche de base. Vous définissez l’ordre des suffixes des fichiers analysés par le serveur d’images, en commençant par les paramètres régionaux requis.

**Méthode de localisation des fichiers**

Les paramètres régionaux pour une demande de diffusion d’image IS (Image Serving) est identifié avec la commande de rendu d’image IS/IR (Image Rendering) suivante :

`locale=`

Cette commande accepte une chaîne d’ID de paramètres régionaux (locId) non sensible à la casse. L’ID de paramètres régionaux est généralement une chaîne de 2 à 6 caractères composée de lettres et de signes « _ ».

IS supports arbitrary printable ASCII strings.The `locale=` command has a global scope, meaning that it is applied to the entire request, including all nested IS and IR requests, referenced templates, and image layers. Plusieurs paramètres régionaux par demande (par exemple un paramètre régional différent pour chaque calque) ne sont pas pris en charge. Toutefois, il est possible d’autoriser les remplacements explicites dans les demandes imbriquées.

If `locale=` is not specified, `attribute::DefaultLocale` is passed to the translation engines. Limited input validation is applied to the `locale=` value. Empty `locale=` values are permitted. Because `locale=` has a global scope, `attribute::DefaultLocale` is provided by the main catalog for the entire request.

Some of the benefits of using `locale=` and `attribute::DefaultLocale` include the following:

* Partage du contenu pour plusieurs paramètres régionaux.
* Accès à un contenu spécifique à un paramètre régional à l’aide des ID génériques.
* Flexibilité par rapport aux conventions d’affection de nom et à la gestion du contenu spécifique à un paramètre régional, par exemple préfixe/suffixe des paramètres régionaux ou contenu spécifique à un paramètre régional dans un catalogue distinct.
* Prise en charge de l’accès direct pour les versions spécifiques à un paramètre régional.
* L’agrégation des objets (visionneuses d’images par exemple) peut contenir des références génériques au contenu potentiellement spécifique à un paramètre régional.
* Prise en charge de tout le contenu géré par des catalogues qui peuvent devoir être localisés, notamment les images, les visionneuses d’images, les vignettes, les brochures et les enregistrements de configuration de la visionneuse.
* Réduction des modifications de la base de données IPS et des mécanismes de manifeste IS.
* La prise en charge du contenu statique (vidéos et habillages par exemple) sera ajoutée lors de la mise en œuvre de RFC IS-63.
* Les paramètres régionaux par défaut sont configurables.

**Scénarios d’application**

| Application | Scénario |
|--- |--- |
| Localisation de la visionneuse | Une fois les catalogues de contenu statique mis en œuvre, la localisation est entièrement contrôlée avec le paramètre locale=, qui est annexé à toutes les demandes envoyées à IS. Il peut exister des variantes spécifiques aux paramètres régionaux pour les enregistrements de configuration, habillages, écrans de démarrage, etc. Le contenu approprié est fourni par IS sans que la visionneuse doive savoir quel contenu est localisé et quels sont ses ID. |
| Images et vidéo | Les entreprises multinationales ont généralement recours à un contenu à la fois générique et spécifique à un paramètre régional. Grâce à ce mécanisme, une référence à une image ou à une vidéo peut être générique, tandis qu’IS diffuse le contenu spécifique à un paramètre régional, s’il existe. |
| Visionneuses d’images et visionneuses de supports | L'ensemble de la visionneuse d'images peut être différent pour certains paramètres régionaux (par exemple, lorsqu'un catalogue électronique est complètement différent) avec la traduction d'une visionneuse générique en visionneuse d'images spécifique à un paramètre régional gérée par la visionneuse. Plus souvent, les ID individuels d'un jeu générique peuvent faire référence au contenu localisé. Par exemple, la plupart des photos d’un appareil peuvent être identiques dans toutes les langues, à l’exception de la photo du panneau de contrôle. IS traduit automatiquement les ID, si bien qu’il n’est pas nécessaire de générer des visionneuses d’images spécifiques aux paramètres régionaux. |

**Mise en œuvre de la localisation des fichiers**

L’interface de Scene7 Publishing et d’Image Serving permet la localisation des images et du contenu statique.

Sans localisation, une URL de serveur d’images ressemble à ce qui suit :

`https://server/is/image/company/image`

With localization, an Image Server URL adds the `locale=` parameter to the path, as in the following:

`https://server/is/image/company/image?locale=de_DE`

On receipt of the http call by the Image Server, the `locale=` parameter is parsed through the localeMap field found in **Setup** &gt; **Application Setup** &gt; **Publish Setup** &gt; **Image Server** &gt; **Localization Support** group.

Le champ de carte de paramètres régionaux contient une liste des entrées séparées à l’aide du symbole de barre verticale (|).

Chaque entrée se compose d’une liste de valeurs séparées par des virgules. The first value is the search value that is passed by the `locale=` parameter. Les autres valeurs sont les valeurs de suffixe/remplacement essayées les unes après les autres jusqu’à ce que l’une d’elles produise une image existante.

L’application d’une valeur de suffixe ou de remplacement dépend du paramètre régional Monde entier dans le groupe **Configuration** &gt;**Configuration de l’application** &gt; **Configuration de la publication** &gt; **Serveur d’images** &gt; **Aide à la localisation**.

>[!NOTE]
>
>le paramètre régional Monde entier est actuellement possible uniquement si vous l’avez défini par l’API, et non dans l’interface de Scene7 Publishing System.

**Exemple de suffixe**

| URL | ID de localeMap | Résultat |
|--- |--- |--- |
| `https://server/is/image/company/image?locale=de_DE` | `de_DE,_DE,|fr_FR,_FR,` | Aucun paramètre GlobalLocale n’est défini. Le paramètre régional de_DE est trié par rapport à la première entrée dans localeMap. La première valeur _DE correspondante est ajoutée sous forme de suffixe au fichier image_DE et est recherchée sur le serveur d’images. Si elle est trouvée sur le serveur, elle est renvoyée. Dans le cas contraire, la seconde valeur “” est utilisée comme suffixe et l’image elle-même est renvoyée. |

**Exemple de remplacement**

| URL | ID de GlobalLocale et localeMap | Résultat |
|--- |--- |--- |
| `https://server/is/image/company/image-main-01?locale=de_DE` | `GlobalLocale=mainlocaleMap -` <br><br/> `de_DE,de,main|fr_FR,fr,main` | Dans l’exemple de remplacement ci-dessus, GlobalLocale est défini sur main. Le paramètre régional de_DE est trié par rapport à la première entrée dans localeMap. La sous-chaîne GlobalLocale est trouvée et remplacée par la première valeur correspondante « de » dans le paramètre localeMap : image-de-01. Si elle est trouvée sur le serveur d’images, elle est renvoyée. Dans le cas contraire, la seconde valeur est remplacée, ce qui donne image-main-01. |

Si aucun paramètre régional n’est défini dans l’URL, le serveur d’images prend l’attribut DefaultLocale, s’il est défini, et l’applique à l’URL.

If an unknown or empty locale parameter is supplied with `locale=`, then the localeMap is scanned for the empty value “starting with,”. Il est important de configurer cette fonction pour qu’un paramètre régional par défaut soit appliqué aux paramètres régionaux inconnus.

**A propos de defaultImage**

Le serveur d’images essaie l’une après l’autre les options pour les paramètres régionaux demandés. Si aucune correspondance n’est trouvée, les options de paramètres régionaux sont appliquées à defaultImage et la version correspondante est renvoyée. Par conséquent, chaque paramètre régional doit inclure une option pour l’image sans localisation ou les versions localisées de defaultImage doivent être rendues disponibles dans Scene7 Publishing System.

**Scénarios de recherche de localeMap**

Supposons que vous deviez prendre en charge les paramètres régionaux suivants :

`en, en_us, en_uk, de, de_at, de_de, fr`

You map these locales to the suffixes `_E`, `_G`, and `_F`, for English, German, and French, respectively. Pour tous les exemples, l’ID de l’image d’entrée générique est `myImg`.

*Comportement standard de recherche de localeMap*

Les ID de paramètres régionaux sont associés à leurs suffixes correspondants. Si aucun ID spécifique aux paramètres régionaux n’est trouvé dans le catalogue, l’ID générique est testée. Observez les valeurs locSuffix vides qui correspondent à l’ID générique.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,`

| locale= | ID de sortie à rechercher |
|--- |--- |
| en,en_us, en_uk | myImg_E,myImg |
| de,de_de,de_at | myImg_D,myImg |
| fr | myImg_F,myImg |
| Tous les autres | - |

*Recherche de localeMap lorsque les paramètres régionaux sont inconnus*

Vous pouvez associer les paramètres régionaux inconnus aux ID spécifiques ou génériques. Dans notre exemple, vous pouvez associer les paramètres régionaux inconnus aux ID Anglais ou, s’ils n’existent pas, aux identifiants génériques.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,_E,`

| locale= | ID de sortie à rechercher |
|--- |--- |
| de,de_de,de_at | myImg_D,myImg |
| fr | myImg_F,myImg |
| Tous les autres | myImg_E,myImg |

You could also have a dedicated locSuffix, such as U, just for unknown locales, and force to the default image if no `_U` exists, as in the following:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,U`

Ou vous pouvez établir la correspondance directement avec l’ID générique, comme dans l’exemple suivant :

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,`

*Recherche de localeMap à l’aide d’une recherche à plusieurs niveaux*

Il est généralement recommandé de regrouper les paramètres régionaux (européens, Moyen-Orient et nord-américains, par exemple) pour se conformer aux normes régionales, telles que l’exposition des habillages. Vous pouvez obtenir cet effet en utilisant une recherche à plusieurs niveaux.

Pour cet exemple, supposons que vous souhaitiez prendre en charge les collections pour une utilisation en Occident et au Moyen-Orient. Les deux collections reposent sur la collection d’images génériques, et ajoutent ou modifient toutes deux certaines images. Both collections are then further refined for specific locales, such as `m1, m2` for two middle-eastern variants, and `w1, w2,` and `w3` for three Western locales, except that images are shared for `w1` and `w3`. Les paramètres régionaux inconnus sont mappés uniquement à la collection générique et n’ont pas accès aux images spécifiques à un paramètre régional. Voici à quoi doit ressembler le mappage :

`attribute::LocaleMap=w1,-W,|w2,-W2,-W,|w3,-W,|m1,-M1,-M,|m2,-M2,-M,|,`

| locale= | ID de sortie à rechercher |
|--- |--- |
| w1, w3 | myImg-W, myImg |
| w2 | myImg-W2, myImg-W, myImg |
| m1 | myImg-M1, myImg-M, myImg |
| m2 | myImg-M2, myImg-M, myImg |
| Tous les autres | mylmg |

*Recherche de localeMap en recherchant des ID spécifiques*

Certaines conventions d’affectation de nom des images peuvent ne pas prendre en charge les ID d’images génériques. Les ID génériques issus de la demande doivent être mappés à l’ID spécifié dans le catalogue. Cependant, il arrive que l’ID spécifique exact ne soit pas connu.

Using the first example as a basis, images for all languages may have the suffixes `_1`, `_2`, or `_3`. Images that are specific to French locales may have the suffixes `_22` or `_23` suffix. And images that are specific to German locales may have the suffixes `_470` or `_480`.

`attribute::LocaleMap=,_1,_2,_3|fr,_22,_23,_1,_2,_3|de,_470,_480,_1,_2,_3|de_at,_470,_480,_1,_2,_3|de_de,_470,_480,_1,_2,_3`

| locale= | ID de sortie à rechercher |
|--- |--- |
| fr | myImg_22, myImg_23, myImg_1, myImg_2, myImg_3 |
| de, de_at, de_de | myImg_470, myImg_480, myImg_1, myImg_2,myImg_3 |
| Tous les autres | myImg_1, myImg_2, myImg_3 |

**Considérations importantes lors de la mise en œuvre de l’aide à la localisation**

* La localisation se limite aux appels de fichier basés sur l’ID et ne peut pas être utilisée pour les appels de fichier basés sur le chemin d’accès. Par conséquent, lors de l’appel de vidéos avec des paramètres régionaux, celles-ci doivent être appelées en tant que company/assetID et non comme chemin d’accès complet à la vidéo. En d’autres termes, vous ne pouvez pas utiliser la méthode rtmp avec la localisation car elle peut uniquement être utilisée avec les appels de vidéos basés sur le chemin d’accès.
* Vous ne pouvez pas utiliser une visionneuse de supports variés contenant une seule vidéo lorsque localeMap est actif ; sinon, l’appel au contenu de la visionneuse échoue. Pour contourner ce problème, vous pouvez ajouter une vidéo unique à une visionneuse de vidéos adaptative. Ensuite, ajoutez la visionneuse de vidéos adaptative à une visionneuse de supports variés.
* Certaines demandes ne sont pas localisées, comme par exemple les demandes de contenu d’une visionneuse de vidéos adaptative. Par conséquent, si vous prévoyez d’utiliser des visionneuses de vidéos adaptatives avec la localisation, vous devez placer la visionneuse de vidéos adaptative dans une visionneuse de supports variés. Then, call the set into a Mixed Media viewer with the `locale=` parameter.

## Image Renderer {#image-renderer}

L’écran Image Renderer définit les paramètres par défaut de la diffusion des visionneuses d’images à partir des serveurs de rendu d’images. Les paramètres sont disponibles dans les 5 catégories suivantes (voir l’écran Image Server pour obtenir des descriptions détaillées des paramètres) :

**Gestion des catalogues** Ces paramètres déterminent comment Scene 7 Publishing System et le fichier de catalogue interagissent. Les appels d'URL de serveur multimédia Classic Media Classic sont dirigés vers le catalogue, qui à son tour lance un appel pour diffuser des images à partir du serveur. Modifiez ces paramètres uniquement avec l'assistance d'une personne prise en charge de Media Classic Classic.

**Attributs de session** Ces paramètres définissent des paramètres d'erreur, l'URL des URL d'image relative et le chevauchement des objets.

**Attributs de matériel par défaut** Ces paramètres définissent les paramètres de résolution et d'accentuation par défaut des images.

**Attributs d'image de réponse** Ces paramètres concernent l'aspect par défaut des images.

**Attributs de gestion des couleurs** Ces paramètres concernent les paramètres de couleur par défaut des images.

## Vignette {#vignette}

L’écran Vignette propose des paramètres permettant de définir l’aspect par défaut des vignettes (voir l’écran pour obtenir une description détaillée des options).
