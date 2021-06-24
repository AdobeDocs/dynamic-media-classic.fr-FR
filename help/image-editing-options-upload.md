---
title: Options d’édition d’images au téléchargement
description: Découvrez les options d’édition d’image disponibles au moment du téléchargement.
uuid: 0912ae6f-41c9-41b5-94d1-e266face782e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: d3f21cdf-2cb3-46e8-955a-b8daf0b233bc
feature: Dynamic Media Classic,Gestion des ressources
role: Business Practitioner
exl-id: 2d9fc6d8-973f-4aaa-bc2c-b49cda2cde58
source-git-commit: 06bd65c92c88595786b14213944a7cebd0d2590b
workflow-type: tm+mt
source-wordcount: '1160'
ht-degree: 59%

---

# Options d’édition d’images au téléchargement{#image-editing-options-at-upload}

Lors du téléchargement des fichiers d’image, y compris des fichiers AI, EPS et PSD, vous pouvez effectuer les opérations de retouche suivantes à partir de la boîte de dialogue Télécharger les options de la tâche :

* Rogner l’espace blanc du contour des images
* Recadrer manuellement des images par leurs côtés
* Choisir un profil de couleurs
* Créer un masque à partir d’un chemin de tracé
* Accentuer les images grâce aux options de masquage flou
* Masquer l’arrière-plan

Ces options se trouvent sur la page Télécharger, sous Options d’édition d’image.

## Suppression de l’espace blanc des images

Pour recadrer automatiquement les pixels d’espace blanc d’une image, dans la boîte de dialogue Télécharger les options de la tâche, cliquez sur **[!UICONTROL Options de recadrage]**. Dans la liste déroulante **[!UICONTROL Recadrer]**, sélectionnez **[!UICONTROL Rogner]**. Ensuite, choisissez les options suivantes :

* **Rogner en fonction de**  : dans cette liste déroulante, choisissez si vous souhaitez recadrer en fonction de la couleur ou de la transparence :

   * **Couleur**  : choisissez l’option  **** Couleur. Ensuite, dans la liste déroulante **[!UICONTROL Coin]** , sélectionnez l’angle de l’image dont la couleur représente le mieux l’espace blanc que vous souhaitez recadrer.

   * **Transparence**  : sélectionnez l’option Transparence.

* **Tolérance**  : faites glisser le curseur pour spécifier une tolérance comprise entre 0 et 1 :

   * **Rognage en fonction de la couleur**  : indiquez 0 pour rogner les pixels uniquement s’ils correspondent exactement à la couleur sélectionnée dans le coin de l’image. Les valeurs qui se rapprochent de 1 admettent un plus grand écart des couleurs.

   * **Rognage en fonction de la transparence**  : spécifiez 0 pour rogner les pixels uniquement s’ils sont transparents. Les valeurs plus proches de 1 permettent une plus grande transparence.

## Recadrage manuel à partir des côtés d’une image

Pour recadrer manuellement une image par ses côtés, sélectionnez le menu Recadrer, puis choisissez Manuel. Ensuite, entrez le nombre de pixels à rogner d’un côté ou de chaque côté de l’image. La proportion de l’image qui est rognée dépend du paramètre ppp (pixels par pouce) défini dans le fichier d’image. Par exemple, si l’image affiche 150 ppp et que vous entrez 75 dans les zones de texte pour les bords supérieur, droit, inférieur et gauche, un demi-pouce est rogné de chaque côté.

## Choix d’un profil colorimétrique

Pour sélectionner un espace colorimétrique pour l’image, choisissez l’option Profil de couleurs :

* **Convertir en sRVB**  : convertit en sRVB (rouge vert bleu standard). sRVB est l’espace colorimétrique recommandé pour l’affichage d’images sur les pages Web.

* **Conserver l’espace colorimétrique d’origine**  : conserve l’espace colorimétrique d’origine.

* **Personnaliser de > à**  : ouvre les menus afin que vous puissiez sélectionner un espace colorimétrique Convertir de et Convertir en. Vous pouvez choisir un espace colorimétrique Photoshop standard ou un espace colorimétrique que vous avez chargé dans Dynamic Media Classic.

