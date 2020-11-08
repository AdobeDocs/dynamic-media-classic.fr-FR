---
title: Création d’un modèle
seo-title: Création d’un modèle
description: 'null'
seo-description: Découvrez comment créer un modèle dans Dynamic Media Classic.
uuid: c762224b-7c6c-4434-bada-c26570079645
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 8f7093da-d215-4337-ac95-69f0a5bf8648
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '3441'
ht-degree: 65%

---


# Création d’un modèle {#creating-a-template}

Pour créer un modèle, cliquez sur Créer > Concepts de base des modèles. Sélectionnez Concepteur ou Développeur. Sur cette page, vous pouvez ajouter des calques d’image et de texte. Vous pouvez également réorganiser les calques, modifier la taille et la position des calques et appliquer des effets d’ombre et d’éclat aux images et au texte.

>[!NOTE]
>
>Si vous modifiez un modèle créé dans une version antérieure de Dynamic Media Classic, vous recevrez peut-être une invite lors de l’enregistrement, vous demandant si vous souhaitez ajouter un calque de zone de travail. Sélectionnez Non pour éviter l’ajout d’un nouveau calque de base. Si, par mégarde, vous avez cliqué sur Oui, supprimez les modificateurs « &amp;allowCanvasPrompt » et « &amp;layer=0 » de l’URL, et appuyez ensuite sur Entrée ou Retour.

## Création du modèle initial {#creating-the-initial-template}

Lorsque vous créez une visionneuse de modèles, l’option **Publish after save** (« Publier après l’enregistrement ») affecte la visionneuse et ses membres comme suit :

| L’option « Publish after save » (« Publier après l’enregistrement ») est-elle sélectionnée avant l’enregistrement ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
|--- |--- |--- |
| Oui | Publié | Publié |
| Non | Non publié | Les membres de la visionneuse conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

Vous pouvez créer un modèle à partir d’un modèle existant. Ouvrez le modèle, cliquez sur **Enregistrer en tant que**, puis entrez un nouveau nom dans la boîte de dialogue Enregistrer en tant que.

**Pour créer la visionneuse de modèles d’origine**

1. Pour créer votre modèle, utilisez l’une des méthodes suivantes :

   **Sélectionnez d’abord** le fichier PSD ou les images Dans le panneau de navigation, sélectionnez le fichier PSD ou les images de votre modèle, puis cliquez sur Créer > Concepts de base des modèles.

   **Début de l’écran** Modèle, cliquez sur Créer > Concepts de base des modèles. Sélectionnez Concepteur ou Développeur.

1. Dans la boîte de dialogue Saisir la taille de la zone de travail, entrez la largeur et la hauteur de votre modèle.
1. Sélectionnez un dossier dans la bibliothèque de fichiers, puis faites glisser le fichier PSD ou les images de votre modèle sur l’écran correspondant.
1. Une fois terminé, près de l’angle inférieur droit de la page, vérifiez que l’option **Publish after save** (« Publier après l’enregistrement ») est sélectionnée (valeur par défaut).
1. Cliquez sur **Enregistrer**.
1. Sélectionnez un dossier de stockage pour votre modèle, nommez le modèle, puis cliquez sur **Envoyer**.

   Dynamic Media Classic réduit les images si nécessaire pour les ajuster à la zone de travail, la zone de l’écran Modèle dans laquelle vous pouvez définir votre modèle.

## Modification d’une visionneuse de modèles {#editing-a-template-set}

Selon que vous modifiez une visionneuse publiée ou une visionneuse de modèles non publiée, l’option **Publish after save** (« Publier après l’enregistrement ») affecte la visionneuse et ses membres comme suit :

