---
title: Création d’un modèle
description: Découvrez comment créer un modèle dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: 23ac1a0f-c90b-4250-ae36-93702fb5ebd9
topic: Content Management
level: Experienced
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '3433'
ht-degree: 36%

---

# Création d’un modèle

Pour créer un modèle, accédez à **[!UICONTROL Créer]** > **[!UICONTROL Principes de base des modèles]**. Sélectionnez Concepteur ou Développeur. Sur cette page, vous pouvez ajouter des calques d’image et de texte. Vous pouvez également réorganiser les calques, modifier la taille et la position des calques et appliquer des effets d’ombre et d’éclat aux images et au texte.

Consultez également la vidéo de formation [Principes de base des modèles](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS).

>[!NOTE]
>
>Si vous modifiez un modèle créé dans une version antérieure d’Adobe Dynamic Media Classic, une invite vous demande, lors de l’enregistrement, « Voulez-vous ajouter un calque de zone de travail ? » Sélectionnez **[!UICONTROL Non]** pour éviter d’ajouter un calque de base. Si vous sélectionnez accidentellement **[!UICONTROL Oui]**, supprimez les modificateurs `&allowCanvasPrompt` et `&layer=0` dans l’URL et appuyez sur **[!UICONTROL Entrée]** ou **[!UICONTROL Retour]**.

## Création du modèle initial {#creating-the-initial-template}

Lorsque vous créez un jeu de modèles, l&#39;option **[!UICONTROL Publier après un enregistrement]** affecte le jeu et les membres du jeu des manières suivantes :

| L’option **[!UICONTROL Publier après un enregistrement]** est-elle sélectionnée avant l’enregistrement ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
| --- | --- | --- |
| Oui | Publié | Publié |
| Non | Non publié | Les membres de la visionneuse conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

Vous pouvez créer un modèle à partir d’un modèle existant. Ouvrez le modèle, sélectionnez **[!UICONTROL Enregistrer sous]**, puis saisissez un nouveau nom dans la boîte de dialogue Enregistrer sous.

**Pour créer le modèle initial, procédez comme suit**

1. Pour créer votre modèle initial, utilisez l’une des méthodes suivantes :

   * **Sélectionnez d’abord le PSD ou les images** : dans le panneau Parcourir , sélectionnez le ou les fichiers PSD à utiliser pour votre modèle, puis accédez à **[!UICONTROL Créer]** > **[!UICONTROL Principes de base des modèles]**.

   * **À partir de l’écran Modèle** : accédez à **[!UICONTROL Créer]** > **[!UICONTROL Principes de base des modèles]**. Sélectionnez Concepteur ou Développeur.

1. Dans la boîte de dialogue Saisir la taille de la zone de travail, saisissez les mesures de largeur et de hauteur de votre modèle.
1. Sélectionnez un dossier dans la bibliothèque de fichiers, puis faites glisser le fichier PSD ou les images de votre modèle sur l’écran correspondant.
1. Lorsque vous avez terminé, en bas à droite de la page, assurez-vous que l’option **[!UICONTROL Publier après un enregistrement]** est sélectionnée (par défaut).
1. Sélectionnez **[!UICONTROL Enregistrer]**.
1. Sélectionnez un dossier pour stocker votre modèle, saisissez un nom pour le modèle, puis sélectionnez **[!UICONTROL Envoyer]**.

   Adobe Dynamic Media Classic réduit les images si nécessaire pour les adapter à la zone de travail, la zone de l’écran Modèle définissant votre modèle.

## Modification d’un ensemble de modèles {#editing-a-template-set}

Que vous modifiiez un ensemble publié ou un ensemble de modèles dépublié, l&#39;option **[!UICONTROL Publier après un enregistrement]** affecte l&#39;ensemble et les membres de l&#39;ensemble des manières suivantes :

| Visionneuse déjà publiée ? | L’option **[!UICONTROL Publier après un enregistrement]** est-elle sélectionnée avant d’enregistrer votre modification ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
| --- | --- | --- | --- |
| Oui | Oui | Publié | Publié |
| Oui | Non | Publié | Les membres d’ensemble existants conservent leur statut publié. Tout nouveau membre de visionneuse que vous ajoutez lors de votre modification conserve son état publié ou non publié. |
| Non | Oui | Publié | Publié |
| Non | Non | Non publié | Les membres de la visionneuse existants, ainsi que tout nouveau membre de la visionneuse que vous ajoutez lors de votre modification conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour modifier un jeu de modèles, procédez comme suit**

