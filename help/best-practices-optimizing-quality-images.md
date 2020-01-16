---
title: Recommandations pour optimiser la qualité des images
seo-title: Recommandations pour optimiser la qualité des images
description: 'null'
seo-description: Découvrez les meilleures pratiques pour optimiser la qualité de vos images.
uuid: 102e83fe-ee2a-443b-ba92-6ad5cc3daef0
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 8164466e-2520-482a-88ec-6191fdc77ea3
translation-type: tm+mt
source-git-commit: 6b0833287291f6475ab15106e8f33ed0dda0b2d4

---


# Recommandations pour optimiser la qualité des images{#best-practices-for-optimizing-the-quality-of-your-images}

L’optimisation de la qualité des images peut prendre un certain temps, car de nombreux facteurs entrent en jeu pour obtenir des résultats de rendu acceptables. Les résultats sont partiellement subjectifs car chaque individu perçoit différemment la qualité des images. La clé réside dans une mise en application structurée.

Dynamic Media Classic comprend plus de 100 commandes de traitement d’images pour le réglage et l’optimisation des images et des résultats de rendu. Les conseils suivants vous aideront à simplifier le processus et à obtenir rapidement de bons résultats en utilisant quelques commandes essentielles et en appliquant les pratiques recommandées.

Voir aussi [Imagerie](https://helpx.adobe.com/experience-manager/6-3/assets/using/imaging-faq.html)dynamique.

## Recommandations relatives au format d’image (&amp;fmt=) {#best-practices-for-image-format-fmt}

* Les formats JPG et PNG sont les mieux adaptés pour obtenir des images de bonne qualité, d’une taille et d’un volume gérables.
* Si aucune commande de format n’est fournie dans l’URL, la diffusion au format JPG par défaut est effectuée.
* Le format JPG compresse les images à un taux de 10:1 et produit généralement des images plus petites. Le format PNG compresse les images à un taux d’environ 2:1, sauf dans certains cas, notamment quand les images comportent un arrière-plan blanc. En général, toutefois, les fichiers PNG sont plus gros que les fichiers JPG.
* JPG utilise une compression avec perte, ce qui signifie que des éléments d’image (pixels) sont perdus lors de la compression. Le format PNG, en revanche, utilise une compression sans perte.
* Généralement, le format JPG compresse les images photographiques avec une plus grande fidélité que les images de synthèse avec des bords nets et un fort contraste.
* Si vos images contiennent de la transparence, utilisez le format PNG car JPG ne prend pas en charge la transparence.

Pour le format des images, il est recommandé de commencer par le paramètre le plus courant, à savoir `&fmt=JPG`.

## Recommandations relatives à la taille des images {#best-practices-for-image-size}

La réduction dynamique de la taille de l’image est l’une des tâches les plus courantes exécutées par le service d’image Contenu multimédia dynamique. Cela implique de définir la taille et, éventuellement, le mode de sous-échantillonnage à utiliser.

* Pour le dimensionnement des images, la meilleure approche et la plus simple consiste à utiliser `&wid=<value>` et `&hei=<value>` ou simplement `&hei=<value>`. Ces paramètres définissent automatiquement la largeur de l’image par rapport à ses proportions.
* `&resMode=<value>` contrôle l’algorithme utilisé pour le sous-échantillonnage. Commencez par `&resMode=sharp2`. Cette valeur fournit la meilleure qualité d’image. While using the downsampling value `=bilin` is faster, it often results in the aliasing of artifacts.

Il est recommandé d’utiliser `&wid=<value>&hei=<value>&resMode=sharp2` ou `&hei=<value>&resMode=sharp2`

## Recommandations relatives à l’accentuation des images {#best-practices-for-image-sharpening}

L’accentuation des images est l’aspect le plus complexe de contrôle des images sur votre site Web, et aussi source de nombreuses erreurs. Prenez le temps d’en savoir plus sur le fonctionnement de l’accentuation et du masquage flou dans Dynamic Media Classic en vous reportant aux ressources utiles suivantes :

Best practices white paper [Sharpening images in Adobe Scene7 Publishing System and on Image Server](/help/assets/s7_sharpening_images.pdf).

Voir aussi [Accentuation d’une image avec un masque](https://helpx.adobe.com/photoshop/atv/cs6-tutorials/sharpening-an-image-with-unsharp-mask.html)flou.

Avec Dynamic Media Classic, vous pouvez accentuer les images lors de l’assimilation, de la diffusion ou des deux. Dans la plupart des cas, cependant, il est préférable d’accentuer les images en utilisant uniquement l’une des deux méthodes, mais pas les deux. L’accentuation des images à la distribution, dans une URL, produit généralement de meilleurs résultats.

Il existe deux méthodes d’accentuation des images que vous pouvez utiliser :

* Simple sharpening ( `&op_sharpen`) - Similar to the sharpen filter used in Photoshop, simple sharpening applies basic sharpening to the final view of the image following dynamic resizing. Toutefois, cette méthode n’est pas configurable par l’utilisateur. The best practice is to not use `&op_sharpen` unless required.
* Unsharp masking ( `&op_USM`) - Unsharp masking is an industry standard sharpening filter. Il est recommandé d’accentuer les images avec le masquage flou en suivant les conseils ci-dessous. Le masquage flou permet de contrôler les trois paramètres suivants :

   * `&op_sharpen=amount,radius,threshold`

      * `amount` (0-5, force de l’effet.)
      * `radius` (0-250, largeur des &quot;lignes d’accentuation&quot; tracées autour de l’objet accentué, mesurée en pixels.)

         Keep in mind that the parameters `radius` and `amount` work against each other. La réduction `radius` peut être compensée par une augmentation `amount`. `Radius` permet un contrôle plus précis car une valeur plus faible n’accentue que les pixels de contour, tandis qu’une valeur plus élevée accentue une bande de pixels plus large.

      * `threshold` (0-255, sensibilité de l&#39;effet.)

         Ce paramètre définit l’écart recherché entre les pixels accentués et la zone environnante avant qu’ils ne soient considérés comme des pixels de contour et ne soient accentués par le filtre. Le seuil permet d’éviter de trop accentuer les zones avec des couleurs similaires, comme des tons chair. Par exemple, une valeur de seuil de 12 ignore les légères variations de luminosité de la peau, afin de ne pas ajouter de bruit, tout en ajoutant un contraste sur les bords dans les zones contrastées, comme la zone où les cils rencontrent la peau.
      Pour plus d’informations sur la façon de définir ces trois paramètres, y compris les pratiques recommandées à appliquer avec le filtre, reportez-vous aux ressources suivantes :

      Rubrique d’aide de Dynamic Media Classic sur l’ [accentuation d’une image](https://help.adobe.com/en_US/scene7/using/WS389B162D-2981-41e5-9253-15D22D2ECBC8.html).

      Best practices white paper [Sharpening images in Adobe Scene7 Publishing System and on Image Server](/help/assets/s7_sharpening_images.pdf).

   * Dynamic Media Classic vous permet également de contrôler un quatrième paramètre : monochrome ( `0,1`). Ce paramètre détermine si le masquage flou est appliqué séparément à chaque composante de couleur en utilisant la valeur `0` ou à la luminosité/intensité de l’image en utilisant la valeur `1`.


En règle générale, il est recommandé de commencer par le paramètre de rayon du masquage flou. Voici les paramètres de rayon que vous pouvez utiliser en premier :

* Site Web : 0,2-0,3 pixel
* Impression photographique (250-300 ppp) : 0,3-0,5 pixel
* Impression offset (266-300 ppp) : 0,7-1,0 pixel
* Impression sur toile (150 ppp) : 1,5-2,0 pixels

Augmentez graduellement la valeur entre 1,75 et 4. Si l’accentuation ne correspond toujours pas à vos attentes, augmentez le rayon d’un point décimal et réaugmentez la quantité entre 1,75 et 4. Répétez l’opération si nécessaire.

Laissez le paramètre monochrome sur 0.

## Recommandations relatives à la compression JPEG (&amp;qlt=) {#best-practices-for-jpeg-compression-qlt}

* Ce paramètre contrôle la qualité du codage JPG. Une valeur élevée produit une image de meilleure qualité mais un fichier plus gros ; en revanche, une valeur faible désigne une image de qualité inférieure mais un fichier plus petit. Ce paramètre est compris entre 0 et 100.
* Pour optimiser la qualité, ne définissez pas ce paramètre sur 100. La différence entre un paramètre de 90, 95 ou 100 est presque imperceptible, mais 100 augmente inutilement la taille du fichier image. Therefore, to optimize for quality but avoid image files becoming too large, set the `qlt=` value to 90 or 95.
* To optimize for a small image file size but keep image quality at an acceptable level, set the `qlt=` value to 80. Les valeurs inférieures à 70-75 se traduisent par une dégradation notable de la qualité d’image.
* As a best practice, to stay in the middle, set the `qlt=` value to 85 to stay in the middle.
* Utilisation de l’indicateur de chrominance dans `qlt=`

   * The `qlt=` parameter has a second setting that lets you turn on RGB chromaticity downsampling using the normal value `,0` (default), or turn it off using the value `,1`.
   * Pour rester simple, commencez par désactiver la réduction de résolution chromatique RVB ( `,1`). Ce paramètre produit généralement une image de meilleure qualité, en particulier pour les images de synthèse contenant beaucoup de contours nets et un fort contraste.

Pour la compression JPG, il est recommandé d’utiliser `&qlt=85,0`.

## Recommandations relatives au dimensionnement JPEG (&amp;jpegSize=) {#best-practices-for-jpeg-sizing-jpegsize}

`jpegSize` est un paramètre utile si vous souhaitez garantir qu’une image ne dépasse pas une certaine taille pour la distribution sur les périphériques ayant une mémoire limitée.

* Ce paramètre est défini en kilo-octets ( `jpegSize=<size_in_kilobytes>`). Il définit la taille maximale autorisée pour la distribution des images.
* `&jpegSize=` interagit avec le paramètre de compression JPG `&qlt=`. If the JPG response with the specified JPG compression parameter ( `&qlt=`) does not exceed the `jpegSize` value, the image is returned with `&qlt=` as defined. Otherwise, `&qlt=` is gradually decreased until the image fits in the maximum allowed size, or until the system determines it cannot fit and returns an error.

As a best practice, set `&jpegSize=` and add the parameter `&qlt=` if you are delivering JPG images to devices with limited memory.

## Résumé des recommandations {#best-practices-summary}

En règle générale, pour obtenir une image de qualité élevée mais un fichier de petite taille, commencez par la combinaison de paramètres suivante :

`fmt=jpg&qlt=85,0&resMode=sharp2&op_usm=1.75,0.3,2,0`

Cette combinaison de paramètres produit d’excellents résultats dans la plupart des cas.

Si l’image doit être davantage optimisée, accentuez-la progressivement (masquage flou) en commençant par un rayon de 0,2 ou 0,3. Ensuite, augmentez graduellement la quantité entre 1,75 et 4 (équivalent de 400 % dans Photoshop). Vérifiez que le résultat escompté est obtenu.

Si les résultats de l’accentuation ne sont toujours pas satisfaisants, augmentez le rayon point décimal par point décimal. Pour chaque incrément décimal, redémarrez la quantité à 1,75 et augmentez-le progressivement jusqu’à 4. Répétez cette procédure jusqu’à ce que vous obteniez le résultat escompté. Les valeurs ci-dessus sont une approche validée par les studios de création ; cela ne vous empêche toutefois pas de commencer par d’autres valeurs et d’appliquer d’autres stratégies. Que vous soyez ou non satisfait par les résultats est subjectif. Par conséquent, la clé réside dans une mise en application structurée.

Tandis que vous testez différentes valeurs, vous trouverez peut-être également les suggestions générales suivantes utiles pour optimiser votre processus :

* Testez différents paramètres en temps réel, soit directement sur une URL de type Contenu multimédia dynamique, soit à l’aide de la fonctionnalité de réglage d’image de Scene7 Publishing System, qui fournit des aperçus en temps réel pour les opérations de réglage.
* En règle générale, n’oubliez pas que vous pouvez regrouper les commandes de diffusion d’images de médias dynamiques dans un paramètre d’image prédéfini. An image preset is basically URL command macros with custom preset names such as `$thumb_low$` and `&product_high$`. Le nom du paramètre prédéfini personnalisé dans un chemin d’URL invoque ces paramètres prédéfinis. Cette fonctionnalité permet de gérer les commandes et les paramètres de qualité de différents gabarits d’utilisation des images sur votre site Web et réduit en outre la longueur totale des URL.
* Dynamic Media Classic propose également des méthodes plus avancées d’optimisation de la qualité d’image, comme l’application d’images d’accentuation lors de l’assimilation. Pour les cas d’utilisation plus complexes où il peut s’avérer nécessaire d’affiner et d’optimiser les résultats de rendu, n’hésitez pas à faire appel à Adobe Professional Services.