| Visionneuse déjà publiée ? | L’option « Publish after save » (« Publier après l’enregistrement ») est-elle sélectionnée avant l’enregistrement de votre modification ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
|--- |--- |--- |--- |
| Oui | Oui | Publié | Publié |
| Oui | Non | Publié | Les membres de visionneuse existants conservent leur état publié. Tous les nouveaux membres de visionneuse que vous avez ajoutés pendant votre modification conservent leur état publié ou non publié. |
| Non | Oui | Publié | Publié |
| Non | Non | Non publié | Les membres de la visionneuse existants, ainsi que tout nouveau membre de la visionneuse que vous ajoutez lors de votre modification conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour modifier une visionneuse de modèles**

1. En mode Affichage de la grille, recherchez une visionneuse de modèles, puis au-dessous de l’image, cliquez sur **Modifier**.
1. Modifiez le modèle selon vos besoins.
1. Une fois les modifications terminées, près de l’angle inférieur droit de la page, vérifiez que l’option **Publish after save** (« Publier après l’enregistrement ») est sélectionnée (valeur par défaut).
1. Cliquez sur **Enregistrer**, sélectionnez un dossier de stockage, attribuez un nom à la visionneuse, puis cliquez sur **Enregistrer**.

## Suppression d&#39;un modèle {#deleting-a-template}

Lorsque vous supprimez une visionneuse de modèles, celle-ci est placée dans la corbeille. Toutefois, les membres (ou « enfants ») de cette visionneuse ne sont pas affectés : ils conservent en fait leur état existant publié ou non publié.

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour supprimer un modèle**

1. En mode Affichage de la grille, Affichage par liste ou Affichage des détails, sélectionnez un ou plusieurs modèles.
1. Sur la barre de navigation globale, cliquez sur **Fichier** > **Supprimer** > **Supprimer**.

## Comprendre l’écran Modèle {#understanding-the-template-screen}

L’écran Modèle contient des outils permettant de manipuler et de paramétrer les calques.

Utilisez les outils suivants de l’écran Modèle pour créer des modèles :

**Outil** Panoramique Vous permet de sélectionner des calques, de les déplacer dans la zone de travail, de les redimensionner ou de les faire pivoter.

**Outil** Texte Crée un calque de texte. Faites glisser le pointeur de l’outil sur la zone de travail pour créer un calque de texte, puis saisissez le texte dans le calque (voir Création d’un calque de texte).

**Bouton** prévisualisation Ouvre l’écran de Prévisualisation et affiche le modèle dans une visionneuse de zoom. Vous pouvez visualiser le modèle en situation réelle sur votre site Web ou dans votre application.

**Bouton** Résumé des paramètres Ouvre l’écran Résumé des paramètres. Vous pouvez voir le nom de tous les calques d’un modèle, et sur chaque calque, le nom des paramètres qui ont été activés.

**Editeur de texte v4.3 et Editeur de texte v4.2** Vous pouvez choisir d’utiliser l’éditeur de texte le plus récent et le plus complet, Editeur de texte v4.3, ou l’éditeur de texte précédent, Editeur de texte v4.2. Lors de la création de nouveaux modèles, l’Editeur de texte v4.3 est sélectionné par défaut. Pour la modification d’anciens modèles, l’Editeur de texte v4.2 est sélectionné par défaut. L’Editeur de texte v4.3 ne prend pas en charge le renvoi à la ligne. Par conséquent, pour modifier d’anciens modèles utilisant le renvoi à la ligne et y rester fidèle, utilisez l’Editeur de texte v4.2. Si un ancien modèle ne prend pas en charge le renvoi à la ligne, choisissez l’Editeur de texte v4.3 pour tirer parti de ses nombreuses nouveautés, telles que ses fonctionnalités Augmenter les marges, Diminuer les marges, Ecrire le texte en lettres capitales et Ajuster le texte.

***remarque **: L’Editeur de texte v4.2 sera finalement supprimé en tant qu’option dans Dynamic Media Classic. Il est donc recommandé d’utiliser l’Editeur de texte 4.3 lorsque cela est possible. L’option Renvoi à la ligne du mot sera intégrée à une prochaine version de l’Editeur de texte.*

