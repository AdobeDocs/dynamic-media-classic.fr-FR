---
title: Accentuation d’une image
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
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '2207'
ht-degree: 30%

---

# Accentuation d’une image {#sharpening-an-image}

L’accentuation est une technique de manipulation d’image qui rend plus nets les contours d’une image numérique. L’accentuation consiste à augmenter le contraste entre les pixels de contour, et ainsi à souligner la transition entre les zones sombres et les zones claires. L’accentuation augmente le contraste local et fait ressortir les détails infimes. Il n’existe pas de formule magique pour accentuer correctement toutes les images. Une accentuation trop faible produit une image douce, tandis qu’une accentuation exagérée crée des halos, des artefacts et du bruit.

Adobe Dynamic Media Classic recommande vivement d’utiliser des paramètres d’image prédéfinis pour toutes les images. Elles garantissent une taille uniforme et l’accentuation est appliquée sur toute image appelée avec un paramètre d’image prédéfini. De plus, vous pouvez facilement modifier et modifier les paramètres d’accentuation d’un paramètre d’image prédéfini. A la prochaine publication, toutes les images appelées avec ces paramètres prédéfinis se voient appliquer les nouvelles valeurs.

Adobe Dynamic Media Classic recommande également d’ajouter de l’accentuation aux paramètres prédéfinis de la visionneuse, puis d’appeler une visionneuse avec ce paramètre prédéfini. Cela garantit que les images de vos visionneuses sont claires et attrayantes.

Cependant, que vous utilisiez des paramètres d’image prédéfinis et des paramètres de visionneuse prédéfinis, ou une méthode d’accentuation, l’essentiel est que vous devez accentuer vos images. Si ce n’est pas le cas, vos images (et votre site web) peuvent sembler douces et floues.

>[!NOTE]
>
>les commandes d’accentuation remplacent les paramètres d’image prédéfinis, notamment les effets d’accentuation. Un paramètre d’image prédéfini détermine la taille et le formatage avec lesquels les images sont diffusées à partir des serveurs d’images Dynamic Media. Adobe Dynamic Media Classic recommande vivement d’utiliser des paramètres d’image prédéfinis pour diffuser toutes les images afin de s’assurer que leur taille et leur accentuation sont uniformes. Cependant, après avoir modifié les paramètres d’accentuation d’une image individuelle, les paramètres d’image prédéfinis relatifs à l’accentuation ne s’appliquent plus à l’image. Elle est diffusée sans ces paramètres.

Il est souvent nécessaire d’accentuer les images. Adobe Dynamic Media Classic et les serveurs d’images offrent plusieurs options d’accentuation. Il est important de comprendre l’impact de l’accentuation sur une image et le degré d’accentuation dont vous avez besoin. La plupart des images ont besoin d’accentuation mais le degré nécessaire dépend de l’image.

L’accentuation de l’image augmente le contraste des pixels pour créer un effet de contours renforcés. Ce contraste amélioré des bords est perçu par les yeux comme de la netteté. S’il est facile d’améliorer une image à l’aide de filtres d’accentuation, il est également facile de trop renforcer la netteté d’une image,

L’accentuation excessive d’une image crée un effet de halo ou de bande des lignes du bord.

Vous pouvez suivre certaines bonnes pratiques pour optimiser l’accentuation de vos images dans Adobe Dynamic Media Classic et sur Dynamic Media Image Server.

Voir [ Bonnes pratiques pour l’accentuation des images dans Adobe Dynamic Media Classic et sur Dynamic Media Image Server](/help/using/assets/s7_sharpening_images.pdf).

Voir aussi la vidéo de formation [Accentuation](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/547_sharpening1_converted%20renamed_Done-AVS).

**Pour accentuer une image :**

Pour accentuer une image, sélectionnez son bouton de survol **[!UICONTROL Modifier]** et choisissez **[!UICONTROL Accentuer]**, ou ouvrez-le dans le panneau Parcourir en mode Affichage des détails, puis sélectionnez **[!UICONTROL Accentuer]**. La page Éditeur d’accentuation s’ouvre avec des commandes d’accentuation. Choisissez les commandes de votre choix, puis cliquez sur **[!UICONTROL Enregistrer]**.

