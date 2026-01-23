---
title: Recommandations pour optimiser la qualité des images
description: Découvrez les bonnes pratiques pour optimiser la qualité de vos images.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 3c50e706-b9ed-49db-8c08-f179de52b9cf
topic: Content Management
level: Intermediate
source-git-commit: c4613c78347c4bda3d84747a72146617158c03b6
workflow-type: tm+mt
source-wordcount: '1604'
ht-degree: 39%

---

# Recommandations pour optimiser la qualité des images{#best-practices-for-optimizing-the-quality-of-your-images}

L’optimisation de la qualité d’image peut prendre beaucoup de temps. De nombreux facteurs contribuent à rendre les résultats acceptables. Les résultats sont partiellement subjectifs car chaque individu perçoit différemment la qualité des images. La clé réside dans une mise en application structurée.

Adobe Dynamic Media Classic comprend plus de 100 commandes de traitement d’images pour affiner et optimiser les images et les rendus. Les conseils suivants vous aideront à simplifier le processus et à obtenir rapidement de bons résultats en utilisant quelques commandes essentielles et en appliquant les pratiques recommandées.

Voir aussi [Imagerie dynamique](https://experienceleague.adobe.com/fr/docs/experience-manager-65/content/assets/dynamic/imaging-faq).

>[!TIP]
>
>Testez et découvrez les avantages des modificateurs d’image Dynamic Media et de l’imagerie dynamique à l’aide de Dynamic Media [_Snapshot_](https://snapshot.scene7.com/).
>
> Snapshot est un outil de démonstration visuel, conçu pour illustrer la puissance de Dynamic Media pour une diffusion d’images optimisée et dynamique. Testez des images de test ou des URL Dynamic Media afin d’observer visuellement la sortie de divers modificateurs d’images Dynamic Media et d’optimiser l’imagerie dynamique pour les éléments suivants :
>
>* Taille de fichier (avec diffusion WebP et AVIF)
>* Bande passante réseau
>* DPR (rapport pixel d’appareil)
>
>Pour découvrir à quel point il est facile d’utiliser Snapshot, regardez la [vidéo de formation Snapshot](https://experienceleague.adobe.com/fr/docs/experience-manager-learn/assets/dynamic-media/images/dynamic-media-snapshot) (3 minutes et 17 secondes).


## Recommandations relatives au format d’image (&amp;fmt=) {#best-practices-for-image-format-fmt}

* Les formats JPG et PNG sont les mieux adaptés pour obtenir des images de bonne qualité, d’une taille et d’un volume gérables.
* Si aucune commande de format n’est fournie dans l’URL, la Diffusion d’images Dynamic Media utilise par défaut JPG pour la diffusion.
* JPG compresse à un rapport de 10 :1 et produit généralement des tailles de fichier image plus petites. Le format PNG compresse à un rapport d’environ 2 :1, sauf parfois lorsque les images contiennent un arrière-plan vide. En général, toutefois, les fichiers PNG sont plus gros que les fichiers JPG.
* JPG utilise une compression avec perte, ce qui signifie que des éléments d’image (pixels) sont perdus lors de la compression. Le format PNG, en revanche, utilise une compression sans perte.
* Généralement, le format JPG compresse les images photographiques avec une plus grande fidélité que les images de synthèse avec des bords nets et un fort contraste.
* Si vos images contiennent de la transparence, utilisez le format PNG car JPG ne prend pas en charge la transparence.

Il est recommandé de commencer par les `&fmt=JPG` de paramètres les plus courants pour le format d’image.

## Recommandations relatives à la taille des images {#best-practices-for-image-size}

La réduction dynamique de la taille de l’image est l’une des tâches les plus courantes effectuées par le service d’images Dynamic Media. Cela implique de définir la taille et, éventuellement, le mode de sous-échantillonnage à utiliser.

* Pour le dimensionnement des images, l’approche la plus simple et la plus adaptée consiste à utiliser `&wid=<value>` et `&hei=<value>` ou simplement `&hei=<value>`. Ces paramètres définissent automatiquement la largeur de l’image par rapport à ses proportions.
* `&resMode=<value>` contrôle l’algorithme utilisé pour le sous-échantillonnage. Commencez par `&resMode=sharp2`. Cette valeur fournit la meilleure qualité d’image. Bien que l’utilisation de la valeur de sous-échantillonnage `=bilin` soit plus rapide, elle entraîne souvent le crénelage d’artefacts.

Il est recommandé d’utiliser `&wid=<value>&hei=<value>&resMode=sharp2` ou `&hei=<value>&resMode=sharp2` pour le dimensionnement des images

## Recommandations relatives à l’accentuation des images {#best-practices-for-image-sharpening}

L’accentuation des images est l’aspect le plus complexe de contrôle des images sur votre site Web, et aussi source de nombreuses erreurs. Prenez le temps d’en savoir plus sur le fonctionnement de l’accentuation et du masquage flou dans Adobe Dynamic Media Classic en vous référant aux ressources suivantes :

Livre blanc sur les bonnes pratiques dans PDF, intitulé [Accentuation des images dans Adobe Dynamic Media Classic et sur le serveur d’images](/help/using/assets/s7_sharpening_images.pdf).

<!-- Give a 404 See also [Sharpening an image with unsharp mask](https://helpx.adobe.com/photoshop/atv/cs6-tutorials/sharpening-an-image-with-unsharp-mask.html). -->

Avec Adobe Dynamic Media Classic, vous pouvez accentuer les images lors de l’ingestion, lors de la diffusion, ou les deux. En règle générale, cependant, vous accentuez les images en utilisant une seule méthode ou l’autre, mais pas les deux. L’accentuation des images à la distribution, dans une URL, produit généralement de meilleurs résultats.

Vous pouvez utiliser deux méthodes d’accentuation d’image :

* Accentuation simple ( `&op_sharpen`) : comme pour le filtre d’accentuation utilisé dans Photoshop, l’accentuation simple applique un accentuation de base à l’affichage final de l’image à la suite du redimensionnement dynamique. Toutefois, cette méthode n’est pas configurable par l’utilisateur. La bonne pratique consiste à éviter l’utilisation de `&op_sharpen`, sauf si nécessaire.
* Masquage flou ( `&op_USM`) : le masquage flou est un filtre standard du secteur pour l’accentuation. Il est recommandé d’accentuer les images avec le masquage flou en suivant les conseils ci-dessous. Le masquage flou permet de contrôler les trois paramètres suivants :

   * `&op_sharpen=amount,radius,threshold`

      * `amount` (0-5, intensité de l&#39;effet.)
      * `radius` (0-250, largeur des « lignes d’accentuation » dessinées autour de l’objet accentué, mesurée en pixels.)

        Gardez à l’esprit que les paramètres `radius` et `amount` fonctionnent l’un contre l’autre. La réduction des `radius` peut être compensée par une augmentation des `amount`. `Radius` permet un contrôle plus fin, car une valeur faible accentue uniquement les pixels de contour, tandis qu’une valeur élevée accentue une bande plus large de pixels.

      * `threshold` (0-255, sensibilité de l&#39;effet.)

        Ce paramètre définit l’écart recherché entre les pixels accentués et la zone environnante avant qu’ils ne soient considérés comme des pixels de contour et ne soient accentués par le filtre. Le seuil permet d’éviter de trop accentuer les zones avec des couleurs similaires, comme des tons chair. Par exemple, une valeur seuil de 12 ignore les légères variations de luminosité de la peau pour éviter d’ajouter du « bruit », tout en ajoutant un contraste sur les bords dans les zones à fort contraste, comme l’endroit où les cils rencontrent la peau.

        Pour plus d’informations sur la définition de ces trois paramètres, y compris les bonnes pratiques relatives à l’utilisation du filtre, voir [Accentuer les images dans Adobe Dynamic Media Classic et sur le serveur d’images](/help/using/assets/s7_sharpening_images.pdf).

      * Adobe Dynamic Media Classic permet également de contrôler un quatrième paramètre : monochrome ( `0,1`). Ce paramètre détermine si le masquage flou est appliqué séparément à chaque composante de couleur à l’aide de la valeur `0` ou à la luminosité/l’intensité de l’image à l’aide de la valeur `1`.

En règle générale, il est recommandé de commencer par le paramètre de rayon du masquage flou. Voici les paramètres de rayon que vous pouvez utiliser en premier :

* Site Web : 0,2-0,3 pixel
* Impression photographique (250-300 ppp) : 0,3-0,5 pixel
* Impression offset (266-300 ppp) : 0,7-1,0 pixel
* Impression sur toile (150 ppp) : 1,5-2,0 pixels

Augmentez graduellement la valeur entre 1,75 et 4. Si l’accentuation ne correspond toujours pas à vos attentes, augmentez le rayon d’un point décimal et réaugmentez la quantité entre 1,75 et 4. Répétez l’opération si nécessaire.

Laissez le paramètre monochrome sur 0.

## Recommandations relatives à la compression JPEG (`&qlt=`) {#best-practices-for-jpeg-compression-qlt}

* Ce paramètre contrôle la qualité du codage JPG. Une valeur élevée produit une image de meilleure qualité mais un fichier plus gros ; en revanche, une valeur faible désigne une image de qualité inférieure mais un fichier plus petit. Ce paramètre est compris entre 0 et 100.
* Pour optimiser la qualité, ne définissez pas ce paramètre sur 100. La différence entre un réglage de 90 ou 95 et 100 est presque imperceptible. Pourtant, 100 augmente inutilement la taille du fichier image. Par conséquent, pour optimiser la qualité tout en évitant que les fichiers image ne deviennent trop volumineux, définissez la valeur `qlt=` sur 90 ou 95.
* Pour optimiser avec une taille de fichier image réduite, mais en maintenant la qualité d’image à un niveau acceptable, définissez la valeur `qlt=` sur 80. Les valeurs inférieures à 70-75 se traduisent par une dégradation notable de la qualité d’image.
* Il est recommandé, pour rester au milieu, de définir la valeur `qlt=` sur 85 pour rester au milieu.
* Utilisation de l’indicateur chroma dans `qlt=`

   * Le paramètre `qlt=` comporte un second paramètre qui permet d’activer le sous-échantillonnage de résolution chromatique de RGB à l’aide de la `,0` de valeurs normales (par défaut) ou de le désactiver à l’aide de la `,1` de valeurs.
   * Pour garder les choses simples, commencez par désactiver le sous-échantillonnage de résolution chromatique de RGB ( `,1`). Ce paramètre produit généralement une image de meilleure qualité, en particulier pour les images de synthèse contenant beaucoup de contours nets et un fort contraste.

Il est recommandé d’utiliser la `&qlt=85,0` de compression JPG.

## Recommandations relatives au dimensionnement JPEG (&amp;jpegSize=) {#best-practices-for-jpeg-sizing-jpegsize}

Le paramètre `jpegSize` est utile pour garantir qu’une image n’excède pas une certaine taille pour sa diffusion sur les appareils dont la mémoire est limitée.

* Ce paramètre est défini en kilo-octets ( `jpegSize=<size_in_kilobytes>`). Il définit la taille maximale autorisée pour la distribution des images.
* `&jpegSize=` interagit avec le `&qlt=` de paramètres de compression JPG. Si la réponse JPG avec le paramètre de compression JPG spécifié ( `&qlt=`) ne dépasse pas la valeur `jpegSize`, l’image est renvoyée avec le `&qlt=` défini. Sinon, la `&qlt=` est progressivement réduite jusqu’à ce que l’image corresponde à la taille maximale autorisée. Ou, jusqu’à ce que le système détermine qu’il ne peut pas tenir et renvoie une erreur.

Il est recommandé de définir `&jpegSize=` et d’ajouter le paramètre `&qlt=` si vous diffusez des images JPG sur des appareils dont la mémoire est limitée.

## Résumé des recommandations {#best-practices-summary}

En règle générale, pour obtenir une qualité d’image élevée et une petite taille de fichier, commencez par la combinaison de paramètres suivante :

`fmt=jpg&qlt=85,0&resMode=sharp2&op_usm=1.75,0.3,2,0`

Cette combinaison de paramètres produit d’excellents résultats dans la plupart des cas.

Si l’image doit être davantage optimisée, accentuez-la progressivement (masquage flou) en commençant par un rayon de 0,2 ou 0,3. Ensuite, augmentez graduellement la quantité entre 1,75 et 4 (équivalent de 400 % dans Photoshop). Vérifiez que le résultat escompté est obtenu.

Si les résultats de l’accentuation ne sont toujours pas satisfaisants, augmentez le rayon point décimal par point décimal. Pour chaque incrément décimal, redémarrez la quantité à 1,75 et augmentez-le progressivement jusqu’à 4. Répétez cette procédure jusqu’à ce que vous obteniez le résultat escompté. Les valeurs ci-dessus sont une approche validée par les studios de création ; cela ne vous empêche toutefois pas de commencer par d’autres valeurs et d’appliquer d’autres stratégies. Que vous soyez ou non satisfait par les résultats est subjectif. Par conséquent, la clé réside dans une mise en application structurée.

Au fur et à mesure que vous testez votre résultat, les suggestions générales suivantes sont utiles pour optimiser votre workflow :

* Testez et testez différents paramètres en temps réel, directement sur une URL ou à l’aide de la fonctionnalité de réglage d’image d’Adobe Dynamic Media Classic. Ce dernier fournit des aperçus en temps réel pour les opérations de réglage.
* N’oubliez pas que vous pouvez regrouper les commandes de diffusion d’images Dynamic Media dans un paramètre d’image prédéfini. Un paramètre prédéfini d’image correspond essentiellement aux macros de commande d’URL avec des noms de paramètres prédéfinis personnalisés, tels que `$thumb_low$` et `&product_high$`. Le nom du paramètre prédéfini personnalisé dans un chemin d’URL appelle ces paramètres prédéfinis. Cette fonctionnalité permet de gérer les commandes et les paramètres de qualité de différents gabarits d’utilisation des images sur votre site Web et réduit en outre la longueur totale des URL.
* Adobe Dynamic Media Classic propose également des méthodes plus élaborées permettant d’optimiser la qualité des images, par exemple en accentuant les images lors de l’ingestion. Pour les cas d’utilisation plus complexes pour lesquels un réglage et une optimisation plus approfondis des résultats rendus sont possibles, Adobe Professional Services peut vous aider à personnaliser insight et les bonnes pratiques.