**Designer et développeur** Sélectionnez l’option qui décrit le mieux votre rôle.

**Zone de travail** Définit la zone totale disponible, en pixels, pour la définition de votre modèle. La taille par défaut est de 300 x 300 pixels. Les calques sont placés sur la zone de travail.

**La liste** Calques Liste le nom des calques du modèle. Pour sélectionner un calque, sélectionnez son nom dans la liste Calques. La liste Calques est assortie d’outils permettant de supprimer, de réorganiser et de paramétrer les calques, et de leur ajouter des effets (voir Utilisation des calques).

**Propriétés de la zone** de calque Offre les outils permettant de modifier la couleur d’arrière-plan, l’opacité, la taille et la position d’un calque, ainsi que la couleur d’arrière-plan, l’opacité et la taille de la zone de travail. Vous pouvez également y régler les effets d’ombre et d’éclat (voir Utilisation des calques).

## Création de calques d’image {#creating-image-layers}

1. Faites glisser l’image de la bibliothèque de fichiers vers la zone de travail.

   Le nom d’identification (ID) de l’image figure dans la liste Calques.

>[!NOTE]
>
>Si nécessaire, Dynamic Media Classic réduit les images pour les ajuster à la zone de travail lorsque vous créez un calque d’image.

## Création d’un calque de texte {#creating-a-text-layer}

1. Cliquez sur l’outil Texte.
1. Faites glisser le curseur de la souris pour créer une zone de texte sur la zone de travail ou sur une image.
1. Sur l’écran Texte qui apparaît, ajoutez le texte en procédant de l’une des façons suivantes sur l’onglet de prévisualisation :

   * Saisissez du texte dans la zone de texte. Choisissez Ajuster le texte pour qu’il tienne dans la zone de texte.
   * Collez du texte dans la zone de texte à partir du Presse-papiers.

1. Cliquez sur Appliquer, puis fermez l’écran Texte.

### Mise en forme de texte {#format-text}

Pour mettre en forme le texte dans un calque de texte, procédez comme suit :

1. Dans la liste Calques, cliquez deux fois sur le nom de la zone de texte à modifier. L’Editeur de texte s’ouvre.
1. Dans la zone de texte, sélectionnez le texte à mettre en forme. Vous pouvez sélectionner une partie ou la totalité du texte, ainsi que des caractères isolés.
1. Définissez les options de mise en forme, puis cliquez sur Appliquer.

   **Police** Choisissez une police dans le menu Police. Si une police de votre choix n’apparaît pas dans le menu, vous pouvez la télécharger dans Dynamic Media Classic. (voir Polices).

   **Taille** de la police Choisissez une taille de police dans le menu, entrez une taille spécifique dans la zone ou cliquez sur les flèches vers le haut ou vers le bas pour augmenter ou diminuer la taille de deux points.

   **Couleur** Cliquez pour choisir une couleur pour le texte.

   **Gras, Italique ou Souligné** Sélectionnez le texte, puis cliquez sur l’icône correspondant au type de mise en forme à appliquer au texte.

   **Tout en majuscules, Exposant ou Indice** Sélectionnez le texte, puis cliquez sur l’icône correspondant au type de formatage à appliquer au texte.

   **Alignement** Choisissez un bouton Alignement pour aligner à gauche, centrer ou aligner à droite le texte du calque de texte.

   **Suivi** Saisissez ou sélectionnez une valeur numérique permettant d’ajuster l’espace entre les mots.

   **Crénage** Saisissez ou sélectionnez une valeur numérique permettant d’ajuster l’espace entre les caractères.

   **Interligne** Saisissez ou sélectionnez une valeur numérique permettant d’ajuster l’espace entre les lignes.

   **Décalage vertical** Saisissez ou sélectionnez une valeur numérique permettant de déplacer un caractère sélectionné vers le haut ou vers le bas par rapport à la ligne de base du texte environnant. Cette option est particulièrement utile lorsque vous composez des fractions manuellement ou que vous modifiez la position des images texte.

