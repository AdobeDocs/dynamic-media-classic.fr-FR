---
title: Accentuation d’une image
description: Découvrez comment accentuer une image dans Adobe Dynamic Media Classic.
uuid: d86af74a-89c5-4f2b-96ba-f2e7da600bca
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 11cd5362-d90a-4c1e-bfbd-46a65a554409
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 4b3e8368-f8f5-46d9-9130-361a8273de2c
source-git-commit: 352b1c383195fa03294ad3501207d63f3cfe3e42
workflow-type: tm+mt
source-wordcount: '2276'
ht-degree: 42%

---

# Accentuation d’une image {#sharpening-an-image}

L’accentuation est une technique de manipulation d’image qui rend plus nets les contours d’une image numérique. L’accentuation consiste à augmenter le contraste entre les pixels de contour, et ainsi à souligner la transition entre les zones sombres et les zones claires. L’accentuation augmente le contraste local et fait ressortir les détails infimes. Il n’existe pas de formule magique pour accentuer correctement toutes les images. Une accentuation trop faible produit une image douce, tandis qu’une accentuation exagérée crée des halos, des artefacts et du bruit.

Adobe Dynamic Media Classic recommande vivement d’utiliser des paramètres d’image prédéfinis pour toutes les images. Elles garantissent une taille uniforme et l’accentuation est appliquée sur toute image appelée avec un paramètre d’image prédéfini. De plus, vous pouvez facilement modifier et modifier les paramètres d’accentuation d’un paramètre d’image prédéfini. A la prochaine publication, toutes les images appelées avec ces paramètres prédéfinis se voient appliquer les nouvelles valeurs.

Adobe Dynamic Media Classic recommande également d’ajouter de l’accentuation aux paramètres prédéfinis de la visionneuse, puis d’appeler une visionneuse avec ce paramètre prédéfini. Cela permet de s’assurer que les images de vos visionneuses sont crise et attrayantes.

Cependant, que vous utilisiez les paramètres d’image prédéfinis et les paramètres de visionneuse prédéfinis, ou une autre méthode d’accentuation, l’essentiel est que vous devez accentuer vos images. Si ce n’est pas le cas, vos images (et votre site web) peuvent sembler douces et floues.

>[!NOTE]
>
>les commandes d’accentuation remplacent les paramètres d’image prédéfinis, notamment les effets d’accentuation. Un paramètre d’image prédéfini détermine la taille et le formatage avec lesquels les images sont diffusées à partir des serveurs d’images Dynamic Media. Adobe Dynamic Media Classic recommande vivement d’utiliser des paramètres d’image prédéfinis pour diffuser toutes les images afin de s’assurer que leur taille et leur accentuation sont uniformes. Cependant, après avoir modifié les paramètres d’accentuation d’une image individuelle, les paramètres d’image prédéfinis relatifs à l’accentuation ne s’appliquent plus à l’image. Elle est diffusée sans ces paramètres.

Il est souvent nécessaire d’accentuer les images. Adobe Dynamic Media Classic et les serveurs d’images offrent plusieurs options d’accentuation. Il est important de comprendre l’impact de l’accentuation sur une image et le degré d’accentuation dont vous avez besoin. La plupart des images ont besoin d’accentuation mais le degré nécessaire dépend de l’image.

L’accentuation de l’image augmente le contraste des pixels pour créer un effet de contours renforcés. Ce contraste amélioré des bords est perçu par les yeux comme de la netteté. S’il est facile d’améliorer une image à l’aide de filtres d’accentuation, il est également facile de trop renforcer la netteté d’une image,

ce qui crée alors un effet de halo ou de bande sur les lignes de la bordure.

Il existe des bonnes pratiques que vous pouvez suivre pour optimiser l’accentuation de vos images dans Adobe Dynamic Media Classic et sur Dynamic Media Image Server.

Voir [Bonnes pratiques relatives à l’accentuation des images dans Adobe Dynamic Media Classic et sur Dynamic Media Image Server](/help/assets/s7_sharpening_images.pdf).

Voir également la [vidéo de formation à l’accentuation](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/547_sharpening1_converted%20renamed_Done-AVS).