(voir [Profils ICC](icc-profiles.md#icc_profiles)).

## Création d’un masque à partir d’un chemin de tracé

Pour créer un masque pour l’image en fonction des informations de son chemin de détourage, cliquez sur **[!UICONTROL Créer un masque à partir du chemin de détourage]**. Cette option s’applique aux images créées à l’aide d’applications de retouche d’images dans lesquelles un chemin de tracé (ou masque) a été créé.

## Accentuation d’une image à l’aide d’un masquage flou

Ce filtre permet d’affiner l’effet d’un filtre d’accentuation sur l’image finale à résolution réduite. Il permet de contrôler l’intensité de l’effet, le rayon de l’effet (mesuré en pixels) et un seuil de contraste qui est ignoré.

Cet effet utilise les mêmes options que le filtre de masquage flou de Photoshop. Contrairement à ce que suggère le nom, le masquage flou est un filtre d’accentuation.

Sous le masquage flou, définissez les options de votre choix. Les options définies sont décrites dans le tableau suivant :

| Options de masquage flou | Description |
|--- |--- |
| Quantité | Contrôle le degré de contraste appliqué aux pixels de contour.<br><br>Considérez ceci comme l’intensité de l’effet. La principale différence entre les valeurs de quantité du masquage flou dans Dynamic Media Classic et les valeurs de quantité dans Adobe Photoshop, est que Photoshop a une plage de quantité comprise entre 1 % et 500 %. En revanche, dans Dynamic Media Classic, la plage de valeurs est comprise entre 0,0 et 5,0. Une valeur de 5,0 dans Dynamic Media Classic est l’équivalent approximatif de 500 % dans Photoshop ; une valeur de 0,9 équivaut à 90 %, etc. |
| Rayon | Contrôle le rayon de l’effet. <br><br>La plage de valeurs varie entre 0 et 250. L’effet est exécuté sur tous les pixels d’une image et s’étend de tous les pixels dans toutes les directions. Le rayon est mesuré en pixels. Par exemple, pour obtenir un effet d’accentuation similaire pour une image de 2 000 x 2 000 pixels et une image de 500 x 500 pixels, définissez un rayon de deux pixels sur l’image de 2 000 x 2 000 pixels. Définissez ensuite une valeur de rayon d’un pixel sur l’image de 500 x 500 pixels. Utilisez une valeur plus élevée pour une image avec plus de pixels.  |
| Seuil | Le seuil est une plage de contraste qui est ignorée lorsque le filtre de masquage flou est appliqué. Cet effet est important, de sorte qu’aucun &quot;bruit&quot; n’est introduit dans une image lorsque ce filtre est utilisé. La plage de valeurs est comprise entre 0 et 255, qui est le nombre de degrés de luminosité dans une image en niveaux de gris. 0 = noir, 128 = 50 % gris et 255 = blanc. <br><br>Par exemple, une valeur de seuil de 12 ignore les légères variations de luminosité de la peau, afin de ne pas ajouter de bruit, tout en ajoutant un contraste sur les bords dans les zones contrastées, comme la zone où les cils rencontrent la peau.<br><br>Si, par exemple, vous disposez d’une photo du visage d’une personne, le masquage flou affecte les parties contrastées de l’image. Par exemple, où les cils et la peau se rencontrent pour créer une zone de contraste évidente, et la peau lisse elle-même. Même la peau la plus lisse affiche des variations subtiles de ses valeurs de luminosité. Si vous n’utilisez aucune valeur de seuil, le filtre accentue ces changements subtils dans les pixels de la peau. Un effet de bruit indésirable est alors créé lorsque le contraste sur les cils est augmenté, ce qui améliore la netteté.<br><br>Pour l’éviter, utilisez une valeur de seuil qui indique au filtre d’ignorer les pixels qui ne modifient pas considérablement le contraste, comme la peau lisse. <br><br>Dans l’image de fermeture éclair présentée plus haut, remarquez la texture en regard des fermetures. Le bruit d’une image est exposé car les valeurs de seuil étaient trop faibles pour supprimer le bruit. |
| Monochrome | Choisissez cette option pour appliquer le masquage flou sur la luminosité de l’image (intensité).<br><br>Désélectionnez-la pour appliquer le masquage flou séparément sur chaque composante de couleur. |

Voir aussi [Accentuation d’une image](sharpening-image.md#sharpening_an_image).

Voir aussi [Accentuation des images dans Scene7 Publishing System et sur le serveur d’images](/help/assets/s7_sharpening_images.pdf).

## Masquer l’arrière-plan

Utilisez l’option Masquer l’arrière-plan pour supprimer automatiquement l’arrière-plan d’une image lorsque vous la transférez. Cette technique est utile pour attirer l’attention sur un objet précis et pour le faire ressortir dans un arrière-plan chargé.

| Options de masquage de l’arrière-plan | Description |
|:--- |:--- |
| Masquer l’arrière-plan | Sélectionnez cette option pour activer la fonction et les options Masquer l’arrière-plan. |
| Coin | Obligatoire.<br><br>Coin de l’image servant à définir la couleur d’arrière-plan à masquer.<br><br>Choisissez <b>Supérieur gauche, Bas et gauche, Supérieur droit ou Bas et droite</b>. |
| Méthode de remplissage | Obligatoire. <br><br>Contrôle la transparence des pixels à partir du coin que vous avez défini.<br><br>Vous pouvez choisir parmi les méthodes de remplissage suivantes : <ul><li><b>Remplissage par diffusion</b> - Rend tous les pixels transparents qui correspondent au coin que vous avez spécifié et qui y sont rattachés.</li><li><b>Correspondance des pixels</b> - Rend tous les pixels correspondants transparents, quel que soit leur emplacement dans l’image.</li></ul> |
| Tolérance | Facultatif.<br><br>Contrôle le degré de variation autorisé dans la couleur des pixels correspondante d’après l’emplacement du coin que vous avez défini.<br><br>Utilisez une valeur de 0,0 pour correspondre exactement aux couleurs de pixels ou utilisez une valeur de 1,0 pour permettre une plus grande variation. |

>[!MORELIKETHIS]
>
>* [Recadrage d’une image](cropping-image.md#cropping_an_image)