>[!NOTE]
>
>Avant d’accentuer une image, vous pouvez sélectionner le menu Appliquer les paramètres prédéfinis et choisir un paramètre d’image prédéfini pour en découvrir les effets. Les effets d’accentuation d’un paramètre d’image prédéfini conviennent à votre image. Le menu **[!UICONTROL Appliquer les paramètres prédéfinis]** se trouve au bas de la page Éditeur de netteté.

**Options d’accentuation**

Le tableau suivant présente les options d’accentuation du serveur Image Server.

| Nom | Protocole d’URL | Valeurs | Exemple |
| --- | --- | --- | --- |
| Accentuation simple | `op_sharpen` | `0` ou `1` | `op_sharpen=1` |
| Mode de ré-échantillonnage | `resMode` | `bilin`, `bicub`, `sharp2`, `trilin`<br><br>`bilin` : sélectionne l’interpolation binaire standard. Méthode de rééchantillonnage la plus rapide ; certains artefacts de crénelage sont souvent visibles.<br>`bicub` : sélectionne l’interpolation bicubique. Plus processeur que `bilin`, mais produit des images plus nettes avec des artefacts de crénelage plus discrets.<br><br>`sharp2` : sélectionne une fonction Lanczos Windows® modifiée comme algorithme d’interpolation. Elle peut produire des résultats légèrement plus nets que le bicube à un coût de processeur plus élevé.<br><br>`trilin` : sélectionne une interpolation trilinéaire modifiée, qui utilise des résolutions supérieure et inférieure, le cas échéant. Méthode recommandée si le crénelage devient problématique. Elle réduit la taille des fichiers JPEG en raison des données à haute fréquence réduites. | `resMode=sharp2` |
| Masquage flou | `op_usm` | `amount`, `radius`, `threshold`, `monochrome`<br><br>`amount` : facteur de force de filtrage (réel 0...5)<br><br>`radius` : rayon du noyau de filtre en pixels (réel 0...250) <br><br>`threshold` : niveau de seuil de filtre (int 0...255)<br><br>`monochrome` : défini sur `0` pour masquer distinctement chaque composant de couleur, défini sur `1` pour masquer l’image flou masquer l’accentuation névence (intensité) | `op_usm=1,1,10,0` |

Sélectionnez le menu **[!UICONTROL Accentuation]** et choisissez une option :

* **None** : désactive l’accentuation.

* **Accentuer** : exécute une simple transmission d’accentuation sur le fichier après son redimensionnement. Il est similaire au filtre &quot;Accentuer&quot; dans Adobe Photoshop et prend en charge tous les paramètres utilisateur. Normalement, vous utiliseriez ce filtre ou **[!UICONTROL Masquage flou]**, mais pas les deux. Cette méthode n’est pas recommandée comme meilleure pratique, mais elle permet de compenser le flou. (URL : `op_sharpen`)

* **Masquage flou** : permet d’affiner l’effet d’un filtre d’accentuation sur l’image finale à résolution réduite. Vous pouvez contrôler l’intensité de l’effet, son rayon (mesuré en pixels) et un seuil de contraste qui est ignoré. Cet effet utilise les mêmes options que le filtre &quot;Masquage flou&quot; de Photoshop. (URL : `op_usm`)

Sélectionnez ces options afin d’affiner l’accentuation à l’aide du masquage flou :

* **Quantité** : contrôle le degré de contraste appliqué aux pixels de contour. La valeur par défaut est de 0. Pour des images à haute résolution, vous pouvez l’augmenter jusqu’à 5. Imaginez la quantité comme étant l’unité de mesure de l’intensité du filtre. Le paramètre **[!UICONTROL Amount]** dans Adobe Dynamic Media Classic n’est pas le même que le paramètre Amount dans Adobe Photoshop. Adobe Photoshop utilise un montant compris entre 1 et 500 %, tandis qu’Adobe Dynamic Media Classic le met à l’échelle de 0,0 à 5,0. (La valeur 5 est environ équivalente à 500 % dans Photoshop, 0,9 à 90 %, et ainsi de suite.)

