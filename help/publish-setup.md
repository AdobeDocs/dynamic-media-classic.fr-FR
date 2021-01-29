---
title: Configuration de la publication
description: Les paramètres de l’écran Configuration de la publication déterminent comment les ressources sont distribuées par défaut depuis les serveurs Dynamic Media Classic vers les sites Web ou les applications.
uuid: 196f25c8-abf5-4c5d-8f6f-bc70007a0301
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: cba59093-28b6-4490-b838-d942b72ad1ec
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '2418'
ht-degree: 64%

---


# Configuration de la publication {#publish-setup}

Les paramètres de l’écran Configuration de la publication déterminent comment les ressources sont distribuées par défaut depuis les serveurs Dynamic Media Classic vers les sites Web ou les applications. Si aucun paramètre n’est spécifié, le serveur Dynamic Media Classic livre un fichier selon un paramètre par défaut sur un écran Configuration de la publication. Par exemple, une requête de diffusion d’une image qui ne contient pas d’attribut de résolution renvoie une image avec le paramètre Résolution d’objet par défaut de l’écran Image Server.

Les administrateurs peuvent modifier les paramètres par défaut sur les écrans Image Server, Image Renderer et Vignette pour définir les paramètres par défaut utilisés pour diffuser des fichiers à partir des serveurs.

Pour ouvrir les écrans Configuration de la publication, cliquez sur Configuration >Configuration de l’application > Configuration de la publication.

>[!NOTE]
>
>les écrans Configuration de la publication s’adressent aux développeurs et programmeurs chevronnés de sites Web. Dynamic Media Classic suppose que les utilisateurs qui modifient les paramètres de ces écrans connaissent Dynamic Media Classic, les normes et conventions de protocole HTTP et la technologie de base de l’imagerie.

## Image Server {#image-server}

L’écran Image Server définit les paramètres par défaut permettant de diffuser les images à partir des serveurs d’images. Les paramètres sont disponibles dans cinq catégories (voir l’écran Image Server pour obtenir une description détaillée des paramètres).

Modifiez ces paramètres uniquement avec l’aide d’une personne chargée du support Dynamic Media Classic.

**Gestion** des cataloguesCes paramètres déterminent comment Dynamic Media Classic et le catalogue interagissent. Contrairement à la plupart des serveurs Web, les appels d’URL du serveur Dynamic Media Image Server s’affichent dans un fichier manifest-or catalog-file plutôt que dans un fichier image proprement dit. Le fichier catalogue (à ne pas confondre avec un catalogue électronique) contient une liste de tous les contenus publiés sur le serveur d’images avec le chemin d’accès à chaque image. Si vous disposez d’un ID Digimarc, entrez vos informations d’utilisateur dans la section Informations d’utilisateur Digimarc.

**Request** AttributesCes paramètres imposent des limites aux images qui peuvent être diffusées à partir du serveur. Par exemple, *maximum* **[!UICONTROL Limite de taille de l’image de réponse]** est **[!UICONTROL Largeur]** 5000 et **[!UICONTROL Hauteur]** 5000.

**Attributs** de requête par défautCes paramètres se rapportent à l’aspect par défaut des images.

**Attributs** de miniature courantsCes paramètres concernent l’aspect par défaut et l’alignement des images miniatures.

**Valeurs par défaut des** champs du catalogue Ces paramètres concernent la résolution et le type de miniature par défaut des images.

**Attributs** de gestion des couleurs Ces paramètres déterminent les profils de couleur ICC utilisés.

**** Attributs de compatibilitéCe paramètre permet de traiter les paragraphes de début et de fin des calques de texte comme dans la version 3.6 pour une compatibilité descendante.

**Prise en** charge des localisationsCes paramètres vous permettent de gérer plusieurs attributs de paramètres régionaux. Il permet également de définir une chaîne de carte de paramètres régionaux pour définir les langues à prendre en charge pour les info-bulles dans les visionneuses.

Par exemple, si votre entreprise est une société multinationale qui vend dans différents pays, chaque pays peut avoir sa propre visionneuse correspondant aux paramètres régionaux. Pour accomplir cette fonctionnalité, vous spécifiez une chaîne de carte de paramètres régionaux. Vous pouvez ensuite modifier le texte d’info-bulle dans un paramètre prédéfini de la visionneuse en ajoutant les chaînes de texte traduites de la langue appropriée.

