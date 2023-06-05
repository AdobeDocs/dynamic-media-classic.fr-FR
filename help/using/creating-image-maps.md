---
title: Création de zones cliquables
description: Découvrez comment créer des zones cliquables dans Adobe Dynamic Media Classic.
uuid: 0dcc4956-006e-4a74-9d6a-6d4bb23790ce
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4eddf983-38cb-4f00-b3be-85c20bdd6f69
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: deafbd03-06bc-4d7e-87a1-5620ebcac426
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '2430'
ht-degree: 50%

---

# Création de zones cliquables {#creating-image-maps}

Une zone cliquable est une partie d’une image, d’une page de catalogue électronique ou d’une image dans une visionneuse à 360°, qui affiche un panneau de survol avec du texte. Lorsque l’utilisateur sélectionne une zone cliquable, une action d’une sorte ou d’une autre est déclenchée. Par exemple, une page Web affiche des informations détaillées sur un produit. Un contour s’affiche autour d’une zone cliquable lorsque l’utilisateur déplace le pointeur dessus.

Outre la possibilité de créer des zones cliquables dans Adobe Dynamic Media Classic, vous pouvez également créer des zones cliquables lors de la conception d’un catalogue dans Adobe Acrobat ou Adobe InDesign.

Lorsque vous créez des zones cliquables, vous pouvez effectuer l’une des opérations suivantes :

* Saisir un texte de survol.
* Entrer du code JavaScript et des URL pour lancer des pages Web.
* Créer des modèles d’URL pour les zones cliquables.
* Copier des zones cliquables dans d’autres images, pages de catalogue électronique ou images dans une visionneuse à 360°.
* Exporter des zones cliquables au format CSV ou XML.
* Importez des métadonnées d’image à partir d’un fichier délimité par des tabulations ou d’un fichier XML.
* Définir d’autres actions conformément aux directives du consortium WWW (World Wide Web).
* Prévisualiser des zones cliquables.

## Dessin et réglage d’une zone cliquable {#drawing-and-adjusting-an-image-map}

1. Effectuez l’une des opérations suivantes :

   * Si vous utilisez une image en mode Grille ou Liste, sélectionnez dans la liste déroulante Modifier **[!UICONTROL Zone cliquable]**. Vous pouvez également l’ouvrir dans la vue Détails, puis sélectionner **[!UICONTROL Zone cliquable]** au-dessus de l’image.
   * Si vous utilisez une visionneuse à 360° en mode Grille ou Liste, sélectionnez **[!UICONTROL Modifier]**. Vous pouvez également l’ouvrir dans la vue Détails, puis sélectionner **[!UICONTROL Modifier]**. Sélectionnez une ressource image, puis sélectionnez **[!UICONTROL Zone cliquable]**.
   * Si vous utilisez un catalogue électronique, en mode Grille, Liste et Détails, sélectionnez **[!UICONTROL Modifier]**. Sélectionnez la **[!UICONTROL Pages de mappage]** .

   ![Image cliquable](assets/ma_image_map.png)

1. Tracez une zone cliquable rectangulaire ou polygonale (avec de nombreux côtés) :

   * **Carte rectangulaire** - Sélectionnez l’outil de zone cliquable Rectangle et faites glisser sur la page pour créer le rectangle. Pour ajouter un point à une carte rectangulaire (pour le transformer en map polygone), appuyez sur Ctrl, puis placez l’outil d’insertion à l’emplacement souhaité et sélectionnez.

   * **map polygonal** - Sélectionnez l’outil de zone cliquable polygonal et sélectionnez des points sur le périmètre de la zone de l’image que vous souhaitez encadrer. A l’aide du curseur de densité du polygone, modulez la densité du point. La densité initiale est conservée si vous sélectionnez d’autres zones. En revanche, si vous ajoutez, supprimez ou modifiez un point du polygone, la densité initiale est perdue et le curseur revient à la valeur maximale.

1. Nommez la zone cliquable, si vous le souhaitez, dans la liste Zone cliquable. Après avoir dessiné une zone cliquable, Adobe Dynamic Media Classic lui attribue un nom.

   Pour créer le nom, Adobe Dynamic Media Classic ajoute un numéro séquentiel au nom de l’image ou de la page de catalogue électronique que vous utilisez. Vous pouvez indiquer le nom de votre choix.

