---
title: Accentuer une image
description: Découvrez comment accentuer une image dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 4b3e8368-f8f5-46d9-9130-361a8273de2c
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T20:13:09.120Z'
TQID: 'https://experienceleague.adobe.com/y5rcs4ohA-zMFKKm1EjsSxuUqgqbp-CVMzRcmTaRs6c'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
source-git-commit: b35d2efa3ef74017ef0505658d2f567a45b234f6
workflow-type: tm+mt
source-wordcount: 2283
ht-degree: 25%

---

# Accentuation d’une image {#sharpening-an-image}

L’accentuation est une technique de manipulation d’image qui rend plus nets les contours d’une image numérique. L’accentuation consiste à augmenter le contraste entre les pixels de contour, et ainsi à souligner la transition entre les zones sombres et les zones claires. L’accentuation augmente le contraste local et révèle des détails précis. Il n’existe pas de formule magique pour accentuer correctement toutes les images. Une accentuation trop faible produit une image douce, tandis qu’une accentuation exagérée crée des halos, des artefacts et du bruit.

Adobe Dynamic Media Classic vous recommande vivement d’utiliser les paramètres d’image prédéfinis pour toutes les images. Ils garantissent une taille uniforme et l’accentuation est appliquée à toute image appelée avec un paramètre d’image prédéfini. De plus, vous pouvez facilement modifier les paramètres d’accentuation d’un paramètre d’image prédéfini. A la prochaine publication, toutes les images appelées avec ces paramètres prédéfinis se voient appliquer les nouvelles valeurs.

Adobe Dynamic Media Classic recommande également d’ajouter un accentuation aux paramètres prédéfinis de la visionneuse, puis d’appeler une visionneuse avec ce paramètre prédéfini. Cela permet de s’assurer que les images de vos visionneuses sont nettes et attrayantes.

Cependant, que vous utilisiez des paramètres d’image prédéfinis et des paramètres de visionneuse prédéfinis, ou une autre méthode d’accentuation, il est essentiel d’accentuer vos images. Si ce n’est pas le cas, vos images (et votre site web) peuvent apparaître floues et floues.

>[!NOTE]
>
>les commandes d’accentuation remplacent les paramètres d’image prédéfinis, notamment les effets d’accentuation. Un paramètre d’image prédéfini régit la taille et la mise en forme avec lesquelles les images sont diffusées à partir des serveurs d’images Dynamic Media. Adobe Dynamic Media Classic recommande vivement d’utiliser les paramètres d’image prédéfinis pour diffuser toutes les images. Cela garantit que les images sont diffusées à une taille et un accentuation uniformes. Cependant, après avoir modifié les paramètres d’accentuation d’une image individuelle, les paramètres d’image prédéfinis relatifs à l’accentuation ne s’appliquent plus à l’image. Elle est diffusée sans ces paramètres.

Il est souvent nécessaire d’accentuer les images. Adobe Dynamic Media Classic et les serveurs d’images proposent plusieurs options d’accentuation. Il est important de comprendre l’impact de l’accentuation sur une image et le degré d’accentuation dont vous avez besoin. La plupart des images ont besoin d’accentuation mais le degré nécessaire dépend de l’image.

L’accentuation de l’image augmente le contraste des pixels pour créer un effet de contours renforcés. Les utilisateurs perçoivent ce contraste amélioré comme une netteté. S’il est facile d’améliorer une image à l’aide de filtres d’accentuation, il est également facile de trop renforcer la netteté d’une image,

L’accentuation excessive d’une image crée un effet de halo ou de bande sur les lignes du bord.

Vous pouvez suivre certaines bonnes pratiques pour optimiser l’accentuation de vos images dans Adobe Dynamic Media Classic et sur le serveur d’images Dynamic Media.

Voir [Bonnes pratiques pour l’accentuation des images dans Adobe Dynamic Media Classic et sur le serveur d’images Dynamic Media](/help/using/assets/s7_sharpening_images.pdf).

Consultez également la vidéo de formation [Accentuation](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/547_sharpening1_converted%20renamed_Done-AVS).