1. Dans la vue Grille, accédez à un jeu de modèles, puis, sous l’image, sélectionnez **[!UICONTROL Modifier]**.
1. Modifiez le modèle si nécessaire.
1. Lorsque vous avez terminé la modification, en bas à droite de la page, assurez-vous que l’option **[!UICONTROL Publier après un enregistrement]** est sélectionnée (par défaut).
1. Sélectionnez **[!UICONTROL Enregistrer]**, sélectionnez un dossier de stockage, saisissez un nom pour la visionneuse, puis sélectionnez **[!UICONTROL Enregistrer]**.

## Suppression d’un modèle

Lorsque vous supprimez un ensemble de modèles, l’ensemble lui-même est déplacé vers la corbeille. Toutefois, les membres (ou « enfants ») de cet ensemble ne sont pas affectés. Ils conservent chacun leur état publié ou dépublié existant.

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour supprimer un modèle, procédez comme suit**

1. En mode Affichage de la grille, Affichage par liste ou Affichage des détails, sélectionnez un ou plusieurs modèles.
1. Sur la barre de navigation globale, accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Supprimer]** > **[!UICONTROL Supprimer]**.

## Présentation de l’écran Modèle {#understanding-the-template-screen}

L’écran Modèle contient des outils permettant de manipuler et de paramétrer les calques.

Utilisez ces outils dans l’écran Modèle pour créer des modèles :

* **[!UICONTROL Panoramique]** : permet de sélectionner des calques, de les déplacer dans la zone de travail, de les redimensionner ou de les faire pivoter.