**Pour accentuer une image:**

Pour accentuer une image, cliquez sur son bouton de survol **[!UICONTROL Modifier]** et choisissez **[!UICONTROL Accentuer]**, ou ouvrez-le dans le panneau de navigation de la vue Détails, puis sélectionnez **[!UICONTROL Accentuer]**. La page Éditeur d’accentuation s’ouvre avec des commandes d’accentuation. Choisissez des commandes, puis sélectionnez **[!UICONTROL Enregistrer]**.

>[!NOTE]
>
>Avant d’accentuer une image, vous pouvez sélectionner le menu Appliquer les paramètres prédéfinis et choisir un paramètre d’image prédéfini pour en découvrir les effets. Les effets d’accentuation d’un paramètre d’image prédéfini conviennent à votre image. Le menu **[!UICONTROL Appliquer les paramètres prédéfinis]** se trouve au bas de la page Éditeur de netteté.

**Options d’accentuation**

Le tableau suivant présente les options d’accentuation du serveur Image Server.

| Nom | Protocole d’URL | Valeurs | Exemple |
| --- | --- | --- | --- |
| Accentuation simple | `op_sharpen` | `0` ou `1` | `op_sharpen=1` |
| Mode de ré-échantillonnage | `resMode` | `bilin`,  `bicub`,  `sharp2`,  `trilin`<br><br>`bilin`: Sélection de l’interpolation binaire standard. méthode de rééchantillonnage la plus rapide; certains artefacts de crénelage sont souvent visibles.<br>`bicub`: Sélectionne l’interpolation bicubique. Bien qu’elle sollicite davantage le processeur que bilin, cette méthode produit des images plus nettes avec des artefacts de crénelage plus discrets.<br><br>`sharp2`: Sélectionne une fonction Lanczos Windows® modifiée comme algorithme d’interpolation. Peut produire des résultats légèrement plus nets que le bi-cube à un coût CPU plus élevé.<br><br>`trilin` : sélectionne une interpolation trilinéaire modifiée qui utilise les deux résolutions supérieure et inférieure lorsqu’elles sont disponibles. Méthode recommandée si le crénelage devient problématique. Elle réduit la taille des fichiers JPEG en raison des données à haute fréquence réduites. | `resMode=sharp2` |
| Masquage flou | `op_usm` | `amount`,  `radius`,  `threshold`,  `monochrome`<br><br>`amount`: facteur de force du filtre (réel 0...5) <br><br>`radius`: rayon du noyau du filtre en pixels (réel 0...250)  <br><br>`threshold`: seuil de filtrage (int 0...255)<br><br>`monochrome` : défini sur  `0` pour masquer séparément chaque composant de couleur, défini sur  `1` pour masquer l’accentuation de la luminosité de l’image (intensité) | `op_usm=1,1,10,0` |

Sélectionnez le menu **[!UICONTROL Accentuation]** et choisissez une option :

* **Aucun**  : désactive l’accentuation.

* **Accentuer**  : exécute une simple transmission d’accentuation sur le fichier après son redimensionnement. Il est similaire au filtre &quot;Accentuer&quot; dans Adobe Photoshop et prend en charge tous les paramètres utilisateur. Normalement, vous utiliseriez ce filtre ou **[!UICONTROL Masquage flou]**, mais pas les deux. Cette méthode n’est pas recommandée comme meilleure pratique, mais elle permet de compenser le flou. (URL: `op_sharpen`)

* **Masquage flou**  : permet d’affiner l’effet d’un filtre d’accentuation sur l’image finale à résolution réduite. Vous pouvez contrôler l’intensité de l’effet, son rayon (mesuré en pixels) et un seuil de contraste qui est ignoré. Cet effet utilise les mêmes options que le filtre de masquage flou de Photoshop. (URL : `op_usm`)

Sélectionnez ces options afin d’affiner l’accentuation à l’aide du masquage flou :