* **Rayon** : détermine le nombre de pixels entourant les pixels de contour qui affectent l’accentuation. L’effet est exécuté sur tous les pixels de l’image et s’étend dans toutes les directions. 

La valeur appropriée du rayon dépend de la taille de l’image. Une valeur faible n’accentue que les pixels de contour. Une valeur élevée accentue une marge de pixels plus large. 

Par exemple, pour obtenir un effet d’accentuation similaire pour une image de 2 000 × 2 000 pixels et une image de 500 × 500 pixels, vous pouvez définir une valeur de rayon de deux pixels sur l’image de 2 000 × 2 000 pixels. Définissez ensuite une valeur de rayon d’un pixel sur l’image de 500 × 500 pixels (une valeur plus grande pour une image contenant plus de pixels).

* **Seuil** : détermine la plage de contraste à ignorer lorsque le filtre Accentuation est appliqué. Cette option détermine la différence entre les pixels accentués et la zone environnante avant l’accentuation des pixels de contour.

Le seuil utilise une valeur comprise entre 0 et 255, qui est le nombre d’étapes de luminosité dans une image en niveaux de gris. 0 = noir, 128 = 50 % gris et 255 = blanc. Par exemple, une valeur de seuil de 12 ignore les légères variations de luminosité de la peau. Cela n’ajoute pas de bruit, tout en ajoutant un contraste sur les bords dans les zones contrastées, comme l’endroit où les cils rencontrent la peau.

Par exemple, supposons que vous ayez une photo du visage de quelqu&#39;un. Le masquage flou accentue les parties de l’image les plus contrastées et la peau lisse. Même la peau la plus lisse affiche des variations subtiles de ses valeurs de luminosité. Si vous n’utilisez pas une valeur de seuil, le filtre accentue ces légères variations dans les pixels de la peau, créant ainsi un effet de bruit (probablement indésirable), tout en augmentant le contraste sur les cils, ce qui améliore la netteté (probablement souhaitable). Pour l’éviter, utilisez une valeur de seuil qui indique au filtre d’ignorer les pixels qui ne modifient pas considérablement le contraste, comme la peau lisse. Pour éviter d’introduire du bruit ou des images de postérisation avec des tons chair, par exemple, essayez d’essayer avec les valeurs **[!UICONTROL Seuil]** de deux à 20. La valeur par défaut **[!UICONTROL Seuil]** de 0 accentue tous les pixels de l’image.

* **Appliquer à** : choisissez **[!UICONTROL Chaque couleur]** si vous souhaitez appliquer l’accentuation séparément à chaque composant de couleur ; choisissez **[!UICONTROL Luminosité]** si vous souhaitez appliquer l’accentuation aux zones de luminosité de l’image.

**Rééchantillonnage**

Sélectionnez le menu **[!UICONTROL Rééchantillonnage]** et choisissez une option. Les options suivantes permettent d’accentuer l’image lorsque sa résolution est réduite :

* **[!UICONTROL None]** : désactive le rééchantillonnage.

* **[!UICONTROL Bilinéaire]** : méthode de rééchantillonnage la plus rapide ; certains artefacts de crénelage sont visibles.

* **[!UICONTROL Bicubique]** : accroît l’utilisation du processeur sur le serveur d’images, mais produit des images plus nettes avec des artefacts de crénelage plus discrets.

* **[!UICONTROL `Sharpen 2`]** : produit des résultats légèrement plus nets que **[!UICONTROL Bicubique]**, mais avec un coût CPU encore plus élevé sur le serveur d’images.

* **[!UICONTROL Trilinéaire]** : utilise des résolutions plus élevées et plus basses si elles sont disponibles ; recommandé uniquement lorsque le crénelage est un problème. Elle réduit la taille du fichier JPEG en raison des données à haute fréquence réduites.

