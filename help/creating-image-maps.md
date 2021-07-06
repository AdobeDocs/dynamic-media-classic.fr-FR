---
title: Création de zones cliquables
description: Découvrez comment créer des zones cliquables.
uuid: 0dcc4956-006e-4a74-9d6a-6d4bb23790ce
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4eddf983-38cb-4f00-b3be-85c20bdd6f69
feature: Dynamic Media Classic,Gestion des ressources
role: User
exl-id: deafbd03-06bc-4d7e-87a1-5620ebcac426
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '2427'
ht-degree: 62%

---

# Création de zones cliquables{#creating-image-maps}

Une zone cliquable est une partie d’une image, d’une page de catalogue électronique ou d’une image dans une visionneuse à 360°, qui affiche un panneau de survol avec du texte. Une action est déclenchée lorsque l’utilisateur clique sur une zone cliquable. Par exemple, une page Web affiche des informations détaillées sur un produit. Un contour s’affiche autour d’une zone cliquable lorsque l’utilisateur déplace le pointeur dessus.

Outre la possibilité de créer des zones cliquables dans Dynamic Media Classic, vous pouvez également créer des zones cliquables lorsque vous créez un catalogue dans Adobe Acrobat ou Adobe InDesign.

Lorsque vous créez des zones cliquables, vous pouvez effectuer l’une des opérations suivantes :

* Saisir un texte de survol.
* Saisissez JavaScript™ et les URL pour lancer les pages web.
* Créer des modèles d’URL pour les zones cliquables.
* Copier des zones cliquables dans d’autres images, pages de catalogue électronique ou images dans une visionneuse à 360°.
* Exporter des zones cliquables au format CSV ou XML.
* Importez des métadonnées d’image à partir d’un fichier délimité par des tabulations ou d’un fichier XML.
* Définir d’autres actions conformément aux directives du consortium WWW (World Wide Web).
* Prévisualiser des zones cliquables.

## Création et modification d’une zone cliquable {#drawing-and-adjusting-an-image-map}

1. Effectuez l’une des opérations suivantes :

   * Si vous utilisez une image en mode Affichage de la grille ou Liste, dans la liste déroulante Modifier , cliquez sur **Zone cliquable**. Vous pouvez également l’ouvrir dans la vue Détails, puis cliquer sur **Zone cliquable** au-dessus de l’image.
   * Si vous utilisez une visionneuse à 360° en mode Grille ou Liste, cliquez sur **Modifier**. Vous pouvez également l’ouvrir dans la vue Détails, puis cliquer sur **Modifier**. Sélectionnez un fichier image, puis cliquez sur **Zone cliquable**.
   * Si vous utilisez un catalogue électronique, en mode Grille, Liste et Détails, cliquez sur **Modifier**. Cliquez sur l’onglet **Pages de mappage** .

   ![](assets/ma_image_map.png)

1. Tracez une zone cliquable rectangulaire ou polygonale (avec de nombreux côtés) :

   **** Zone rectangulaire : sélectionnez l’outil Zone cliquable de rectangle et faites glisser sur la page pour créer le rectangle. Pour ajouter un point à un rectangle et en faire un polygone, appuyez sur la touche Ctrl, placez l’outil d’insertion à l’endroit souhaité, puis cliquez.

   **Polygonal** map : sélectionnez l’outil de zone cliquable polygonal et cliquez sur les points du périmètre de la zone de l’image à fermer. A l’aide du curseur de densité du polygone, modulez la densité du point. La densité initiale est conservée si vous sélectionnez d’autres zones. En revanche, si vous ajoutez, supprimez ou modifiez un point du polygone, la densité initiale est perdue et le curseur revient à la valeur maximale.

1. Nommez la zone cliquable, si vous le souhaitez, dans la liste Zone cliquable. Après avoir dessiné une zone cliquable, Dynamic Media Classic lui attribue un nom.

   Pour créer le nom, Dynamic Media Classic ajoute un numéro séquentiel au nom de l’image ou de la page de catalogue électronique que vous utilisez. Vous pouvez indiquer le nom de votre choix.