* **Quantité**  : contrôle le degré de contraste appliqué aux pixels de contour. La valeur par défaut est de 0. Pour des images à haute résolution, vous pouvez l’augmenter jusqu’à 5. Imaginez la quantité comme étant l’unité de mesure de l’intensité du filtre. Le paramètre **[!UICONTROL Amount]** dans Adobe Dynamic Media Classic n’est pas le même que le paramètre Amount dans Adobe Photoshop. Adobe Photoshop utilise un montant compris entre 1 et 500 %, tandis qu’Adobe Dynamic Media Classic le met à l’échelle de 0,0 à 5,0. (La valeur 5 est environ équivalente à 500 % dans Photoshop, 0,9 à 90 %, et ainsi de suite.)

* **Rayon**  : détermine le nombre de pixels entourant les pixels de contour qui affectent l’accentuation. L’effet est exécuté sur tous les pixels de l’image et s’étend dans toutes les directions. 

La valeur appropriée du rayon dépend de la taille de l’image. Une valeur faible n’accentue que les pixels de contour. Une valeur élevée accentue une marge de pixels plus large. 

Par exemple, pour obtenir un effet d’accentuation similaire pour une image de 2 000 x 2 000 pixels et une image de 500 x 500 pixels, vous pouvez définir une valeur de rayon de deux pixels sur l’image de 2 000 x 2 000 pixels. Ensuite, définissez une valeur de rayon d’un pixel pour l’image de 500 x 500 pixels (définissez une valeur plus élevée pour une image contenant plus de pixels).

* **Seuil**  : détermine la plage de contraste à ignorer lorsque le filtre de masquage flou est appliqué. Cette option définit l’écart recherché entre les pixels et la zone environnante avant qu’ils ne soient considérés comme des pixels de contour et ne soient accentués. 

Le seuil utilise une valeur comprise entre 0 et 255, qui est le nombre d’étapes de luminosité dans une image en niveaux de gris. 0 = noir, 128 = 50 % gris et 255 = blanc. Par exemple, une valeur de seuil de 12 ignore les légères variations de luminosité de la peau, afin de ne pas ajouter de bruit, tout en ajoutant un contraste sur les bords dans les zones contrastées, comme la zone où les cils rencontrent la peau. 

Par exemple, supposons que vous ayez une photo d’un visage. Le masquage flou accentue les parties de l’image les plus contrastées et la peau lisse. Même la peau la plus lisse affiche des variations subtiles de ses valeurs de luminosité. Si vous n’utilisez pas une valeur de seuil, le filtre accentue ces légères variations dans les pixels de la peau, créant ainsi un effet de bruit (probablement indésirable), tout en augmentant le contraste sur les cils, ce qui améliore la netteté (probablement souhaitable). Pour l’éviter, utilisez une valeur de seuil qui indique au filtre d’ignorer les pixels qui ne modifient pas considérablement le contraste, comme la peau lisse. Pour éviter d’introduire du bruit ou des images de postérisation avec des tons chair, par exemple, essayez d’essayer avec les valeurs **[!UICONTROL Seuil]** comprises entre 2 et 20. La valeur par défaut **[!UICONTROL Seuil]** de 0 accentue tous les pixels de l’image.

* **Appliquer à**  : sélectionnez  **[!UICONTROL chaque]** couleur pour appliquer l’accentuation séparément à chaque composant de couleur. choisissez  **** Luminosité si vous souhaitez appliquer l’accentuation aux zones de luminosité de l’image.

**Ré-échantillonnage**

Sélectionnez le menu **[!UICONTROL Rééchantillonnage]** et choisissez une option. Les options suivantes permettent d’accentuer l’image lorsque sa résolution est réduite :

* **[!UICONTROL Aucun]**  : désactive le rééchantillonnage.

* **[!UICONTROL Bilinéaire]**  : méthode de rééchantillonnage la plus rapide. certains artefacts de crénelage sont visibles.

* **[!UICONTROL Bicubique]**  : accroît l’utilisation du processeur sur le serveur d’images, mais produit des images plus nettes avec des artefacts de crénelage plus discrets.

* **[!UICONTROL Accentuer]**  2 : produit des résultats légèrement plus nets que  **[!UICONTROL Bicubique]**, mais avec un coût de processeur encore plus élevé sur le serveur d’images.

