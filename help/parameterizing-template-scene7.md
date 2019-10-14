---
title: Paramétrage d’un modèle dans Dynamic Media Classic
seo-title: Paramétrage d’un modèle dans Dynamic Media Classic
description: 'null'
seo-description: Découvrez comment paramétrer un modèle dans Dynamic Media Classic
uuid: 27c8c8b4-47f3-4270-a6db-d304648ba357
contentOwner: admin
content-type: référence
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template-publishing
discoiquuid: df1a9ff5-a5ba-4480-ba0d-a19bc665f907
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Paramétrage d’un modèle dans Dynamic Media Classic{#parameterizing-a-template-in-scene}

Après avoir téléchargé un modèle Illustrator que vous avez enregistré au format FXG Dynamic Media Classic vers Scene7 Publishing System, vous pouvez définir ses éléments variables. Pour ce faire, paramétrez les éléments variables dans les écrans de création et de prévisualisation du module de publication à l’aide de modèles prédéfinis. Dynamic Media Classic propose des outils permettant de définir des paramètres de texte et d’objet sur les calques et leurs propriétés respectives. Vous pouvez également créer différentes versions d’un même modèle.

Le paramétrage d’un modèle FXG vous permet de personnaliser la variabilité du texte, des images et des graphiques dans le modèle. Par exemple, vous pouvez paramétrer une ligne de texte pour que les utilisateurs finals puissent modifier le texte via une interface Web. Vous pouvez définir des zones de texte vides en tant que variables pour que les utilisateurs finals puissent les remplir avec du texte personnalisé. Vous pouvez également paramétrer les attributs et les propriétés des éléments de conception dans l’écran Dynamic Media Classic Template Publishing Build.

>[!NOTE]
>
>Le paramétrage du modèle dans Dynamic Media Classic n’est pas obligatoire si vous prévoyez d’utiliser la manipulation DOM.

## Définition des paramètres d’un modèle FXG {#defining-parameters-in-fxg-templates}

Pour définir les paramètres d’un modèle FXG, procédez comme suit dans Dynamic Media Classic :

1. Sélectionnez le fichier FXG dans la fenêtre de navigation.
1. Click **Build** and choose **Template Publishing**, or click the file’s **Edit** button.

   L’écran Module de publication à l’aide de modèles prédéfinis s’ouvre. 

1. Sélectionnez LRCo\FXG\Welcome_Summit_10 (fichier FXG) et cliquez sur **Créer** &gt; Publication de **modèles**.</p>

   ![](assets/wp_fxg_edit.png)

1. Dans le panneau Calques de l’écran Module de publication à l’aide de modèles prédéfinis, sélectionnez le calque comprenant les éléments que vous souhaitez paramétrer.

   >[!NOTE]
   >
   >Cliquez sur l’icône en forme d’œil pour l’activer et la désactiver. Vous avez ainsi la certitude de sélectionner l’objet souhaité.

1. Dans le panneau Propriétés, cliquez sur un paramètre dans la colonne Nom (pour paramétrer du texte) ou Paramètre (pour paramétrer des objets).

   * **Texte** Cliquez dans le champ de texte (faites défiler la liste Propriétés pour le trouver). La boîte de dialogue Paramètres s’affiche. Select the text that you want to parameterize and click **Add**. Pour créer plusieurs paramètres pour une même propriété de texte, sélectionnez diverses parties du texte et ajoutez des paramètres pour chacune d’elles. To change the name of the parameter, click it, enter a new name, and click **Close**.

   * **Objets** Cliquez sur une zone dans la colonne Paramètre. La boîte de dialogue Modifier le paramètre s’affiche. Enter a name and click **OK**.
   Pour personnaliser simultanément plusieurs attributs avec la même valeur, utilisez le même nom de paramètre pour chacun d’eux. A titre d’exemple, si votre modèle comporte un rectangle et une étoile, vous pouvez entrer `newcolor` comme nom de paramètre pour chaque attribut Couleur unie. Toute modification de la valeur `newcolor` est alors répercutée sur le rectangle et l’étoile.

1. Dans le champ Valeur ou Données, spécifiez une valeur par défaut pour l’attribut. Définissez toutes les propriétés de l’objet sélectionné pour définir précisément l’apparence souhaitée.
1. (Facultatif) Répétez les étapes 3 à 5 pour tous les objets ou calques à paramétrer.
1. Cliquez sur **Enregistrer** ou sur **Enregistrer sous**.
1. Click **Preview** to open the FXG Preview window and see the parameters you created with their default values.

## Affichage ou masquage d’un objet ou d’un calque dans un modèle FXG {#show-or-hide-an-object-or-layer-in-the-fxg-template}

Bien qu’ils soient invisibles sur la prévisualisation ou la sortie, les objets et calques masqués ne sont pas supprimés du fichier. Vous pouvez, si vous le souhaitez, les rendre à nouveau visibles. La visibilité est un attribut que vous pouvez rendre variable. Activez ou désactivez l’icône en forme d’œil pour définir la valeur de visibilité par défaut d’un objet ou calque.

1. Dans le panneau Objets, cliquez sur l’icône en forme d’œil située en regard du nom d’un objet ou d’un calque pour masquer l’élément en question dans le fichier.
1. Cliquez à nouveau dessus pour rendre l’objet visible.

## Création de différentes versions d’un modèle {#create-different-versions-of-a-template}

Vous pouvez créer plusieurs versions du modèle en modifiant les attributs d’une version à l’autre pour servir diverses utilisations.

Dans l’écran Module de publication à l’aide de modèles prédéfinis, cliquez sur le bouton Enregistrer comme pour enregistrer le fichier en tant que nouveau modèle FXG sans écraser le modèle FXG d’origine.

## Utilisation du texte avec contour {#using-stroked-text}

Le texte avec contour est un exemple de paramétrage des attributs. Dynamic Media Classic prend en charge les fonctions de texte avec contour suivantes :

* Epaisseur du contour
* Motif de contour en pointillé
* Styles de sommet différents
* Styles d’extrémité différents
* Surimpression du contour
* Traitement des couleurs séparé pour le contour, incluant la prise en charge du ton direct

Ce tableau décrit les options d’objet qui prennent en charge le texte avec contour.

| Attribut | Description |
|--- |--- |
| s7:fill `<Boolean>`(S7FXG Only) | Précise si le fond est activé pour le texte. Vrai par défaut. |
| s7:stroke `<Boolean>` (S7FXG Only) | Précise si le contour est activé pour le texte. Faux par défaut. |
| s7:weight `<number>` (S7FXG Only) | Précise l’épaisseur du contour du texte en points. Par défaut : 1 point. |
| s7:joints `<string>` (miter, round, bevel) (S7FXG Only) | Précise le type de sommet du contour. Par défaut : arrondi. |
| s7:caps `<string>` (none, round, square) (S7FXG Only) | Précise le type d’extrémité du contour. Par défaut : arrondi. |
| s7:miterLimit `<number>` (S7FXG Only) | Précise la limite de la pointe lorsque le sommet du contour est en pointe. Par défaut : 4. |
| s7:strokeOverprint `<Boolean>` (S7FXG Only) | Précise si la surimpression est activée pour le contour. Faux par défaut. |
| s7:strokeColorName (S7FXG uniquement) | Identique à s7:colorName, à la différence près qu’il définit le nom de la couleur du contour. |
| s7:strokeColorValue (S7FXG uniquement) | Identique à s7:colorValue, à la différence près qu’il définit la valeur de la couleur utilisée pour le contour. |
| s7:strokeColorspace (S7FXG uniquement) | Identique à s7:colorspace, à la différence près qu’il définit l’espace colorimétrique utilisé pour le contour. |
| flm:dashPattern `<array>` (S7FXG Only) | Par défaut, il n’y a pas de motifs pour les tirets et les espaces. Cet attribut définit le motif tiret/espace du contour. La première valeur est le tiret du contour. La seconde est l’espace entre deux tirets. Vous pouvez étendre le tableau pour plusieurs valeurs de la même manière avec les autres valeurs spécifiées comme tiret et espace. |

## Utilisation de texte déformé {#using-warped-text}

Le texte déformé vous permet de modifier l’apparence du texte avec effets tels que l’ondulation, l’indicateur, l’étirement, etc.

Le texte déformé est pris en charge pour les objets RichText. Le texte peut être vertical ou horizontal, et peut être texte de point, texte de zone et de texte curviligne. L’objet texte doit être entièrement sélectionné pour que la déformation puisse être appliquée.

Le texte déformé peut être créé dans Adobe Illustrator.

Lorsqu’une déformation est appliquée à un texte, vous pouvez définir les attributs suivants :

* Style
* Direction
* Courbure
* Déformation horizontale
* Déformation verticale

Chaque attribut contient un ensemble de valeurs.

| Attribut | Valeurs | Par défaut |
|--- |--- |--- |
| Styles7:warpStyle | nonearcarcLowerarcUpperarchbulgeshellLowershellUpperflagwavefishrisefishEyeinflatesqueezetwist | aucun |
| Direction7:warpDirection | horizontalvertical | horizontal |
| Courbure7:warpBend | -1 à 1 | 0,5 |
| Déformation horizontale7:warpHorizontalDistortion | -1 à 1 | 01 |
| Déformation verticale7:warpVerticalDistortion | -1 à 1 | 01 |

>[!NOTE]
>
>For `inflate` and `fishEye`, changing the `s7:warpDirection` flag between horizontal and vertical does not have any effect on the output.

Pour plus d’informations sur la création et l’utilisation de texte déformé, reportez-vous à la documentation Adobe Illustrator.

>[!MORELIKETHIS]
>
>* [Création d’un modèle initial dans Illustrator](create-initial-template-illustrator.md#create_the_initial_template_in_illustrator)
>* [Téléchargement de fichiers pour le module de publication à l’aide de modèles prédéfinis](upload-files-template-publishing.md#upload_files_for_template-publishing)

