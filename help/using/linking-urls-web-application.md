---
title: Liaison d’URL à une application web
description: Découvrez comment lier des URL à votre application web à partir d’Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic
role: User
exl-id: ca629427-da33-4bab-9d08-6d9368042f7e
topic: Administration, Content Management, Development
level: Intermediate
autotag-review: '2026-05-13T20:03:48.579Z'
TQID: 'https://experienceleague.adobe.com/c8e722KVmasJVtoVl8k7-5vGjvs4Lm-GZavm-TF9fk0'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 1960799e4144942d4d9443196e6db425f87c7686
workflow-type: tm+mt
source-wordcount: 821
ht-degree: 16%

---

# Liaison d’URL à une application web{#linking-urls-to-your-web-application}

Vos sites web et applications accèdent au contenu du serveur d’images Dynamic Media à l’aide de chaînes URL. Après la publication d’une image, Adobe Dynamic Media Classic active une chaîne d’URL qui fait référence au paramètre prédéfini d’image sur les serveurs d’images Dynamic Media. Vous pouvez utiliser ces URL dans un navigateur web à des fins de test.

Pour placer ces chaînes URL dans vos pages Web et applications, copiez-les depuis Adobe Dynamic Media Classic. Pour obtenir une chaîne d’URL générée avec un paramètre d’image prédéfini, accédez à l’écran de prévisualisation ou au panneau Parcourir (dans la vue Détail).

## Obtention d’une URL de paramètre d’image prédéfini {#obtaining-an-image-preset-url}

Vous pouvez obtenir une chaîne URL générée par un paramètre d’image prédéfini à partir de l’écran Prévisualisation ou Affichage des détails. Une fois l’URL copiée, elle est enregistrée dans le Presse-papiers afin que vous puissiez la coller si nécessaire.

>[!NOTE]
>
>l’URL n’est activée qu’une fois le fichier publié.

### Obtention d’une URL de paramètre d’image prédéfini à partir de l’aperçu {#obtaining-an-image-preset-url-from-preview}

1. Dans le panneau Bibliothèque de ressources sur le côté gauche, accédez au dossier de ressources contenant la ressource d’image à prévisualiser.
1. Effectuez l’une des opérations suivantes :

   * Au-dessus de la fenêtre Assets, dans la partie droite de la barre d’outils, sélectionnez **[!UICONTROL Vue Grille]**. Dans la fenêtre Ressource, sélectionnez une ressource d’image unique, puis, sous l’image miniature, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des paramètres d’image prédéfinis]**.
   * Au-dessus de la fenêtre Assets, dans la partie droite de la barre d’outils, sélectionnez **[!UICONTROL Vue Liste]**. Dans la fenêtre Ressource, sélectionnez une seule ressource image, puis à droite de l’image miniature, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des paramètres d’image prédéfinis]**.
   * Au-dessus de la fenêtre Assets, dans la partie droite de la barre d’outils, sélectionnez **[!UICONTROL Affichage des détails]**. Dans la même barre d’outils, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des paramètres prédéfinis d’image]**.

1. (Facultatif) Dans la liste Préréglage d’image , dans la liste déroulante Codage d’URL pour la génération d’URL de copie , sélectionnez le Codage d’URL à appliquer à l’URL de la ressource d’image lors de sa copie.
1. Dans la fenêtre Liste des paramètres d’image prédéfinis , dans la zone supérieure droite du volet d’aperçu, sélectionnez **[!UICONTROL Copier l’URL]** pour le type de paramètre prédéfini sélectionné.
1. Dans le coin inférieur droit de la fenêtre Liste des paramètres d’image prédéfinis , sélectionnez **[!UICONTROL Fermer]** pour revenir à l’écran Assets.

### Obtention d’une URL de paramètre d’image prédéfini à partir du panneau Parcourir {#obtaining-an-image-preset-url-from-the-browse-panel}

1. Dans le panneau Bibliothèque de ressources sur le côté gauche, accédez au dossier de ressources contenant la ressource d’image à prévisualiser.
1. Au-dessus de la fenêtre Assets, dans la partie droite de la barre d’outils, sélectionnez **[!UICONTROL Vue Grille]**. Dans la fenêtre Fichiers, sélectionnez un seul fichier d’image.
1. Au-dessus de la fenêtre Assets, dans la partie droite de la barre d’outils, sélectionnez **[!UICONTROL Affichage des détails]**.
1. Sélectionnez **[!UICONTROL URL]** dans le panneau de droite pour afficher la liste des paramètres d’image prédéfinis.
1. Sélectionnez le lien **[!UICONTROL Copier l’URL]** en regard du nom du paramètre d’image prédéfini avec l’URL à copier dans le Presse-papiers.

## Présentation des chaînes URL de paramètre d’image prédéfini {#about-image-preset-url-strings}

Un appel URL pour le dimensionnement d’image sur les serveurs d’images Dynamic Media présente la syntaxe de base suivante :

*chemin*/*nom du serveur d’images*/*nom du compte*/*nom de l’image*?*modificateur1*&amp;*modificateur2*&amp;...

Dans une URL de serveur d’images Dynamic Media, les instructions données au serveur pour afficher l’image suivent le point d’interrogation (?). Par exemple, cet appel d’URL renvoie une image nommée « sac à dos » avec une largeur de 250 pixels :

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250
```

Une URL de paramètre d’image prédéfini contient toutes les instructions de modificateur pour présenter l’image conformément aux spécifications de taille et de formatage. Sans paramètre d’image prédéfini, notez toutes les instructions de modification après le point d’interrogation (?) dans cette chaîne URL :

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250&fmt=jpeg&qlt=80,0&resMode=sharp&op_usm=1.1,0.5,1,0
```

Cependant, dans une chaîne d’URL générée avec un paramètre d’image prédéfini, le nom du paramètre d’image prédéfini remplace les instructions définies par le paramètre d’image prédéfini. Par exemple, en prenant pour référence l’URL longue ci-dessus, la chaîne URL se présente comme suit :

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?$Large$
```

Les noms des paramètres d’image prédéfinis dans les URL utilisent des signes dollar ($). Lorsqu’un serveur d’images Dynamic Media traite la partie du paramètre d’image prédéfini de l’URL (le `Large` dans ce cas), il utilise les instructions de taille et de formatage définies par le paramètre d’image prédéfini « Grand ».

## Ajout d’images dynamiques à une page web {#adding-dynamic-images-to-your-web-page}

Lors de l’ajout d’images dynamiques à vos pages web, la balise `<IMG>` est généralement modifiée à l’aide de la chaîne d’URL Adobe Dynamic Media Classic pour demander des images aux serveurs d’images Dynamic Media. Cette chaîne produit l’image conformément aux spécifications de taille et de formatage définies par le paramètre d’image prédéfini.

Par exemple, à la place de l’appel type pour ouvrir une image statique telle que

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

Vous utilisez maintenant la balise `<IMG>` pour remplacer la référence à une image statique par un appel de paramètre d’image prédéfini à la plateforme Adobe Dynamic Media Classic. Exemple d’appel :

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$"
```

Dans cet exemple, un serveur d’images Dynamic Media récupère la définition de `$thumbnail$` et génère dynamiquement l’image appropriée avec les spécifications de dimensionnement et de formatage définies par le paramètre prédéfini d’image `thumbnail`. Dans une chaîne d’URL, tous les éléments à l’exception du nom de fichier de l’image du produit ( `backpack_trns` dans ce cas) sont généralement configurés pour le modèle de page. Le seul élément automatiquement inséré dans le modèle de page, à partir de votre serveur commercial, est l’ID du système de traitement de l’information ou le nom de l’image.