* **[!UICONTROL Trilinéaire]**  : utilise des résolutions plus élevées et plus basses si elles sont disponibles ; recommandé uniquement lorsque le crénelage est un problème. Elle réduit la taille du fichier JPEG en raison des données à haute fréquence réduites.

**Accentuation et paramètres d’image prédéfinis**

Vous pouvez incorporer les trois effets d’accentuation pour obtenir votre résultat final. Cependant, cette méthode n’est pas recommandée. Adobe Dynamic Media Classic vous recommande d’enregistrer vos effets d’accentuation dans le cadre d’un paramètre d’image prédéfini. Les paramètres d’image prédéfinis vous permettent de regrouper les modificateurs d’image les plus souvent utilisés afin de créer une image redimensionnée dynamiquement dans une petite chaîne de texte. Un paramètre d’image prédéfini contient des valeurs pour le format de fichier (généralement JPEG pour le web), le nombre de pixels et l’accentuation de l’image. Au lieu d’ajouter l’URL à chaque modificateur d’image que vous devez utiliser pour créer un type spécifique de taille d’image, créez un paramètre d’image prédéfini nommé, tel que &quot;miniature&quot;. Ensuite, configurez le paramètre prédéfini d’image miniature avec la taille, le format de fichier et les options d’accentuation appropriés. Appelez l’image à l’aide du nom du paramètre d’image prédéfini. Les paramètres d’image prédéfinis raccourcissent la longueur de l’URL globale. Ces deux URL produisent la même image de JPEG 350x350 avec accentuation :

* `https://sample.scene7.com/is/image/S7train/Backpack_A?wid=350&hei=350&fmt=jpeg&qlt=85,0&resMode=sharp2&op_usm=0.9,1.0,8,0`
* `https://sample.scene7.com/is/image/S7train/Backpack_A?$!_s7product$`

Les paramètres d’image prédéfinis peuvent être modifiés et mis à jour à tout moment. Vous voyez les résultats d’une modification d’un paramètre d’image prédéfini après la publication et une fois que le cache de l’URL est effacé.

Si vous utilisez un paramètre prédéfini pour chaque image dans une catégorie de taille, tout administrateur d’entreprise peut mettre à jour ce paramètre d’image prédéfini, republier et affecter toutes les images qui utilisent ce format, sans aucune modification du code du site Web. En règle générale, utilisez un paramètre d’image prédéfini par taille unique sur votre site. Pour ajouter un paramètre d’image prédéfini, dans la barre de navigation globale, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Paramètres de l’application]** > **[!UICONTROL Paramètres d’image prédéfinis]**. Sélectionnez ensuite **[!UICONTROL Ajouter]** ou **[!UICONTROL Modifier]** pour modifier un paramètre prédéfini existant. Le seul champ obligatoire est le nom du paramètre prédéfini lui-même. Cependant, il est préférable d’inclure un certain niveau d’accentuation dans chaque paramètre prédéfini.

**Qualité JPG**

Les options de qualité JPG contrôlent le niveau de compression JPG :

* **Qualité du JPG**  : sélectionnez cette option si vous souhaitez contrôler les niveaux de compression et le sous-échantillonnage de chrominance.

* **Curseur**  : détermine le niveau de compression du JPG. Ce paramètre affecte à la fois la taille du fichier et la qualité de l’image. L’échelle de qualité du JPG est de 1 à 100.

* **Activer le sous-échantillonnage de la chrominance du JPG**  : comme l’oeil est moins sensible aux informations colorimétriques à haute fréquence qu’à la luminance à haute fréquence, les images du JPEG divisent les informations d’image en composantes de luminance et de couleur. Lorsqu’une image JPEG est compressée, la composante de luminance conserve sa pleine résolution, tandis que les composantes de couleur sont sous-échantillonnées par interpolation, c’est-à-dire le calcul de la moyenne de groupes de pixels. La réduction de résolution (sous-échantillonnage) réduit de moitié ou d’un tiers le volume de données, quasiment sans nuire à la qualité perceptible par l’œil humain. La réduction de résolution ne s’applique pas aux images en niveaux de gris. Cette technique réduit le niveau de compression nécessaire pour les images présentant un contraste élevé (par exemple, les images contenant du texte superposé).