**Pour accentuer une image :**

Pour accentuer une image, sélectionnez le bouton d’accentuation **[!UICONTROL Modifier]** et choisissez **[!UICONTROL Accentuer]**, ou ouvrez-la dans l’affichage des détails du panneau Parcourir, puis sélectionnez **[!UICONTROL Accentuer]**. La page Éditeur de netteté s’ouvre avec des commandes d’accentuation. Choisissez les commandes souhaitées, puis cliquez sur **[!UICONTROL Enregistrer]**.

>[!NOTE]
>
>Avant d’accentuer une image, vous pouvez sélectionner le menu Appliquer les paramètres prédéfinis et choisir un paramètre d’image prédéfini pour en découvrir les effets. Les effets d’accentuation d’un paramètre d’image prédéfini conviennent à votre image. Le menu **[!UICONTROL Appliquer le paramètre prédéfini]** se trouve au bas de la page de l’éditeur de netteté.

**Options d’accentuation**

Le tableau suivant présente les options d’accentuation du serveur Image Server.

| Nom | Protocole d’URL | Valeurs | Exemple |
| --- | --- | --- | --- |
| Accentuation simple | `op_sharpen` | `0` ou `1` | `op_sharpen=1` |
| Mode de ré-échantillonnage | `resMode` | `bilin`, `bicub`, `sharp2`, `trilin`<br><br>`bilin` : sélectionne une interpolation bilinéaire standard. Méthode de rééchantillonnage la plus rapide ; certains artefacts d’alias sont souvent perceptibles. <br>`bicub` : sélectionne l’interpolation bi-cubique. Plus gourmand en CPU que `bilin`, mais produit des images plus nettes avec des artefacts d’alias moins visibles.<br><br>`sharp2` : sélectionne une fonction Lanczos Windows® modifiée comme algorithme d’interpolation. Elle peut produire des résultats légèrement plus nets que la bicube pour un coût CPU plus élevé.<br><br>`trilin` : sélectionne une interpolation trilinéaire modifiée, qui utilise des résolutions plus élevées et plus basses, le cas échéant. Méthode recommandée si le crénelage devient problématique. Elle réduit la taille des fichiers JPEG en raison des données à haute fréquence réduites. | `resMode=sharp2` |
| Masquage flou | `op_usm` | `amount`, `radius`, `threshold`, `monochrome`<br><br>`amount` : facteur d’intensité du filtre (réel 0...5)<br><br>`radius` : rayon du noyau du filtre en pixels (réel 0...250) <br><br>`threshold` : niveau de seuil du filtre (entier 0...255)<br><br>`monochrome` : défini sur `0` pour appliquer l’accentuation à chaque composante de couleur séparément, défini sur `1` pour appliquer l’accentuation à la luminosité de l’image (intensité) du masque | `op_usm=1,1,10,0` |

Sélectionnez le menu **[!UICONTROL Accentuation]** et choisissez une option :

* **Aucune** : permet de désactiver l’accentuation.

* **Accentuer** : exécute une simple passe d’accentuation sur le fichier après son redimensionnement. Elle est similaire au filtre « Accentuer » d’Adobe Photoshop et ne prend en charge aucun paramètre utilisateur. Utilisez ce filtre ou **[!UICONTROL Accentuation]**, mais pas les deux. Cette méthode n’est pas recommandée comme meilleure pratique, mais elle permet de compenser le flou. (URL : `op_sharpen`)

* **Accentuation** : permet d’affiner l’effet d’un filtre d’accentuation sur l’image finale sous-échantillonnée. Vous pouvez contrôler l’intensité de l’effet, le rayon de l’effet (mesuré en pixels) et un seuil de contraste qui est ignoré. Cet effet utilise les mêmes options que le filtre Adobe Photoshop « Accentuation ». (URL : `op_usm`)

Choisissez les options suivantes pour affiner l’accentuation avec l’accentuation :

