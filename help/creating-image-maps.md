---
title: Création de zones cliquables
seo-title: Création de zones cliquables
description: 'null'
seo-description: Découvrez comment créer des zones cliquables.
uuid: 0dcc4956-006e-4a74-9d6a-6d4bb23790ce
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4eddf983-38cb-4f00-b3be-85c20bdd6f69
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '2444'
ht-degree: 75%

---


# Création de zones cliquables{#creating-image-maps}

Une zone cliquable est une partie d’une image, d’une page de catalogue électronique ou d’une image dans une visionneuse à 360°, qui affiche un panneau de survol avec du texte. Une action est déclenchée lorsque l’utilisateur clique sur une zone cliquable. Par exemple, une page Web affiche des informations détaillées sur un produit. Un contour apparaît autour de la zone cliquable lorsque l’utilisateur passe le pointeur dessus, pour la faire ressortir.

Outre la possibilité de créer une zone cliquable dans Dynamic Media Classic, vous pouvez également créer des zones cliquables lors de la conception d’un catalogue dans Adobe Acrobat ou Adobe InDesign.

Lorsque vous créez des zones cliquables, vous pouvez effectuer l’une des opérations suivantes :

* Saisir un texte de survol.
* Entrer du code JavaScript et des URL pour lancer des pages Web.
* Créer des modèles d’URL pour les zones cliquables.
* Copier des zones cliquables dans d’autres images, pages de catalogue électronique ou images dans une visionneuse à 360°.
* Exporter des zones cliquables au format CSV ou XML.
* Importer les métadonnées de l’image à partir d’un fichier délimité par des tabulations ou d’un fichier XML.
* Définir d’autres actions conformément aux directives du consortium WWW (World Wide Web).
* Prévisualiser des zones cliquables.

## Création et modification d’une zone cliquable {#drawing-and-adjusting-an-image-map}

1. Effectuez l’une des opérations suivantes :

   * If you are working with an image in the Grid View or List View, in the Edit drop-down list click **Image Map**. Or, open it in Detail View, and then click **Image Map** above the image.
   * If you are working with a SpinSet in the Grid View or List View, click **Edit**. Or, open it in Detail View, and then click **Edit**. Select an image asset, and then click **Image Map**.
   * If you are working with an eCatalog, in the Grid View, List View, Detail View, click **Edit**. Click the **Map Pages** tab.

   ![](assets/ma_image_map.png)

1. Tracez une zone cliquable rectangulaire ou polygonale (avec de nombreux côtés) :

   **Mappage** rectangulaire Sélectionnez l’outil de zone cliquable rectangulaire et faites glisser le pointeur sur la page pour créer le rectangle. Pour ajouter un point à un rectangle et en faire un polygone, appuyez sur la touche Ctrl, placez l’outil d’insertion à l’endroit souhaité, puis cliquez.

   **Zone cliquable** polygonale Sélectionnez l’outil Zone cliquable polygonale, puis cliquez sur les points du périmètre de la zone de l’image à encadrer. A l’aide du curseur de densité du polygone, modulez la densité du point. La densité initiale est conservée si vous sélectionnez d’autres zones. En revanche, si vous ajoutez, supprimez ou modifiez un point du polygone, la densité initiale est perdue et le curseur revient à la valeur maximale.

1. Nommez la zone cliquable, si vous le souhaitez, dans la liste Zone cliquable. Après avoir tracé une zone cliquable, Dynamic Media Classic lui attribue un nom.

   Pour créer le nom, Dynamic Media Classic ajoute un numéro séquentiel au nom de l’image ou de la page de catalogue électronique que vous utilisez. Vous pouvez indiquer le nom de votre choix.