**Définition des options d’accentuation à l’échelle de l’entreprise**

Sans paramètre d’image prédéfini ou de protocole d’accentuation spécifique au serveur Image Server en plus de la chaîne de l’URL, votre image n’est pas accentuée lorsque sa résolution est réduite. Cependant, si cette absence d’accentuation se produit, vous pouvez définir des valeurs d’accentuation par défaut, puis n’importe quelle image est toujours accentuée.

Pour définir les options d’accentuation par défaut de votre entreprise, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Configuration de la publication]** > **[!UICONTROL Serveur d’images]**. Si vous définissez le mode Rééchantillonnage par défaut sur **[!UICONTROL Sharp2]**, l’image est toujours accentuée lors du sous-échantillonnage.

**Ajout de l’accentuation aux paramètres prédéfinis de la visionneuse**

Sauf si vous ajoutez des modificateurs d’accentuation de l’image aux paramètres prédéfinis, la petite image de chargement initial peut paraître floue car sa résolution est réduite sans accentuation pour s’ajuster à la fenêtre de la visionneuse.

Les paramètres prédéfinis de la visionneuse (tels que les paramètres d’image prédéfinis) vous permettent de centraliser de nombreuses options à un seul emplacement, y compris le choix de l’habillage et les options de la visionneuse (comme un bouton Imprimer ou le contrôle de la vitesse de l’animation du zoom). Les paramètres de visionneuse prédéfinis se trouvent dans la même section que les paramètres d’image prédéfinis, sous **[!UICONTROL Configuration]** > **[!UICONTROL Paramètres de l’application]** > **[!UICONTROL Paramètres prédéfinis de la visionneuse]**.

Voir la vidéo de formation [Paramètres prédéfinis de la visionneuse](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS).

Les options des modificateurs se trouvent dans la section des paramètres principaux de tous les paramètres prédéfinis de visionneuse de zoom personnalisés, du catalogue électronique et de rotation. En ajoutant les commandes d’accentuation de l’URL à la boîte de dialogue des modificateurs, vous ajoutez l’accentuation chaque fois que cette visionneuse est appelée avec ce paramètre prédéfini de visionneuse.

Pour appeler le paramètre prédéfini de la visionneuse, utilisez la commande `config=` sur l’URL de la visionneuse. Voici un exemple de l’appel d’une visionneuse d’images (chaussures) avec un paramètre prédéfini de la visionneuse (`FantasticoZoom2022`):

`https://s7d9.scene7.com/s7viewers/html5/ZoomViewer.html?asset=Scene7SharedAssets/ImageSet-Views-Sample&config=S7train/FantasticoZoom2022`

Dans ce cas, les paramètres prédéfinis renforcent et modifient l’habillage par défaut de la visionneuse.

**Création de remplacements spécifiques à une image**

La dernière méthode d’accentuation, et la moins recommandée, consiste à créer des valeurs de remplacement d’accentuation pour chaque image. Cette méthode remplace l’accentuation dans un paramètre d’image prédéfini par ses propres valeurs spécifiques. Cependant, cette méthode remplace également toutes les autres méthodes d’accentuation à n’importe quelle taille. Le meilleur scénario d’utilisation de cette méthode se présente dans le cas où certaines images ne sont pas haute résolution et que les valeurs dans les paramètres d’image prédéfinis sont trop élevées pour ces petites images. Dans ce cas, une accentuation par image est peut-être nécessaire.

Dans Adobe Dynamic Media Classic, sélectionnez une image, accédez à la vue Détails (en double-cliquant ou en appuyant sur le bouton **[!UICONTROL Affichage des détails]**), puis sélectionnez **[!UICONTROL Accentuer]**. Modifiez n’importe quel paramètre, puis sélectionnez **[!UICONTROL Enregistrer]**. Ce processus demande au serveur d’images d’utiliser ces paramètres d’accentuation plutôt que toute commande appelée dans l’URL, comme un modificateur d’accentuation ou un paramètre d’image prédéfini. Veillez à publier pour que les modifications prennent effet.