* **Quantité** : contrôle l’intensité du contraste appliqué aux pixels de contour. La valeur par défaut est 0,0. Pour les images à haute résolution, vous pouvez l’augmenter jusqu’à 5.0. Considérez la valeur comme une mesure de l’intensité du filtre. Le paramètre **[!UICONTROL Montant]** dans Adobe Dynamic Media Classic n’est pas identique au paramètre Montant dans Adobe Photoshop. Adobe Photoshop utilise un montant compris entre 1 % et 500 %, tandis qu’Adobe Dynamic Media Classic peut passer de 0,0 à 5,0. (5,0 équivaut environ à 500 % dans Adobe Photoshop, 0,9 est similaire à 90 %, etc.)

* **Rayon** : détermine le nombre de pixels entourant les pixels de contour qui affectent l’accentuation. L’effet s’exécute sur tous les pixels de l’image et rayonne dans toutes les directions.

La valeur appropriée du rayon dépend de la taille de l’image. Une valeur faible n’accentue que les pixels de contour. Une valeur élevée accentue une marge de pixels plus large.

Par exemple, pour obtenir un effet d’accentuation similaire pour une image de 2 000 × 2 000 pixels et une image de 500 × 500 pixels, vous pouvez définir une valeur de rayon de deux pixels sur l’image de 2 000 × 2 000 pixels. Définissez ensuite une valeur de rayon d’un pixel sur l’image de 500 × 500 pixels (une valeur plus grande pour une image avec plus de pixels).

* **Seuil** : utilisez ce paramètre pour ignorer une plage de contraste lorsque le filtre d’accentuation est appliqué. Cette option détermine l’écart recherché entre les pixels accentués et la zone environnante avant l’accentuation des pixels de contour.

Le seuil utilise une valeur comprise entre 0 et 255, qui correspond au nombre d’étapes de luminosité d’une image en niveaux de gris. 0 = noir, 128 = 50 % gris et 255 = blanc. Par exemple, une valeur seuil de 12 ignore les légères variations de la luminosité de la peau. Cela évite l’ajout de bruit, tout en ajoutant un contraste sur les bords dans les zones contrastées, comme la zone où les cils rencontrent la peau.

Par exemple, supposons que vous ayez une photo du visage d&#39;une personne. Le masquage flou accentue les parties de l’image les plus contrastées et la peau lisse. Même la peau la plus lisse affiche des variations subtiles de ses valeurs de luminosité. Si vous n’utilisez pas une valeur de seuil, le filtre accentue ces légères variations dans les pixels de la peau, créant ainsi un effet de bruit (probablement indésirable), tout en augmentant le contraste sur les cils, ce qui améliore la netteté (probablement souhaitable). Pour l’éviter, utilisez une valeur de seuil qui indique au filtre d’ignorer les pixels qui ne modifient pas considérablement le contraste, comme la peau lisse. Pour éviter d’introduire du bruit ou de la postérisation dans les images avec des tons chair, par exemple, essayez d’utiliser les valeurs **[!UICONTROL Seuil]** comprises entre 2 et 20. La valeur par défaut **[!UICONTROL Seuil]** de 0 accentue tous les pixels de l’image.

* **Appliquer à** : sélectionnez **[!UICONTROL Chaque couleur]** si vous souhaitez appliquer l’accentuation séparément à chaque composant de couleur ; sélectionnez **[!UICONTROL Luminosité]** si vous souhaitez appliquer l’accentuation aux zones de luminosité de l’image.

**Rééchantillonnage**

Sélectionnez le menu **[!UICONTROL Rééchantillonnage]** et choisissez une option. Les options suivantes permettent d’accentuer l’image lorsque sa résolution est réduite :

* **[!UICONTROL Aucune]** : désactive le rééchantillonnage.

* **[!UICONTROL Bilinéaire]** : méthode de rééchantillonnage la plus rapide ; certains artefacts de crénelage sont visibles.

* **[!UICONTROL Bicubique]** : augmente l’utilisation de CPU sur le serveur d’images, mais produit des images plus nettes avec des artefacts d’alias moins visibles.

* **[!UICONTROL `Sharpen 2`]** : produit des résultats légèrement plus nets que **[!UICONTROL bicubique]**, mais à un coût CPU encore plus élevé sur le serveur d’images.