1. Si vous souhaitez que les utilisateurs ouvrent une nouvelle page web lorsqu’ils sélectionnent la zone cliquable, saisissez l’URL dans la liste Zone cliquable.

   Voir [Utilisation d’un modèle pour définir du code JavaScript et des URL](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. Pour qu’un texte de survol s’affiche lorsque les utilisateurs déplacent le pointeur sur la zone cliquable, saisissez le texte dans la liste Zone cliquable. Dans la liste Zone cliquable, sélectionnez la variable **[!UICONTROL Afficher]** et sélectionnez **[!UICONTROL Texte de survol]**. Saisissez ensuite le texte que vous souhaitez que les utilisateurs voient à l’écran. Vous pouvez rédiger le texte dans une application de traitement de texte et le copier dans le champ Texte de survol.

1. Si vous souhaitez qu’une autre action se déclenche lorsque les utilisateurs déplacent la souris sur une zone cliquable, définissez l’action. Dans le **[!UICONTROL Afficher]** liste déroulante, sélectionnez **[!UICONTROL Autres actions]**. Spécifiez les attributs de l’action. (Accédez à **[!UICONTROL Afficher]** > **[!UICONTROL Les]** pour créer du texte de survol et une action pour une zone cliquable.)

   Voir [Définition d’autres actions pour les zones cliquables](creating-image-maps.md#defining_other_actions_for_image_maps).

1. (Facultatif) Utilisez l’une des méthodes suivantes :

   * Pour prévisualiser les zones cliquables, sélectionnez **[!UICONTROL Aperçu]**.
   * Pour supprimer une zone cliquable ou un sommet polygone, sélectionnez une forme sur l’image, puis sélectionnez **[!UICONTROL Supprimer]**. Ou, pour un catalogue électronique, dans l’onglet Ordre des pages, sélectionnez **[!UICONTROL Effacer les mappages]** pour supprimer les zones cliquables de toutes les pages.
   * Pour retirer provisoirement une zone cliquable d’une image, d’une image dans une visionneuse à 360° ou d’une page de catalogue électronique sans la supprimer, désélectionnez l’option Oui appropriée dans la liste Zone cliquable.

1. Sélectionner **[!UICONTROL Enregistrer]**.

### Ajuster la position, la forme et la taille des zones cliquables {#adjusting-the-position-shape-and-size-of-image-maps}

Pour modifier la position, la forme et la taille d’une zone cliquable, cliquez sur le bouton Zone cliquable. Sélectionnez ensuite le **[!UICONTROL Panoramique]** et suivez ces instructions :

* **Modifier la position** - Déplacez le pointeur près de la bordure de la zone cliquable, mais pas dessus. Lorsque le pointeur prend la forme d’une flèche à quatre pointes, faites glisser la zone à l’emplacement voulu.

* **Modifier la taille et la forme** - La manière dont vous modifiez la forme et la taille d’une zone cliquable varie selon que vous utilisez une zone cliquable rectangulaire ou polygonal :

>[!TIP]
>
>Vous pouvez faire glisser le curseur Taille situé dans la partie inférieure de l’écran pour modifier les vues et avoir une idée plus précise de l’aspect de votre zone cliquable.

* **Zone cliquable rectangulaire** - Déplacez le pointeur sur un côté ou un coin de la zone cliquable. Lorsque le pointeur prend la forme d’une flèche à double pointe, faites glisser la souris. Maintenez la touche Maj enfoncée lorsque vous faites glisser la souris pour modifier la taille tout en conservant le format (la forme).

* **Zone cliquable polygonal** - Faites glisser une poignée de sélection carrée. Pour créer une poignée de sélection, sélectionnez la bordure de la zone cliquable et commencez à la faire glisser.

### Gestion des zones cliquables se chevauchant {#handling-overlapping-image-maps}

Si votre image (ou page de catalogue électronique) comprend plusieurs zones cliquables et si ces zones se superposent, vous pouvez contrôler cette superposition. Pour ce faire, changez l’ordre des zones dans la liste Zone cliquable en faisant glisser leur nom vers le haut ou vers le bas. Une position élevée dans la liste indique que la zone cliquable associée se superpose avec d’autres zones cliquables.

### Importation des données de zone cliquable {#importing-image-map-data}

Plutôt que de saisir les données de zone cliquable sur chacune des pages, vous avez la possibilité d’importer les données de l’ensemble de votre image, visionneuse à 360° ou catalogue électronique dans l’écran Résumé de zone cliquable. Vous importez les données de zone cliquable sous la forme d’un fichier délimité par des tabulations ou d’un fichier DTD XML. Les champs du fichier doivent être dans l’ordre indiqué sur l’écran de résumé de zone cliquable : Nom, Etiquettes de table des matières, Zones, URL, Texte de survol, Autres actions et Chaînes de recherche. Vous évitez ainsi d’avoir à saisir les données dans la liste de zones cliquables au fur et à mesure que vous créez ces dernières.

**Pour importer des données de zone cliquable:**

1. Aller à la page d’édition des zones cliquables (pour des images ou des images dans des visionneuses à 360°) ou l’onglet Pages de zones de l’écran d’édition du catalogue électronique.
1. Sélectionner **[!UICONTROL Importation de métadonnées]**.
1. Dans la boîte de dialogue Télécharger les métadonnées , sélectionnez Image ou Zone cliquable pour télécharger les métadonnées à partir du type de propriété de ressource souhaité.
1. Dans la liste déroulante Générer un fichier, sélectionnez le type de fichier que vous souhaitez créer.
1. (Facultatif) Sélectionnez **[!UICONTROL Générer]** pour prévisualiser les données obtenues en fonction du type de fichier que vous souhaitez créer. Sélectionner **[!UICONTROL Fermer]** pour revenir à la boîte de dialogue Télécharger les métadonnées .
1. Naviguez jusqu’au fichier que vous souhaitez télécharger. Dans le champ de texte Nom de fichier, spécifiez le nom du fichier généré.
1. (Facultatif) Dans le champ Nom de la tâche, spécifiez un nom pour la tâche de téléchargement des métadonnées.
1. Sélectionner **[!UICONTROL Télécharger]**.

### Copier des zones cliquables {#copying-image-maps}

Vous pouvez copier des zones cliquables d’une image (ou d’une page de catalogue électronique) à l’autre. Utilisation **[!UICONTROL Copier la zone cliquable]** pour commencer à les créer. Vous pouvez également copier les zones cliquables pour les recréer dans des images ou des pages partageant la mise en page ou la structure de mappage.

Par exemple, copier des zones cliquables dans un catalogue électronique permet de copier facilement toutes les zones cliquables entre les versions de langue étrangère du même catalogue électronique. Pour obtenir de meilleurs résultats, il est préférable d’effectuer une copie entre des catalogues électroniques ayant le même nombre de pages et les mêmes images. Si le catalogue électronique dans lequel vous copiez déjà contient des zones cliquables, ces zones cliquables sont supprimées lors de la copie.

**Pour copier des zones cliquables:**

1. Aller à la page d’édition des zones cliquables (pour des images ou des images dans des visionneuses à 360°) ou l’onglet Pages de zones de l’écran d’édition du catalogue électronique.
1. Sélectionner **[!UICONTROL Copier les mappages vers]**.
1. Effectuez l’une des opérations suivantes, selon que vous souhaitiez copier des zones cliquables à partir d’images ou à partir d’un catalogue électronique :

   * (Images) Dans l’écran Sélectionner des images, sélectionnez les images dans lesquelles vous souhaitez copier les zones cliquables.
   * (Catalogue électronique) Dans l’écran Sélectionner un fichier, sélectionnez les images ou les pages de catalogue électronique dans lesquelles vous souhaitez copier les zones cliquables.

1. Choisir **[!UICONTROL Sélectionner]**.

## Utiliser un modèle pour saisir du code JavaScript et des URL {#using-a-template-to-enter-javascript-and-urls}

Vous pouvez définir un modèle d’URL (également appelé modèle Href) pour faciliter et améliorer la saisie des URL de zones cliquables. Définissez un modèle d’URL si la plupart des URL des zones cliquables partagent un format commun et fixe. Si vous définissez la partie de l’URL fixe comme modèle d’URL, vous êtes dispensé de l’entrer chaque fois que vous créez une zone cliquable. Le modèle d’URL peut également contenir des commandes JavaScript, des chemins d’accès et des paramètres. Par défaut, le modèle d’URL contient un gestionnaire JavaScript Adobe Dynamic Media Classic propriétaire appelé `loadProduct` qui ouvre l’image dans une nouvelle fenêtre.

>[!NOTE]
>
>Lorsque vous ajoutez le code JavaScript dans l’attribut HREF de votre zone cliquable, celui-ci est exécuté sur l’ordinateur du client. Par conséquent, assurez-vous que le code JavaScript est sécurisé.

### A propos des modèles d’URL {#about-url-templates}

Avec un modèle d’URL, le contenu de la colonne URL dans la liste Zone cliquable est remplacé par le double signe dollar ($$) dans le modèle :

```as3
Javascript:loadProduct(‘$$’);void(0);
```

Vous placez toutes les valeurs qui ne changent pas entre les zones cliquables dans le modèle d’URL. N’ajoutez que les valeurs variables dans la colonne URL de la liste Zone cliquable. Par exemple :

* Modèle d’URL - `javascript:loadProduct(‘https://www.examplesitehere.com/$$’);void(0);`
* Valeur d’URL - `product.htm`
* URL réelle générée - `javascript:loadProduct(‘https://www.examplesitehere.com/product.html);void(0);`

Par défaut, le modèle d’URL comprend un gestionnaire JavaScript Adobe Dynamic Media Classic propriétaire appelé `loadProduct` qui ouvre une nouvelle fenêtre avec la destination de l’URL. Cependant, vous pouvez utiliser n’importe quel code JavaScript pour remplacer ce gestionnaire JavaScript ou utiliser l’un des gestionnaires Adobe Dynamic Media Classic suivants :

* `loadProductCW` - Affiche l’URL cible spécifiée dans la colonne URL de la fenêtre active. Ce code est réservé principalement aux catalogues électroniques intégrés dans une page d’un site Web.

* `loadProductPW` - Affiche l’URL cible spécifiée dans la colonne URL de la fenêtre parente (la page d’où la page active a été ouverte). La fenêtre active reste ouverte, mais la fenêtre parent change pour afficher l’URL cible.

   >[!NOTE]
   >
   >Le code `loadProductPW` ne prend pas en charge les visionneuses DHTML et HTML5.

### Création d’un modèle d’URL {#creating-a-url-template}

1. Sur l’écran Editeur de zone cliquable (images ou visionneuses à 360°) ou l’onglet Pages de zones de l’écran Catalogue électronique (catalogues électroniques), cliquez sur Modifier en regard de l’option Modèle d’URL. La boîte de dialogue Modifier le modèle de zone apparaît.
1. Entrez le code JavaScript et l’URL complète (en remplaçant la partie variable par le double signe dollar [$$]). Vous pouvez coller le code en cliquant avec le bouton droit de la souris et en choisissant **[!UICONTROL Coller]**.
1. Sélectionner **[!UICONTROL Enregistrer]**.

### Gestion des modèles d’URL {#handling-url-templates}

La page Editeur de zone cliquable (images et visionneuses à 360°) et l’onglet Pages de zones de l’écran Catalogue électronique (catalogues électroniques) contiennent les commandes de gestion des modèles d’URL suivantes :

* **Option Modèle d’URL** - Sélectionnez l’option Modèle d’URL pour appliquer votre modèle d’URL à toutes les zones cliquables d’une image ou d’une page de catalogue électronique.

* **Option Modèle** - Désélectionnez une option Modèle dans la liste Zone cliquable des URL si vous ne souhaitez pas qu’une zone cliquable individuelle utilise le modèle d’URL.

## Définition d’autres actions pour les zones cliquables {#defining-other-actions-for-image-maps}

Vous pouvez sélectionner la variable **[!UICONTROL Afficher]** et choisissez **[!UICONTROL Autres actions]** pour déclencher des actions autres que le texte de survol et les lancements de pages web. Lorsque l’utilisateur amène le pointeur sur une zone cliquable, vous pouvez initier une action. Ces actions sont des attributs définis pour les zones cliquables côté client conformément aux spécifications HTML du consortium WWW (World Wide Web). Elles comptent notamment :

* **`accesskey`** - Déclenche une action lorsque l’utilisateur appuie sur la touche spécifiée du clavier.

* **`onfocus`** - Déclenche un événement lorsque la zone cliquable devient active grâce au curseur, à une tabulation ou à une touche d’accès. Par exemple, vous pouvez lancer une page Web lorsque la zone cliquable devient active et la refermer lorsqu’elle ne l’est plus.

* **`onblur`** - Déclenche un événement lorsque la zone cliquable n’est plus active, grâce au curseur ou à la tabulation.

**Pour définir d’autres actions pour les zones cliquables:**

1. Sur l’écran de l’éditeur de cartes (images et visionneuses à 360°) ou de l’onglet Pages de cartes de l’écran Catalogue électronique (catalogues électroniques), sélectionnez l’option **[!UICONTROL Afficher]** et sélectionnez **[!UICONTROL Autres actions]**.
1. Selon la syntaxe conforme aux spécifications HTML du consortium WWW (World Wide Web), ajoutez les attributs pris en charge dans la colonne Autres actions de la liste Zone cliquable.
1. Sélectionner **[!UICONTROL Enregistrer]**.

Sélectionnez la **[!UICONTROL Afficher]** et sélectionnez **[!UICONTROL Les]** si vous souhaitez qu’une zone cliquable comporte un texte de survol et une action.

## Création de zones cliquables dans Adobe Acrobat ou Adobe InDesign {#creating-image-maps-in-adobe-acrobat-or-adobe-indesign}

Vous pouvez créer des zones cliquables lors de la conception de votre catalogue électronique dans Adobe Acrobat ou Adobe InDesign.

Dans Adobe Acrobat ou Adobe InDesign, créez des références de lien hypertexte à l’emplacement où vous souhaitez que les zones cliquables apparaissent, puis spécifiez l’emplacement des URL de la zone cliquable. Lorsque vous sélectionnez l’option Extract Links (Extraire les liens) lors du téléchargement du fichier du PDF dans Adobe Dynamic Media Classic, les liens sont automatiquement convertis en zones cliquables.

Pour plus d’informations, voir Aide d’Adobe InDesign ou Aide d’Adobe Acrobat.

### Création de zones cliquables dans Adobe InDesign {#to-create-image-maps-in-adobe-indesign}

1. Dans Adobe InDesign, accédez à **[!UICONTROL Windows®]** > **[!UICONTROL Interactif]** > **[!UICONTROL Hyperliens]**.
1. Dans le panneau Hyperliens, sélectionnez le texte, le cadre ou le graphique à transformer en zone cliquable.
1. Sélectionner **[!UICONTROL Nouveau lien hypertexte]** dans le menu du panneau.
1. Dans la boîte de dialogue Nouveau lien hypertexte, dans la **[!UICONTROL Lier à]** menu, choisissez **[!UICONTROL URL]**.
1. Saisissez ou collez l’ID du produit dans la zone URL.
1. Sélectionner **[!UICONTROL OK]**. (Adobe Dynamic Media Classic complète l’URL à l’aide du modèle d’URL de zone cliquable.)

   >[!NOTE]
   >
   >Vous n’avez pas besoin de définir les options d’aspect dans Adobe InDesign. Vous pouvez spécifier l’aspect dans Adobe Dynamic Media Classic.

1. Répétez les étapes 2 à 6 pour toutes les zones cliquables que vous souhaitez créer.
1. Exportez les fichiers au format PDF.
1. Téléchargez le PDF vers Adobe Dynamic Media Classic.
1. Dans **[!UICONTROL Options de PDF]**, sélectionnez **[!UICONTROL Extraction de liens]**.

### Création de zones cliquables dans Adobe Acrobat {#to-create-image-maps-in-adobe-acrobat}

1. Dans Adobe Acrobat, accédez à **[!UICONTROL Outils]** > **[!UICONTROL Modification avancée]** > **[!UICONTROL Outil Lien]**.
1. Faites glisser la souris pour créer la zone cliquable.
1. Dans la zone Créer un lien , sélectionnez **[!UICONTROL Lien personnalisé]**, puis sélectionnez **[!UICONTROL Suivant]**.

>[!NOTE]
>
>Vous n’avez pas besoin de définir les options d’aspect dans Adobe Acrobat. Vous pouvez spécifier l’aspect dans Adobe Dynamic Media Classic.

1. Dans la zone Propriétés du lien , sélectionnez **[!UICONTROL Actions]**.
1. Sélectionner **[!UICONTROL Ouvrir Un Lien Web]** dans le menu Sélectionner une action , puis sélectionnez **[!UICONTROL Ajouter]**.
1. Saisissez l’ID du produit pour la zone Zone cliquable dans la zone Modifier l’URL, puis sélectionnez **[!UICONTROL OK]**. (Adobe Dynamic Media Classic complète l’URL à l’aide du modèle d’URL de zone cliquable.)
1. Répétez les étapes 1 à 7 pour toutes les zones cliquables que vous souhaitez créer.
1. Enregistrez le fichier.
1. Téléchargez le PDF dans Adobe Dynamic Media Classic et sélectionnez Extraire les liens dans les options du PDF.