>[!NOTE]
>
>Cliquez sur Annuler pour annuler votre dernière opération. Cliquez sur Rétablir si vous changez d’avis après avoir annulé une action.

### Mise en forme de paragraphes {#format-paragraphs}

1. Dans la liste Calques, cliquez deux fois sur le nom de la zone de texte à modifier. L’Editeur de texte s’ouvre.
1. Sélectionnez le paragraphe que vous souhaitez mettre en forme.
1. Définissez les options de mise en forme, puis cliquez sur Appliquer.

   **Alignement** Cliquez pour spécifier le type d&#39;alignement : aligner à gauche, aligner au centre, aligner à droite ou justifier.

   **Justification** de la fin du paragraphe Cliquez pour préciser le type de justification de la dernière ligne du paragraphe : dernière ligne aligne à gauche ; la dernière ligne aligne le centre ; et la dernière ligne s’aligne à droite.

   **Interligne** Saisissez ou sélectionnez une valeur numérique permettant d’ajuster la quantité d’espace entre toutes les lignes du paragraphe.

   **Retrait total** Cliquez pour augmenter la valeur de mise en retrait du texte.

   **Supprimer le retrait** Cliquez pour diminuer la valeur de mise en retrait du texte.

   **Retrait de la première ligne** Indiquez la valeur de retrait de la première ligne de texte.

   **Espace avant le paragraphe** Indiquez l’espace à afficher au-dessus de la première ligne de texte du paragraphe.

   **Espace après le paragraphe** Indiquez l’espace à afficher sous la dernière ligne de texte du paragraphe.

   **Alignement** vertical Sélectionnez l’emplacement où le texte doit apparaître verticalement dans la zone de texte : Haut, Milieu, Bas.

   **Orientation** du texte Sélectionnez la direction dans laquelle le texte doit s’afficher : De droite à gauche ou de gauche à droite.

### Modification des propriétés du calque de texte {#adjust-text-layer-properties}

1. Dans l’écran Concepts de base des modèles, sélectionnez la zone de texte à modifier.
1. Dans le panneau Propriétés du calque, sélectionnez l’une des options suivantes :

   **Réduire le texte (Editeur de texte v4.2 uniquement)** Sélectionnez cette option pour réduire la taille du texte dans la zone de texte.

   **Renvoi à la ligne (Editeur de texte v4.2 uniquement)** Sélectionnez une option de renvoi à la ligne pour indiquer si le texte est renvoyé à la ligne ou comment :

   **Placer** le texte dans une zone de texte trop petite horizontalement.

   **Aucun renvoi à la ligne** Ne renvoie pas le texte lorsque la zone de texte est trop petite horizontalement et coupe une partie du texte à la place.

   **Renvoi à la ligne** NB (renvoi à la ligne non déchirant) Envoie le texte pour l’adapter à une zone de texte et ne casse pas les mots.

   **Position** Indique l’emplacement de la zone de texte sur la trame.

   **Le remplissage** Ajoute des marges ou recadre le rectangle du calque. Indiquez le nombre de pixels à ajouter aux bords gauche, supérieur, inférieur et droit, ou à leur retrancher. Entrez des valeurs positives pour ajouter une marge, et des valeurs négatives pour effectuer un recadrage.

### Affichage et modification du code source du texte {#view-and-edit-text-source-code}

Les informations fournies dans l’onglet Source de l’Editeur de texte vous serviront de référence. Ne modifiez le texte que si vous êtes rompu à l’édition du code source.

1. Dans la liste Calques, cliquez deux fois sur le nom de la zone de texte à modifier. L’Editeur de texte s’ouvre.
1. Cliquez sur l’onglet Source de l’Editeur de texte pour afficher le code source du texte.
1. Affichez le texte ou apportez-y les modifications nécessaires.

   Les changements sont conservés lorsque vous basculez entre les vues Prévisualiser et Source.