1. Si vous souhaitez permettre aux utilisateurs d’accéder à une nouvelle page Web lorsqu’ils cliquent sur la zone cliquable, indiquez l’URL correspondante dans la liste Zone cliquable.

   Voir [pour saisir du code JavaScript™ et des URL](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. Pour qu’un texte de survol s’affiche lorsque les utilisateurs déplacent le pointeur sur la zone cliquable, saisissez le texte dans la liste Zone cliquable. Dans la liste Zone cliquable, sélectionnez le menu Afficher, puis choisissez l’option Texte de survol. Ensuite, entrez le texte que vous souhaitez présenter à l’écran aux utilisateurs. Vous pouvez rédiger le texte dans une application de traitement de texte et le copier dans le champ Texte de survol.
1. Si vous souhaitez qu’une autre action se déclenche lorsque les utilisateurs déplacent la souris sur une zone cliquable, définissez l’action. Dans la liste déroulante Afficher, cliquez sur Autres actions. Spécifiez les attributs de l’action. (Cliquez sur Afficher > Les deux pour créer un texte de survol et une action pour une zone cliquable.)

   Voir [Définition d’autres actions relatives aux zones cliquables](creating-image-maps.md#defining_other_actions_for_image_maps).

1. (Facultatif) Utilisez l’une des méthodes suivantes :

   * Pour prévisualiser les zones cliquables, cliquez sur **[!UICONTROL Aperçu]**.
   * Pour supprimer une zone cliquable ou un sommet polygone, sélectionnez une forme sur l’image, puis cliquez sur **[!UICONTROL Supprimer]**. Ou, pour un catalogue électronique, dans l’onglet Ordre des pages, cliquez sur **[!UICONTROL Effacer les zones]** pour supprimer les zones cliquables de toutes les pages.
   * Pour retirer provisoirement une zone cliquable d’une image, d’une image dans une visionneuse à 360° ou d’une page de catalogue électronique sans la supprimer, désélectionnez l’option Oui appropriée dans la liste Zone cliquable.

1. Cliquez sur **[!UICONTROL Enregistrer]**.

### Ajustement de la position, de la forme et de la taille des zones cliquables {#adjusting-the-position-shape-and-size-of-image-maps}

Pour modifier la position, la forme et la taille d’une zone cliquable, cliquez sur le bouton Zone cliquable. Sélectionnez ensuite l’outil **[!UICONTROL Panoramique]** et suivez les instructions suivantes :

**Modification de la position**  : déplace le pointeur près de la bordure de la zone cliquable, mais pas dessus. Lorsque le pointeur prend la forme d’une flèche à quatre pointes, faites glisser la zone à l’emplacement voulu.

**Modification de la taille et de la forme**  : la manière dont vous modifiez la forme et la taille d’une zone cliquable varie selon que vous utilisez une zone cliquable rectangulaire ou polygonal :

>[!TIP]
>
>Vous pouvez faire glisser le curseur Taille situé dans la partie inférieure de l’écran pour modifier les vues et avoir une idée plus précise de l’aspect de votre zone cliquable.

**Zone cliquable rectangulaire**  : déplace le pointeur sur un côté ou un coin de la zone cliquable. Lorsque le pointeur prend la forme d’une flèche à double pointe, faites glisser la souris. Maintenez la touche Maj enfoncée lorsque vous faites glisser la souris pour modifier la taille tout en conservant le format (la forme).

**Zone cliquable polygonale**  : faites glisser une poignée de sélection carrée. Pour obtenir une poignée de sélection, cliquez sur la bordure de la zone cliquable, puis commencez à la faire glisser.

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

Vous pouvez copier des zones cliquables d’une image (ou d’une page de catalogue électronique) à l’autre. Utilisez **[!UICONTROL Copier la carte d’image]** pour commencer à les créer d’une manière anticipée. Vous pouvez également copier les zones cliquables afin de les recréer dans des images ou des pages qui partagent la même disposition ou structure de mappage. 

Par exemple, copier des zones cliquables dans un catalogue électronique permet de copier facilement toutes les zones cliquables entre les versions de langue étrangère du même catalogue électronique. Pour obtenir de meilleurs résultats, il est préférable d’effectuer une copie entre des catalogues électroniques ayant le même nombre de pages et les mêmes images. Si le catalogue électronique dans lequel vous copiez déjà contient des zones cliquables, ces zones cliquables sont supprimées lors de la copie.

**Pour copier des zones cliquables**

1. Aller à la page d’édition des zones cliquables (pour des images ou des images dans des visionneuses à 360°) ou l’onglet Pages de zones de l’écran d’édition du catalogue électronique.
1. Cliquez sur Copier les zones dans.
1. Effectuez l’une des opérations suivantes, selon que vous souhaitiez copier des zones cliquables à partir d’images ou à partir d’un catalogue électronique :

   * (Images) Dans l’écran Sélectionner des images, sélectionnez les images dans lesquelles vous souhaitez copier les zones cliquables.
   * (Catalogue électronique) Dans l’écran Sélectionner un fichier, sélectionnez les images ou les pages de catalogue électronique dans lesquelles vous souhaitez copier les zones cliquables.

1. Cliquez sur Sélectionner.

## Utilisation d’un modèle pour saisir du code JavaScript™ et des URL {#using-a-template-to-enter-javascript-and-urls}

Vous pouvez définir un modèle d’URL (également appelé modèle Href) pour faciliter et améliorer la saisie des URL de zones cliquables. Définissez un modèle d’URL si la plupart des URL des zones cliquables partagent un format commun et fixe. Si vous définissez la partie de l’URL fixe comme modèle d’URL, vous êtes dispensé de l’entrer chaque fois que vous créez une zone cliquable. Votre modèle d’URL peut également contenir des commandes JavaScript™, des noms de chemin d’accès et des paramètres. Par défaut, le modèle d’URL contient un gestionnaire JavaScript™ Dynamic Media Classic propriétaire appelé `loadProduct` qui ouvre l’image dans une nouvelle fenêtre.

>[!NOTE]
>
>Lorsque vous ajoutez le code JavaScript™ dans l’attribut HREF de votre zone cliquable, celui-ci est exécuté sur l’ordinateur du client. Par conséquent, assurez-vous que le code JavaScript™ est sécurisé.

### A propos des modèles d’URL {#about-url-templates}

Avec un modèle d’URL, le contenu de la colonne URL dans la liste Zone cliquable est remplacé par le double signe dollar ($$) dans le modèle :

```as3
Javascript:loadProduct(‘$$’);void(0);
```

Vous placez toutes les valeurs qui ne changent pas entre les zones cliquables dans le modèle d’URL. N’ajoutez que les valeurs variables dans la colonne URL de la liste Zone cliquable. Par exemple :

* Modèle d’URL : j `avascript:loadProduct(‘https://www.examplesitehere.com/$$’);void(0);`
* Valeur d’URL : `product.htm`
* URL réelle générée : `javascript:loadProduct(‘https://www.examplesitehere.com/product.html);void(0);`

Par défaut, le modèle d’URL comprend un gestionnaire JavaScript™ Dynamic Media Classic propriétaire appelé `loadProduct` qui ouvre une nouvelle fenêtre avec la destination de l’URL. Cependant, vous pouvez utiliser n’importe quel code JavaScript™ pour remplacer ce gestionnaire JavaScript™ ou utiliser l’un des gestionnaires Dynamic Media Classic suivants :

* `loadProductCW`

   Affiche l’URL cible spécifiée dans la colonne URL de la fenêtre active. Ce code est réservé principalement aux catalogues électroniques intégrés dans une page d’un site Web.

* `loadProductPW`

   Affiche l’URL cible spécifiée dans la colonne URL de la fenêtre parente (la page d’où la page active a été ouverte). La fenêtre active reste ouverte, mais la fenêtre parent change pour afficher l’URL cible.

   >[!NOTE]
   >
   >Le code `loadProductPW` ne prend pas en charge les visionneuses DHTML et HTML5.

### Création d’un modèle d’URL {#creating-a-url-template}

Pour créer un modèle d’URL, procédez comme suit :

1. Sur l’écran Editeur de zone cliquable (images ou visionneuses à 360°) ou l’onglet Pages de zones de l’écran Catalogue électronique (catalogues électroniques), cliquez sur Modifier en regard de l’option Modèle d’URL. La boîte de dialogue Modifier le modèle de zone apparaît.
1. Saisissez le code JavaScript™ et l’URL complète (avec la partie variable remplacée par des signes dollar [$]). Vous pouvez coller le code en cliquant avec le bouton droit de la souris et en choisissant l’option Coller.
1. Cliquez sur le bouton Enregistrer.

### Gestion des modèles d’URL {#handling-url-templates}

La page Editeur de zone cliquable (images et visionneuses à 360°) et l’onglet Pages de zones de l’écran Catalogue électronique (catalogues électroniques) contiennent les commandes de gestion des modèles d’URL suivantes :

* **** Option Modèle d’URL : sélectionnez l’option Modèle d’URL pour appliquer votre modèle d’URL à toutes les zones cliquables d’une image ou d’une page de catalogue électronique.

* **** Option Modèle : désélectionnez une option Modèle dans la liste Zone cliquable des URL si vous ne souhaitez pas qu’une zone cliquable individuelle utilise le modèle d’URL.

## Définition d’autres actions relatives aux zones cliquables {#defining-other-actions-for-image-maps}

Dans le menu Afficher, choisissez Autres actions pour déclencher des actions autres que le texte de survol et le lancement d’une page Web. Lorsque l’utilisateur amène le pointeur sur une zone cliquable, vous pouvez initier une action. Ces actions sont des attributs définis pour les zones cliquables côté client conformément aux spécifications HTML du consortium WWW (World Wide Web). Elles comptent notamment :

* **touche d’accès**  : déclenche une action lorsque l’utilisateur appuie sur une touche désignée du clavier.

* **onfocus**  : déclenche un événement lorsque la zone cliquable reçoit le focus, par le curseur, par tabulation ou en appuyant sur une touche d’accès. Par exemple, vous pouvez lancer une page Web lorsque la zone cliquable devient active et la refermer lorsqu’elle ne l’est plus.

* **onblur**  : déclenche un événement lorsque la zone cliquable n’est plus sélectionnée, que ce soit par le curseur ou par la tabulation.

**Pour définir d’autres actions pour les zones cliquables:**

1. Sur l’écran Editeur de zone cliquable (images et visionneuses à 360°) ou l’onglet Pages de zones de l’écran Catalogue électronique (catalogues électroniques), sélectionnez le menu Afficher, puis choisissez Autres actions.
1. Selon la syntaxe conforme aux spécifications HTML du consortium WWW (World Wide Web), ajoutez les attributs pris en charge dans la colonne Autres actions de la liste Zone cliquable.
1. Cliquez sur **[!UICONTROL Enregistrer]**.

Sélectionnez le menu **[!UICONTROL Afficher]** et choisissez **[!UICONTROL Les deux]** si vous souhaitez qu’une zone cliquable comporte un texte de survol et une action.

## Création de zones cliquables dans Adobe Acrobat ou Adobe InDesign {#creating-image-maps-in-adobe-acrobat-or-adobe-indesign}

Vous pouvez créer des zones cliquables lors de la conception de votre catalogue électronique dans Adobe Acrobat ou Adobe InDesign.

Dans Acrobat ou InDesign, créez un lien hypertexte à l’emplacement auquel vous souhaitez faire apparaître la zone cliquable et spécifiez l’URL à laquelle elle doit renvoyer. Lorsque vous sélectionnez l’option Extract Links (Extraire les liens) lors du téléchargement du fichier PDF dans Dynamic Media Classic, les liens sont automatiquement convertis en zones cliquables.

Pour plus d’informations, voir Aide d’Adobe InDesign ou Aide d’Adobe Acrobat.

### Création de zones cliquables dans Adobe InDesign {#to-create-image-maps-in-adobe-indesign}

1. Dans InDesign, cliquez sur **[!UICONTROL Windows®]** > **[!UICONTROL Interactive]** > **[!UICONTROL Hyperliens]** pour ouvrir le panneau Hyperliens.
1. Sélectionnez le texte, le bloc ou le graphique que vous souhaitez transformer en zone cliquable.
1. Dans le panneau Hyperliens, cliquez sur **[!UICONTROL Nouvel hyperlien]** dans le menu du panneau.
1. Dans la boîte de dialogue Nouvel hyperlien, sélectionnez **[!UICONTROL URL]** dans le menu Lien vers .
1. Saisissez ou collez l’ID du produit dans la zone URL, puis cliquez sur **[!UICONTROL OK]**. (Dynamic Media Classic complète l’URL à l’aide du modèle d’URL de zone cliquable.)

   >[!NOTE]
   >
   >Vous n’avez pas besoin de définir les options d’aspect dans Adobe InDesign. Vous pouvez spécifier l’aspect dans Dynamic Media Classic.

1. Répétez les étapes 2 à 5 pour toutes les zones cliquables que vous souhaitez créer.
1. Exportez les fichiers au format PDF.
1. Téléchargez le fichier PDF dans Dynamic Media Classic et sélectionnez Extract Links from PDF Options.

### Création de zones cliquables dans Adobe Acrobat {#to-create-image-maps-in-adobe-acrobat}

1. Dans Acrobat, cliquez sur **[!UICONTROL Outils]** > **[!UICONTROL Modification avancée]** > **[!UICONTROL Outil de lien]**.
1. Faites glisser la souris pour créer la zone cliquable. La boîte de dialogue Créer un lien s’ouvre.
1. Sélectionnez **[!UICONTROL Lien personnalisé]**, puis cliquez sur **[!UICONTROL Suivant]**.

>[!NOTE]
>
>Vous n’avez pas besoin de définir les options d’aspect dans Adobe Acrobat. Vous pouvez spécifier l’aspect dans Dynamic Media Classic.

1. Dans la zone Propriétés du lien, cliquez sur **[!UICONTROL Actions]**.
1. Sélectionnez **[!UICONTROL Ouvrir un lien Web]** dans le menu Sélectionner une action , puis cliquez sur **[!UICONTROL Ajouter]**.
1. Saisissez l’ID du produit pour la zone Zone cliquable dans la zone Modifier l’URL, puis cliquez sur **[!UICONTROL OK]**. (Dynamic Media Classic complète l’URL à l’aide du modèle d’URL de zone cliquable.)
1. Répétez les étapes 1 à 7 pour toutes les zones cliquables que vous souhaitez créer.
1. Enregistrez le fichier.
1. Téléchargez le fichier PDF dans Dynamic Media Classic et sélectionnez Extract Links from PDF Options.