**Paramètres d’image prédéfinis et accentuation**

Vous pouvez incorporer les trois effets d’accentuation pour obtenir votre résultat final. Cependant, cette méthode n’est pas recommandée. Adobe Dynamic Media Classic vous recommande d’enregistrer vos effets d’accentuation dans le cadre d’un paramètre d’image prédéfini. Les paramètres d’image prédéfinis vous permettent de regrouper les modificateurs d’image les plus souvent utilisés afin de créer une image redimensionnée dynamiquement dans une petite chaîne de texte. Un paramètre d’image prédéfini contient des valeurs pour le format de fichier (généralement JPEG pour le web), le nombre de pixels et l’accentuation de l’image. Au lieu d’ajouter l’URL à chaque modificateur d’image que vous devez utiliser pour créer un type spécifique de taille d’image, créez un paramètre d’image prédéfini nommé, tel que &quot;miniature&quot;. Ensuite, configurez le paramètre prédéfini d’image miniature avec la taille, le format de fichier et les options d’accentuation appropriés. Appelez l’image à l’aide du nom du paramètre d’image prédéfini. Les paramètres d’image prédéfinis raccourcissent la longueur de l’URL globale. Ces deux URL produisent la même image de JPEG 350x350 avec accentuation :

* `https://sample.scene7.com/is/image/S7train/Backpack_A?wid=350&hei=350&fmt=jpeg&qlt=85,0&resMode=sharp2&op_usm=0.9,1.0,8,0`
* `https://sample.scene7.com/is/image/S7train/Backpack_A?$!_s7product$`

Les paramètres d’image prédéfinis peuvent être modifiés et mis à jour à tout moment. Vous voyez les résultats d’une modification d’un paramètre d’image prédéfini après la publication et une fois que le cache de l’URL est effacé.

Si vous utilisez un paramètre prédéfini pour chaque image d’une catégorie de taille, tout administrateur d’entreprise peut mettre à jour la définition de ce paramètre d’image prédéfini. Ils peuvent ensuite republier et affecter chaque image utilisant ce format. Tout cela sans modifier aucun code Web. En règle générale, utilisez un paramètre d’image prédéfini par taille unique sur votre site. Pour ajouter un paramètre d’image prédéfini, dans la barre de navigation globale, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Paramètres de l’application]** > **[!UICONTROL Paramètres d’image prédéfinis]**. Sélectionnez ensuite **[!UICONTROL Ajouter]** ou **[!UICONTROL Modifier]** pour modifier un paramètre prédéfini existant. Le seul champ obligatoire est le nom du paramètre prédéfini lui-même. Cependant, il est préférable d’inclure un certain niveau d’accentuation dans chaque paramètre prédéfini.

**Qualité JPG**

Les options de qualité JPG contrôlent le niveau de compression JPG :

* **JPG Qualité du** : sélectionnez cette option si vous souhaitez contrôler les niveaux de compression et le sous-échantillonnage de chrominance.

* **Curseur** : détermine le niveau de compression du JPG. Ce paramètre affecte à la fois la taille du fichier et la qualité de l’image. L’échelle de la qualité JPG s’étend de 1 à 100.

* **Activer le sous-échantillonnage de la chrominance JPG** : comme l’oeil est moins sensible aux informations colorimétriques à haute fréquence qu’à la luminance à haute fréquence, les images de JPEG divisent les informations d’image en composantes de luminance et de couleur. Lorsqu’une image JPEG est compressée, la composante de luminance conserve sa pleine résolution, tandis que les composantes de couleur sont sous-échantillonnées par interpolation, c’est-à-dire le calcul de la moyenne de groupes de pixels. Le sous-échantillonnage réduit le volume des données d’un demi-tiers ou d’un tiers, sans pratiquement avoir d’incidence sur la qualité perçue. La réduction de résolution ne s’applique pas aux images en niveaux de gris. Cette technique réduit le niveau de compression nécessaire pour les images présentant un contraste élevé (par exemple, les images contenant du texte superposé).

**Définition des options d’accentuation à l’échelle de l’entreprise**