1. Cliquez sur Appliquer pour effectuer le rendu des modifications.

## Utilisation des calques {#working-with-layers}

Utilisez la liste Calques et la zone Propriétés calque pour manipuler les calques. Vous pouvez réorganiser les calques, modifier leur taille et leur position, leur appliquer une rotation et définir leur couleur d’arrière-plan ou de premier plan, leur opacité et leur mode de fusion.

Vous pouvez également modifier la taille de la zone de travail, sélectionner sa couleur d’arrière-plan et modifier son paramètre d’opacité.

### Réagencement des calques {#reordering-layers}

La réorganisation des calques peut avoir une incidence sur leur apparence, surtout si cela concerne la transparence ou la surimpression. Veillez à prévisualiser le résultat avant de valider vos modifications.

1. Pour réorganiser les calques dans un modèle, utilisez l’une des méthodes suivantes :

   * Sélectionnez un calque dans la liste Calques, puis cliquez sur le bouton Haut ou Bas autant de fois que nécessaire pour placer le calque à la position souhaitée dans la liste.
   * Faites glisser un calque vers le haut ou vers le bas dans la liste Calques.

### Modification de la taille et de la position des calques et de la zone de travail {#changing-the-size-and-position-of-layers-and-the-canvas}

Les calques doivent être suffisamment petits pour tenir dans la zone de travail. Vous pouvez modifier la taille d’un calque ou d’une zone de travail manuellement ou en spécifiant des mesures. Vous pouvez changer la position d’un calque manuellement ou en spécifiant des valeurs de décalage. Vous pouvez également appliquer une rotation à un calque.

