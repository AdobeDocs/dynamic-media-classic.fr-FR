---
title: Créer des zones cliquables de catalogue électronique
description: Découvrez comment créer des zones cliquables de catalogue électronique dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 5e7f39a5-36a6-40df-8752-064a582c9346
topic: Integrations, Development
level: Experienced
source-git-commit: c4613c78347c4bda3d84747a72146617158c03b6
workflow-type: tm+mt
source-wordcount: '1494'
ht-degree: 26%

---

# Créer des zones cliquables de catalogue électronique{#creating-ecatalog-image-maps}

Une zone cliquable est une zone d’une page de catalogue électronique que vous pouvez survoler à l’aide de la souris ou sélectionner pour déclencher différents types d’actions. Lorsque vous déplacez le pointeur sur une zone cliquable, par exemple, une description d’élément sous forme de texte de survol s’affiche. Lorsque vous sélectionnez une zone cliquable, une autre action est lancée. Par exemple, vous pouvez ouvrir une page web pour que les visiteurs puissent en savoir plus sur un article ou l’acheter, ou vous pouvez lancer une vidéo pour voir un article en cours d’utilisation.

## Dessiner des zones cliquables de catalogue électronique {#drawing-ecatalog-image-maps}

Vous dessinez les zones cliquables des catalogues sur l’onglet Pages de zones de l’écran Catalogue électronique. Cet écran contient une section Zone cliquable dans laquelle les pages du catalogue électronique sont affichées, ainsi qu’une liste des zones cliquables, à droite. Lorsque vous créez des zones cliquables, leur nom est saisi dans la liste Zone cliquable .

1. Sélectionnez le bouton de substitution du catalogue électronique **[!UICONTROL Modifier]**.
1. Sélectionnez **[!UICONTROL Mapper des pages]**.
1. Sur le côté gauche de l’écran Pages de zones, sélectionnez la page souhaitée.
1. Dans la section Zone cliquable, tracez une zone rectangulaire ou polygonale (à plusieurs côtés) :

   * **Zone rectangulaire** : sélectionnez l’outil Rectangle Image Map et faites glisser le pointeur sur la page pour créer le rectangle.

   * **Zone polygonale** : sélectionnez l’outil Zone cliquable polygonale, puis sélectionnez autant de fois que nécessaire autour du périmètre de l’image. Au fur et à mesure que vous sélectionnez, Adobe Dynamic Media Classic dessine les bordures de la zone cliquable.

     Après avoir dessiné une zone cliquable, Adobe Dynamic Media Classic lui attribue un nom dans la liste Zone cliquable. Pour former le nom, Adobe Dynamic Media Classic ajoute un numéro séquentiel au nom de la page de catalogue électronique dans laquelle vous travaillez.

1. (Facultatif) Dans la liste Zone cliquable de la colonne [!UICONTROL Nom], vous pouvez saisir un nouveau nom pour la zone cliquable. N’insérez pas d’espaces dans le nom que vous saisissez.
1. Les visiteurs peuvent ouvrir une nouvelle page web lorsqu’ils sélectionnent la zone cliquable. Dans le panneau Liste de zones cliquables, saisissez l’URL de la page web dans la colonne URL.

   Pour faciliter la saisie des URL (modèles Href), sélectionnez **[!UICONTROL Modifier]** et saisissez un modèle.

