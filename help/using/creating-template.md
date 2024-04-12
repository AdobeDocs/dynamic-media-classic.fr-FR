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
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '3418'
ht-degree: 41%

---

# Création d’un modèle

Pour créer un modèle, accédez à **[!UICONTROL Build]** > **[!UICONTROL Concepts de base des modèles]**. Sélectionnez Concepteur ou Développeur. Sur cette page, vous pouvez ajouter des calques d’image et de texte. Vous pouvez également réorganiser les calques, modifier la taille et la position des calques et appliquer des effets d’ombre et d’éclat aux images et au texte.

Voir aussi [Concepts de base des modèles](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) vidéo de formation.

>[!NOTE]
>
>Si vous modifiez un modèle créé dans une version antérieure d’Adobe Dynamic Media Classic, une invite vous demande lors de l’enregistrement &quot;Voulez-vous ajouter un calque de zone de travail ?&quot;. Sélectionner **[!UICONTROL Non]** pour éviter d’ajouter un calque de base. Si vous sélectionnez accidentellement **[!UICONTROL Oui]**, supprimez la variable `&allowCanvasPrompt` et `&layer=0` modificateurs dans l’URL et appuyez sur **[!UICONTROL Entrée]** ou **[!UICONTROL Retour]**.

## Créer le modèle initial {#creating-the-initial-template}

Lorsque vous créez une visionneuse de modèles, l’option **[!UICONTROL Publish after save]** (« Publier après l’enregistrement ») affecte la visionneuse et ses membres comme suit :

| **[!UICONTROL Publier après enregistrement]** l’option sélectionnée avant l’enregistrement ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
| --- | --- | --- |
| Oui | Publié | Publié |
| Non | Non publié | Les membres de la visionneuse conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

Vous pouvez créer un modèle à partir d’un modèle existant. Ouvrez le modèle, puis sélectionnez **[!UICONTROL Enregistrer sous]**, puis saisissez un nouveau nom dans la boîte de dialogue Enregistrer sous .

**Pour créer le modèle initial :**

1. Pour créer votre modèle initial, utilisez l’une des méthodes suivantes :

   * **Sélectionner d’abord le PSD ou les images** - Dans le panneau de navigation, sélectionnez le fichier de PSD ou les images de votre modèle, accédez à **[!UICONTROL Build]** > **[!UICONTROL Concepts de base des modèles]**.

   * **Démarrage à partir de l’écran Modèle** - Accédez à **[!UICONTROL Build]** > **[!UICONTROL Concepts de base des modèles]**. Sélectionnez Concepteur ou Développeur.

1. Dans la boîte de dialogue Saisir la taille de la zone de travail, saisissez les mesures de largeur et de hauteur de votre modèle.
1. Sélectionnez un dossier dans la bibliothèque de fichiers, puis faites glisser le fichier PSD ou les images de votre modèle sur l’écran correspondant.
1. Une fois terminé, près de l’angle inférieur droit de la page, vérifiez que l’option **[!UICONTROL Publish after save]** (« Publier après l’enregistrement ») est sélectionnée (valeur par défaut).
1. Sélectionner **[!UICONTROL Enregistrer]**.
1. Sélectionnez un dossier de stockage du modèle, attribuez-lui un nom, puis sélectionnez **[!UICONTROL Envoyer]**.

   Adobe Dynamic Media Classic réduit les images si nécessaire pour les adapter à la zone de travail, c’est-à-dire la zone de l’écran Modèle pour définir votre modèle.

## Modifier un jeu de modèles {#editing-a-template-set}

Si vous modifiez un jeu publié ou non publié, la variable **[!UICONTROL Publier après enregistrement]** L’option affecte les membres de l’ensemble et de l’ensemble comme suit :

| Visionneuse déjà publiée ? | **[!UICONTROL Publier après enregistrement]** sélectionnée avant d’enregistrer votre modification ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
| --- | --- | --- | --- |
| Oui | Oui | Publié | Publié |
| Oui | Non | Publié | Les membres de visionneuse existants conservent leur état publié. Tout nouveau membre de visionneuse que vous ajoutez lors de votre modification conserve son état publié ou non publié. |
| Non | Oui | Publié | Publié |
| Non | Non | Non publié | Les membres de la visionneuse existants, ainsi que tout nouveau membre de la visionneuse que vous ajoutez lors de votre modification conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour modifier un jeu de modèles :**

