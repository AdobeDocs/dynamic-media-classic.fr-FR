---
title: Accentuation d’une image
description: Découvrez comment accentuer une image.
uuid: d86af74a-89c5-4f2b-96ba-f2e7da600bca
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 11cd5362-d90a-4c1e-bfbd-46a65a554409
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '2155'
ht-degree: 73%

---


# Accentuation d’une image {#sharpening-an-image}

L’accentuation est une technique de manipulation d’image qui rend plus nets les contours d’une image numérique. L’accentuation consiste à augmenter le contraste entre les pixels de contour, et ainsi à souligner la transition entre les zones sombres et les zones claires. L’accentuation augmente le contraste local et fait ressortir les détails infimes. Il n’existe pas de formule magique pour accentuer correctement toutes les images. Une accentuation trop faible produit une image douce, tandis qu’une accentuation exagérée crée des halos, des artefacts et du bruit.

Dynamic Media Classic recommande vivement d’utiliser des paramètres d’image prédéfinis pour toutes les images. Vous vous assurez ainsi que toutes les images sont de taille uniforme et que l’accentuation est appliquée à chaque image avec des paramètres prédéfinis. En outre, vous pouvez modifier et remplacer facilement les paramètres d’accentuation prédéfinis des images. A la prochaine publication, toutes les images appelées avec ces paramètres prédéfinis se voient appliquer les nouvelles valeurs.

Dynamic Media Classic recommande également d’ajouter l’accentuation aux paramètres prédéfinis de la visionneuse, puis d’appeler une visionneuse avec ce paramètre prédéfini. Les images apparaissent ainsi de façon nette et attrayante dans vos visionneuses.

Cependant, que vous utilisiez les paramètres prédéfinis de la visionneuse ou des images, ou une autre méthode d’accentuation, l’important est que vous devez accentuer vos images. Si vous ne le faites pas, vos images (et votre site Web) peuvent prendre un aspect flou.

>[!NOTE]
>
>les commandes d’accentuation remplacent les paramètres d’image prédéfinis, notamment les effets d’accentuation. Un paramètre d’image prédéfini régit la taille et le formatage des images diffusées à partir des serveurs Dynamic Media Image Server. Dynamic Media Classic recommande vivement d’utiliser des paramètres d’image prédéfinis pour diffuser toutes les images afin de s’assurer que leur taille et leur accentuation sont uniformes. Cependant, après avoir modifié les paramètres d’accentuation d’une image individuelle, les paramètres d’image prédéfinis relatifs à l’accentuation ne s’appliquent plus à l’image. Elle est diffusée sans ces paramètres.

Il est souvent nécessaire d’accentuer les images. Dynamic Media Classic et les serveurs d’images offre plusieurs options d’accentuation. Il est important de comprendre l’impact de l’accentuation sur une image et le degré d’accentuation dont vous avez besoin. La plupart des images ont besoin d’accentuation mais le degré nécessaire dépend de l’image.

L’accentuation de l’image augmente le contraste des pixels pour créer un effet de contours renforcés. Ce contraste amélioré des bords est perçu par les yeux comme de la netteté. S’il est facile d’améliorer une image à l’aide de filtres d’accentuation, il est également facile de trop renforcer la netteté d’une image,

ce qui crée alors un effet de halo ou de bande sur les lignes de la bordure.

Vous pouvez suivre les meilleures pratiques pour optimiser l’accentuation de vos images dans Dynamic Media Classic et sur Dynamic Media Image Server.

Voir [Meilleures pratiques pour l’accentuation des images dans Dynamic Media Classic et sur Dynamic Media Image Server](/help/assets/s7_sharpening_images.pdf).

**Pour accentuer une image**

Pour accentuer une image, cliquez sur son bouton de survol **Modifier** et choisissez Accentuer, ou ouvrez-la dans le panneau de navigation de la vue de détails, puis cliquez sur **Accentuer**. L’écran Editeur de netteté apparaît avec les commandes d’accentuation. Choisissez les commandes et cliquez sur **Enregistrer**.

>[!NOTE]
>
>Avant d’accentuer une image, vous pouvez sélectionner le menu Appliquer les paramètres prédéfinis et choisir un paramètre d’image prédéfini pour en découvrir les effets. Les effets d’accentuation d’un paramètre d’image prédéfini peuvent être adaptés à votre image. Le menu Appliquer les paramètres prédéfinis se trouve dans la partie inférieure de l’écran Editeur de netteté.

**Options d’accentuation**

Le tableau suivant présente les options d’accentuation du serveur Image Server.

