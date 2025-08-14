---
title: Configuration de la publication
description: Les paramètres de configuration de la publication vous permettent de déterminer comment les ressources sont diffusées par défaut des serveurs Adobe Dynamic Media Classic vers les sites web ou les applications.
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

Les paramètres de la page Configuration de la publication déterminent la manière dont les ressources sont diffusées par défaut des serveurs Adobe Dynamic Media Classic vers les sites web ou les applications. Si aucun paramètre n’est spécifié, le serveur Adobe Dynamic Media Classic diffuse une ressource selon un paramètre par défaut sur une page de configuration de la publication. Par exemple, une demande de diffusion d’une image qui n’inclut pas d’attribut de résolution génère une image avec le paramètre Résolution d’objet par défaut sur la page du serveur d’images.

Les administrateurs peuvent modifier les paramètres par défaut sur les pages Serveur d’images, Moteur de rendu d’image et Vignette afin d’établir les paramètres par défaut pour la diffusion de ressources à partir des serveurs .

Pour ouvrir les pages de la configuration de la publication, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Configuration de la publication]**.

>[!NOTE]
>
>Les pages de configuration de la publication sont destinées aux développeurs et programmeurs chevronnés de sites Web. Adobe Dynamic Media Classic suppose que les utilisateurs qui modifient les paramètres de ces pages connaissent Adobe Dynamic Media Classic, les normes et conventions de protocole HTTP et la technologie d’imagerie de base.

## Image Server {#image-server}

La page Serveur d’images établit les paramètres par défaut pour la diffusion d’images à partir des serveurs d’images. Les paramètres sont disponibles dans ces cinq catégories (pour obtenir une description détaillée des paramètres, reportez-vous à la page Serveur d’images elle-même).

Modifiez ces paramètres uniquement avec l’aide d’une personne d’assistance Adobe Dynamic Media Classic.

* **[!UICONTROL Gestion des catalogues]** : ces paramètres déterminent la manière dont Adobe Dynamic Media Classic et le catalogue interagissent. Contrairement à la plupart des serveurs Web, les appels d’URL du serveur d’images Dynamic Media sont dirigés vers un fichier manifeste ou catalogue plutôt que vers un fichier image proprement dit. Le fichier catalogue (à ne pas confondre avec un catalogue électronique) contient une liste de tout le contenu publié sur le serveur d’images. Il contient également le chemin d’accès à chaque image. Si vous disposez d’un ID Digimarc, entrez vos informations d’utilisateur dans la section Informations d’utilisateur Digimarc.

* **[!UICONTROL Attributs de requête]** : ces paramètres imposent des limites aux images qui peuvent être diffusées à partir du serveur. Par exemple, la *taille maximale* **[!UICONTROL limite de taille de l’image de réponse]** est **[!UICONTROL largeur]** 5 000 et **[!UICONTROL hauteur]** 5 000.

* **[!UICONTROL Attributs de requête par défaut]** : ces paramètres concernent l’aspect par défaut des images.

* **[!UICONTROL Attributs de miniature courants]** : ces paramètres concernent l’aspect par défaut et l’alignement des images miniatures.

* **[!UICONTROL Valeurs par défaut des champs de catalogue]** : ces paramètres concernent la résolution et le type de miniature par défaut des images.

* **[!UICONTROL Attributs de gestion des couleurs]** : ces paramètres déterminent les profils de couleurs ICC utilisés.

* **[!UICONTROL Attributs de compatibilité]** : ce paramètre permet de traiter les paragraphes de début et de fin des calques de texte comme ils l’étaient dans la version 3.6 à des fins de rétrocompatibilité.