1. En mode d’affichage Grille, accédez à un jeu de modèles, puis, sous l’image, sélectionnez **[!UICONTROL Modifier]**.
1. Modifiez le modèle selon vos besoins.
1. Une fois les modifications terminées, près de l’angle inférieur droit de la page, vérifiez que l’option **[!UICONTROL Publish after save]** (« Publier après l’enregistrement ») est sélectionnée (valeur par défaut).
1. Sélectionner **[!UICONTROL Enregistrer]**, sélectionnez un dossier de stockage, saisissez un nom pour la visionneuse, puis sélectionnez **[!UICONTROL Enregistrer]**.

## Suppression d’un modèle

Lorsque vous supprimez une visionneuse de modèles, celle-ci est placée dans la corbeille. Cependant, les membres (ou &quot;enfants&quot;) de cet ensemble ne sont pas affectés ; au lieu de cela, ils conservent chacun leur état publié ou non publié existant.

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour supprimer un modèle :**

1. En mode Affichage de la grille, Affichage par liste ou Affichage des détails, sélectionnez un ou plusieurs modèles.
1. Dans la barre de navigation globale, accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Supprimer]** > **[!UICONTROL Supprimer]**.

## Présentation de l’écran Modèle {#understanding-the-template-screen}

L’écran Modèle contient des outils permettant de manipuler et de paramétrer les calques.

Utilisez ces outils dans l’écran Modèle pour créer des modèles :

* **[!UICONTROL Panoramique]** - Permet de sélectionner des calques, de les déplacer sur la zone de travail, de les redimensionner ou de les faire pivoter.

