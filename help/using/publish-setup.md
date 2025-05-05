---
title: Configuration de la publication
description: Les paramètres de configuration de Publish vous permettent de déterminer comment les ressources sont diffusées par défaut des serveurs Adobe Dynamic Media Classic aux sites Web ou aux applications.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Admin
exl-id: 699d4c12-e47b-4c6b-86f3-dc7aaaa56c1e
topic: Administration, Content Management
level: Intermediate
source-git-commit: 29752cf9eca0fc9bb760c721e1c3dc8e4ef912c3
workflow-type: tm+mt
source-wordcount: '2383'
ht-degree: 30%

---

# Configuration de la publication {#publish-setup}

Les paramètres de la page Configuration de Publish déterminent la manière dont les ressources sont diffusées par défaut des serveurs Adobe Dynamic Media Classic vers les sites Web ou les applications. Si aucun paramètre n’est spécifié, le serveur Adobe Dynamic Media Classic diffuse une ressource selon un paramètre par défaut sur une page de configuration de Publish. Par exemple, une demande de diffusion d’une image qui n’inclut pas d’attribut de résolution génère une image avec le paramètre de résolution d’objet par défaut sur la page Serveur d’images.

Les administrateurs peuvent modifier les paramètres par défaut sur les pages Image Server, Image Renderer et Vignette afin de définir les paramètres par défaut de diffusion des ressources à partir des serveurs.

Pour ouvrir les pages de la configuration de Publish, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Configuration de Publish]**.

>[!NOTE]
>
>Les pages Configuration de Publish sont destinées aux développeurs et programmeurs de sites Web expérimentés. Adobe Dynamic Media Classic suppose que les utilisateurs qui modifient les paramètres de ces pages connaissent Adobe Dynamic Media Classic, les normes et conventions de protocole HTTP, ainsi que la technologie d’imagerie de base.

## Image Server {#image-server}

La page Serveur d’images définit les paramètres par défaut de la diffusion des images à partir des serveurs d’images. Les paramètres sont disponibles dans ces cinq catégories (voir la page Image Server elle-même pour des descriptions détaillées des paramètres).

Modifiez ces paramètres uniquement avec l’aide d’un agent de support Adobe Dynamic Media Classic.

* **[!UICONTROL Gestion de catalogue]** : ces paramètres déterminent la manière dont Adobe Dynamic Media Classic et le catalogue interagissent. Contrairement à la plupart des serveurs Web, les appels d’URL de serveur d’images Dynamic Media sont dirigés vers un fichier manifeste ou catalogue plutôt qu’un fichier image proprement dit. Le fichier catalogue (à ne pas confondre avec un catalogue électronique) contient une liste de tout le contenu publié sur le serveur d’images. Il contient également le chemin d’accès à chaque image. Si vous disposez d’un ID Digimarc, entrez vos informations d’utilisateur dans la section Informations d’utilisateur Digimarc.

* **[!UICONTROL Attributs de requête]** : ces paramètres imposent des limites aux images qui peuvent être diffusées à partir du serveur. Par exemple, la *taille maximale* **[!UICONTROL Limite de taille de l’image de réponse]** est **[!UICONTROL largeur]** 5000 et **[!UICONTROL hauteur]** 5000.

* **[!UICONTROL Attributs de requête par défaut]** : ces paramètres concernent l’aspect par défaut des images.

* **[!UICONTROL Attributs de miniature courants]** : ces paramètres concernent l’aspect par défaut et l’alignement des images miniatures.

* **[!UICONTROL Valeurs par défaut des champs de catalogue]** : ces paramètres concernent la résolution et le type de miniature par défaut des images.

* **[!UICONTROL Attributs de gestion des couleurs]** : ces paramètres déterminent les profils de couleurs ICC utilisés.

* **[!UICONTROL Attributs de compatibilité]** : ce paramètre permet aux paragraphes de début et de fin des calques de texte d’être traités tels qu’ils l’étaient dans la version 3.6 pour une compatibilité descendante.