* **[!UICONTROL Trilinéaire]** : utilise des résolutions plus élevées et plus basses, le cas échéant. Recommandé uniquement lorsque le crénelage pose problème. Elle réduit la taille du fichier JPEG en raison des données à haute fréquence réduites.

**Paramètres d’image prédéfinis et accentuation**

Intégrez les trois effets d’accentuation pour obtenir votre résultat final. Cependant, cette méthode n’est pas recommandée. Adobe Dynamic Media Classic vous recommande d’enregistrer vos effets d’accentuation dans le cadre d’un paramètre d’image prédéfini. Les paramètres d’image prédéfinis vous permettent de compresser les modificateurs d’image les plus souvent utilisés afin de créer une image redimensionnée dynamiquement dans une petite chaîne de texte. Un paramètre d’image prédéfini contient des valeurs pour le format de fichier (généralement JPEG pour le web), le nombre de pixels et l’accentuation de l’image. Au lieu d’ajouter l’URL avec chaque modificateur d’image que vous devez utiliser pour créer un type spécifique de taille d’image, créez un paramètre d’image prédéfini nommé, tel que « miniature ». Ensuite, configurez le paramètre prédéfini d’image miniature avec la taille, le format de fichier et les options d’accentuation appropriés. Appelez l’image à l’aide du nom du paramètre d’image prédéfini. Les paramètres d’image prédéfinis raccourcissent la longueur globale de l’URL. Ces deux URL produisent la même image JPEG 350x350 avec accentuation :

* `https://sample.scene7.com/is/image/S7train/Backpack_A?wid=350&hei=350&fmt=jpeg&qlt=85,0&resMode=sharp2&op_usm=0.9,1.0,8,0`
* `https://sample.scene7.com/is/image/S7train/Backpack_A?$!_s7product$`

Les paramètres d’image prédéfinis peuvent être modifiés et mis à jour à tout moment. Les résultats d’une modification apportée à un paramètre d’image prédéfini s’affichent après la publication et après l’effacement du cache de l’URL.

Si vous utilisez un paramètre prédéfini pour chaque image d’une catégorie de taille, tout administrateur d’entreprise peut mettre à jour la définition de ce paramètre d’image prédéfini. Ils peuvent ensuite republier et affecter chaque image utilisant ce format. Le tout sans modifier de code Web. En règle générale, utilisez un paramètre d’image prédéfini par taille unique sur votre site. Pour ajouter un paramètre d’image prédéfini, sur la barre de navigation globale, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Paramètres de l’application]** > **[!UICONTROL Paramètres d’image prédéfinis]**. Sélectionnez ensuite **[!UICONTROL Ajouter]** ou sélectionnez **[!UICONTROL Modifier]** pour modifier un paramètre prédéfini existant. Le seul champ obligatoire est le nom du paramètre prédéfini lui-même. Cependant, il est préférable d’inclure un certain niveau d’accentuation dans chaque paramètre prédéfini.

**Qualité**

Les options de qualité JPG contrôlent le niveau de compression JPG :

* **Qualité JPG** : sélectionnez cette option si vous souhaitez contrôler les niveaux de compression et le sous-échantillonnage de chrominance.

* **Curseur** : détermine le niveau de compression JPG. Ce paramètre affecte à la fois la taille du fichier et la qualité de l’image. L’échelle de qualité de JPG s’étend de 1 à 100.

* **Activer le sous-échantillonnage de la chrominance JPG** : l’œil étant moins sensible aux informations de couleur haute fréquence que la luminance haute fréquence, les images JPEG divisent les informations d’image en composants de luminance et de couleur. Lorsqu’une image JPEG est compressée, la composante de luminance conserve sa pleine résolution, tandis que les composantes de couleur sont sous-échantillonnées par interpolation, c’est-à-dire le calcul de la moyenne de groupes de pixels. Le sous-échantillonnage réduit le volume de données de moitié ou d’un tiers, sans avoir d’incidence sur la qualité perçue. La réduction de résolution ne s’applique pas aux images en niveaux de gris. Cette technique réduit le niveau de compression nécessaire pour les images présentant un contraste élevé (par exemple, les images contenant du texte superposé).