Voir [Utiliser un modèle pour saisir le JavaScript et les URL](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. (Facultatif) Dans la liste déroulante Afficher, sélectionnez **[!UICONTROL Texte de survol]**, puis saisissez le texte que vous souhaitez que les utilisateurs voient à l’écran lorsqu’ils déplacent leurs pointeurs sur la zone cliquable.
1. (Facultatif) Dans la liste déroulante Afficher, sélectionnez **[!UICONTROL Autres actions]** et saisissez un attribut pour déclencher une action de flou ou de mise au point lorsque les utilisateurs déplacent leurs pointeurs sur une zone cliquable.

   Voir [Définition d’autres actions pour les zones cliquables](creating-image-maps.md#defining_other_actions_for_image_maps).

1. Sélectionnez **[!UICONTROL Enregistrer]**.
1. (Facultatif) Sélectionnez **[!UICONTROL Aperçu]** pour afficher le catalogue électronique avec le paramètre prédéfini de la visionneuse de catalogue électronique.

Pour supprimer une zone cliquable, sélectionnez son nom dans la liste Zone cliquable et sélectionnez **[!UICONTROL Supprimer]**. Vous pouvez temporairement désactiver une zone cliquable sur une page sans supprimer la zone cliquable. Sélectionnez l’option Zones cliquables activées dans le panneau Liste des zones cliquables.

## Incorporation de contenu multimédia enrichi dans un catalogue électronique {#embedding-rich-media-in-an-ecatalog}

Vous pouvez utiliser l’option Média enrichi du catalogue électronique pour ajouter des vidéos au format MP4 ou des visionneuses à 360° aux zones cliquables que vous avez ajoutées à un catalogue électronique. Lorsqu’un utilisateur sélectionne la zone Zone cliquable dans le catalogue électronique, la visionneuse à 360° ou la vidéo associée s’affiche. Cette fonctionnalité est particulièrement utile si vous souhaitez que les clients puissent voir un élément en cours d’utilisation ou le voir sous d’autres angles et perspectives.

Vous pouvez également afficher de manière facultative le texte de l’info-bulle lorsque les clients déplacent leurs pointeurs sur votre zone cliquable afin de savoir ce qu’ils sélectionnent.

**Pour incorporer des médias riches dans un catalogue électronique, procédez comme suit**

1. Tracez une zone cliquable dans un catalogue électronique.

   Voir [Dessiner des zones cliquables de catalogue électronique](creating-ecatalog-image-maps.md#drawing_ecatalog_image_maps).

1. Dans la liste déroulante Afficher, sélectionnez **[!UICONTROL Média enrichi]**.
1. Dans le panneau Ajouter Assets sur la gauche, accédez à un dossier contenant la visionneuse à 360° ou la ressource vidéo (format MP4) à incorporer.
1. Faites glisser le fichier sur la zone cliquable.
1. (Facultatif) Dans le panneau Liste de zones cliquables, sous l’en-tête de colonne **[!UICONTROL Info-bulle]**, saisissez le texte que vous souhaitez que les visiteurs voient à l’écran lorsqu’ils placent leur pointeur sur la zone cliquable.
1. Sélectionnez **[!UICONTROL Enregistrer]**.

## Edition des zones cliquables d’un catalogue électronique {#editing-ecatalog-image-maps}

En commençant par l’onglet Pages de zones de l’écran Catalogue électronique, utilisez ces techniques pour éditer les zones cliquables d’un catalogue électronique :

* **Ajuster la position** : sélectionnez l’outil Panoramique et déplacez le pointeur près de la bordure de la carte, mais pas au-dessus. Lorsque le pointeur affiche une flèche à quatre pointes, faites glisser l’ensemble de la zone cliquable vers un nouvel emplacement.

  Voir [Réglage de la position, de la forme et de la taille des zones cliquables](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

* **Modifier la forme et la taille** : pour redimensionner une zone cliquable rectangulaire, sélectionnez l’outil Panoramique. Puis déplacez le pointeur au-dessus d’une ligne de bordure ou d’un coin, et lorsque vous voyez apparaître l’icône en forme de flèche à deux pointes, faites glisser. Pour redimensionner une zone cliquable polygonale, faites glisser une poignée de sélection carrée. Pour créer une poignée de sélection, sélectionnez la bordure de la zone cliquable et faites glisser.

  Voir [Réglage de la position, de la forme et de la taille des zones cliquables](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

* **Suppression de zones cliquables** : sélectionnez l’outil Panoramique, sélectionnez la zone cliquable pour la sélectionner, puis sélectionnez **[!UICONTROL Supprimer]**.

  Pour supprimer toutes les zones cliquables d’un catalogue électronique, sélectionnez l’onglet **[!UICONTROL Classer les pages]**, puis sélectionnez **[!UICONTROL Effacer les zones cliquables]**.

* **Gestion des zones cliquables se chevauchant** : faites glisser l’élément pour modifier l’ordre des zones cliquables dans la liste des zones cliquables.

  Voir [Gérer les zones cliquables se chevauchant](creating-image-maps.md#handling_overlapping_image_maps).

* **Copie de zones cliquables vers d’autres pages** : sélectionnez **[!UICONTROL Copier les zones cliquables vers]** (vérifiez que vous êtes sur l’onglet Mapper des pages). Sur l’écran de sélection des images, sélectionnez la ou les pages où vous souhaitez copier les zones cliquables, puis sélectionnez **[!UICONTROL Sélectionner]**.

  Voir [Copier des zones cliquables dans d’autres images](creating-image-maps.md#copying_image_maps).

>[!NOTE]
>
>Lorsque vous copiez des zones cliquables dans différentes pages d’un catalogue électronique, vous pouvez copier toutes les zones cliquables d’un catalogue électronique dans un autre catalogue électronique. Voir [Copier des zones cliquables parmi d’autres catalogues électroniques](creating-ecatalog-image-maps.md#copying_image_maps_between_ecatalogs).

## Vérifier et importer des données de zone cliquable {#reviewing-and-importing-image-map-data}

L’écran de résumé de zone cliquable fournit des métadonnées concernant votre catalogue électronique. Il permet également l’importation par lots des données de zone cliquable pour votre catalogue électronique. Cette méthode d’importation des données facilite la saisie des URL et du texte de survol des zones cliquables.

Pour afficher l’écran Mapper le résumé, dans l’onglet Mapper les pages de l’écran Catalogue électronique, sélectionnez **[!UICONTROL Résumé]**.

### Vérification du résumé des données de zone cliquable {#review-image-map-data-summary}

1. Sur l’écran Mapper des pages, sélectionnez **[!UICONTROL Résumé]**.

   L’écran Résumé de la carte affiche le nombre de zones cliquables, d’URL, de descriptions de texte de survol et d’autres actions figurant dans votre catalogue électronique.

1. Si des erreurs de clé de survol se produisent, sélectionnez-les dans la colonne **[!UICONTROL Erreur Rollover_Key]** pour voir ce qui doit être modifié dans votre feuille de calcul pour corriger l&#39;erreur. Vous pouvez sélectionner et copier le texte contenu dans ce message et le coller dans la feuille de calcul.
1. Sélectionnez **[!UICONTROL Aperçu]** afin de pouvoir examiner une page dans la visionneuse de catalogue électronique. Sélectionnez X pour fermer l’écran Résumé et revenir à l’écran Mapper des pages, ou sélectionnez **[!UICONTROL Fermer]** pour revenir à Parcourir.

### Importation des données de zone cliquable {#import-image-map-data}

Plutôt que de saisir les données de zone cliquable sur chacune des pages, vous avez la possibilité d’importer les données de l’ensemble de votre catalogue électronique dans l’écran de résumé de zone cliquable. Vous importez les données de zone cliquable sous la forme d’un fichier délimité par des tabulations ou d’un fichier DTD XML. Les champs du fichier doivent être dans l’ordre indiqué sur l’écran de résumé de zone cliquable : Nom, Etiquettes de table des matières, Zones, URL, Texte de survol, Autres actions et Chaînes de recherche. L’importation de données de zone cliquable vous évite de saisir les données dans la liste des zones cliquables au fur et à mesure de leur création.

>[!NOTE]
>
>vous devez avoir créé les zones cliquables avant d’importer les données correspondantes.

Depuis l’écran de résumé de zone cliquable, procédez comme suit pour importer les données des zones cliquables que vous avez créées :

1. Sélectionnez **[!UICONTROL Importer les données de mappage]**.
1. Dans la boîte de dialogue Importer des métadonnées, sélectionnez **[!UICONTROL Parcourir]**, puis sélectionnez le fichier DTD XML ou délimité par des tabulations.
1. Dans le champ Nom de la tâche, saisissez le nom du fichier (en veillant à bien indiquer l’extension).
1. Sélectionnez **[!UICONTROL Charger]**.

## Copier des zones cliquables parmi d’autres catalogues électroniques {#copying-image-maps-between-ecatalogs}

Vous pouvez copier toutes les zones cliquables d’un catalogue électronique dans un autre catalogue électronique. Il s’agit d’une méthode pratique de copie de zones cliquables entre les traductions en langues étrangères du même catalogue électronique. Pour que la copie soit réussie, Adobe Dynamic Media Classic recommande de copier entre des catalogues électroniques avec le même nombre de pages et les mêmes images.

>[!NOTE]
>
>si le catalogue électronique dans lequel vous copiez des zones cliquables contient déjà des zones cliquables, celles-ci sont supprimées lors de la copie.

Pour copier toutes les zones cliquables d’un catalogue électronique dans un autre catalogue électronique, procédez comme suit :

1. Sélectionnez le catalogue électronique avec les zones cliquables à copier, puis sélectionnez le bouton de survol **[!UICONTROL Modifier]** du catalogue électronique.
1. Dans l’onglet Pages de commande, sélectionnez **[!UICONTROL Copier les cartes]**.
1. Dans la boîte de dialogue Sélectionner une ressource, sélectionnez le catalogue électronique dans lequel vous souhaitez copier les zones cliquables, puis sélectionnez **[!UICONTROL Sélectionner]**.

Adobe Dynamic Media Classic affiche un message d’avertissement si le catalogue électronique cible à partir duquel vous copiez les zones cliquables comporte un nombre différent de pages ou d’images d’une taille différente. Sélectionnez **[!UICONTROL Continuer]** pour copier les zones cliquables malgré l’avertissement.