>[!NOTE]
>
>Dynamic Media Classic recommande de créer un paramètre d’image prédéfini de la taille exacte de votre modèle. Travailler avec un paramètre d’image prédéfini et un modèle de taille identique permet de définir correctement la taille de sortie finale et les options d’accentuation du modèle. Une fois que vous avez créé ce paramètre d’image prédéfini, vous pouvez le sélectionner dans le menu Appliquer le paramètre prédéfini de l’écran Prévisualisation du modèle. L’écran montre l’image telle qu’elle sera diffusée depuis le serveur (voir [Configuration des paramètres d’image prédéfinis](setting-image-presets.md#setting_up_image_presets)).

**Modification de la taille d’un calque**

Pour modifier la taille d’un calque ou de la zone de travail, sélectionnez le calque ou la zone de travail dans la liste Calques, puis utilisez l’une des méthodes suivantes :

**Modification manuelle de la taille** Sélectionnez et faites glisser un coin du calque ou de la zone de travail. Avec les calques de texte, vous pouvez également faire glisser un côté du calque. Maintenez la touche Maj enfoncée lorsque vous faites glisser la souris pour modifier la taille tout en conservant le format (la forme).

**Saisir des mesures** de taille de calque Entrez des mesures en pixels dans les zones de texte W (Largeur) et H (Hauteur) de la zone Propriétés du calque.

En plus de modifier la taille d’un calque, vous pouvez lui appliquer un remplissage. Pour ce faire, entrez une mesure de remplissage dans les cases des bords gauche, droit, supérieur et inférieur de la zone Propriétés calque. Le remplissage permet d’ajouter une marge au calque actif pour le décaler du périmètre de son calque de base. Il est pratique pour faire ressortir l’effet d’ombre portée ou d’ombre extérieure ajouté, le cas échéant. De plus, il augmente la taille d’un calque et affiche sa couleur d’arrière-plan dans la zone de remplissage étendue. Le calque de base se repositionne en fonction de la nouvelle taille du calque. Par exemple, si le calque actif est centré sur le calque de base, lorsque vous étendez le côté gauche du calque actif, il s’éloigne d’autant vers la droite du calque de base.

**Modification de la position d’un calque**

Pour modifier la position d’un calque dans la zone de travail, sélectionnez-le dans la liste Calques, puis utilisez l’une des méthodes suivantes :

**Modification manuelle de la position** Déplacez le pointeur près d’une limite de calque mais pas au-dessus de celle-ci. Lorsque vous voyez le curseur à quatre pointes, cliquez et faites glisser le début.

**Saisir des mesures** de décalage de position Saisissez des mesures de décalage X et Y dans les zones de texte X et Y. Ces valeurs représentent le décalage du point d’ancrage sur les axes x et y, exprimé en pixels.

**Rotation d’un calque**

La zone Pivoter indique l’angle de rotation du calque. Pour faire pivoter un calque, sélectionnez son nom dans la liste Calques, puis utilisez l’une des méthodes suivantes :

**Rotation** manuelle Déplacez le curseur à proximité d’un coin du calque, mais pas dessus. Lorsque le curseur de rotation apparaît, faites glisser l’angle du calque. Maintenez la touche Maj enfoncée lorsque vous faites glisser pour faire pivoter par incréments de 15 degrés.

**Saisir une mesure** du degré Entrez le nombre de degrés de rotation du calque. La rotation s’effectue dans le sens horaire. Pour appliquer une rotation dans le sens anti-horaire, entrez un nombre négatif.

**Masquage d’un calque ou d’un effet de calque**

Vous pouvez masquer un calque ou un effet de calque en cliquant sur l’icône représentant un œil  en regard du nom du calque ou de l’effet. Les calques masqués n’apparaissent pas sur les prévisualisations, ni sur la sortie. Les informations sur le calque sont conservées dans l’URL. « hide=1 » est cependant ajouté à l’URL pour indiquer que le calque est actuellement masqué. Par exemple :

layer=5&amp;src=is{PortalCo/title}&amp;pos=274,192&amp;effect=-1&amp;.effect=Drop Shadow&amp;blendmode

layer=5&amp;src=is{PortalCo/title}&amp;pos=274,192&amp;hide=1&amp;effect=-1&amp;.effect=Drop Shadow&amp;blendmode

### Détermination de la couleur de fond, de l’opacité et du mode de fusion {#determining-the-background-color-opacity-and-blend-mode}

Pour choisir une couleur d’arrière-plan, une opacité et un mode de fusion pour un calque ou la zone de travail, sélectionnez le calque ou la zone de travail, puis utilisez les techniques suivantes :

**Couleur** de premier plan Cliquez sur le bouton Couleur de premier plan et choisissez une nuance pour modifier la couleur de l’ombre ou de l’éclat. Vous pouvez également entrer une valeur chromatique dans la zone. La couleur d’arrière-plan ne s’applique qu’aux calques qui utilisent la transparence. Par exemple, elle s’applique partiellement à un calque transparent d’une étiquette de prix ou l’arrière-plan d’une zone de texte. Les calques composés d’une image PSD, TIFF ou PNG dont la transparence est activée peuvent avoir un arrière-plan transparent.

**Couleur** d’arrière-plan Cliquez sur le bouton Couleur d’arrière-plan et choisissez une nuance pour modifier la couleur des zones de remplissage.

**Opacité** Faites glisser le curseur Opacité pour rendre n’importe quel calque translucide et ainsi faire transparaître une partie de l’image sous-jacente. Le paramètre 100 % définit une opacité totale ; le paramètre 0 % définit la transparence.

**Mode** de fusion Choisissez une option pour simuler l&#39;un des modes de fusion disponibles dans Photoshop. Les options disponibles sont les suivantes : Normal, Fondu, Eclaircir, Assombrir, Multiplier et Ecran. Ces options sont disponibles pour les calques, non pour la zone de travail.

## Utilisation des effets d’ombre et d’éclat sur les calques {#using-shadow-and-glow-effects-on-layers}

Vous pouvez appliquer une ombre ou un éclat à un calque. L’ombre ou l’éclat est appliqué au périmètre du calque et s’étend vers l’intérieur ou l’extérieur, en fonction de l’option sélectionnée. Si votre modèle est issu d’un fichier PSD avec des effets d’ombre et d’éclat, vous pouvez ajuster ces effets dans Contenu multimédia dynamique classique.

Une fois que vous avez appliqué un effet d’ombre ou d’éclat, vous pouvez régler sa taille, sa couleur, son opacité et sa position dans la zone Propriétés calque de l’écran Modèle.

### Application d’un effet d’ombre ou d’éclat à un calque {#applying-a-shadow-or-glow-effect-to-a-layer}

Pour appliquer un effet d’ombre ou d’éclat, procédez comme suit :

1. Sélectionnez un calque dans la liste Calques.
1. Sélectionnez le menu Ajouter un effet, puis choisissez une option :

   **Ombre portée** Applique une ombre au côté inférieur et droit du calque.

   **Ombre** interne Applique un effet d’ombre à l’intérieur de tous les bords du calque.

   **Luminosité** extérieure Applique un effet d’éclat autour de tous les bords du calque.

   **Luminosité** interne Applique un effet d’éclat à l’intérieur de tous les bords du calque.

Un nom d’effet apparaît dans la liste Calques après l’application d’un effet. Pour supprimer un effet, sélectionnez son nom dans la liste Calques, puis sélectionnez le bouton Supprimer.

>[!NOTE]
>
>parfois, l’effet d’une ombre portée ou d’un éclat extérieur n’est pas visible, notamment lorsque le calque sous-jacent est trop petit pour l’afficher. Si l’ombre ou l’éclat est invisible, essayez d’ajouter du remplissage au calque ou de le réorganiser (voir les sections [Modification de la taille et de la position des calques et de la zone de travail](creating-template.md#changing_the_size_and_position_of_layers_and_the_canvas) et [Réagencement des calques](creating-template.md#reordering_layers)).

### Ajustement d’un effet d’ombre ou d’éclat {#adjusting-a-shadow-or-glow-effect}

Pour ajuster un effet d’ombre ou d’éclat, sélectionnez d’abord son nom dans la liste Calques. Ensuite, modifiez ses paramètres dans la zone Propriétés calque de l’écran Modèle :

**Couleur** Sélectionnez le bouton Couleur et choisissez une nuance pour modifier la couleur de l’ombre ou de l’éclat. Vous pouvez également saisir une valeur chromatique dans la zone.

**Opacité** Faites glisser le curseur pour déterminer l’intensité de l’effet. Les effets moins opaques sont plus transparents.

**Mode** de fusion Choisissez une option pour simuler l&#39;un des modes de fusion disponibles dans Photoshop. Les options disponibles sont les suivantes : Normal, Fondu, Eclaircir, Assombrir, Multiplier et Ecran. 

**Taille** Entrez les mesures dans les zones X et Y pour augmenter ou réduire l’effet d’ombre. Les options de taille ne sont disponibles que pour les ombres intérieures et les ombres portées.

**Agrandissement** Faites glisser le curseur pour étendre l’effet vers l’intérieur ou vers l’extérieur.

**Flou** Faites glisser le curseur pour contrôler l’aplatissement des bords de l’effet. Plus le degré de flou est élevé, plus les contours sont atténués.

## Masquage des calques {#masking-layers}

La liste Calques comporte un bouton Masque qui définit le mode d’utilisation du masque ou de la couche alpha d’un calque. A l’aide du bouton Masque, vous pouvez appliquer l’effet d’un calque d’arrière-plan à un calque particulier ou au calque parent entier de votre modèle. Sélectionnez un calque dans la liste Calques, puis sélectionnez le bouton Masque  pour parcourir les états suivants :

* L’arrière-plan du calque est opaque.
* Le contenu du calque est inversé, et une couleur noire unie est appliquée à l’arrière-plan du calque.
* Une couleur noire unie est appliquée à l’arrière-plan du calque.