* **[!UICONTROL Texte]** - Crée un calque de texte. Faites glisser le pointeur de l’outil sur la zone de travail pour créer un calque de texte, puis saisissez le texte dans le calque Voir [Créer un calque de texte](#creating-a-text-layer).

* **[!UICONTROL Aperçu]** : ouvre l’écran Aperçu et affiche le modèle dans une visionneuse de zoom. Vous pouvez visualiser le modèle en situation réelle sur votre site Web ou dans votre application.

* **[!UICONTROL Résumé des paramètres]** Ouvre l’écran Résumé des paramètres. Vous pouvez voir le nom de tous les calques d’un modèle, et sur chaque calque, le nom des paramètres qui ont été activés.

* **[!UICONTROL Éditeur de texte v4.3 et Éditeur de texte v4.2]** - Vous pouvez choisir d’utiliser la dernière version et la version la plus complète de l’éditeur de texte, l’éditeur de texte v4.3, ou l’ancien éditeur de texte, l’éditeur de texte v4.2. Lors de la création de modèles, l’éditeur de texte v4.3 est sélectionné par défaut. Pour la modification d’anciens modèles, l’Editeur de texte v4.2 est sélectionné par défaut. L’éditeur de texte v4.3 ne prend actuellement pas en charge le retour automatique à la ligne. Par conséquent, lors de la modification d’anciens modèles qui utilisent le retour automatique à la ligne, utilisez l’éditeur de texte v4.2 pour préserver la fidélité du modèle. Si votre ancien modèle n’utilise pas de retour automatique à la ligne, vous pouvez choisir l’éditeur de texte v4.3 pour profiter des nombreuses nouvelles fonctionnalités qu’il propose. Par exemple, Augmentez les marges, Réduisez les marges, Définissez le texte en majuscules et Copiez le texte dans la zone appropriée.

  >[!NOTE]
  >
  >La suppression de l’éditeur de texte v4.2 est prévue comme option dans Adobe Dynamic Media Classic. Il est donc recommandé d’utiliser l’éditeur de texte 4.3 dans la mesure du possible. La variable **[!UICONTROL Retour à la ligne]** sera intégrée dans une prochaine version de l’éditeur de texte.

* **[!UICONTROL Designer et développeur]** - Sélectionnez l’option qui décrit le mieux votre rôle.

* **[!UICONTROL Canevas]** - Définit la zone totale disponible, en pixels, pour la définition de votre modèle. La taille par défaut est de 300 × 300 pixels. Les calques sont placés sur la zone de travail.

* **[!UICONTROL Liste Calques]** - Répertorie le nom des calques dans le modèle. Pour sélectionner un calque, sélectionnez son nom dans la liste Calques. La liste Calques est assortie d’outils permettant de supprimer, de réorganiser et de paramétrer les calques, et de leur ajouter des effets Voir [Utilisation des calques](#working-with-layers).

* **[!UICONTROL Zone Propriétés du calque]** - Offre des outils permettant de modifier la couleur, l’opacité, la taille et la position d’un calque, ainsi que la couleur, l’opacité et la taille de l’arrière-plan du canevas. Vous pouvez également y régler les effets d’ombre et d’éclat Voir [Utilisation des calques](#working-with-layers).

## Création de calques d’image {#creating-image-layers}

1. Faites glisser l’image de la bibliothèque de fichiers vers la zone de travail.

   Le nom d’identification (ID) de l’image figure dans la liste Calques.

   >[!NOTE]
   >
   >Si nécessaire, Adobe Dynamic Media Classic réduit les images pour les ajuster à la zone de travail lors de la création d’un calque d’image.

## Création d’un calque de texte {#creating-a-text-layer}

1. Sélectionnez la variable **[!UICONTROL Texte]** outil.
1. Faites glisser le curseur de la souris pour créer une zone de texte sur la zone de travail ou sur une image.
1. Sur l’écran Texte qui apparaît, ajoutez le texte en procédant de l’une des façons suivantes sur l’onglet de prévisualisation :

   * Saisissez du texte dans la zone de texte. Choisissez Ajuster le texte pour qu’il tienne dans la zone de texte.
   * Collez du texte dans la zone de texte à partir du Presse-papiers.

1. Sélectionner **[!UICONTROL Appliquer]**, puis fermez l’écran Texte .

### Mise en forme de texte {#format-text}

Pour mettre en forme le texte dans un calque de texte, procédez comme suit :

1. Dans la liste Calques, cliquez deux fois sur le nom de la zone de texte à modifier. L’Editeur de texte s’ouvre.
1. Dans la zone de texte de l’éditeur de texte, sélectionnez le texte à mettre en forme. Vous pouvez sélectionner tout le texte, des parties du texte ou des caractères individuels.
1. Spécifiez l’une des options de formatage suivantes, puis sélectionnez **[!UICONTROL Appliquer]**.

   * **[!UICONTROL Police]** - Sélectionnez une police dans le menu Police. Si une police souhaitée n’apparaît pas dans le menu, vous pouvez la charger dans Adobe Dynamic Media Classic. Voir Polices.

   * **[!UICONTROL Taille de police]** - Choisissez une taille de police dans le menu, saisissez une taille spécifique dans la zone ou sélectionnez l’option **[!UICONTROL Monter]** ou **[!UICONTROL Descendre]** flèches permettant d&#39;augmenter ou de réduire la taille de deux points.

   * **[!UICONTROL Couleur]** - Sélectionnez cette option pour choisir une couleur pour le texte.

   * **[!UICONTROL Gras]**, **[!UICONTROL Italique]**, ou **[!UICONTROL Souligner]** - Sélectionnez le texte, puis l’icône correspondant au type de formatage à appliquer au texte.

   * **[!UICONTROL Toutes les zones]**, **[!UICONTROL Exposant]**, ou **[!UICONTROL Indice]** - Sélectionnez le texte, puis l’icône correspondant au type de formatage à appliquer au texte.

   * **[!UICONTROL Alignement]** - Sélectionnez un bouton Alignement pour aligner le texte à gauche, au centre ou à droite dans le calque de texte.

   * **[!UICONTROL Tracking]** - Saisissez ou sélectionnez une valeur numérique en fonction de laquelle ajuster l’espace entre les mots.

   * **[!UICONTROL Crénage]** : saisissez ou sélectionnez une valeur numérique en fonction de laquelle ajuster l’espace entre les caractères.

   * **[!UICONTROL Interligne]** : saisissez ou sélectionnez une valeur numérique en fonction de laquelle ajuster l’espace entre les lignes.

   * **[!UICONTROL Décalage vertical]** : saisissez ou sélectionnez une valeur numérique par laquelle déplacer un caractère sélectionné vers le haut ou vers le bas par rapport à la ligne de base du texte environnant. Cette option est particulièrement utile lorsque vous définissez des fractions manuellement ou que vous ajustez la position des graphiques intégrés.

>[!NOTE]
>
>Sélectionner **[!UICONTROL Annuler]** si vous souhaitez annuler votre dernière action. Sélectionner **[!UICONTROL Rétablir]** si vous changez d’avis sur l’annulation d’une action après avoir sélectionné **[!UICONTROL Annuler]**.

### Mise en forme de paragraphes {#format-paragraphs}

1. Dans la liste Calques, cliquez deux fois sur le nom de la zone de texte à modifier. L’Editeur de texte s’ouvre.
1. Sélectionnez le paragraphe à mettre en forme.
1. Spécifiez l’une des options de formatage suivantes, puis sélectionnez **[!UICONTROL Appliquer]**.

   * **[!UICONTROL Alignement]** - Sélectionnez cette option pour spécifier le type d’alignement : aligner à gauche, aligner au centre, aligner à droite ou justifier.

   * **[!UICONTROL Justification de fin de paragraphe]** - Sélectionnez cette option pour spécifier le type de justification de la dernière ligne du paragraphe : la dernière ligne s’aligne à gauche, la dernière ligne s’aligne au centre et la dernière ligne s’aligne à droite.

   * **[!UICONTROL Interligne]** : saisissez ou sélectionnez une valeur numérique en fonction de laquelle ajuster l’espace entre toutes les lignes du paragraphe.

   * **[!UICONTROL Retirer tout]** - Sélectionnez cette option pour augmenter la quantité de texte mise en retrait.

   * **[!UICONTROL Retrait]** - Sélectionnez cette option pour diminuer la quantité de texte mise en retrait.

   * **[!UICONTROL Retrait de la première ligne]** - Indiquez la valeur de mise en retrait de la première ligne de texte.

   * **[!UICONTROL Espace avant le paragraphe]** - Indiquez l’espace devant s’afficher au-dessus de la première ligne de texte du paragraphe.

   * **[!UICONTROL Espace après le paragraphe]** - Indiquez l’espace devant s’afficher sous la dernière ligne de texte du paragraphe.

   * **[!UICONTROL Alignement vertical]** - Sélectionnez l’endroit où vous souhaitez que le texte s’affiche verticalement dans la zone de texte : Haut, Milieu, Bas.

   * **[!UICONTROL Orientation du texte]** - Sélectionnez la direction dans laquelle vous souhaitez que le texte s’affiche : de droite à gauche ou de gauche à droite.

### Modification des propriétés du calque de texte {#adjust-text-layer-properties}

1. Dans l’écran Concepts de base des modèles, sélectionnez la zone de texte à modifier.
1. Dans le panneau Propriétés du calque, sélectionnez l’une des options suivantes :

   * **[!UICONTROL Réduire le texte (Éditeur de texte v4.2 uniquement)]** - Pour l’insérer dans la zone de texte, sélectionnez cette option pour réduire le texte.

   * **[!UICONTROL Retour à la ligne (Éditeur de texte v4.2 uniquement)]** - Pour spécifier si le texte est renvoyé à la ligne ou de quelle façon, sélectionnez une option de retour à la ligne :

   * **[!UICONTROL Retour]** : entoure le texte pour qu’il s’insère dans une zone de texte trop petite horizontalement.

   * **[!UICONTROL Aucun retour]** - Ne renvoie pas le texte à la ligne lorsque la zone de texte est trop petite horizontalement et coupe une partie du texte.

   * **[!UICONTROL Intervalle insécable]** : entoure le texte de la zone de texte et ne rompt pas les mots.

   * **[!UICONTROL Position]** - Indique l’emplacement de la zone de texte sur la zone de travail.

   * **[!UICONTROL Marge intérieure]** - Ajoute des marges ou recadre le rectangle du calque. Spécifiez le nombre de pixels à ajouter ou à supprimer pour Gauche, Haut, Bas et Droite. Saisissez des nombres positifs si vous souhaitez ajouter une marge ou des nombres négatifs au recadrage.

### Affichage et modification du code source du texte {#view-and-edit-text-source-code}

Les informations fournies dans l’onglet Source de l’Editeur de texte vous serviront de référence. Ne modifiez le texte que si vous êtes rompu à l’édition du code source.

1. Dans la liste Calques, cliquez deux fois sur le nom de la zone de texte à modifier. L’Editeur de texte s’ouvre.
1. Dans l’éditeur de texte, pour afficher le code source du texte, sélectionnez l’option **[!UICONTROL Source]** dans l’éditeur de texte.
1. Affichez le texte ou apportez-y les modifications nécessaires.

   Les changements sont conservés lorsque vous basculez entre les vues Prévisualiser et Source.

1. Sélectionner **[!UICONTROL Appliquer]** pour générer les modifications.

## Utilisation des calques {#working-with-layers}

Utilisez la liste Calques et la zone Propriétés calque pour manipuler les calques. Vous pouvez réorganiser les calques, modifier leur taille et leur position, leur appliquer une rotation et définir leur couleur d’arrière-plan ou de premier plan, leur opacité et leur mode de fusion.

Vous pouvez également modifier la taille de la zone de travail, sélectionner sa couleur d’arrière-plan et modifier son paramètre d’opacité.

### Réorganiser les calques {#reordering-layers}

La modification de l’ordre des calques peut avoir une incidence sur l’aspect, en particulier en cas de transparence ou de surimpression. Veillez à prévisualiser le résultat avant de valider vos modifications.

1. Pour réorganiser les calques dans un modèle, utilisez l’une des méthodes suivantes :

   * Sélectionnez un calque dans la liste Calques, Sélectionnez **[!UICONTROL Monter]** ou **[!UICONTROL Descendre]** autant de fois que nécessaire pour le placer à la bonne position dans la liste.
   * Faites glisser un calque vers le haut ou vers le bas dans la liste Calques.

### Modifier la taille et la position des calques et de la zone de travail {#changing-the-size-and-position-of-layers-and-the-canvas}

Les calques doivent être suffisamment petits pour tenir dans la zone de travail. Vous pouvez modifier la taille d’un calque ou d’une zone de travail manuellement ou en spécifiant des mesures. Vous pouvez changer la position d’un calque manuellement ou en spécifiant des valeurs de décalage. Vous pouvez également appliquer une rotation à un calque.

>[!NOTE]
>
>Adobe Dynamic Media Classic recommande de créer un paramètre d’image prédéfini de la taille exacte de votre modèle. Travailler avec un paramètre d’image prédéfini et un modèle de taille identique permet de définir correctement la taille de sortie finale et les options d’accentuation du modèle. Après avoir créé ce paramètre d’image prédéfini, vous pouvez le choisir dans le menu Appliquer le paramètre prédéfini de l’écran Aperçu du modèle. L’écran montre l’image telle qu’elle sera diffusée depuis le serveur Voir [Configuration des paramètres d’image prédéfinis](setting-image-presets.md#setting_up_image_presets).

* **Modification de la taille d’un calque** - Pour modifier la taille d’un calque ou de la zone de travail, sélectionnez le calque ou la zone de travail dans la liste Calques et utilisez l’une des techniques suivantes :

* **Modification manuelle de la taille** - Sélectionnez et faites glisser un coin du calque ou de la zone de travail. Avec les calques de texte, vous pouvez également faire glisser un côté du calque. Maintenez la touche Maj enfoncée lorsque vous faites glisser la souris pour modifier la taille tout en conservant le format (la forme).

* **Saisie des mesures de la taille du calque** - Entrez des mesures en pixels dans les zones de texte W (Largeur) et H (Hauteur) de la zone Propriétés du calque.

En plus de modifier la taille d’un calque, vous pouvez lui appliquer un remplissage. Pour ce faire, entrez une mesure de remplissage dans les cases des bords gauche, droit, supérieur et inférieur de la zone Propriétés calque. Le remplissage permet d’ajouter une marge au calque actif pour le décaler du périmètre de son calque de base. Il est pratique pour faire ressortir l’effet d’ombre portée ou d’ombre extérieure ajouté, le cas échéant. De plus, il augmente la taille d’un calque et affiche sa couleur d’arrière-plan dans la zone de remplissage étendue. Le calque de base se repositionne en fonction de la nouvelle taille du calque. Par exemple, si le calque actif est centré sur le calque de base, lorsque vous étendez le côté gauche du calque actif, il s’éloigne d’autant vers la droite du calque de base.

* **Modification de la position d’un calque** - Pour modifier la position d’un calque sur la zone de travail, sélectionnez son nom dans la liste Calques et utilisez l’une des techniques suivantes :

* **Modification manuelle de la position** - Déplacez le pointeur près d’une limite de calque, mais pas au-dessus de celle-ci. Lorsque vous voyez le curseur en forme de flèche à quatre pointes, sélectionnez et commencez à faire glisser le curseur.

* **Saisir des mesures de décalage de position** - Entrez les mesures de décalage X et Y dans les zones de texte X et Y. Ces valeurs représentent le décalage du point d’ancrage sur les axes x et y, exprimé en pixels.

* **Rotation d’un calque** - La zone Rotation liste l’angle de rotation du calque. Pour faire pivoter un calque, sélectionnez son nom dans la liste Calques, puis utilisez l’une des méthodes suivantes :

* **Rotation manuelle** - Déplacez le curseur près d’un coin du calque, mais pas dessus. Lorsque le curseur de rotation apparaît, faites glisser l’angle du calque. Maintenez la touche Maj enfoncée lorsque vous faites glisser pour faire pivoter par incréments de 15 degrés.

* **Saisie d’une mesure de degré** - Saisissez le nombre de degrés de rotation du calque. La rotation s’effectue dans le sens horaire. Pour appliquer une rotation dans le sens anti-horaire, entrez un nombre négatif.

**Masquer un calque ou un effet de calque :**

Vous pouvez masquer un calque ou un effet de calque en cliquant sur l’icône représentant un oeil en regard du nom d’un calque ou d’un effet. Les calques masqués n’apparaissent pas sur les prévisualisations, ni sur la sortie. Les informations sur le calque sont conservées dans l’URL. Au lieu de cela, `hide=1` est ajouté à l’URL pour noter que le calque est masqué de la vue. Par exemple :

`layer=5&src=is{PortalCo/title}&pos=274,192&effect=-1&.effect=Drop Shadow&blendmode`

`layer=5&src=is{PortalCo/title}&pos=274,192&hide=1&effect=-1&.effect=Drop Shadow&blendmode`

### Déterminer la couleur de fond, l’opacité et le mode de fusion

Pour choisir une couleur d’arrière-plan, une opacité et un mode de fusion pour un calque ou la zone de travail, sélectionnez le calque ou la zone de travail, puis utilisez les techniques suivantes :

* **Couleur de premier plan** - Sélectionner **[!UICONTROL Couleur de premier plan]** et choisissez un échantillon de couleur pour modifier la couleur de l’ombre ou de l’éclat. Vous pouvez également entrer une valeur chromatique dans la zone. La couleur d’arrière-plan ne s’applique qu’aux calques qui utilisent la transparence. Par exemple, elle s’applique partiellement à un calque transparent d’une étiquette de prix ou l’arrière-plan d’une zone de texte. Les calques composés d’une image PSD, TIFF ou PNG dont la transparence est activée peuvent avoir un arrière-plan transparent.

* **Couleur d’arrière-plan** - Sélectionner **[!UICONTROL Couleur d’arrière-plan]** et choisissez un échantillon de couleur pour modifier la couleur des zones remplies.

* **Opacité** - Faites glisser le curseur Opacité pour rendre n’importe quel calque transparent afin qu’une partie de l’image sous-jacente s’affiche. Le paramètre 100 % est opaque ; 0 est transparent.

* **Mode de fusion** - Pour simuler l’un des modes de fusion disponibles dans Photoshop, sélectionnez une option. Les options disponibles sont les suivantes : Normal, Fondu, Eclaircir, Assombrir, Multiplier et Ecran. Ces options sont disponibles pour les calques, non pour la zone de travail.

## Utiliser des effets d’ombre et d’éclat sur les calques {#using-shadow-and-glow-effects-on-layers}

Vous pouvez appliquer une ombre ou un éclat à un calque. L’ombre ou l’éclat est appliqué au périmètre du calque et s’étend vers l’intérieur ou l’extérieur, en fonction de l’option sélectionnée. Si votre modèle est issu d’un fichier de PSD avec des effets d’ombre et de lueur, vous pouvez ajuster ces effets dans Adobe Dynamic Media Classic.

Une fois que vous avez appliqué un effet d’ombre ou d’éclat, vous pouvez régler sa taille, sa couleur, son opacité et sa position dans la zone Propriétés calque de l’écran Modèle.

### Application d’un effet d’ombre ou d’éclat à un calque {#applying-a-shadow-or-glow-effect-to-a-layer}

1. Sélectionnez un calque dans la liste Calques.
1. Sélectionnez la variable **[!UICONTROL `Add Effect`]** et choisissez une option :

   * **[!UICONTROL Ombre portée]** : applique une ombre au bas et à droite du calque.

   * **[!UICONTROL Ombre interne]** : applique un effet d’ombre à l’intérieur de tous les bords du calque.

   * **[!UICONTROL Luminosité extérieure]** - Applique un effet d’éclat sur tous les bords du calque.

   * **[!UICONTROL Luminosité interne]** - Applique un effet d’éclat à l’intérieur de tous les bords du calque.

Un nom d’effet apparaît dans la liste Calques après l’application d’un effet. Pour supprimer un effet, sélectionnez son nom dans la liste Calques, puis sélectionnez **[!UICONTROL Supprimer]**.

>[!NOTE]
>
>Vous ne pouvez parfois pas voir l’effet d’une ombre portée ou d’une lueur extérieure si le calque sous-jacent n’est pas assez grand pour l’afficher. Si vous ne pouvez pas voir l’ombre ou l’éclat, pensez à ajouter des valeurs de remplissage au calque ou à réorganiser le calque. (voir les sections [Modification de la taille et de la position des calques et de la zone de travail](creating-template.md#changing_the_size_and_position_of_layers_and_the_canvas) et [Réagencement des calques](creating-template.md#reordering_layers)).

### Réglage d’un effet d’ombre ou d’éclat {#adjusting-a-shadow-or-glow-effect}

Pour ajuster un effet d’ombre ou d’éclat, sélectionnez d’abord son nom dans la liste Calques. Ensuite, modifiez ses paramètres dans la zone Propriétés calque de l’écran Modèle :

* **[!UICONTROL Couleur]** - Sélectionnez le bouton Couleur et choisissez un échantillon de couleur pour modifier la couleur de l’ombre ou de l’éclat. Vous pouvez également saisir une valeur chromatique dans la zone.

* **[!UICONTROL Opacité]** - Faites glisser le curseur pour déterminer l’intensité de l’effet. Les effets moins opaques sont plus transparents.

* **[!UICONTROL Mode de fusion]** - Pour simuler l’un des modes de fusion disponibles dans Photoshop, sélectionnez une option. Les options disponibles sont les suivantes : Normal, Fondu, Eclaircir, Assombrir, Multiplier et Ecran. 

* **[!UICONTROL Taille]** - Saisissez des mesures dans les zones X et Y pour agrandir ou réduire l’effet d’ombre. Les options de taille ne sont disponibles que pour les ombres intérieures et les ombres portées.

* **[!UICONTROL Développer]** - Faites glisser le curseur pour étendre l’effet vers l’intérieur ou l’extérieur.

* **[!UICONTROL Flou]** - Faites glisser le curseur pour contrôler le contour de l’effet. Plus le degré de flou est élevé, plus les contours sont atténués.

## Masquer les calques {#masking-layers}

La liste Calques comporte un bouton Masque qui définit le mode d’utilisation du masque ou de la couche alpha d’un calque. A l’aide du bouton Masque, vous pouvez appliquer l’effet d’un calque d’arrière-plan à un calque particulier ou au calque parent entier de votre modèle. Sélectionnez un calque dans la liste Calques, puis sélectionnez **[!UICONTROL Masque]** pour parcourir ces états :

* L’arrière-plan du calque est opaque.
* Le contenu du calque est inversé, et une couleur noire unie est appliquée à l’arrière-plan du calque.
* Une couleur noire unie est appliquée à l’arrière-plan du calque.