**Définir des options d’accentuation pour l’ensemble de l’entreprise**

Si vous n’avez pas utilisé de paramètre d’image prédéfini ou transmis des protocoles d’accentuation spécifiques au serveur d’images le long de la chaîne URL, l’accentuation de votre image ne se produit pas en cas de sous-échantillonnage. Pour vous assurer qu’une image a toujours un certain accentuation si ce manque d’accentuation se produit, définissez les valeurs d’accentuation par défaut.

Pour définir les options d’accentuation par défaut de votre entreprise, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Configuration de la publication]** > **[!UICONTROL Serveur d’images]**. Si vous définissez le Mode de rééchantillonnage par défaut sur **`Sharp2`**, l’image est toujours plus nette lors du sous-échantillonnage.

**Ajouter un accentuation aux paramètres prédéfinis de visionneuse**

À moins que vous n’ayez ajouté des modificateurs d’image d’accentuation au paramètre prédéfini, la petite image de charge initiale peut sembler douce, car elle est sous-échantillonnée pour s’adapter à la fenêtre de la visionneuse sans être accentuée.

Les paramètres prédéfinis de la visionneuse (tels que les paramètres d’image prédéfinis) centralisent les options telles que l’habillage, les boutons et la vitesse d’animation. Les paramètres prédéfinis de la visionneuse se trouvent dans la même section que Paramètres d’image prédéfinis, sous **[!UICONTROL Configuration]** > **[!UICONTROL Paramètres de l’application]** > **[!UICONTROL Paramètres prédéfinis de la visionneuse]**.

Voir la vidéo de formation [Paramètres prédéfinis de la visionneuse](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS).

Les options des modificateurs se trouvent dans la section des paramètres principaux de tous les paramètres prédéfinis de visionneuse de zoom personnalisés, du catalogue électronique et de rotation. En ajoutant les commandes d’accentuation des URL à la zone Modificateurs, vous ajoutez l’accentuation chaque fois que cette visionneuse est appelée avec ce paramètre prédéfini de visionneuse.

Pour appeler le paramètre prédéfini de visionneuse, utilisez la commande `config=` sur l’URL de la visionneuse. Voici un exemple d’appel d’une visionneuse d’images avec un paramètre prédéfini de visionneuse (`FantasticoZoom2022`) :

`https://s7d9.scene7.com/s7viewers/html5/ZoomViewer.html?asset=Scene7SharedAssets/ImageSet-Views-Sample&config=S7train/FantasticoZoom2022`

Le paramètre prédéfini ici accentue et modifie l’aspect par défaut de la visionneuse.

**Création de remplacements spécifiques à l’image**

La dernière méthode d’accentuation, et la moins recommandée, consiste à créer des valeurs de remplacement d’accentuation pour chaque image. Cette méthode remplace l’accentuation dans un paramètre d’image prédéfini par ses propres valeurs spécifiques. Toutefois, cette méthode remplace également toutes les autres méthodes d’accentuation, quelle que soit leur taille. Le meilleur scénario d’utilisation de cette méthode se présente dans le cas où certaines images ne sont pas haute résolution et que les valeurs dans les paramètres d’image prédéfinis sont trop élevées pour ces petites images. Dans ce cas, un accentuation par image est nécessaire.

Dans Adobe Dynamic Media Classic, sélectionnez une image, accédez à l’affichage des détails (en double-cliquant ou en appuyant sur le bouton **[!UICONTROL Affichage des détails]**), puis sélectionnez **[!UICONTROL Accentuer]**. Modifiez un paramètre, puis sélectionnez **[!UICONTROL Enregistrer]**. Ce processus indique au serveur d’images d’utiliser ces paramètres d’accentuation plutôt qu’une commande que vous appelez dans l’URL, telle qu’un modificateur d’accentuation ou un paramètre d’image prédéfini. Veillez à procéder à la publication pour que les modifications soient prises en compte.
