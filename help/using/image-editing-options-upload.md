---
title: Options de réglage fin des images lors du chargement
description: Découvrez les options d’optimisation des images disponibles au moment du chargement dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 2d9fc6d8-973f-4aaa-bc2c-b49cda2cde58
topic: Administration, Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '1200'
ht-degree: 28%

---

# Options de réglage fin des images lors du chargement{#image-editing-options-at-upload}

Lors du téléchargement des fichiers d’image, y compris des fichiers AI, EPS et PSD, vous pouvez effectuer les opérations de retouche suivantes à partir de la boîte de dialogue Télécharger les options de la tâche :

* Recadrez l’espace blanc à partir du bord des images.
* Recadrer manuellement des images par leurs côtés
* Choisir un profil de couleurs
* Créer un masque à partir d’un chemin de tracé
* Accentuer les images grâce aux options de masquage flou
* Masquer l’arrière-plan

Ces options se trouvent sur la page Charger sous l’en-tête **[!UICONTROL Options de modification d’imagerie]**.

## Recadrer l’espace blanc des images

Vous pouvez supprimer automatiquement d’une image les pixels représentant des espaces blancs. Dans la boîte de dialogue Charger les options de la tâche, sélectionnez **[!UICONTROL Options de recadrage]**. Dans la liste déroulante **[!UICONTROL Recadrer]**, choisissez **[!UICONTROL Rogner]**. Ensuite, choisissez les options suivantes :

* **[!UICONTROL Rogner en fonction de]** : dans cette liste déroulante, choisissez de recadrer en fonction de la couleur ou de la transparence :

   * **[!UICONTROL Couleur]** : sélectionnez l’option **[!UICONTROL Couleur]**. Ensuite, dans la liste déroulante **[!UICONTROL Coin]**, sélectionnez l’angle de l’image présentant la couleur qui représente le mieux l’espace blanc à rogner.

   * **[!UICONTROL Transparence]** : sélectionnez l’option Transparence.

* **[!UICONTROL Tolérance]** : faites glisser le curseur pour définir une tolérance comprise entre 0 et 1 :

   * **Rognage en fonction de la couleur** : spécifiez 0 pour rogner les pixels uniquement s’ils correspondent exactement à la couleur que vous avez sélectionnée dans le coin de l’image. Les valeurs qui se rapprochent de 1 admettent un plus grand écart des couleurs.

   * **Rognage en fonction de la transparence** : spécifiez 0 pour rogner les pixels uniquement s’ils sont transparents ; les nombres plus proches de 1 permettent une plus grande transparence.

## Recadrer manuellement sur les côtés des images

Pour recadrer manuellement une image par ses côtés, sélectionnez le menu Recadrer, puis choisissez Manuel. Ensuite, entrez le nombre de pixels à rogner d’un côté ou de chaque côté de l’image. La proportion de l’image qui est rognée dépend du paramètre ppp (pixels par pouce) défini dans le fichier d’image. Supposons, par exemple, que l’image affiche 150 ppp. Ensuite, saisissez 75 dans les zones de texte Haut, Droite, Bas et Gauche. À ce stade, chaque côté est rogné de 0,5 pouce.

## Choisir un profil de couleurs

Pour sélectionner un espace colorimétrique pour l’image, choisissez une option de profil de couleurs :

* **[!UICONTROL Convertir en sRGB]** : permet de convertir le format sRGB (rouge standard, vert, bleu). sRGB est l’espace colorimétrique recommandé pour afficher les images sur les pages web.

* **[!UICONTROL Conserver l’espace colorimétrique d’origine]** : conserve l’espace colorimétrique d’origine.

* **[!UICONTROL Personnaliser à partir de]** > **[!UICONTROL À]** : ouvre les menus afin que vous puissiez choisir un espace colorimétrique Convertir à partir de et Convertir en . Vous pouvez choisir un espace colorimétrique Photoshop standard ou un espace colorimétrique que vous avez téléchargé sur Adobe Dynamic Media Classic.