| Nom | Protocole d’URL | Valeurs | Exemple |
|--- |--- |--- |--- |
| Accentuation simple | op_sharpen | `0 | 1` | op_sharpen=1 |
| Mode de ré-échantillonnage | resMode | `bilin | bicub | sharp2 | trilin`<br><br>bilin : sélectionne l’interpolation bilinéaire standard. Il s’agit de la méthode de ré-échantillonnage la plus rapide ; certains artefacts de crénelage peuvent être visibles.<br>bicub : sélectionne l’interpolation bicubique. Bien qu’elle sollicite davantage le processeur que bilin, cette méthode produit des images plus nettes avec des artefacts de crénelage plus discrets.<br><br>sharp2 : sélectionne une fonction de fenêtrage Lanczos modifiée comme algorithme d’interpolation. Peut produire des images légèrement plus nettes que la méthode bicubique en sollicitant toutefois davantage le processeur.<br><br>trilin : sélectionne une interpolation trilinéaire modifiée qui utilise les deux résolutions supérieure et inférieure lorsqu’elles sont disponibles. Méthode recommandée si le crénelage devient problématique. Elle réduit la taille des fichiers JPEG en raison des données à haute fréquence réduites. | resMode=sharp2 |
| Masquage flou | op_usm | quantité, rayon, seuil, monochrome<br><br>quantité : facteur de résistance du filtre (réel 0...5)<br><br>rayon : rayon du noyau du filtre en pixels (réel 0...250) <br><br>seuil : seuil de filtre (int 0...255)<br><br>monochrome: a été défini sur 0 pour masquer de façon précise chaque composante de couleur séparément, et sur 1 pour masquer de façon précise la luminosité de l’image (intensité) | op_usm=1,1,10,0 |

Dans le menu Accentuation, choisissez une option :

**** AucunDésactive l’accentuation.

**** AccentuerExécute une passe d’accentuation simple sur le fichier après son redimensionnement. Cette fonction ressemble au filtre « Accentuer » de Photoshop et prend en charge tous les paramètres de l’utilisateur. Normalement, vous pouvez utiliser ce filtre ou le masquage flou, mais pas les deux. Cette méthode n’est pas recommandée comme meilleure pratique, mais elle permet de compenser le flou. (URL: op_sharpen)

**Accentuation** MasquePermet d’affiner l’effet d’un filtre d’accentuation sur l’image finale sous-échantillonnée. Vous pouvez contrôler l’intensité de l’effet, le rayon de l’effet (mesuré en pixels) et un seuil de contraste qui seront ignorés. Cet effet utilise les mêmes options que le filtre de masquage flou de Photoshop. (URL: op_usm)

Choisissez les options suivantes pour préciser l’accentuation avec le masquage flou :

**** AmountContrôle le degré de contraste appliqué aux pixels de contour. La valeur par défaut est de 0. Pour des images à haute résolution, vous pouvez l’augmenter jusqu’à 5. Imaginez la quantité comme étant l’unité de mesure de l’intensité du filtre. Notez que le paramètre Montant dans Dynamic Media Classic n’est pas identique au paramètre Montant dans Photoshop. Photoshop utilise un montant compris entre 1 % et 500 %, tandis que Dynamic Media Classic effectue une mise à l’échelle de 0,0 à 5,0. (La valeur 5 est environ équivalente à 500 % dans Photoshop, 0,9 à 90 %, et ainsi de suite.)

**** Rayon Détermine le nombre de pixels entourant les pixels de contour qui affectent l’accentuation. L’effet est exécuté sur tous les pixels de l’image et s’étend dans toutes les directions. 

La valeur appropriée du rayon dépend de la taille de l’image. Une valeur faible n’accentue que les pixels de contour. Une valeur élevée accentue une marge de pixels plus large. 

Par exemple, pour obtenir un effet d’accentuation similaire pour une image de 2 000 x 2 000 pixels et une image de 500 x 500 pixels, vous pouvez définir une valeur de rayon de deux pixels sur l’image de 2 000 x 2 000 pixels. Ensuite, définissez une valeur de rayon d’un pixel pour l’image de 500 x 500 pixels (définissez une valeur plus élevée pour une image contenant plus de pixels).

**** SeuilDétermine la plage de contraste à ignorer lorsque le filtre de masquage flou est appliqué. Cette option définit l’écart recherché entre les pixels et la zone environnante avant qu’ils ne soient considérés comme des pixels de contour et ne soient accentués. 

Le seuil utilise une valeur de 0 à 255, qui est le nombre de degrés de luminosité dans une image en niveaux de gris. 0 = noir, 128 = 50 % gris et 255 = blanc. Par exemple, une valeur de seuil de 12 ignore les légères variations de luminosité de la peau, afin de ne pas ajouter de bruit, tout en ajoutant un contraste sur les bords dans les zones contrastées, comme la zone où les cils rencontrent la peau. 