>[!NOTE]
> Pour configurer les options de prise en charge des Localisations, [utilisez le Admin Console pour créer un dossier de prise en charge.](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/support-for-experience-cloud.ug.html) Dans votre cas d’assistance, demandez de l’aide sur la configuration.

Pour plus d’informations sur la configuration de l’**Aide à la localisation**, voir [Considérations à prendre en compte lors de la configuration de la localisation des fichiers](publish-setup.md#considerations_when_setting_up_localization_of_assets).

### Considérations à prendre en compte lors de la configuration de la localisation des fichiers {#considerations-when-setting-up-localization-of-assets}

>[!NOTE]
>
>Si vous souhaitez configurer des options de prise en charge des Localisations dans Dynamic Media Classic, telles que le champ de carte des paramètres régionaux, [utilisez le Admin Console pour créer un dossier de prise en charge.](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/support-for-experience-cloud.ug.html) Dans votre cas d’assistance, demandez de l’aide sur la configuration.

Une manière courante d’utiliser Dynamic Media Classic consiste à gérer les images de produit sur les sites Web de commerce électronique. Les sociétés internationales doivent gérer le fait que l’aspect des fichiers pour des produits similaires diffère d’un pays à l’autre. En général, ces différences concernent une petite partie seulement de l’ensemble des médias. Le fait de gérer de telles différences en copiant tous les fichiers pour chacun des pays et en remplaçant uniquement les différences représente un effort considérable et contredit la métaphore du fichier original unique. De telles différences de fichiers peuvent impliquer, en raison des vidéos spécifiques aux pays avec différentes pistes audio, des différences importantes bien que très subtiles des câbles d’alimentation utilisés avec le produit. Dynamic Media Classic utilise un mécanisme de recherche de base. Vous définissez l’ordre des suffixes des fichiers analysés par le serveur d’images, en commençant par les paramètres régionaux requis.

**Méthode de localisation des fichiers**

Les paramètres régionaux pour une demande de diffusion d’image IS (Image Serving) est identifié avec la commande de rendu d’image IS/IR (Image Rendering) suivante :

`locale=`

Cette commande accepte une chaîne d’ID de paramètres régionaux (locId) non sensible à la casse. L’ID de paramètres régionaux est généralement une chaîne de 2 à 6 caractères composée de lettres et de signes « _ ».

IS prend en charge des chaînes ASCII imprimables arbitraires. La commande `locale=` a une portée globale, ce qui signifie qu&#39;elle est appliquée à la demande entière, y compris toutes les requêtes IS et IR imbriquées, les modèles référencés et les calques d&#39;image. Plusieurs paramètres régionaux par demande (par exemple un paramètre régional différent pour chaque calque) ne sont pas pris en charge. Toutefois, il est possible d’autoriser les remplacements explicites dans les demandes imbriquées.

Si `locale=` n&#39;est pas spécifié, `attribute::DefaultLocale` est transmis aux moteurs de traduction. La validation d&#39;entrée limitée est appliquée à la valeur `locale=`. Les valeurs `locale=` vides sont autorisées. Comme `locale=` a une portée globale, `attribute::DefaultLocale` est fourni par le catalogue principal pour l’ensemble de la demande.

L&#39;utilisation de `locale=` et `attribute::DefaultLocale` présente certains avantages, notamment :

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
| Visionneuses d’images et visionneuses de supports | La visionneuse d’images entière peut être différente pour certains paramètres régionaux (par exemple, lorsqu’un catalogue électronique est complètement différent) avec la conversion d’une visionneuse d’images générique en visionneuse d’images spécifique à un paramètre régional gérée par la visionneuse. Plus couramment, les ID individuels d’une visionneuse générique peuvent faire référence au contenu localisé. Par exemple, la plupart des photos d’un appareil peuvent être identiques dans toutes les langues, à l’exception de la photo du panneau de contrôle. IS traduit automatiquement les ID, si bien qu’il n’est pas nécessaire de générer des visionneuses d’images spécifiques aux paramètres régionaux. |

**Mise en œuvre de la localisation des fichiers**

Dynamic Media Classic et la diffusion d’images disposent d’une interface qui permet la localisation des images et du contenu statique.

Sans localisation, une URL de serveur d’images ressemble à ce qui suit :

`https://server/is/image/company/image`

Avec localisation, une URL de serveur d’images ajoute le paramètre `locale=` au chemin d’accès, comme dans l’exemple suivant :

`https://server/is/image/company/image?locale=de_DE`

A réception de l’appel http par le serveur d’images, le paramètre `locale=` est analysé dans le champ localeMap situé dans **Configuration** > **Configuration de l’application** > **Configuration de la publication** > **Image Server** > **Prise en charge de la Localisation**.

Le champ de carte de paramètres régionaux contient une liste des entrées séparées à l’aide du symbole de barre verticale (|).

Chaque entrée se compose d’une liste de valeurs séparées par des virgules. La première valeur est la valeur de recherche transmise par le paramètre `locale=`. Les autres valeurs sont les valeurs de suffixe/remplacement essayées les unes après les autres jusqu’à ce que l’une d’elles produise une image existante.

L’application d’une valeur de suffixe ou de remplacement dépend du paramètre régional Monde entier dans le groupe **Configuration** >**Configuration de l’application** > **Configuration de la publication** > **Serveur d’images** > **Aide à la localisation**.

>[!NOTE]
>
>Le paramètre régional global n’est actuellement possible que lorsque vous le définissez via l’API, et non dans l’interface Dynamic Media Classic.

**Exemple de suffixe**

| URL | ID de localeMap | Résultat |
|--- |--- |--- |
| `https://server/is/image/company/image?locale=de_DE` | `de_DE,_DE,|fr_FR,_FR,` | Aucun paramètre GlobalLocale n’est défini. Le paramètre régional de_DE est trié par rapport à la première entrée dans localeMap. La première valeur _DE correspondante est ajoutée sous forme de suffixe au fichier image_DE et est recherchée sur le serveur d’images. Si elle est trouvée sur le serveur, elle est renvoyée. Dans le cas contraire, la seconde valeur “” est utilisée comme suffixe et l’image elle-même est renvoyée. |

**Exemple de remplacement**

| URL | ID de GlobalLocale et localeMap | Résultat |
|--- |--- |--- |
| `https://server/is/image/company/image-main-01?locale=de_DE` | `GlobalLocale=mainlocaleMap -` <br><br/> `de_DE,de,main|fr_FR,fr,main` | Dans l’exemple de remplacement ci-dessus, GlobalLocale est défini sur main. Le paramètre régional de_DE est trié par rapport à la première entrée dans localeMap. La sous-chaîne GlobalLocale est trouvée et remplacée par la première valeur correspondante « de » dans le paramètre localeMap : image-de-01. Si elle est trouvée sur le serveur d’images, elle est renvoyée. Dans le cas contraire, la seconde valeur est remplacée, ce qui donne image-main-01. |

Si aucun paramètre régional n’est défini dans l’URL, le serveur d’images prend l’attribut DefaultLocale, s’il est défini, et l’applique à l’URL.

Si un paramètre régional inconnu ou vide est fourni avec `locale=`, la valeur vide &quot;starting with&quot; est recherchée dans localeMap. Il est important de configurer cette fonction pour qu’un paramètre régional par défaut soit appliqué aux paramètres régionaux inconnus.

**A propos de defaultImage**

Le serveur d’images essaie l’une après l’autre les options pour les paramètres régionaux demandés. Si aucune correspondance n’est trouvée, les options de paramètres régionaux sont appliquées à defaultImage et la version correspondante est renvoyée. Par conséquent, chaque paramètre régional doit inclure une option pour l’image sans localisation, ou les versions localisées de defaultImage doivent être rendues disponibles dans Dynamic Media Classic.

**Scénarios de recherche de localeMap**

Supposons que vous deviez prendre en charge les paramètres régionaux suivants :

`en, en_us, en_uk, de, de_at, de_de, fr`

Vous mappez ces paramètres régionaux aux suffixes `_E`, `_G` et `_F`, respectivement pour l’anglais, l’allemand et le français. Pour tous les exemples, l’ID de l’image d’entrée générique est `myImg`.

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

Vous pouvez également avoir un locSuffix dédié, tel que U, uniquement pour les paramètres régionaux inconnus, et forcer l’image par défaut si `_U` n’existe pas, comme dans l’exemple suivant :

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,U`

Ou vous pouvez établir la correspondance directement avec l’ID générique, comme dans l’exemple suivant :

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,`

*Recherche de localeMap à l’aide d’une recherche à plusieurs niveaux*

Il est généralement recommandé de regrouper les paramètres régionaux (européens, Moyen-Orient et nord-américains, par exemple) pour se conformer aux normes régionales, telles que l’exposition des habillages. Vous pouvez obtenir cet effet en utilisant une recherche à plusieurs niveaux.

Pour cet exemple, supposons que vous souhaitiez prendre en charge les collections pour une utilisation en Occident et au Moyen-Orient. Les deux collections reposent sur la collection d’images génériques, et ajoutent ou modifient toutes deux certaines images. Les deux collections sont ensuite affinées pour des paramètres régionaux spécifiques, tels que `m1, m2` pour deux variantes du Moyen-Orient et `w1, w2,` et `w3` pour trois paramètres régionaux occidentaux, à l’exception des images partagées pour `w1` et `w3`. Les paramètres régionaux inconnus sont mappés uniquement à la collection générique et n’ont pas accès aux images spécifiques à un paramètre régional. Voici à quoi doit ressembler le mappage :

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

En se basant sur le premier exemple, les images pour toutes les langues peuvent avoir les suffixes `_1`, `_2` ou `_3`. Les images propres aux paramètres régionaux français peuvent avoir le suffixe `_22` ou `_23`. Et les images propres aux paramètres régionaux allemands peuvent avoir le suffixe `_470` ou `_480`.

`attribute::LocaleMap=,_1,_2,_3|fr,_22,_23,_1,_2,_3|de,_470,_480,_1,_2,_3|de_at,_470,_480,_1,_2,_3|de_de,_470,_480,_1,_2,_3`

| locale= | ID de sortie à rechercher |
|--- |--- |
| fr | myImg_22, myImg_23, myImg_1, myImg_2, myImg_3 |
| de, de_at, de_de | myImg_470, myImg_480, myImg_1, myImg_2,myImg_3 |
| Tous les autres | myImg_1, myImg_2, myImg_3 |

**Considérations importantes lors de la mise en œuvre de l’aide à la localisation**

* La localisation se limite aux appels de fichier basés sur l’ID et ne peut pas être utilisée pour les appels de fichier basés sur le chemin d’accès. Par conséquent, lors de l’appel de vidéos avec des paramètres régionaux, celles-ci doivent être appelées en tant que company/assetID et non comme chemin d’accès complet à la vidéo. En d’autres termes, vous ne pouvez pas utiliser la méthode rtmp avec la localisation car elle peut uniquement être utilisée avec les appels de vidéos basés sur le chemin d’accès.
* Vous ne pouvez pas utiliser une visionneuse de supports variés contenant une seule vidéo lorsque localeMap est actif ; sinon, l’appel au contenu de la visionneuse échoue. Pour contourner ce problème, vous pouvez ajouter une vidéo unique à une visionneuse de vidéos adaptative. Ensuite, ajoutez la visionneuse de vidéos adaptative à une visionneuse de supports variés.
* Certaines demandes ne sont pas localisées, comme par exemple les demandes de contenu d’une visionneuse de vidéos adaptative. Par conséquent, si vous prévoyez d’utiliser des visionneuses de vidéos adaptatives avec la localisation, vous devez placer la visionneuse de vidéos adaptative dans une visionneuse de supports variés. Ensuite, appelez la visionneuse dans une visionneuse de supports variés avec le paramètre `locale=`.

## Image Renderer {#image-renderer}

L’écran Image Renderer définit les paramètres par défaut de la diffusion des visionneuses d’images à partir des serveurs de rendu d’images. Les paramètres sont disponibles dans les 5 catégories suivantes (voir l’écran Image Server pour obtenir des descriptions détaillées des paramètres) :

**Gestion** des cataloguesCes paramètres déterminent comment Dynamic Media Classic et le fichier catalogue interagissent. Les appels d’URL Dynamic Media Classic Render Server sont effectués vers le catalogue, qui à son tour appelle à diffuser des images à partir du serveur. Modifiez ces paramètres uniquement avec l’aide d’une personne chargée du support Dynamic Media Classic.

**Attributs** de sessionCes paramètres définissent les paramètres d&#39;erreur, l&#39;URL des URL d&#39;image relatives et si le chevauchement d&#39;objets est autorisé.

**Attributs de matériau par défaut** Ces paramètres définissent les paramètres de résolution et d’accentuation par défaut des images.

**Attributs** d&#39;image de réponseCes paramètres se rapportent à l&#39;aspect par défaut des images.

**Attributs de gestion des couleurs** Ces paramètres concernent les paramètres de couleur par défaut des images.

## Vignette {#vignette}

L’écran Vignette propose des paramètres permettant de définir l’aspect par défaut des vignettes (voir l’écran pour obtenir une description détaillée des options).