Si vous n’avez pas utilisé de paramètre d’image prédéfini ou si vous avez transmis des protocoles d’accentuation spécifiques au serveur d’images le long de la chaîne URL, aucune accentuation de l’image ne se produit lorsque la résolution est réduite. Cependant, si cette absence d’accentuation se produit, vous pouvez définir des valeurs d’accentuation par défaut afin de vous assurer que toute image présente toujours une certaine accentuation.

Pour définir les options d’accentuation par défaut de votre entreprise, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Configuration de Publish]** > **[!UICONTROL Serveur d’images]**. Si vous définissez le mode Rééchantillonnage par défaut sur **`Sharp2`**, l’image est toujours accentuée lors du sous-échantillonnage.

**Ajouter une accentuation aux paramètres prédéfinis de la visionneuse**

À moins que vous n’ajoutiez des modificateurs d’accentuation à l’image prédéfinie, la petite image de chargement initial peut sembler douce, car elle est sous-échantillonnée pour s’adapter à la fenêtre de la visionneuse sans être accentuée.

Les paramètres prédéfinis de la visionneuse (tels que les paramètres d’image prédéfinis) vous permettent de centraliser de nombreuses options à un seul emplacement, y compris le choix de l’habillage et les options de la visionneuse (comme un bouton Imprimer ou le contrôle de la vitesse de l’animation du zoom). Les paramètres de visionneuse prédéfinis se trouvent dans la même section que les paramètres d’image prédéfinis, sous **[!UICONTROL Configuration]** > **[!UICONTROL Paramètres de l’application]** > **[!UICONTROL Paramètres de visionneuse prédéfinis]**.

Voir la vidéo de formation [Paramètres visionneuse prédéfinis](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) .

Les options des modificateurs se trouvent dans la section des paramètres principaux de tous les paramètres prédéfinis de visionneuse de zoom personnalisés, du catalogue électronique et de rotation. En ajoutant les commandes d’accentuation d’URL à la zone Modificateurs, vous ajoutez une accentuation chaque fois que cette visionneuse est appelée avec ce paramètre prédéfini de visionneuse.

Pour appeler le paramètre prédéfini de la visionneuse, utilisez la commande `config=` sur l’URL de la visionneuse. Voici un exemple d’appel d’une visionneuse d’images (chaussures) avec un paramètre prédéfini de visionneuse (`FantasticoZoom2022`) :

`https://s7d9.scene7.com/s7viewers/html5/ZoomViewer.html?asset=Scene7SharedAssets/ImageSet-Views-Sample&config=S7train/FantasticoZoom2022`

Dans ce cas, les paramètres prédéfinis renforcent et modifient l’habillage par défaut de la visionneuse.

**Créer des remplacements spécifiques à une image**

La dernière méthode d’accentuation, et la moins recommandée, consiste à créer des valeurs de remplacement d’accentuation pour chaque image. Cette méthode remplace l’accentuation dans un paramètre d’image prédéfini par ses propres valeurs spécifiques. Cependant, cette méthode remplace également toutes les autres méthodes d’accentuation à n’importe quelle taille. Le meilleur scénario d’utilisation de cette méthode se présente dans le cas où certaines images ne sont pas haute résolution et que les valeurs dans les paramètres d’image prédéfinis sont trop élevées pour ces petites images. Dans ce cas, une certaine accentuation de l’image est peut-être nécessaire.

Dans Adobe Dynamic Media Classic, sélectionnez une image, accédez à la vue Détails (en double-cliquant ou en appuyant sur le bouton **[!UICONTROL Affichage des détails]**), puis sélectionnez **[!UICONTROL Accentuer]**. Modifiez n&#39;importe quel paramètre, puis sélectionnez **[!UICONTROL Enregistrer]**. Ce processus demande au serveur d’images d’utiliser ces paramètres d’accentuation plutôt que toute commande appelée dans l’URL, comme un modificateur d’accentuation ou un paramètre d’image prédéfini. Veillez à publier pour que les modifications prennent effet.