* **[!UICONTROL Prise en charge de la localisation]** : ces paramètres vous permettent de gérer plusieurs attributs de paramètres régionaux. Il permet également de définir une chaîne de carte de paramètres régionaux pour définir les langues à prendre en charge pour les info-bulles dans les visionneuses.

  Par exemple, si votre entreprise est une société multinationale qui vend dans différents pays, chaque pays peut avoir sa propre visionneuse correspondant aux paramètres régionaux. Pour accomplir cette fonctionnalité, vous spécifiez une chaîne de carte de paramètres régionaux. Vous modifiez ensuite le texte de l’info-bulle dans le paramètre prédéfini d’une visionneuse. Ajoutez simplement les chaînes de texte traduites pour la langue souhaitée.

  >[!NOTE]
  > Pour configurer les options de prise en charge de la localisation, [utilisez Admin Console pour créer un dossier de support.](https://helpx.adobe.com/fr/enterprise/using/support-for-experience-cloud.html) Dans votre dossier de support, demandez de l&#39;aide pour la configuration.

  Pour plus d’informations sur la configuration de l’**[!UICONTROL Aide à la localisation]**, voir [Considérations à prendre en compte lors de la configuration de la localisation des fichiers](publish-setup.md#considerations_when_setting_up_localization_of_assets).

### Considérations à prendre en compte lors de la configuration de la localisation des fichiers {#considerations-when-setting-up-localization-of-assets}

>[!NOTE]
>
>Si vous souhaitez configurer des options de prise en charge de la localisation dans Adobe Dynamic Media Classic, telles que le champ Carte des paramètres régionaux, [utilisez Admin Console pour créer un dossier de prise en charge.](https://helpx.adobe.com/fr/enterprise/using/support-for-experience-cloud.html) Dans votre dossier de support, demandez de l&#39;aide pour la configuration.

Une façon courante d’utiliser Adobe Dynamic Media Classic est de gérer les images du produit sur les sites Web e-Commerce. Les sociétés internationales doivent gérer le fait que l’aspect des fichiers pour des produits similaires diffère d’un pays à l’autre. Généralement, les différences concernent quelques parties du média global. Remédier à ces différences en copiant tous les éléments d’actif pour chacun des pays et en ne remplaçant que les différences est un effort énorme qui contredit la métaphore du bien primaire unique. De telles différences de fichiers peuvent impliquer, en raison des vidéos spécifiques aux pays avec différentes pistes audio, des différences importantes bien que très subtiles des câbles d’alimentation utilisés avec le produit. Adobe Dynamic Media Classic utilise un mécanisme de recherche de base. Vous définissez l’ordre des suffixes des fichiers analysés par le serveur d’images, en commençant par les paramètres régionaux requis.

#### Localisation des ressources

Les paramètres régionaux pour une demande de diffusion d’image IS (Image Serving) est identifié avec la commande de rendu d’image IS/IR (Image Rendering) suivante :

`locale=`

Cette commande accepte une chaîne d’ID de paramètre régional (locId) qui n’est pas sensible à la casse. L’identifiant du paramètre régional est généralement une chaîne de 2 à 6 caractères composée de lettres et de « `_` ».

IS prend en charge les chaînes ASCII imprimables arbitraires. La commande `locale=` a une portée globale, ce qui signifie qu’elle est appliquée à l’ensemble de la requête, y compris toutes les requêtes IMBRIQUÉES d’ID et d’IR, les modèles référencés et les calques d’image. Plusieurs paramètres régionaux par demande (par exemple un paramètre régional différent pour chaque calque) ne sont pas pris en charge. Toutefois, il est possible d’autoriser les remplacements explicites dans les demandes imbriquées.

Si `locale=` n’est pas spécifié, `attribute::DefaultLocale` est transmis aux moteurs de traduction. La validation d’entrée limitée est appliquée à la valeur `locale=`. Des valeurs de `locale=` vides sont autorisées. Étant donné que `locale=` a une portée globale, `attribute::DefaultLocale` est fourni par le catalogue principal pour l’ensemble de la requête.

Voici quelques-uns des avantages de l’utilisation de `locale=` et `attribute::DefaultLocale` :

* Partage du contenu pour plusieurs paramètres régionaux.
* Accès à un contenu spécifique à un paramètre régional à l’aide des ID génériques.
* Flexibilité par rapport aux conventions d’affection de nom et à la gestion du contenu spécifique à un paramètre régional, par exemple préfixe/suffixe des paramètres régionaux ou contenu spécifique à un paramètre régional dans un catalogue distinct.
* Prise en charge de l’accès aux versions spécifiques aux paramètres régionaux.
* Les objets d’agrégat, tels que les visionneuses d’images, peuvent parfois contenir des références génériques à des contenus potentiellement spécifiques aux paramètres régionaux.
* Prend en charge tous les contenus gérés par des catalogues qui doivent être localisés, notamment les images, les visionneuses d’images, les vignettes, les documents et les enregistrements de configuration de visionneuse.
* Réduction des modifications de la base de données IPS et des mécanismes de manifeste IS.
* La prise en charge de contenus statiques tels que des vidéos et des habillages est ajoutée lorsque la norme RFC IS-63 est implémentée.
* Les paramètres régionaux par défaut sont configurables.

#### Scénarios d’application

| Application | Scénario |
| --- | --- |
| Localisation de la visionneuse | Une fois les catalogues de contenu statiques implémentés, la localisation est entièrement contrôlée par le paramètre locale= , ajouté à toutes les requêtes envoyées à IS. Il peut exister des variantes spécifiques aux paramètres régionaux pour les enregistrements de configuration, habillages, écrans de démarrage, etc. Le contenu approprié est fourni par IS sans que la visionneuse doive savoir quel contenu est localisé et quels sont ses ID. |
| Images et vidéo | Les entreprises multinationales ont généralement recours à un contenu à la fois générique et spécifique à un paramètre régional. Grâce à ce mécanisme, une référence à une image ou à une vidéo peut être générique, tandis qu’IS diffuse le contenu spécifique à un paramètre régional, s’il existe. |
| Visionneuses d’images et de médias | La visionneuse d’images entière peut être différente pour certains paramètres régionaux, par exemple lorsqu’un catalogue électronique est différent, avec la traduction d’une visionneuse d’images générique en une visionneuse d’images spécifique aux paramètres régionaux gérée par la visionneuse. Plus fréquemment, les identifiants individuels d’un jeu générique peuvent faire référence à un contenu localisé. Par exemple, la plupart des photos d&#39;un appareil peuvent être les mêmes dans toutes les langues, à l&#39;exception de la photo du Panneau de Contrôle. Les identifiants sont automatiquement traduits dans par le service d’identités, de sorte qu’il n’est pas nécessaire de générer des visionneuses d’images spécifiques aux paramètres régionaux. |

#### Implémenter la localisation des ressources

Adobe Dynamic Media Classic et la diffusion d’images ont une interface qui permet la localisation des images et du contenu statique.

Sans localisation, une URL de serveur d’images ressemble à ce qui suit :

`https://server/is/image/company/image`

Avec la localisation, une URL de serveur d’images ajoute le paramètre `locale=` au chemin d’accès, comme dans ce qui suit :

`https://server/is/image/company/image?locale=de_DE`

À la réception de l’appel http par le serveur d’images, le paramètre `locale=` est analysé dans le champ `localeMap` figurant dans le groupe **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Configuration de la publication]** > **[!UICONTROL Serveur d’images]** > **[!UICONTROL Prise en charge de la localisation]**.

Le champ de carte de paramètres régionaux contient une liste des entrées séparées à l’aide du symbole de barre verticale (|).

Chaque entrée se compose d’une liste de valeurs séparées par des virgules. La première valeur est la valeur de recherche transmise par le biais du paramètre `locale=`. Les valeurs restantes sont des valeurs de suffixe/remplacement qui sont ensuite essayées jusqu’à ce que l’une d’elles génère une image existante.

L’application d’une valeur de suffixe ou de remplacement dépend du paramètre régional Monde entier dans le groupe **[!UICONTROL Configuration]** >**[!UICONTROL Configuration de l’application]** > **[!UICONTROL Configuration de la publication]** > **[!UICONTROL Serveur d’images]** > **[!UICONTROL Aide à la localisation]**.

>[!NOTE]
>
>Le paramètre régional global n’est possible que lorsque vous le définissez via l’API, et non dans l’interface d’Adobe Dynamic Media Classic.

**Exemple de suffixe :**

| URL | ID de localeMap | Résultat | Remarques |
| --- | --- | --- | --- |
| `https://server/is/image/company/image?locale=de_DE` | `de_DE,_DE,` | `fr_FR,_FR,` | Aucun paramètre GlobalLocale n’est défini. Le paramètre régional de_DE est mis en correspondance avec la première entrée de la `localeMap`. La première valeur _DE correspondante est ajoutée comme suffixe à la ressource image_DE et une tentative est effectuée pour la trouver sur le serveur d’images. S’il se trouve sur le serveur, il est renvoyé. Dans le cas contraire, la deuxième valeur « » est utilisée comme suffixe, ce qui entraîne le renvoi de l’image elle-même. |

**Exemple de remplacement :**

| URL | `GlobalLocale` et ID de `localeMap` | Résultat | Remarques |
| --- | --- | --- | --- |
| `https://server/is/image/company/image-main-01?locale=de_DE` | `GlobalLocale=mainlocaleMap -` <br><br/> `de_DE,de,main` | `fr_FR,fr,main` | Dans l’exemple de remplacement ci-dessus, GlobalLocale est défini sur principal. Le paramètre régional de_DE est mis en correspondance avec la première entrée de la `localeMap`. La sous-chaîne GlobalLocale a été trouvée et remplacée par la première valeur correspondante `de` dans le `localeMap` : `image-de-01`. S’il se trouve sur le serveur d’images, il est renvoyé. Si ce n’est pas le cas, la deuxième valeur est remplacée, ce qui entraîne une `image-main-01`. |

Si aucun paramètre régional n’est défini dans l’URL, le serveur d’images prend l’attribut DefaultLocale, s’il est défini, et l’applique à l’URL.

Si un paramètre régional inconnu ou vide est fourni avec `locale=`, la `localeMap` est analysée pour rechercher la valeur vide « commençant par ». Il est important d’appliquer un paramètre régional par défaut pour les paramètres régionaux inconnus.

#### À propos de defaultImage

Le serveur d’images essaie l’une après l’autre les options pour les paramètres régionaux demandés. Si aucune correspondance n’est trouvée, les options des paramètres régionaux sont appliquées à defaultImage et la version correspondante est renvoyée. Par conséquent, chaque paramètre régional doit inclure une option pour l’image sans localisation, ou des versions d’image par défaut localisées sont disponibles dans Adobe Dynamic Media Classic.

#### Scénarios de recherche de localeMap

Supposons que vous deviez prendre en charge les paramètres régionaux suivants :

`en, en_us, en_uk, de, de_at, de_de, fr`

Vous mappez ces paramètres régionaux aux suffixes `_E` (anglais), `_G` (allemand) et `_F` (français). Pour tous les exemples, l’ID d’image d’entrée générique est `myImg`.

##### Comportement standard pour la recherche de localeMap

Les ID de paramètres régionaux sont associés à leurs suffixes correspondants. Si aucun ID spécifique aux paramètres régionaux n’est trouvé dans le catalogue, l’ID générique est testée. Notez les valeurs locSuffix vides qui correspondent à l’ID générique.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,`

| locale= | ID de sortie à rechercher |
| --- | --- |
| en, en_us, en_uk | myImg_E, myImg |
| de, de_de, de_at | myImg_D, myImg |
| fr | myImg_F, myImg |
| Tous les autres | : |

##### Recherche de localeMap lorsque le paramètre régional est inconnu

Vous pouvez associer les paramètres régionaux inconnus aux ID spécifiques ou génériques. Par exemple, vous pouvez mapper des paramètres régionaux inconnus aux ID anglais ou, s’ils n’existent pas, aux ID génériques.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,_E,`

| locale= | ID de sortie à rechercher |
| --- | --- |
| de, de_de, de_at | myImg_D, myImg |
| fr | myImg_F, myImg |
| Tous les autres | myImg_E, myImg |

Vous pouvez également avoir un locSuffix dédié, tel que U, uniquement pour les paramètres régionaux inconnus, et forcer l’image par défaut s’il n’existe aucun `_U`, comme dans ce qui suit :

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,U`

Ou vous pouvez établir la correspondance directement avec l’ID générique, comme dans l’exemple suivant :

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,`

##### Recherche de localeMap à l’aide d’une recherche à plusieurs niveaux

Il est généralement recommandé de regrouper les paramètres régionaux (européens, Moyen-Orient et nord-américains, par exemple) pour se conformer aux normes régionales, telles que l’exposition des habillages. Vous pouvez obtenir cet effet en utilisant une recherche à plusieurs niveaux.

Supposons, par exemple, que vous souhaitiez prendre en charge les collections destinées à une utilisation en Occident et au Moyen-Orient. Les deux collections reposent sur la collection d’images génériques, et ajoutent ou modifient toutes deux certaines images. Les deux collections sont ensuite affinées pour des paramètres régionaux spécifiques. Par exemple, `m1, m2` pour deux variantes du Moyen-Orient, et `w1, w2,` et `w3` pour trois paramètres régionaux occidentaux, sauf que les images sont partagées pour `w1` et `w3`. Les paramètres régionaux inconnus sont mappés uniquement à la collection générique et n’ont pas accès aux images spécifiques à un paramètre régional. Voici à quoi doit ressembler le mappage :

`attribute::LocaleMap=w1,-W,|w2,-W2,-W,|w3,-W,|m1,-M1,-M,|m2,-M2,-M,|,`

| locale= | ID de sortie à rechercher |
| --- | --- |
| w1, w3 | myImg-W, myImg |
| w2 | myImg-W2, myImg-W, myImg |
| m1 | myImg-M1, myImg-M |
| m2 | myImg-M2, myImg-M, myImg |
| Tous les autres | mylmg |

##### Recherche de localeMap en recherchant des identifiants spécifiques

Certaines conventions de dénomination des images ne prennent pas en charge les identifiants d’image génériques. Les ID génériques issus de la demande doivent être mappés à l’ID spécifié dans le catalogue. Cependant, il existe des cas où l’identifiant spécifique exact n’est pas connu.

En prenant comme base le premier exemple, les suffixes des images pour toutes les langues peuvent être `_1`, `_2` ou `_3`. Les suffixes des images spécifiques aux paramètres régionaux français peuvent être `_22` ou `_23`. De plus, les suffixes des images spécifiques aux paramètres régionaux allemands peuvent être `_470` ou `_480`.

`attribute::LocaleMap=,_1,_2,_3|fr,_22,_23,_1,_2,_3|de,_470,_480,_1,_2,_3|de_at,_470,_480,_1,_2,_3|de_de,_470,_480,_1,_2,_3`

| locale= | ID de sortie à rechercher |
| --- | --- |
| fr | myImg_22, myImg_23, myImg_1, myImg_2, myImg_3 |
| de, de_at, de_de | myImg_470, myImg_480, myImg_1, myImg_2,myImg_3 |
| Tous les autres | myImg_1, myImg_2, myImg_3 |

##### Points importants à prendre en compte lors de la mise en œuvre de la localisation

* La localisation se limite aux appels de fichier basés sur l’ID et ne peut pas être utilisée pour les appels de fichier basés sur le chemin d’accès. Par conséquent, lors de l’appel de vidéos avec des paramètres régionaux, celles-ci doivent être appelées en tant que company/assetID et non comme chemin d’accès complet à la vidéo. Vous ne pouvez pas utiliser `RTMP` avec la localisation, car cette méthode est réservée aux appels vidéo basés sur les chemins d’accès.
* Vous ne pouvez pas utiliser une visionneuse de supports variés contenant une seule vidéo lorsque localeMap est actif ; sinon, l’appel au contenu de la visionneuse échoue. Pour contourner ce problème, vous pouvez ajouter une seule vidéo à une visionneuse de vidéos adaptative. Ensuite, ajoutez la visionneuse de vidéos adaptative à une visionneuse de supports variés.
* Certaines demandes ne sont pas localisées, comme par exemple les demandes de contenu d’une visionneuse de vidéos adaptative. Par conséquent, si vous envisagez d’utiliser des visionneuses de vidéos adaptatives avec la localisation, placez-la dans une visionneuse de médias mixtes. Ensuite, appelez la visionneuse dans une visionneuse de médias mixtes avec le paramètre `locale=` .

## Image Renderer {#image-renderer}

La page Moteur de rendu d’image établit les paramètres par défaut pour la diffusion des visionneuses d’images à partir des serveurs de rendu d’image. Les paramètres sont disponibles dans ces cinq catégories (pour obtenir une description détaillée des paramètres, reportez-vous à la page Serveur d’images elle-même) :

* **[!UICONTROL Gestion des catalogues]** : ces paramètres déterminent la manière dont Adobe Dynamic Media Classic et le fichier catalogue interagissent. Les appels d’URL du serveur de rendu Adobe Dynamic Media Classic sont effectués vers le catalogue, qui à son tour appelle pour diffuser des images à partir du serveur. Modifiez ces paramètres uniquement avec l’aide d’une personne d’assistance Adobe Dynamic Media Classic.

* **[!UICONTROL Attributs de session]** : ces paramètres établissent les paramètres d’erreur, l’URL des URL d’images relatives et si le chevauchement d’objets est autorisé.

* **[!UICONTROL Attributs de matériau par défaut]** : ces paramètres définissent les paramètres de résolution et d’accentuation par défaut des images.

* **[!UICONTROL Attributs d’image de réponse]** : ces paramètres concernent l’aspect par défaut des images.

* **[!UICONTROL Attributs de gestion des couleurs]** : ces paramètres concernent les paramètres de couleur par défaut des images.

## Vignette {#vignette}

La page Vignette propose des paramètres permettant de définir l&#39;apparence par défaut des vignettes (voir la page elle-même pour une description détaillée des options).