Par exemple, supposons que vous ayez une photo d’un visage. Le masquage flou accentue les parties de l’image les plus contrastées et la peau lisse. Même la peau la plus lisse affiche des variations subtiles de ses valeurs de luminosité. Si vous n’utilisez pas une valeur de seuil, le filtre accentue ces légères variations dans les pixels de la peau, créant ainsi un effet de bruit (probablement indésirable), tout en augmentant le contraste sur les cils, ce qui améliore la netteté (probablement souhaitable). Pour l’éviter, utilisez une valeur de seuil qui indique au filtre d’ignorer les pixels qui ne modifient pas considérablement le contraste, comme la peau lisse. Pour éviter d’introduire du bruit ou de la postérisation (dans les images avec des tonalités de chair, par exemple), essayez d’expérimenter des valeurs de seuil comprises entre 2 et 20. La valeur de seuil par défaut de 0 accentue tous les pixels de l’image.

**Appliquer** à chaque couleur pour appliquer l’accentuation séparément à chaque composante de couleur ; choisissez Luminosité pour appliquer l’accentuation aux zones de luminosité de l’image.

**Ré-échantillonnage**

Sélectionnez le menu Ré-échantillonnage, puis choisissez une option. Les options suivantes permettent d’accentuer l’image lorsque sa résolution est réduite :

**** AucunDésactive le rééchantillonnage.

**** BilinéaireLa méthode de rééchantillonnage la plus rapide ; certains artefacts de crénelage sont visibles.

**** BicubiqueAugmente l’utilisation du processeur sur le serveur Image Server, mais produit des images plus nettes avec des artefacts de crénelage moins visibles.

**Sharpen2** peut produire des résultats légèrement plus nets que l’option Bicubique, mais à un coût CPU encore plus élevé sur le serveur Image Server.

**** TrilinéaireUtilise des résolutions supérieures et inférieures si elles sont disponibles ; recommandé uniquement lorsque le crénelage est un problème. Elle réduit la taille du fichier JPEG en raison des données à haute fréquence réduites.

**Accentuation et paramètres d’image prédéfinis**

Vous pouvez mélanger les trois effets d’accentuation pour obtenir votre résultat final. Cette approche n’est toutefois pas recommandée. Dynamic Media Classic vous recommande d’enregistrer vos effets d’accentuation dans le cadre d’un paramètre d’image prédéfini.Les paramètres d’image prédéfinis vous permettent de regrouper les modificateurs d’image les plus souvent utilisés afin de créer une image redimensionnée dynamiquement dans une petite chaîne de texte. Un paramètre d’image prédéfini contient des valeurs pour le format de fichier (généralement en format JPEG pour le Web), le nombre de pixels et l’accentuation d’image. Au lieu d’ajouter à l’URL chaque modificateur d’image nécessaire à la création d’un certain type de taille d’image, vous créez des paramètres d’image prédéfinis, par exemple « Miniature », vous configurez les paramètres prédéfinis de la miniature en indiquant les options appropriées de taille, de fichier et d’accentuation, puis vous appelez l’image avec le nom du paramètre d’image prédéfini. Les paramètres d’image prédéfinis raccourcissent la longueur globale de l’URL. Ces deux URL produisent la même image JPEG 350 x 350 avec accentuation : 

* `https://sample.scene7.com/is/image/S7train/Backpack_A?wid=350&hei=350&fmt=jpeg&qlt=85,0&resMode=sharp2&op_usm=0.9,1.0,8,0`
* `https://sample.scene7.com/is/image/S7train/Backpack_A?$!_s7product$`

Les paramètres d’image prédéfinis peuvent être modifiés et mis à jour à tout moment. Vous pouvez voir les résultats de la modification d’un paramètre d’image prédéfini après la publication et une fois que le cache pour l’URL est effacé.

Si vous utilisez un paramètre prédéfini pour chaque image dans une catégorie de taille, tout administrateur d’entreprise peut mettre à jour ce paramètre d’image prédéfini, republier et affecter toutes les images qui utilisent ce format, sans aucune modification du code du site Web. En règle générale, utilisez un paramètre d’image prédéfini par taille unique sur votre site. Pour ajouter un paramètre d’image prédéfini, sélectionnez Configuration > Paramètres de l’application > Paramètres d’image prédéfinis. Ensuite, choisissez d’ajouter ou de modifier un paramètre prédéfini existant. Le seul champ obligatoire est le nom du paramètre prédéfini lui-même. Toutefois, vous devez inclure un certain degré d’accentuation dans chaque paramètre prédéfini.

**Qualité JPG**

Les options de qualité JPG contrôlent le niveau de compression JPG :

**JPG** QualitySélectionnez cette option si vous souhaitez contrôler les niveaux de compression et le sous-échantillonnage de chrominance.