1. Si vous souhaitez permettre aux utilisateurs d’accéder à une nouvelle page Web lorsqu’ils cliquent sur la zone cliquable, indiquez l’URL correspondante dans la liste Zone cliquable.

   Voir [Utilisation d’un modèle pour définir du code JavaScript et des URL](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. Pour qu’un texte de survol s’affiche lorsque les utilisateurs déplacent le pointeur sur la zone cliquable, saisissez le texte dans la liste Zone cliquable. Dans la liste Zone cliquable, sélectionnez le menu Afficher, puis choisissez l’option Texte de survol. Ensuite, entrez le texte que vous souhaitez présenter à l’écran aux utilisateurs. Vous pouvez rédiger le texte dans une application de traitement de texte et le copier dans le champ Texte de survol.
1. Si vous souhaitez qu’une autre action se déclenche lorsque les utilisateurs déplacent la souris sur une zone cliquable, définissez l’action. Dans la liste déroulante Afficher, cliquez sur Autres actions. Spécifiez les attributs de l’action. (Cliquez sur Afficher > Les deux pour créer un texte de survol et une action pour une zone cliquable.)

   Voir [Définition d’autres actions relatives aux zones cliquables](creating-image-maps.md#defining_other_actions_for_image_maps).

1. (Facultatif) Utilisez l’une des méthodes suivantes :

   * Cliquez sur Prévisualiser pour afficher un aperçu des zones cliquables.
   * Pour supprimer une zone cliquable ou les sommets du polygone, sélectionnez une forme sur l’image, puis cliquez sur Supprimer. Ou, pour un catalogue électronique, sous l’onglet Ordre des pages, cliquez sur Effacer les zones cliquables pour les supprimer de toutes les pages.
   * Pour retirer provisoirement une zone cliquable d’une image, d’une image dans une visionneuse à 360° ou d’une page de catalogue électronique sans la supprimer, désélectionnez l’option Oui appropriée dans la liste Zone cliquable.

1. Cliquez sur Enregistrer.

### Ajustement de la position, de la forme et de la taille des zones cliquables {#adjusting-the-position-shape-and-size-of-image-maps}

Pour modifier la position, la forme et la taille d’une zone cliquable, cliquez sur le bouton Zone cliquable. Sélectionnez ensuite l’outil Panoramique, puis suivez les instructions suivantes :

**Modification de la position** Déplacez le pointeur près de la bordure de la zone cliquable, mais pas dessus. Lorsque le pointeur prend la forme d’une flèche à quatre pointes, faites glisser la zone à l’emplacement voulu.

**Modification de la taille et de la forme** La modification de la forme et de la taille d’une zone cliquable dépend de l’utilisation d’une zone cliquable rectangulaire ou polygonale :

***Conseil **: Vous pouvez faire glisser le curseur Taille au bas de l’écran pour modifier les vues et mieux visualiser votre zone cliquable.*

**Zone cliquable** rectangulaire Déplacez le pointeur sur un côté ou un angle de la zone cliquable. Lorsque le pointeur prend la forme d’une flèche à double pointe, faites glisser la souris. Maintenez la touche Maj enfoncée lorsque vous faites glisser la souris pour modifier la taille tout en conservant le format (la forme).

**Zone cliquable** polygonale Faites glisser une poignée de sélection carrée. Pour obtenir une poignée de sélection, cliquez sur la bordure de la zone cliquable, puis commencez à la faire glisser.

### Gestion des zones cliquables superposées {#handling-overlapping-image-maps}

Si votre image (ou page de catalogue électronique) comprend plusieurs zones cliquables et si ces zones se superposent, vous pouvez contrôler cette superposition. Pour ce faire, changez l’ordre des zones dans la liste Zone cliquable en faisant glisser leur nom vers le haut ou vers le bas. Une position élevée dans la liste indique que la zone cliquable associée se superpose avec d’autres zones cliquables.

### Importation des données de zone cliquable {#importing-image-map-data}

Plutôt que de saisir les données de zone cliquable sur chacune des pages, vous avez la possibilité d’importer les données de l’ensemble de votre image, visionneuse à 360° ou catalogue électronique dans l’écran Résumé de zone cliquable. Vous importez les données de zone cliquable sous la forme d’un fichier délimité par des tabulations ou d’un fichier DTD XML. Les champs du fichier doivent être dans l’ordre indiqué sur l’écran de résumé de zone cliquable : Nom, Etiquettes de table des matières, Zones, URL, Texte de survol, Autres actions et Chaînes de recherche. Vous évitez ainsi d’avoir à saisir les données dans la liste de zones cliquables au fur et à mesure que vous créez ces dernières.

**Pour importer des données de zone cliquable**

1. Aller à la page d’édition des zones cliquables (pour des images ou des images dans des visionneuses à 360°) ou l’onglet Pages de zones de l’écran d’édition du catalogue électronique.
1. Cliquez sur Importer les métadonnées.
1. Dans la boîte de dialogue Télécharger les métadonnées, cliquez sur Image ou Zone cliquable pour télécharger les métadonnées à partir du type de propriété de fichier souhaité.
1. Dans la liste déroulante Générer un fichier, sélectionnez le type de fichier que vous souhaitez créer.
1. (Facultatif) Cliquez sur Générer pour afficher un aperçu des données résultantes en fonction du type de fichier que vous voulez créer. Cliquez sur Fermer pour revenir à la boîte de dialogue Télécharger les métadonnées.
1. Naviguez jusqu’au fichier que vous souhaitez télécharger. Dans le champ de texte Nom de fichier, spécifiez le nom du fichier généré.
1. (Facultatif) Dans le champ Nom de la tâche, spécifiez un nom pour la tâche de téléchargement des métadonnées.
1. Cliquez sur Télécharger.

### Copie de zones cliquables {#copying-image-maps}

Vous pouvez copier des zones cliquables d’une image (ou d’une page de catalogue électronique) à l’autre. Utilisez l’option de copie des zones cliquables pour mieux préparer leur création. Vous pouvez également copier les zones cliquables afin de les recréer dans des images ou des pages qui partagent la même disposition ou structure de mappage. 

Par exemple, copier des zones cliquables dans un catalogue électronique permet de copier facilement toutes les zones cliquables entre les versions de langue étrangère du même catalogue électronique. Pour obtenir de meilleurs résultats, il est préférable d’effectuer une copie entre des catalogues électroniques ayant le même nombre de pages et les mêmes images. Si le catalogue électronique dans lequel vous copiez des zones cliquables contient déjà des zones cliquables, notez que celles-ci sont supprimées lors de la copie.

**Pour copier des zones cliquables**

1. Aller à la page d’édition des zones cliquables (pour des images ou des images dans des visionneuses à 360°) ou l’onglet Pages de zones de l’écran d’édition du catalogue électronique.
1. Cliquez sur Copier les zones dans.
1. Effectuez l’une des opérations suivantes, selon que vous souhaitiez copier des zones cliquables à partir d’images ou à partir d’un catalogue électronique :

   * (Images) Dans l’écran Sélectionner des images, sélectionnez les images dans lesquelles vous souhaitez copier les zones cliquables.
   * (Catalogue électronique) Dans l’écran Sélectionner un fichier, sélectionnez les images ou les pages de catalogue électronique dans lesquelles vous souhaitez copier les zones cliquables.

1. Cliquez sur Sélectionner.

## Utilisation d’un modèle pour définir du code JavaScript et des URL {#using-a-template-to-enter-javascript-and-urls}

Vous pouvez définir un modèle d’URL (également appelé modèle Href) pour faciliter et améliorer la saisie des URL de zones cliquables. Définissez un modèle d’URL si la plupart des URL des zones cliquables partagent un format commun et fixe. Si vous définissez la partie de l’URL fixe comme modèle d’URL, vous êtes dispensé de l’entrer chaque fois que vous créez une zone cliquable. Le modèle d’URL peut également contenir des commandes JavaScript, des chemins d’accès et des paramètres. By default, the URL template contains a proprietary Dynamic Media Classic JavaScript handler called `loadProduct` that opens the image in a new window.

>[!NOTE]
>
>Notez que lorsque vous ajoutez du code Javascript dans l’attribut HREF de votre zone cliquable, le code s’exécute sur l’ordinateur du client. Veillez donc vous assurer que le code Javascript est sécurisé.

### A propos des modèles d’URL {#about-url-templates}

Avec un modèle d’URL, le contenu de la colonne URL dans la liste Zone cliquable est remplacé par le double signe dollar ($$) dans le modèle :

```as3
Javascript:loadProduct(‘$$’);void(0);
```

Toutes les valeurs invariables entre les zones cliquables doivent être insérées dans le modèle d’URL. N’ajoutez que les valeurs variables dans la colonne URL de la liste Zone cliquable. Par exemple :

* Modèle d’URL : j `avascript:loadProduct(‘https://www.examplesitehere.com/$$’);void(0);`
* Valeur de l’URL : `product.htm`
* URL réelle générée : `javascript:loadProduct(‘https://www.examplesitehere.com/product.html);void(0);`

By default, the URL template includes a proprietary Dynamic Media Classic JavaScript handler called `loadProduct` that opens a new window with the URL destination. Cependant, vous pouvez utiliser n’importe quel code JavaScript pour remplacer ce gestionnaire JavaScript ou utiliser l’un des gestionnaires Dynamic Media Classic suivants :

* `loadProductCW`

   Affiche l’URL cible spécifiée dans la colonne URL de la fenêtre active. Ce code est réservé principalement aux catalogues électroniques intégrés dans une page d’un site Web.

* `loadProductPW`

   Affiche l’URL cible spécifiée dans la colonne URL de la fenêtre parente (la page d’où la page active a été ouverte). La fenêtre active reste ouverte, mais la fenêtre parent change pour afficher l’URL cible.

   ***remarque **: Le gestionnaire`loadProductPW`ne prend pas en charge les visionneuses DHTML et HTML5.*

### Création d’un modèle d’URL {#creating-a-url-template}

Pour créer un modèle d’URL, procédez comme suit :

1. Sur l’écran Editeur de zone cliquable (images ou visionneuses à 360°) ou l’onglet Pages de zones de l’écran Catalogue électronique (catalogues électroniques), cliquez sur Modifier en regard de l’option Modèle d’URL. La boîte de dialogue Modifier le modèle de zone apparaît.
1. Entrez le code JavaScript et l’URL complète (en remplaçant la partie variable par le double signe dollar [$$]). Vous pouvez coller le code en cliquant avec le bouton droit de la souris et en choisissant l’option Coller.
1. Cliquez sur le bouton Enregistrer.

### Gestion des modèles d’URL {#handling-url-templates}

La page Editeur de zone cliquable (images et visionneuses à 360°) et l’onglet Pages de zones de l’écran Catalogue électronique (catalogues électroniques) contiennent les commandes de gestion des modèles d’URL suivantes :

**Option** Modèle d’URL Sélectionnez l’option Modèle d’URL pour appliquer votre modèle d’URL à toutes les zones cliquables d’une image ou d’une page de catalogue électronique.

**Option** Modèle Désélectionnez une option Modèle dans la liste de zone cliquable URL si vous ne souhaitez pas qu’une zone cliquable individuelle utilise le modèle d’URL.

## Définition d’autres actions relatives aux zones cliquables {#defining-other-actions-for-image-maps}

Dans le menu Afficher, choisissez Autres actions pour déclencher des actions autres que le texte de survol et le lancement d’une page Web. Lorsque l’utilisateur amène le pointeur sur une zone cliquable, vous pouvez initier une action. Ces actions sont des attributs définis pour les zones cliquables côté client conformément aux spécifications HTML du consortium WWW (World Wide Web). Elles comptent notamment :

**touche** d&#39;accès Déclenche une action lorsque l&#39;utilisateur appuie sur une touche spécifiée du clavier.

**onfocus** Déclenche un événement lorsque la zone cliquable est sélectionnée (par le curseur, en appuyant sur la touche de tabulation ou en appuyant sur une touche d’accès). Par exemple, vous pouvez lancer une page Web lorsque la zone cliquable devient active et la refermer lorsqu’elle ne l’est plus.

**onblur** Déclenche un événement lorsque la zone cliquable n’est plus active, que ce soit par le curseur ou par tabulation.

**Pour définir d’autres actions pour les zones cliquables**

1. Sur l’écran Editeur de zone cliquable (images et visionneuses à 360°) ou l’onglet Pages de zones de l’écran Catalogue électronique (catalogues électroniques), sélectionnez le menu Afficher, puis choisissez Autres actions.
1. Selon la syntaxe conforme aux spécifications HTML du consortium WWW (World Wide Web), ajoutez les attributs pris en charge dans la colonne Autres actions de la liste Zone cliquable.
1. Cliquez sur **Enregistrer**.

Dans le menu Afficher, choisissez Les deux pour associer à une zone cliquable un texte de survol ainsi qu’une action.

## Création de zones cliquables dans Adobe Acrobat ou Adobe InDesign {#creating-image-maps-in-adobe-acrobat-or-adobe-indesign}

Vous pouvez créer des zones cliquables lors de la conception de votre catalogue électronique dans Adobe Acrobat ou Adobe InDesign.

Dans Acrobat ou InDesign, créez un lien hypertexte à l’emplacement auquel vous souhaitez faire apparaître la zone cliquable et spécifiez l’URL à laquelle elle doit renvoyer. Lorsque vous sélectionnez l’option Extraire les liens lors du téléchargement du fichier PDF dans Dynamic Media Classic, les liens sont automatiquement convertis en zones cliquables.

Pour plus d’informations, reportez-vous à l’aide d’InDesign ou d’Acrobat.

### Création de zones cliquables dans Adobe InDesign {#to-create-image-maps-in-adobe-indesign}

1. Dans InDesign, sélectionnez Fenêtre > Objet interactif > Hyperliens pour ouvrir le panneau Hyperliens.
1. Sélectionnez le texte, le bloc ou le graphique que vous souhaitez transformer en zone cliquable.
1. Dans le menu du panneau Hyperliens, cliquez sur Nouvel hyperlien.
1. Dans la boîte de dialogue Nouvel hyperlien, sélectionnez l’URL dans le menu Lien vers.
1. Tapez ou collez l’ID du produit dans le champ URL et cliquez sur OK. (Dynamic Media Classic complète l’URL à l’aide du modèle d’URL de zone cliquable.)

   >[!NOTE]
   >
   >vous n’avez pas besoin de définir les options d’apparence dans InDesign. Vous pouvez spécifier l’aspect dans Dynamic Media Classic.

1. Répétez les étapes 2 à 5 pour toutes les zones cliquables que vous souhaitez créer.
1. Exportez les fichiers au format PDF.
1. Téléchargez le fichier PDF dans Dynamic Media Classic et sélectionnez Extraire les liens dans les options PDF.

### Création de zones cliquables dans Adobe Acrobat {#to-create-image-maps-in-adobe-acrobat}

1. Dans Acrobat, sélectionnez Outils > Modifications avancées > Outil Lien.
1. Faites glisser la souris pour créer la zone cliquable. La boîte de dialogue Créer un lien s’ouvre.
1. Sélectionnez Lien personnalisé et cliquez sur Suivant.

   ***remarque **: Il n’est pas nécessaire de définir les options d’aspect dans Acrobat. Vous pouvez spécifier l’aspect dans Dynamic Media Classic.*

1. Dans la boîte de dialogue Propriétés du lien, cliquez sur Actions.
1. Sélectionnez Ouvrir un lien Web dans le menu Sélectionner l’action, puis cliquez sur Ajouter.
1. Tapez l’ID du produit pour la zone cliquable dans la boîte de dialogue Modifier l’URL. (Dynamic Media Classic complète l’URL à l’aide du modèle d’URL de zone cliquable.)
1. Répétez les étapes 1 à 7 pour toutes les zones cliquables que vous souhaitez créer.
1. Enregistrez le fichier.
1. Téléchargez le fichier PDF dans Dynamic Media Classic et sélectionnez Extraire les liens dans les options PDF.