(voir [Profils ICC](icc-profiles.md#icc_profiles)).

## Création d’un masque à partir d’une trajectoire d’écrêtage

Pour créer un masque pour l’image en fonction des informations de son tracé d’écrêtage, sélectionnez **[!UICONTROL Créer un masque à partir du tracé d’écrêtage]**. Cette option s’applique aux images créées à l’aide d’applications de retouche d’images dans lesquelles un chemin de tracé (ou masque) a été créé.

## Accentuer une image à l’aide de l’option Accentuer le masque

Ce filtre vous permet d’affiner un effet de filtre d’accentuation sur l’image finale sous-échantillonnée. Il permet de contrôler l’intensité de l’effet, le rayon de l’effet (mesuré en pixels) et un seuil de contraste qui est ignoré.

Cet effet utilise les mêmes options que le filtre d’accentuation de Photoshop. Contrairement à ce que suggère le nom, le masquage flou est un filtre d’accentuation.

Sous le masquage flou, définissez les options de votre choix. Les options définies sont décrites dans le tableau suivant :

| Options de masquage flou | Description |
| --- | --- |
| Quantité | L’option Quantité contrôle l’intensité du contraste appliqué aux pixels de contour.<br><br>Considérez cela comme l’intensité de l’effet. Il existe une différence entre les valeurs de quantité de l’accentuation dans Dynamic Media Classic et dans Adobe Photoshop. La principale différence réside dans le fait que Photoshop a une plage de montants comprise entre 1 % et 500 %. En revanche, dans Adobe Dynamic Media Classic, la plage de valeurs est comprise entre 0,0 et 5,0. Une valeur de 5,0 dans Adobe Dynamic Media Classic équivaut approximativement à 500 % dans Photoshop ; une valeur de 0,9 équivaut à 90 %, etc. |
| Rayon | Contrôle le rayon de l’effet. <br><br>La plage de valeurs est comprise entre 0 et 250. L’effet est exécuté sur tous les pixels d’une image et s’étend de tous les pixels dans toutes les directions. Le rayon est mesuré en pixels. Par exemple, pour obtenir un effet d’accentuation similaire pour une image de 2 000 × 2 000 pixels et une image de 500 × 500 pixels, définissez un rayon de deux pixels sur l’image de 2 000 × 2 000 pixels. Définissez ensuite une valeur de rayon d’un pixel sur l’image de 500 × 500 pixels. Utilisez une valeur plus élevée pour une image avec plus de pixels.  |
| Seuil | Le seuil est une plage de contraste qui est ignorée lorsque le filtre de masquage flou est appliqué. Cet effet est important pour qu’aucun « bruit » ne soit introduit dans une image lorsque ce filtre est utilisé. La plage de valeurs est comprise entre 0 et 255, qui est le nombre de degrés de luminosité dans une image en niveaux de gris. 0 = noir, 128 = 50 % gris et 255 = blanc. <br><br>Par exemple, une valeur seuil de 12 ignore les légères variations de luminosité de la peau, afin de ne pas ajouter de bruit, mais ajoute un contraste sur les bords dans les zones contrastées, comme la zone où les cils rencontrent la peau.<br><br>Par exemple, si vous disposez d’une photo du visage d’une personne, l’accentuation affecte les parties contrastées de l’image. Par exemple, où les cils et la peau se rencontrent pour créer une zone de contraste évidente, et la peau lisse elle-même. Même la peau la plus lisse affiche des variations subtiles de ses valeurs de luminosité. Si vous n’utilisez aucune valeur de seuil, le filtre accentue ces changements subtils dans les pixels de la peau. Un effet de bruit indésirable est alors créé lorsque le contraste sur les cils est augmenté, ce qui améliore la netteté.<br><br>Pour éviter ce problème, utilisez une valeur de seuil qui indique au filtre d’ignorer les pixels qui ne modifient pas considérablement le contraste, comme la peau lisse. <br><br>Dans l’image de fermeture éclair présentée précédemment, remarquez la texture en regard des fermetures. Le bruit d’une image est exposé, car les valeurs de seuil sont trop faibles pour supprimer le bruit. |
| Monochrome | Choisissez cette option pour appliquer le masquage flou sur la luminosité de l’image (intensité).<br><br>Désélectionnez-la pour appliquer l’accentuation sur chaque composante de couleur séparément. |

Voir aussi [Accentuer une image](sharpening-image.md#sharpening_an_image).

Voir aussi [Accentuer les images dans Adobe Dynamic Media et sur le serveur d’images](/help/using/assets/s7_sharpening_images.pdf).

## Masquer l’arrière-plan

Utilisez l’arrière-plan du K.O. pour supprimer automatiquement l’arrière-plan d’une image lors de son chargement. Cette technique est utile pour attirer l’attention sur un objet précis et pour le faire ressortir dans un arrière-plan chargé.

| Options de masquage de l’arrière-plan | Description |
| --- | --- |
| Masquer l’arrière-plan | Sélectionnez cette option pour activer la fonction et les options d&#39;arrière-plan de masquage. |
| Coin | Obligatoire.<br>Coin de l’image utilisé pour définir la couleur d’arrière-plan à masquer.<br>Vous pouvez choisir parmi <b>Haut à gauche, Bas à gauche, Haut à droite ou Bas à droite</b>. |
| Méthode de remplissage | Obligatoire. <br>Contrôle la transparence en pixels à partir de l’emplacement d’angle que vous avez défini.<br>Vous pouvez choisir l’une des méthodes de remplissage suivantes :<br>· <b>Remplissage avec inondation</b> : rend transparents tous les pixels qui correspondent au coin que vous avez spécifié et auquel ils sont connectés.<br>· <b>Pixel de correspondance</b> : rend transparents tous les pixels correspondants, quel que soit leur emplacement sur l’image. |
| Tolérance | Facultatif.<br>Contrôle la variation autorisée de la correspondance des couleurs en pixels en fonction de l’emplacement du coin que vous avez défini.<br>Utilisez une valeur de 0,0 pour faire correspondre exactement les couleurs en pixels. Ou utilisez une valeur de 1,0 pour permettre la plus grande variation. |

>[!MORELIKETHIS]
>
>* [Recadrer une image](cropping-image.md#cropping_an_image)