**** SliderDétermine le niveau de compression JPG. Ce paramètre affecte à la fois la taille du fichier et la qualité de l’image. L’échelle de qualité JPG est de 1 à 100.

**Activer le** sous-échantillonnage de la chrominance JPGEtant donné que l’oeil est moins sensible aux informations sur les couleurs à haute fréquence qu’à la luminance à haute fréquence, les images JPEG divisent les informations sur les images en composantes de luminance et de couleur. Lorsqu’une image JPEG est compressée, la composante de luminance conserve sa pleine résolution, tandis que les composantes de couleur sont sous-échantillonnées par interpolation, c’est-à-dire le calcul de la moyenne de groupes de pixels. La réduction de résolution (sous-échantillonnage) réduit de moitié ou d’un tiers le volume de données, quasiment sans nuire à la qualité perceptible par l’œil humain. La réduction de résolution ne s’applique pas aux images en niveaux de gris. Cette technique réduit le niveau de compression nécessaire pour les images présentant un contraste élevé (par exemple, les images contenant du texte superposé).

**Définition des options de l’accentuation dans toute l’entreprise**

Sans paramètre d’image prédéfini ou de protocole d’accentuation spécifique au serveur Image Server en plus de la chaîne de l’URL, votre image n’est pas accentuée lorsque sa résolution est réduite. Cependant, vous pouvez définir des valeurs d’accentuation par défaut pour ce cas. Ainsi, toutes les images sont accentuées.

Pour définir les options d’accentuation par défaut de votre entreprise, sélectionnez Configuration > Configuration de l’application > Configuration de la publication > Image Server. Si vous définissez le mode de ré-échantillonnage par défaut sur Sharp2, l’image est toujours accentuée lorsque la résolution est réduite.

**Ajout de l’accentuation aux paramètres prédéfinis de la visionneuse**

Sauf si vous ajoutez des modificateurs d’accentuation de l’image aux paramètres prédéfinis, la petite image de chargement initial peut paraître floue car sa résolution est réduite sans accentuation pour s’ajuster à la fenêtre de la visionneuse.

Dans Dynamic Media Classic, les paramètres prédéfinis de la visionneuse (tels que les paramètres d’image prédéfinis) vous permettent de centraliser de nombreuses options en un seul emplacement, y compris le choix de l’habillage et les options de la visionneuse (telles qu’un bouton Imprimer ou le contrôle de la vitesse de l’animation de zoom). Les paramètres prédéfinis de la visionneuse se trouvent dans la même section que les paramètres d’image prédéfinis, sous Configuration > Paramètres de l’application > Paramètres prédéfinis de la visionneuse.

Les options des modificateurs se trouvent dans la section des paramètres principaux de tous les paramètres prédéfinis de visionneuse de zoom personnalisés, du catalogue électronique et de rotation. En ajoutant les commandes d’accentuation de l’URL à la boîte de dialogue des modificateurs, vous ajoutez l’accentuation chaque fois que cette visionneuse est appelée avec ce paramètre prédéfini de visionneuse.

Pour appeler le paramètre prédéfini de la visionneuse, utilisez la commande config= dans l’URL de la visionneuse. Voici un exemple de l’appel d’une visionneuse d’images (chaussures) avec un paramètre prédéfini de la visionneuse (FantasticoZoom2009) :

`https://s7d9.scene7.com/s7viewers/html5/ZoomViewer.html?asset=Scene7SharedAssets/ImageSet-Views-Sample&config=S7train/FantasticoZoom2009`

Dans ce cas, les paramètres prédéfinis renforcent et modifient l’habillage par défaut de la visionneuse.

**Création de remplacements selon l’image**

La dernière méthode d’accentuation, et la moins recommandée, consiste à créer des valeurs de remplacement d’accentuation pour chaque image. Cette méthode remplace l’accentuation renforcée via des paramètres prédéfinis avec des valeurs propres spécifiques. Toutefois, cette valeur remplace toutes les autres méthodes d’accentuation pour toutes les tailles. Le meilleur scénario d’utilisation de cette méthode se présente dans le cas où certaines images ne sont pas haute résolution et que les valeurs dans les paramètres d’image prédéfinis sont trop élevées pour ces petites images. Une accentuation au cas par cas peut alors être nécessaire.

Dans Dynamic Media Classic, sélectionnez une image, accédez à la Vue de détails (en cliquant sur le doublon ou en appuyant sur le bouton de Vue des détails), puis cliquez sur Accentuer. Modifiez les paramètres souhaités, puis cliquez sur Enregistrer. Cette option indique au serveur Image Server d’utiliser ces paramètres d’accentuation plutôt que toute autre commande appelée dans l’URL, comme un modificateur d’accentuation ou un paramètre prédéfini. Vous devez publier pour voir l’effet des modifications.