* **[!UICONTROL Texte]** : crée un calque de texte. Faites glisser le pointeur de l’outil sur la zone de travail pour créer un calque de texte, puis saisissez le texte dans le calque Voir [Création d’un calque de texte](#creating-a-text-layer).

* **[!UICONTROL Aperçu]** : ouvre l’écran d’aperçu et affiche le modèle dans une visionneuse Zoom. Vous pouvez voir à quoi ressemble le modèle pour les utilisateurs et utilisatrices de votre site web ou de votre application.

* **[!UICONTROL Synthèse des paramètres]** ouvre l&#39;écran Synthèse des paramètres. Vous pouvez voir le nom de tous les calques d’un modèle, et sur chaque calque, le nom des paramètres qui ont été activés.

* **[!UICONTROL Éditeur de texte v4.3 et Éditeur de texte v4.2]** : utilisez l’éditeur de texte le plus récent et le plus complet. Vous pouvez choisir d’utiliser l’éditeur de texte v4.3 ou l’éditeur de texte précédent, l’éditeur de texte v4.2. Lors de la création de modèles, l’éditeur de texte v4.3 est sélectionné par défaut. Pour la modification d’anciens modèles, l’Editeur de texte v4.2 est sélectionné par défaut. Actuellement, l’éditeur de texte v4.3 ne prend pas en charge le retour à la ligne. Par conséquent, lors de la modification d’anciens modèles utilisant le retour à la ligne, utilisez l’éditeur de texte v4.2 pour conserver la fidélité du modèle entièrement intacte. Si votre ancien modèle n’utilise pas le renvoi à la ligne, vous pouvez choisir l’éditeur de texte v4.3 pour tirer parti des nombreuses nouvelles fonctionnalités qu’il offre. Par exemple, augmentez les marges, réduisez les marges, définissez le texte en majuscules et copiez le texte ajusté.

  >[!NOTE]
  >
  >La suppression de l’éditeur de texte v4.2 est prévue en tant qu’option dans Adobe Dynamic Media Classic. Il est recommandé d’utiliser l’éditeur de texte 4.3 lorsque cela est possible. L’option **[!UICONTROL Retour à la ligne]** sera incorporée dans une prochaine version de l’éditeur de texte.

* **[!UICONTROL Designer et développeur]** : sélectionnez l’option qui décrit le mieux votre rôle.

* **[!UICONTROL Zone de travail]** : définit la zone disponible totale, en pixels, pour définir votre modèle. La taille par défaut est de 300 × 300 pixels. Les calques sont placés sur la zone de travail.

* **[!UICONTROL Liste Calques]** : répertorie le nom des calques du modèle. Pour sélectionner un calque, sélectionnez son nom dans la liste Calques. La liste Calques est assortie d’outils permettant de supprimer, de réorganiser et de paramétrer les calques, et de leur ajouter des effets Voir [ Utilisation des calques ](#working-with-layers).

* **[!UICONTROL Zone Propriétés du calque]** : cette zone propose des outils permettant de modifier la couleur, l’opacité, la taille et la position de l’arrière-plan d’un calque. Vous pouvez également modifier la couleur, l’opacité et la taille de l’arrière-plan de la zone de travail. Vous pouvez également y régler les effets d’ombre et d’éclat Voir [ Utilisation des calques ](#working-with-layers).

## Création de calques d’image {#creating-image-layers}

1. Faites glisser l’image de la bibliothèque de fichiers vers la zone de travail.

   Le nom d’identification (ID) de l’image figure dans la liste Calques.

   >[!NOTE]
   >
   >Si nécessaire, Adobe Dynamic Media Classic réduit les images pour les faire tenir dans la zone de travail lorsque vous créez un calque d’image.

## Création d’un calque de texte {#creating-a-text-layer}

1. Sélectionnez l’outil **[!UICONTROL Texte]**.
1. Faites glisser le curseur de la souris pour créer une zone de texte sur la zone de travail ou sur une image.
1. Dans l’écran Texte qui s’ouvre, ajoutez du texte en procédant de l’une des manières suivantes dans l’onglet Aperçu :

   * Saisissez du texte dans la zone de texte. Choisissez Ajuster le texte pour qu’il tienne dans la zone de texte.
   * Collez du texte dans la zone de texte à partir du Presse-papiers.

1. Sélectionnez **[!UICONTROL Appliquer]**, puis fermez l’écran Texte.

### Mise en forme de texte {#format-text}

Pour mettre en forme le texte dans un calque de texte, procédez comme suit :

1. Dans la liste Calques, cliquez deux fois sur le nom de la zone de texte à modifier. L’Editeur de texte s’ouvre.
1. Dans la zone de texte de l’éditeur de texte, sélectionnez le texte à mettre en forme. Vous pouvez sélectionner tout le texte, des parties du texte ou des caractères individuels.
1. Spécifiez l’une des options de mise en forme suivantes, puis sélectionnez **[!UICONTROL Appliquer]**.

   * **[!UICONTROL Police]** : sélectionnez une police dans le menu Police. Si une police de votre choix n’apparaît pas dans le menu, vous pouvez la charger dans Adobe Dynamic Media Classic. Voir Polices.

   * **[!UICONTROL Taille de police]** : sélectionnez une taille de police dans le menu, saisissez une taille spécifique dans la zone ou sélectionnez les flèches **[!UICONTROL Haut]** ou **[!UICONTROL Bas]** pour augmenter ou réduire la taille de deux points.

   * **[!UICONTROL Couleur]** : sélectionnez cette option pour choisir une couleur pour le texte.

   * **[!UICONTROL Gras]**, **[!UICONTROL Italique]** ou **[!UICONTROL Souligné]** : sélectionnez le texte, puis l’icône correspondant au type de mise en forme à appliquer au texte.

   * **[!UICONTROL Toutes les majuscules]**, **[!UICONTROL Exposant]** ou **[!UICONTROL Indice]** : sélectionnez le texte, puis l’icône correspondant au type de mise en forme à appliquer au texte.

   * **[!UICONTROL Alignement]** : sélectionnez un bouton d’alignement pour aligner à gauche, centrer ou aligner à droite le texte du calque de texte.

   * **[!UICONTROL Suivi]** : saisissez ou sélectionnez une valeur numérique pour ajuster l’espace entre les mots.

   * **[!UICONTROL Crénage]** : saisissez ou sélectionnez une valeur numérique pour ajuster l’espace entre les caractères.

   * **[!UICONTROL Espacement des lignes]** : saisissez ou sélectionnez une valeur numérique pour ajuster l’espace entre les lignes.

   * **[!UICONTROL Décalage de ligne de base]** : saisissez ou sélectionnez une valeur numérique pour déplacer un caractère sélectionné vers le haut ou vers le bas par rapport à la ligne de base du texte environnant. Cette option est particulièrement utile lorsque vous définissez des fractions à la main ou ajustez la position des graphiques intégrés.

>[!NOTE]
>
>Sélectionnez **[!UICONTROL Annuler]** si vous souhaitez annuler votre dernière action. Sélectionnez **[!UICONTROL Rétablir]** si vous changez d’avis sur l’inversion d’une action après avoir sélectionné **[!UICONTROL Annuler]**.

### Mise en forme de paragraphes {#format-paragraphs}

1. Dans la liste Calques, cliquez deux fois sur le nom de la zone de texte à modifier. L’Editeur de texte s’ouvre.
1. Sélectionnez le paragraphe à mettre en forme.
1. Spécifiez l’une des options de mise en forme suivantes, puis sélectionnez **[!UICONTROL Appliquer]**.

   * **[!UICONTROL Alignement]** : indiquez le type d’alignement en cliquant sur **[!UICONTROL Aligner à gauche]**, **[!UICONTROL Aligner au centre]**, **[!UICONTROL Aligner à droite]** ou **[!UICONTROL Justifier]**.

   * **[!UICONTROL Justification de la fin du paragraphe]** : sélectionnez cette option pour spécifier le type de justification de la dernière ligne du paragraphe : la dernière ligne s’aligne à gauche, la dernière ligne s’aligne au centre et la dernière ligne s’aligne à droite.

   * **[!UICONTROL Espacement des lignes]** : saisissez ou sélectionnez une valeur numérique pour ajuster l’espace entre toutes les lignes du paragraphe.

   * **[!UICONTROL Tout mettre en retrait]** : sélectionnez cette option pour augmenter la mise en retrait du texte.

   * **[!UICONTROL Supprimer le retrait]** : sélectionnez cette option pour réduire la mise en retrait du texte.

   * **[!UICONTROL Mettre en retrait la première ligne]** : indiquez l’excédent de mise en retrait de la première ligne de texte.

   * **[!UICONTROL Espace avant le paragraphe]** : indiquez l’espace à afficher au-dessus de la première ligne de texte du paragraphe.

   * **[!UICONTROL Espace après le paragraphe]** : indiquez l’espace qui doit apparaître sous la dernière ligne de texte du paragraphe.

   * **[!UICONTROL Alignement vertical]** : sélectionnez l’endroit où vous souhaitez que le texte apparaisse verticalement dans la zone de texte : Haut, Milieu, Bas.

   * **[!UICONTROL Direction du texte]** : sélectionnez la direction dans laquelle vous souhaitez que le texte s’affiche : de droite à gauche ou de gauche à droite.

### Modification des propriétés du calque de texte {#adjust-text-layer-properties}

1. Dans l’écran Concepts de base des modèles, sélectionnez la zone de texte à modifier.
1. Dans le panneau Propriétés du calque, sélectionnez l’une des options suivantes :

   * **[!UICONTROL Réduire le texte (éditeur de texte v4.2 uniquement)]** : sélectionnez cette option pour réduire le texte afin qu’il s’adapte à la zone de texte.

   * **[!UICONTROL Retour à la ligne automatique (éditeur de texte v4.2 uniquement)]** : pour spécifier si ou comment le texte est renvoyé à la ligne, sélectionnez une option de retour à la ligne automatique :

   * **[!UICONTROL Habiller]** : permet d’habiller le texte dans une zone de texte trop petite horizontalement.

   * **[!UICONTROL Pas d’habillage]** : n’effectue pas d’habillage lorsque la zone de texte est trop petite horizontalement et, à la place, coupe une partie du texte.

   * **[!UICONTROL Retour à la ligne sans rupture]** : recouvre le texte pour qu’il s’adapte à une zone de texte et ne rompt pas les mots.

   * **[!UICONTROL Position]** : indique l’emplacement de la zone de texte sur la zone de travail.

   * **[!UICONTROL Marge intérieure]** : permet d’ajouter des marges ou de recadrer le rectangle du calque. Spécifiez le nombre de pixels à ajouter ou à supprimer pour Gauche, Haut, Bas et Droite. Entrez des nombres positifs si vous voulez ajouter une marge ou des nombres négatifs au recadrage.

### Affichage et modification du code source du texte {#view-and-edit-text-source-code}

Les informations fournies dans l’onglet Source de l’éditeur de texte sont à titre de référence. Ne modifiez le texte que si vous êtes rompu à l’édition du code source.

1. Dans la liste Calques, cliquez deux fois sur le nom de la zone de texte à modifier. L’Editeur de texte s’ouvre.
1. Dans l’éditeur de texte, pour afficher le code source du texte, sélectionnez l’onglet **[!UICONTROL Source]** dans l’éditeur de texte.
1. Affichez le texte ou apportez-y les modifications nécessaires.

   Les changements sont conservés lorsque vous basculez entre les vues Prévisualiser et Source.

1. Sélectionnez **[!UICONTROL Appliquer]** pour effectuer le rendu des modifications.

## Utilisation des calques {#working-with-layers}

Utilisez la liste Calques et la zone Propriétés calque pour manipuler les calques. Vous pouvez réorganiser les calques, modifier leur taille et leur position, leur appliquer une rotation et définir leur couleur d’arrière-plan ou de premier plan, leur opacité et leur mode de fusion.

Vous pouvez également modifier la taille de la zone de travail, sélectionner sa couleur d’arrière-plan et modifier son paramètre d’opacité.

### Réorganiser les calques {#reordering-layers}

La modification de l’ordre des calques peut affecter l’aspect, en particulier en cas de transparence ou de surimpression. Veillez à prévisualiser le résultat avant de valider vos modifications.

1. Pour réorganiser les calques dans un modèle, utilisez l’une des méthodes suivantes :

   * Sélectionnez un calque dans la liste Calques, Sélectionnez ensuite **[!UICONTROL Vers le haut]** ou **[!UICONTROL Vers le bas]** autant de fois que nécessaire pour le placer à la bonne position dans la liste.
   * Faites glisser un calque vers le haut ou vers le bas dans la liste Calques.

### Modifier la taille et la position des calques et de la zone de travail {#changing-the-size-and-position-of-layers-and-the-canvas}

Les calques doivent être suffisamment petits pour tenir dans la zone de travail. Vous pouvez modifier la taille d’un calque ou d’une zone de travail manuellement ou en spécifiant des mesures. Vous pouvez changer la position d’un calque manuellement ou en spécifiant des valeurs de décalage. Vous pouvez également appliquer une rotation à un calque.

>[!NOTE]
>
>Adobe Dynamic Media Classic recommande de créer un paramètre d’image prédéfini ayant la taille exacte de votre modèle. Travailler avec un paramètre d’image prédéfini et un modèle de taille identique permet de définir correctement la taille de sortie finale et les options d’accentuation du modèle. Après avoir créé ce paramètre d’image prédéfini, vous pouvez le choisir dans le menu Appliquer le paramètre prédéfini de l’écran Aperçu du modèle . L’écran montre l’image telle qu’elle sera diffusée depuis le serveur Voir [Configuration des paramètres d’image prédéfinis](setting-image-presets.md#setting_up_image_presets).

* **Modification de la taille d’un calque** : pour modifier la taille d’un calque ou de la zone de travail, sélectionnez le calque ou la zone de travail dans la liste Calques et utilisez l’une des techniques suivantes :

* **Modification manuelle de la taille** : sélectionnez et faites glisser un coin du calque ou de la zone de travail. Avec les calques de texte, vous pouvez également faire glisser un côté du calque. Maintenez la touche Maj enfoncée tout en faisant glisser pour modifier la taille, mais conservez les proportions (la forme).

* **Saisie des mesures de taille de calque** : saisissez les mesures en pixels dans les zones de texte W (Largeur) et H (Hauteur) dans la zone Propriétés du calque.

En plus de modifier la taille d’un calque, vous pouvez lui appliquer un remplissage. Pour ce faire, entrez une mesure de remplissage dans les cases des bords gauche, droit, supérieur et inférieur de la zone Propriétés calque. Le remplissage permet d’ajouter une marge au calque actif pour le décaler du périmètre de son calque de base. Il est pratique pour faire ressortir l’effet d’ombre portée ou d’ombre extérieure ajouté, le cas échéant. De plus, il augmente la taille d’un calque et affiche sa couleur d’arrière-plan dans la zone de remplissage étendue. Le calque de base se repositionne en fonction de la nouvelle taille du calque. Par exemple, si le calque actif est centré sur le calque de base, lorsque vous étendez le côté gauche du calque actif, il s’éloigne d’autant vers la droite du calque de base.

* **Modification de la position d’un calque** : pour modifier la position d’un calque sur la zone de travail, sélectionnez son nom dans la liste Calques et utilisez l’une des techniques suivantes :

* **Changement manuel de position** : déplacez le pointeur près d’une limite de calque, mais pas au-dessus, puis lorsque le curseur à quatre pointes s’affiche, sélectionnez-la et commencez à la faire glisser.

* **Saisie des mesures de décalage de position** : saisissez les mesures de décalage X et Y dans les zones de texte X et Y. Ces valeurs représentent le décalage du point d’ancrage sur les axes x et y, exprimé en pixels.

* **Rotation d’un calque** : la zone Rotation répertorie l’angle de rotation du calque. Pour faire pivoter un calque, sélectionnez son nom dans la liste Calques, puis utilisez l’une des méthodes suivantes :

* **Rotation manuelle** : déplacez le curseur près d’un coin du calque, mais pas au-dessus. Lorsque le curseur de rotation apparaît, faites glisser l’angle du calque. Maintenez la touche Maj enfoncée lorsque vous faites glisser pour faire pivoter par incréments de 15 degrés.

* **Saisie d’une mesure de degré** : saisissez le nombre de degrés de rotation du calque. La rotation s’effectue dans le sens horaire. Pour appliquer une rotation dans le sens anti-horaire, entrez un nombre négatif.

**Masquer un calque ou un effet de calque :**

Vous pouvez masquer un calque ou un effet de calque en sélectionnant l’icône représentant un œil à côté d’un nom de calque ou d’effet. Les calques masqués n’apparaissent pas sur les prévisualisations, ni sur la sortie. Les informations sur le calque sont conservées dans l’URL. Au lieu de cela, `hide=1` est ajouté à l’URL pour noter que le calque est masqué de la vue. Par exemple :

`layer=5&src=is{PortalCo/title}&pos=274,192&effect=-1&.effect=Drop Shadow&blendmode`

`layer=5&src=is{PortalCo/title}&pos=274,192&hide=1&effect=-1&.effect=Drop Shadow&blendmode`

### Déterminez la couleur d’arrière-plan, l’opacité et le mode de fusion

Pour choisir une couleur d’arrière-plan, une opacité et un mode de fusion pour un calque ou la zone de travail, sélectionnez le calque ou la zone de travail, puis utilisez les techniques suivantes :

* **Couleur de premier plan** : sélectionnez **[!UICONTROL Couleur de premier plan]** et choisissez un échantillon de couleur pour modifier la couleur de l’ombre ou de la lueur. Vous pouvez également entrer une valeur chromatique dans la zone. La couleur d’arrière-plan ne s’applique qu’aux calques qui utilisent la transparence. Par exemple, elle s’applique partiellement à un calque transparent d’une étiquette de prix ou l’arrière-plan d’une zone de texte. Les calques composés d’une image PSD, TIFF ou PNG dont la transparence est activée peuvent avoir un arrière-plan transparent.

* **Couleur d’arrière-plan** : sélectionnez **[!UICONTROL Couleur d’arrière-plan]** et choisissez une nuance de couleur pour modifier la couleur des zones matelassées.

* **Opacité** : faites glisser le curseur Opacité pour rendre un calque translucide, de sorte qu’une partie de l’image sous-jacente s’affiche. Le paramètre de 100 % est opaque ; 0 est transparent.

* **Mode de fusion** : pour simuler l’un des modes de fusion disponibles dans Photoshop, choisissez une option. Les options disponibles sont les suivantes : Normal, Fondu, Eclaircir, Assombrir, Multiplier et Ecran. Ces options sont disponibles pour les calques, non pour la zone de travail.

## Utilisation d’effets d’ombre et de lueur sur les calques {#using-shadow-and-glow-effects-on-layers}

Vous pouvez appliquer une ombre ou un éclat à un calque. L’ombre ou la lueur s’applique au périmètre du calque et s’étend vers l’intérieur ou vers l’extérieur, selon l’option d’ombre ou de lueur que vous choisissez. Si votre modèle provient d’un fichier PSD avec des effets d’ombre et de lueur, vous pouvez ajuster ces effets dans Adobe Dynamic Media Classic.

Une fois que vous avez appliqué un effet d’ombre ou d’éclat, vous pouvez régler sa taille, sa couleur, son opacité et sa position dans la zone Propriétés calque de l’écran Modèle.

### Application d’un effet d’ombre ou de lueur à un calque {#applying-a-shadow-or-glow-effect-to-a-layer}

1. Sélectionnez un calque dans la liste Calques.
1. Sélectionnez le menu **[!UICONTROL `Add Effect`]** et choisissez une option :

   * **[!UICONTROL Ombre portée]** : applique une ombre aux côtés inférieur et droit du calque.

   * **[!UICONTROL Ombre interne]** : applique un effet d’ombre à tous les bords du calque.

   * **[!UICONTROL Lueur externe]** : applique un effet de lueur sur tous les bords du calque.

   * **[!UICONTROL Lueur interne]** : applique un effet de lueur à tous les bords du calque.

Un nom d’effet apparaît dans la liste Calques après l’application d’un effet. Pour supprimer un effet, sélectionnez son nom dans la liste Calques, puis sélectionnez **[!UICONTROL Supprimer]**.

>[!NOTE]
>
>Parfois, vous ne pouvez pas voir l’effet d’une ombre portée ou d’une lueur externe si le calque sous-jacent n’est pas assez grand pour l’afficher. Si l’ombre ou la lueur ne s’affiche pas, pensez à ajouter des valeurs de remplissage au calque ou à réorganiser le calque. (voir les sections [Modification de la taille et de la position des calques et de la zone de travail](creating-template.md#changing_the_size_and_position_of_layers_and_the_canvas) et [Réagencement des calques](creating-template.md#reordering_layers)).

### Ajuster un effet d&#39;ombre ou de lueur {#adjusting-a-shadow-or-glow-effect}

Pour ajuster un effet d’ombre ou d’éclat, sélectionnez d’abord son nom dans la liste Calques. Ensuite, modifiez ses paramètres dans la zone Propriétés calque de l’écran Modèle :

* **[!UICONTROL Couleur]** : sélectionnez le bouton Couleur et choisissez un échantillon de couleur pour modifier la couleur de l’ombre ou de la lueur. Vous pouvez également saisir une valeur chromatique dans la zone.

* **[!UICONTROL Opacité]** : faites glisser le curseur pour déterminer l’intensité de l’effet. Les effets moins opaques sont plus transparents.

* **[!UICONTROL Mode de fusion]** : pour simuler l’un des modes de fusion disponibles dans Photoshop, choisissez une option. Les options disponibles sont les suivantes : Normal, Fondu, Eclaircir, Assombrir, Multiplier et Ecran. 

* **[!UICONTROL Taille]** : saisissez les mesures dans la zone X et Y pour agrandir ou réduire l’effet d’ombre. Les options de taille ne sont disponibles que pour les ombres intérieures et les ombres portées.

* **[!UICONTROL Agrandir]** : faites glisser le curseur pour étendre l’effet vers l’intérieur ou vers l’extérieur.

* **[!UICONTROL Flou]** : faites glisser le curseur pour contrôler le contour progressif sur les bords de l’effet. Plus le degré de flou est élevé, plus les contours sont atténués.

## Masquer les calques {#masking-layers}

La liste Calques comporte un bouton Masque qui définit le mode d’utilisation du masque ou de la couche alpha d’un calque. A l’aide du bouton Masque, vous pouvez appliquer l’effet d’un calque d’arrière-plan à un calque particulier ou au calque parent entier de votre modèle. Sélectionnez un calque dans la liste Calques, puis sélectionnez **[!UICONTROL Masque]** pour parcourir les états suivants :

* L’arrière-plan du calque est opaque.
* Le contenu du calque est inversé, et une couleur noire unie est appliquée à l’arrière-plan du calque.
* Une couleur noire unie est appliquée à l’arrière-plan du calque.