* **[!UICONTROL Aide à la localisation]** : ces paramètres vous permettent de gérer plusieurs attributs de paramètres régionaux. Il permet également de définir une chaîne de carte de paramètres régionaux pour définir les langues à prendre en charge pour les info-bulles dans les visionneuses.

  Par exemple, si votre entreprise est une société multinationale qui vend dans différents pays, chaque pays peut avoir sa propre visionneuse correspondant aux paramètres régionaux. Pour accomplir cette fonctionnalité, vous spécifiez une chaîne de carte de paramètres régionaux. Vous modifiez ensuite le texte de l’info-bulle dans le paramètre prédéfini d’une visionneuse. Il vous suffit d’ajouter les chaînes de texte traduites pour la langue souhaitée.

  >[!NOTE]
  > Pour configurer les options de prise en charge de la localisation, [ utilisez l&#39;Admin Console pour créer un cas de prise en charge.](https://helpx.adobe.com/fr/enterprise/using/support-for-experience-cloud.html) Dans votre cas d’assistance, demandez de l’aide sur la configuration.

  Pour plus d’informations sur la configuration de l’**[!UICONTROL Aide à la localisation]**, voir [Considérations à prendre en compte lors de la configuration de la localisation des fichiers](publish-setup.md#considerations_when_setting_up_localization_of_assets).

### Considérations à prendre en compte lors de la configuration de la localisation des fichiers {#considerations-when-setting-up-localization-of-assets}

>[!NOTE]
>
>Si vous souhaitez configurer les options de prise en charge de la localisation dans Adobe Dynamic Media Classic, telles que le champ Carte des paramètres régionaux, [ utilisez l’Admin Console pour créer un cas de prise en charge.](https://helpx.adobe.com/fr/enterprise/using/support-for-experience-cloud.html) Dans votre cas d’assistance, demandez de l’aide sur la configuration.

Une méthode courante d’utilisation d’Adobe Dynamic Media Classic consiste à gérer l’imagerie du produit sur les sites web e-Commerce. Les sociétés internationales doivent gérer le fait que l’aspect des fichiers pour des produits similaires diffère d’un pays à l’autre. Généralement, les différences concernent quelques parties du média global. Résoudre de telles différences en copiant toutes les ressources pour chacun des pays et en remplaçant uniquement les différences est un énorme effort et contredit la métaphore de la ressource principale unique. De telles différences de fichiers peuvent impliquer, en raison des vidéos spécifiques aux pays avec différentes pistes audio, des différences importantes bien que très subtiles des câbles d’alimentation utilisés avec le produit. Adobe Dynamic Media Classic utilise un mécanisme de recherche de base. Vous définissez l’ordre des suffixes des fichiers analysés par le serveur d’images, en commençant par les paramètres régionaux requis.

#### Comment les ressources sont localisées

Les paramètres régionaux pour une demande de diffusion d’image IS (Image Serving) est identifié avec la commande de rendu d’image IS/IR (Image Rendering) suivante :

`locale=`

Cette commande accepte une chaîne d’ID de paramètre régional (locId) qui n’est pas sensible à la casse. L’ID de paramètre régional est généralement une chaîne de 2 à 6 caractères composée de lettres et de &quot;`_`&quot;.

IS prend en charge les chaînes ASCII imprimables arbitraires. La commande `locale=` a une portée globale, ce qui signifie qu’elle est appliquée à l’ensemble de la requête, y compris toutes les requêtes IS et IR imbriquées, les modèles référencés et les calques d’image. Plusieurs paramètres régionaux par demande (par exemple un paramètre régional différent pour chaque calque) ne sont pas pris en charge. Toutefois, il est possible d’autoriser les remplacements explicites dans les demandes imbriquées.

Si `locale=` n’est pas spécifié, `attribute::DefaultLocale` est transmis aux moteurs de traduction. Une validation d’entrée limitée est appliquée à la valeur `locale=`. Les valeurs `locale=` vides sont autorisées. `locale=` ayant une portée globale, `attribute::DefaultLocale` est fourni par le catalogue principal pour l’ensemble de la requête.

Voici quelques-uns des avantages de l&#39;utilisation de `locale=` et `attribute::DefaultLocale` :

* Partage du contenu pour plusieurs paramètres régionaux.
* Accès à un contenu spécifique à un paramètre régional à l’aide des ID génériques.
* Flexibilité par rapport aux conventions d’affection de nom et à la gestion du contenu spécifique à un paramètre régional, par exemple préfixe/suffixe des paramètres régionaux ou contenu spécifique à un paramètre régional dans un catalogue distinct.
* Prise en charge de l’accès aux versions spécifiques aux paramètres régionaux.
* Les objets agrégés, tels que les visionneuses d’images, peuvent parfois contenir des références génériques à des contenus potentiellement spécifiques à des paramètres régionaux.
* Prend en charge tous les contenus gérés par des catalogues qui doivent être localisés, y compris les images, les visionneuses d’images, les vignettes, les matériaux et les enregistrements de configuration de la visionneuse.
* Réduction des modifications de la base de données IPS et des mécanismes de manifeste IS.
* La prise en charge des contenus statiques tels que les vidéos et les habillages est ajoutée lors de la mise en oeuvre de la norme RFC IS-63.
* Les paramètres régionaux par défaut sont configurables.

#### Scénarios d’application

| Application | Scénario |
| --- | --- |
| Localisation du lecteur | Une fois les catalogues de contenu statique mis en oeuvre, la localisation est entièrement contrôlée avec le paramètre locale= , ajouté à toutes les requêtes effectuées sur IS. Il peut exister des variantes spécifiques aux paramètres régionaux pour les enregistrements de configuration, habillages, écrans de démarrage, etc. Le contenu approprié est fourni par IS sans que la visionneuse doive savoir quel contenu est localisé et quels sont ses ID. |
| Images et vidéo | Les entreprises multinationales ont généralement recours à un contenu à la fois générique et spécifique à un paramètre régional. Grâce à ce mécanisme, une référence à une image ou à une vidéo peut être générique, tandis qu’IS diffuse le contenu spécifique à un paramètre régional, s’il existe. |
| Visionneuses d’images et de médias | La visionneuse d’images entière peut être différente pour certains paramètres régionaux, par exemple lorsqu’un catalogue électronique est différent, avec la traduction d’un ensemble d’images générique à un jeu d’images spécifique à un paramètre régional gérée par la visionneuse. Plus généralement, les identifiants individuels d’un ensemble générique peuvent faire référence à des contenus localisés. Par exemple, la plupart des photos d’un appareil peuvent être identiques dans toutes les langues, à l’exception de la photo du Panneau de Contrôle. IS traduit automatiquement les identifiants. Il n’est donc pas nécessaire de générer des visionneuses d’images spécifiques aux paramètres régionaux. |

#### Mise en oeuvre de la localisation des ressources

Adobe Dynamic Media Classic et la diffusion d’images disposent d’une interface qui permet de localiser les images et le contenu statique.

Sans localisation, une URL de serveur d’images ressemble à ce qui suit :

`https://server/is/image/company/image`

Avec la localisation, une URL de serveur d’images ajoute le paramètre `locale=` au chemin d’accès, comme dans l’exemple suivant :

`https://server/is/image/company/image?locale=de_DE`

À réception de l’appel http par le serveur d’images, le paramètre `locale=` est analysé via le champ `localeMap` situé dans le groupe **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Configuration de Publish]** > **[!UICONTROL Serveur d’images]** > **[!UICONTROL Assistance à la localisation]**.

Le champ de carte de paramètres régionaux contient une liste des entrées séparées à l’aide du symbole de barre verticale (|).

Chaque entrée se compose d’une liste de valeurs séparées par des virgules. La première valeur est la valeur de recherche transmise par le biais du paramètre `locale=`. Les valeurs restantes sont des suffixes/valeurs de remplacement qui sont ensuite essayées jusqu’à ce qu’une image existante se produise.

L’application d’une valeur de suffixe ou de remplacement dépend du paramètre régional Monde entier dans le groupe **[!UICONTROL Configuration]** >**[!UICONTROL Configuration de l’application]** > **[!UICONTROL Configuration de la publication]** > **[!UICONTROL Serveur d’images]** > **[!UICONTROL Aide à la localisation]**.

>[!NOTE]
>
>Le paramètre Global Locale n’est possible que lorsque vous le définissez via l’API, et non dans l’interface Adobe Dynamic Media Classic.

**Exemple de suffixe :**

| URL | ID de localeMap | Résultat | Remarques |
| --- | --- | --- | --- |
| `https://server/is/image/company/image?locale=de_DE` | `de_DE,_DE,` | `fr_FR,_FR,` | Aucun paramètre GlobalLocale n’est défini. Le paramètre de paramètre régional de_DE est mis en correspondance avec la première entrée dans `localeMap`. La première valeur correspondante _DE est ajoutée en tant que suffixe à la ressource image_DE et une tentative de recherche est effectuée sur le serveur d’images. S’il est trouvé sur le serveur, il est renvoyé. Dans le cas contraire, la seconde valeur &quot;&quot; est utilisée comme suffixe, ce qui entraîne le renvoi de l’image elle-même. |

**Exemple de remplacement :**

| URL | `GlobalLocale` et `localeMap` ID | Résultat | Remarques |
| --- | --- | --- | --- |
| `https://server/is/image/company/image-main-01?locale=de_DE` | `GlobalLocale=mainlocaleMap -` <br><br/> `de_DE,de,main` | `fr_FR,fr,main` | Dans l’exemple de remplacement ci-dessus, GlobalLocale est défini sur main. Le paramètre de paramètre régional de_DE est mis en correspondance avec la première entrée dans `localeMap`. La sous-chaîne GlobalLocale est trouvée et remplacée par la première valeur correspondante `de` dans `localeMap`: `image-de-01`. S’il est trouvé sur le serveur d’images, il est renvoyé. Dans le cas contraire, la seconde valeur est remplacée, ce qui entraîne `image-main-01`. |

Si aucun paramètre régional n’est défini dans l’URL, le serveur d’images prend l’attribut DefaultLocale, s’il est défini, et l’applique à l’URL.

Si un paramètre régional vide ou inconnu est fourni avec `locale=`, la valeur vide &quot;commence par&quot; est analysée dans `localeMap`. Il est important d’appliquer un paramètre régional par défaut pour les paramètres régionaux inconnus.

#### À propos de defaultImage

Le serveur d’images essaie l’une après l’autre les options pour les paramètres régionaux demandés. Si aucune correspondance n’est trouvée, les options des paramètres régionaux sont appliquées à defaultImage et la version correspondante est renvoyée. Par conséquent, chaque paramètre régional doit inclure une option pour l’image sans localisation ou les versions localisées defaultImage sont rendues disponibles dans Adobe Dynamic Media Classic.

#### Scénarios de recherche de localeMap

Supposons que vous deviez prendre en charge les paramètres régionaux suivants :

`en, en_us, en_uk, de, de_at, de_de, fr`

Vous mappez ces paramètres régionaux avec les suffixes `_E` (anglais), `_G` (allemand) et `_F` (français). Pour tous les exemples, l’ID d’image d’entrée générique est `myImg`.

##### Comportement standard pour rechercher la carte locale

Les ID de paramètres régionaux sont associés à leurs suffixes correspondants. Si aucun ID spécifique aux paramètres régionaux n’est trouvé dans le catalogue, l’ID générique est testée. Notez les valeurs locSuffix vides qui correspondent à l’ID générique.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,`

| locale= | ID de sortie à rechercher |
| --- | --- |
| en, en_us, en_uk | myImg_E, myImg |
| de, de_de, de_at | myImg_D, myImg |
| fr | myImg_F, myImg |
| Tous les autres | : |

##### Recherche de localeMap lorsque le paramètre régional est inconnu

Vous pouvez associer les paramètres régionaux inconnus aux ID spécifiques ou génériques. Par exemple, vous pouvez mapper des paramètres régionaux inconnus aux identifiants anglais ou, s’ils n’existent pas, aux identifiants génériques.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,_E,`

| locale= | ID de sortie à rechercher |
| --- | --- |
| de, de_de, de_at | myImg_D, myImg |
| fr | myImg_F, myImg |
| Tous les autres | myImg_E, myImg |

Vous pouvez également avoir un locSuffix dédié, tel que U, uniquement pour les paramètres régionaux inconnus, et forcer l’image par défaut si aucun `_U` n’existe, comme dans l’exemple suivant :

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,U`

Ou vous pouvez établir la correspondance directement avec l’ID générique, comme dans l’exemple suivant :

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,`

##### Recherche de localeMap à l’aide d’une recherche à plusieurs niveaux

Il est généralement recommandé de regrouper les paramètres régionaux (européens, Moyen-Orient et nord-américains, par exemple) pour se conformer aux normes régionales, telles que l’exposition des habillages. Vous pouvez obtenir cet effet en utilisant une recherche à plusieurs niveaux.

Supposons, par exemple, que vous souhaitiez prendre en charge les collections pour une utilisation occidentale et moyen-orientale. Les deux collections reposent sur la collection d’images génériques, et ajoutent ou modifient toutes deux certaines images. Les deux collections sont ensuite affinées pour des paramètres régionaux spécifiques. Par exemple, `m1, m2` pour deux variantes du Moyen-Orient et `w1, w2,` et `w3` pour trois paramètres régionaux occidentaux, sauf que les images sont partagées pour `w1` et `w3`. Les paramètres régionaux inconnus sont mappés uniquement à la collection générique et n’ont pas accès aux images spécifiques à un paramètre régional. Voici à quoi doit ressembler le mappage :

`attribute::LocaleMap=w1,-W,|w2,-W2,-W,|w3,-W,|m1,-M1,-M,|m2,-M2,-M,|,`

| locale= | ID de sortie à rechercher |
| --- | --- |
| w1, w3 | myImg-W, myImg |
| w2 | myImg-W2, myImg-W, myImg |
| m1 | myImg-M1, myImg-M, myImg |
| m2 | myImg-M2, myImg-M, myImg |
| Tous les autres | mylmg |

##### Recherchez localeMap en recherchant des identifiants spécifiques.

Certaines conventions de dénomination d’image ne prennent pas en charge les ID d’image génériques. Les ID génériques issus de la demande doivent être mappés à l’ID spécifié dans le catalogue. Cependant, il existe des cas où l’identifiant spécifique exact n’est pas connu.

En reprenant le premier exemple comme base, les images pour toutes les langues peuvent avoir les suffixes `_1`, `_2` ou `_3`. Les images spécifiques aux paramètres régionaux français peuvent avoir le suffixe `_22` ou `_23`. Et les images spécifiques aux paramètres régionaux allemands peuvent avoir les suffixes `_470` ou `_480`.

`attribute::LocaleMap=,_1,_2,_3|fr,_22,_23,_1,_2,_3|de,_470,_480,_1,_2,_3|de_at,_470,_480,_1,_2,_3|de_de,_470,_480,_1,_2,_3`

| locale= | ID de sortie à rechercher |
| --- | --- |
| fr | myImg_22, myImg_23, myImg_1, myImg_2, myImg_3 |
| de, de_at, de_de | myImg_470, myImg_480, myImg_1, myImg_2,myImg_3 |
| Tous les autres | myImg_1, myImg_2, myImg_3 |

##### Remarques importantes concernant la mise en oeuvre de la prise en charge de la localisation

* La localisation se limite aux appels de fichier basés sur l’ID et ne peut pas être utilisée pour les appels de fichier basés sur le chemin d’accès. Par conséquent, lors de l’appel de vidéos avec des paramètres régionaux, celles-ci doivent être appelées en tant que company/assetID et non comme chemin d’accès complet à la vidéo. Vous ne pouvez pas utiliser `RTMP` avec la localisation, car cette méthode est réservée aux appels vidéo basés sur un chemin d’accès.
* Vous ne pouvez pas utiliser une visionneuse de supports variés contenant une seule vidéo lorsque localeMap est actif ; sinon, l’appel au contenu de la visionneuse échoue. Pour contourner ce problème, vous pouvez ajouter une seule vidéo à une visionneuse de vidéos adaptative. Ensuite, ajoutez la visionneuse de vidéos adaptative à une visionneuse de supports variés.
* Certaines demandes ne sont pas localisées, comme par exemple les demandes de contenu d’une visionneuse de vidéos adaptative. Par conséquent, si vous envisagez d’utiliser des visionneuses de vidéos adaptatives avec une localisation, placez la visionneuse de vidéos adaptative dans une visionneuse de médias mixtes. Ensuite, appelez la visionneuse dans une visionneuse de supports variés avec le paramètre `locale=` .

## Image Renderer {#image-renderer}

La page Image Renderer définit les paramètres par défaut pour la diffusion de visionneuses d’images à partir des serveurs de rendu d’image. Les paramètres sont disponibles dans ces cinq catégories (voir la page Image Server elle-même pour obtenir des descriptions détaillées des paramètres) :

* **[!UICONTROL Gestion de catalogue]** : ces paramètres déterminent la manière dont Adobe Dynamic Media Classic et le fichier de catalogue interagissent. Les appels d’URL de serveur de rendu Adobe Dynamic Media Classic sont effectués vers le catalogue, qui à son tour appelle pour diffuser des images à partir du serveur. Modifiez ces paramètres uniquement avec l’aide d’un agent de support Adobe Dynamic Media Classic.

* **[!UICONTROL Attributs de session]** : ces paramètres établissent des paramètres d’erreur, l’URL des URL d’image relatives et si le recouvrement d’objets est autorisé.

* **[!UICONTROL Attributs de matière par défaut]** : ces paramètres définissent les paramètres de résolution et d’accentuation par défaut des images.

* **[!UICONTROL Attributs d’image de réponse]** : ces paramètres concernent l’aspect par défaut des images.

* **[!UICONTROL Attributs de gestion des couleurs]** : ces paramètres concernent les paramètres de couleurs par défaut des images.

## Vignette {#vignette}

La page Vignette propose des paramètres pour définir l’aspect par défaut des vignettes (voir la page elle-même pour obtenir une description détaillée des options).
