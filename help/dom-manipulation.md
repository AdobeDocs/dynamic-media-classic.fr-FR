---
title: Manipulation DOM
seo-title: Manipulation DOM
description: 'null'
seo-description: Découvrez la manipulation DOM.
uuid: 275 cd 49 d -2 a 55-41 f 9-80 b 0-e 147 d 0 cd 2907
contentOwner: admin
content-type: référence
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/template-publishing
discoiquuid: 890 ca 93 e -3146-4347-864 b-bd 5 e 94037038
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Manipulation DOM{#dom-manipulation}

La manipulation DOM (document object model) est une technique permettant de modifier un fichier de création en manipulant directement son code XML. La manipulation DOM vous permet de mieux contrôler les éléments de création variables, y compris en modifiant leur contenu et leur aspect ; vous pouvez également créer de nouveaux éléments selon vos besoins.

Dynamic Media Classic vous permet de manipuler le DOM d'un modèle FXG Dynamic Media Classic au moyen de commandes URL après la publication du modèle. Les éléments de création du modèle FXG sont manipulés par le biais de commandes URL. Vous pouvez ainsi manipuler et ajouter des attributs aux graphiques de façon dynamique.

Pour utiliser la manipulation DOM, vous devez créer s 7 : Identifiants d'élément contenus dans votre fichier Illustrator avant de les convertir en fichier FXG Dynamic Media Classic et de les télécharger vers SPS.

>[!NOTE]
>
>lors de l’utilisation des commandes de manipulation DOM, toutes les valeurs transmises doivent être codées en URL.

>[!NOTE]
>
>Illustrator Plug-in for Web-to-Print (for converting Illustrator files) converts to FXG 2.0. For information about this specification, see [www.adobe.com/go/learn_s7_fxg2_en](https://www.adobe.com/go/learn_s7_fxg2_en).

## Création d’identifiants d’élément Scene7 dans des fichiers Illustrator {#creating-s-elementids-in-illustrator-files}

Pour utiliser la méthode de manipulation DOM avec un fichier créé dans Illustrator, vous devez créer des identifiants d’élément Scene7 dans ce fichier. La création d’identifiants d’élément Scene7 permet la modification d’éléments de création à l’aide de commandes URL après la publication du modèle.

### Création d’identifiants d’élément Scene7 pour la manipulation DOM de texte {#creating-s-elementids-for-dom-manipulation-of-text}

Pour créer un identifiant d’élément Scene7 en vue de la manipulation DOM d’un objet texte, ouvrez le panneau Calques dans Illustrator. Puis, sur le calque de texte qui contient du texte variable, nommez le calque à l’aide d’un identifiant d’élément Scene7. To do so, enter the letters `id` (for identification), a colon ( `:`), and a name. Voici quelques exemples de noms de calques de texte sous forme d’identifiants d’élément Scene7 :

`id:BirthdayBoyName`

`id:DateofBirth`

`id:EnterFirstNameHer`

### Création d’identifiants d’élément Scene7 pour la manipulation DOM d’objets {#creating-s-elementids-for-dom-manipulation-of-objects}

Si vous souhaitez que les utilisateurs finals puissent modifier les attributs des objets, créez des identifiants d’élément Scene7 pour les objets. Les objets peuvent être des blocs de texte entiers, des graphiques ou des images. Un arrière-plan de couleur constitue un exemple d’identifiant d’élément d’objet. L’utilisateur final peut, par exemple, modifier la couleur d’arrière-plan d’une affiche au gré des saisons.

Avant de créer un identifiant d’élément Scene7 pour un objet dans Illustrator, créez un calque distinct pour cet objet.

Pour créer un identifiant d’élément Scene7 pour un objet dans Illustrator, procédez comme suit :

1. Sélectionnez l’objet.
1. Cliquez **sur Fenêtre** &gt; **Calques**.
1. Dans le panneau Calques, nommez le calque d'objet avec une valeur s 7 : Identifiant d'élément. To do so, enter the letters `id` (for identification), a colon ( `:`), and description to identify the element. Voici quelques exemples de noms de calques d’objet sous forme d’identifiants d’élément Scene7 :

   `id:BackgroundColor`

   `id:RotationPercentage`

   `id:JacketJPG`

## Publication de modèles FXG {#publish-fxg-templates}

Lorsque vous publiez votre modèle FXG, il est placé sur les serveurs Dynamic Media Classic où il est disponible pour votre site Web et votre application. En outre, durant le processus de publication, Scene7 Publishing System active les URL nécessaires à votre site Web ou à votre application.

>[!NOTE]
>
>pour utiliser votre modèle FXG, publiez tout le contenu qui a servi à le créer, y compris les polices et les images. Si vous n’incluez pas tous les fichiers requis, un message d’erreur s’affiche lors de la publication.

### Marquage de modèles FXG pour publication {#mark-fxg-templates-for-publish}

Les modèles et tous leurs fichiers de support doivent être marqués pour publication pour être placés sur les serveurs d'images de médias dynamiques.

1. Dans le panneau de navigation, sélectionnez le modèle FXG avec les graphiques, images et polices utilisés.
1. Cliquez **sur Marquer pour publication**.

### Publication de votre modèle FXG {#publish-your-fxg-template}

1. Sur la barre de navigation générale, cliquez sur **Publier**, 
1. Sélectionnez une option d’occurrence et saisissez éventuellement un nom pour la tâche de publication.
1. Click **Start Publish**.

### Affichage de l’indicateur de dépassement de texte {#text-overflow-indicator-display}

Un *indicateur de dépassement de texte* indique quand le texte dépasse l’espace qui lui est attribué dans un bloc de texte (ou dans le dernier bloc de texte dans le cas d’un texte lié). Cet indicateur est représenté sous la forme d’un cadre rouge avec un signe plus. Les indicateurs de dépassement de texte sont toujours activés sous SPS.

Les indicateurs de dépassement de texte sont contrôlés avec le modificateur `markOverflowingTextFrame` Utilisez le modificateur comme suit :

| Modificateur/valeurs | Description |
|--- |--- |
| Markoverflowingtextframe = 0,1 | La valeur 1 fait apparaître les indicateurs d’enchaînement. Valeur par défaut : 0. (Même si la valeur par défaut est 0, les indicateurs de dépassement de texte sont toujours activés dans SPS.) Remarque : le modificateur markOverflowingTextFrame est sensible à la casse. |

>[!MORELIKETHIS]
>
>* [Définition de la variabilité : paramétrage et manipulation DOM](defining-variability-parameterization-versus-dom.md#defining_variability_parameterization_versus_dom_manipulation)
>* [Publication](publishing-files.md#publishing_files)

