---
title: Liaison des URL à une application Web
seo-title: Liaison des URL à une application Web
description: 'null'
seo-description: Découvrez comment lier des URL à votre application Web.
uuid: 1179bdd3-9b39-47f9-945d-1c1ca186bf96
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 71299640-676d-49b7-841d-6118f31044e8
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 72%

---


# Liaison des URL à une application Web{#linking-urls-to-your-web-application}

Vos sites Web et applications accèdent au contenu du serveur d’images Dynamic Media au moyen de chaînes URL. Après avoir publié une image, Dynamic Media Classic active une chaîne URL qui référence le paramètre d’image prédéfini sur les serveurs d’images de Contenu multimédia dynamique. Vous pouvez coller ces URL dans un navigateur Web pour procéder à des essais.

Pour placer ces chaînes URL dans vos pages Web et applications, copiez-les à partir de Contenu multimédia dynamique classique. Pour obtenir une chaîne URL générée avec un paramètre d’image prédéfini, atteignez l’écran de prévisualisation ou le panneau de navigation (Affichage des détails).

## Obtention d’une URL de paramètre d’image prédéfini {#obtaining-an-image-preset-url}

Vous pouvez obtenir une chaîne URL générée par un paramètre d’image prédéfini à partir de l’écran Prévisualisation ou Affichage des détails. Une fois l’URL copiée, elle est stockée dans le Presse-papiers ; vous pouvez ainsi la coller si nécessaire.

***Remarque **: L’URL n’est pas principale tant que vous n’avez pas publié le fichier.*

### Obtention d’une URL de paramètre d’image prédéfini depuis l’écran Prévisualisation {#obtaining-an-image-preset-url-from-preview}

1. Dans le panneau Bibliothèque de fichiers situé à gauche, accédez au dossier Fichiers qui contient le fichier d’image à prévisualiser.
1. Utilisez l’une des méthodes suivantes :

   * Au-dessus de la fenêtre Fichiers, dans la partie droite de la barre d’outils, cliquez sur Affichage de la grille. Dans la fenêtre Fichiers, sélectionnez un seul fichier d’image, puis au-dessous de l’image miniature, cliquez sur Prévisualiser > Liste des paramètres prédéfinis de l’image.
   * Au-dessus de la fenêtre Fichiers, dans la partie droite de la barre d’outils, cliquez sur Affichage par liste. Dans la fenêtre Fichiers, sélectionnez un seul fichier d’image, puis sur la droite de l’image miniature, cliquez sur Prévisualiser > Liste des paramètres prédéfinis de l’image.
   * Au-dessus de la fenêtre Fichiers, dans la partie droite de la barre d’outils, cliquez sur Affichage des détails. Sur la même barre d’outils, cliquez sur Prévisualiser > Liste des paramètres prédéfinis de l’image.

1. (Facultatif) Dans la fenêtre Liste des paramètres prédéfinis de l’image, dans la liste déroulante Codage de l’URL pour la génération de copies d’URL située dans la partie inférieure, sélectionnez le codage URL à appliquer à l’URL du fichier d’image lorsqu’il est copié.
1. Dans la fenêtre Liste des paramètres prédéfinis de l’image, située dans l’angle supérieur droit du volet de prévisualisation, cliquez sur Copier l’URL pour le type de paramètre prédéfini sélectionné.
1. Dans le coin inférieur droit de la fenêtre Liste des paramètres prédéfinis de l’image, cliquez sur Fermer pour revenir à l’écran Fichiers.

### Obtention d’une URL de paramètre d’image prédéfini à partir du panneau de navigation {#obtaining-an-image-preset-url-from-the-browse-panel}

1. Dans le panneau Bibliothèque de fichiers situé à gauche, accédez au dossier Fichiers qui contient le fichier d’image à prévisualiser.
1. Au-dessus de la fenêtre Fichiers, dans la partie droite de la barre d’outils, cliquez sur Affichage de la grille. Dans la fenêtre Fichiers, sélectionnez un seul fichier d’image.
1. Au-dessus de la fenêtre Fichiers, dans la partie droite de la barre d’outils, cliquez sur Affichage des détails. 
1. Cliquez sur des URL dans le panneau situé du côté droit de l’écran afin d’afficher la liste des paramètres d’image prédéfinis.
1. Activez le lien Copier l’URL situé en regard du nom du paramètre d’image prédéfini dont vous souhaitez copier l’URL dans le Presse-papiers.

## A propos des chaînes URL de paramètre d’image prédéfini {#about-image-preset-url-strings}

Un appel d’URL pour le dimensionnement d’image sur les serveurs d’images de médias dynamiques a la syntaxe de base suivante :

*chemin*/*nom_serveur_Image_Server*/*nom_compte*/*nom_image*?*modificateur1*&amp;*modificateur2*&amp;…

Dans une URL de serveur d’images de médias dynamiques, les instructions à l’intention du serveur pour l’affichage de l’image s’affichent après le point d’interrogation (?). Par exemple, cet appel d’URL fournit une image nommée « backpack » à une largeur de 250 pixels :

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250
```

Une URL de paramètre d’image prédéfini contient toutes les instructions de modificateur pour présenter l’image conformément aux spécifications de taille et de formatage. Sans paramètre d’image prédéfini, notez toutes les instructions de modificateur après le point d’interrogation (?) dans cette chaîne URL :

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250&fmt=jpeg&qlt=80,0&resMode=sharp&op_usm=1.1,0.5,1,0
```

Toutefois, dans une chaîne URL générée avec un paramètre d’image prédéfini, le nom du paramètre apparaît à la place des instructions définies par ce même paramètre. Par exemple, en prenant pour référence l’URL longue ci-dessus, la chaîne URL se présente comme suit :

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?$Large$
```

Dans les URL, le nom du paramètre d’image prédéfini est compris entre des signes dollar ($). When a Dynamic Media Image Server encounters the Image Preset portion of the URL (the `Large` in this case), using the size and formatting instructions defined by the “Large” Image Preset.

## Ajout d’images dynamiques à une page Web {#adding-dynamic-images-to-your-web-page}

To add dynamic images to your web page, the `<IMG>` tag in your HTML web page code typically is modified using the Dynamic Media Classic URL string to make a request to Dynamic Media Image Servers. Cette chaîne produit l’image conformément aux spécifications de taille et de formatage définies par le paramètre d’image prédéfini.

Par exemple, à la place de l’appel type pour ouvrir une image statique telle que

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

you now use the `<IMG>`tag to replace the reference to a static image with an Image Preset call to the Dynamic Media Classic platform. Exemple d’appel :

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$”
```

In this example, a Dynamic Media Image Server “looks up” the definition of `$thumbnail$` and dynamically generates the appropriate image with the sizing and formatting specifications defined by the `thumbnail`Image Preset. Dans une chaîne URL, tous les éléments, à l’exception du nom de fichier de l’image du produit (dans le cas présent, `backpack_trns`), sont généralement reliés pour le modèle de page. Le seul élément automatiquement inséré dans le modèle de page, à partir de votre serveur commercial, est l’ID du système de traitement de l’information ou le nom de l’image.
