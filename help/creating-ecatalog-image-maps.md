---
title: Création de zones cliquables dans un catalogue électronique
description: Découvrez comment créer des zones cliquables dans un catalogue électronique.
uuid: 943ad3f7-a885-4bc2-88cb-77083384bdf8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 4cf63359-63b5-4da7-9498-335d91b4776c
feature: Dynamic Media Classic, Visionneuses, Catalogue électronique
role: Business Practitioner
exl-id: 5e7f39a5-36a6-40df-8752-064a582c9346
translation-type: tm+mt
source-git-commit: 98463dbc24e141547d01bd3f71b1b9fe3a692c14
workflow-type: tm+mt
source-wordcount: '1488'
ht-degree: 60%

---

# Création de zones cliquables dans un catalogue électronique{#creating-ecatalog-image-maps}

Une zone cliquable est une zone d’une page de catalogue électronique sur laquelle vous pouvez faire survoler le curseur ou cliquer pour déclencher diverses actions. Par exemple, le positionnement du pointeur sur une zone cliquable entraîne l’affichage d’une description d’objet. Lorsque vous cliquez sur une zone cliquable, une autre action est déclenchée. Par exemple, vous pouvez ouvrir une page Web pour que les utilisateurs qui la consultent puissent en savoir plus sur un élément ou l’acheter, ou vous pouvez lancer une vidéo pour afficher un élément en cours d’utilisation.

## Traçage de zones cliquables dans un catalogue électronique  {#drawing-ecatalog-image-maps}

Vous dessinez les zones cliquables des catalogues sur l’onglet Pages de zones de l’écran Catalogue électronique. Cet écran contient une section Zone cliquable dans laquelle les pages du catalogue électronique sont affichées, ainsi qu’une liste des zones cliquables, à droite. Au fur et à mesure que vous tracez les zones cliquables, leur nom est ajouté à cette liste.

1. Cliquez sur le bouton de survol Modifier du catalogue électronique.
1. Cliquez sur **[!UICONTROL Pages de zones]**.
1. Sur le côté gauche de l’écran Pages de zones, sélectionnez la page souhaitée.
1. Dans la section Zone cliquable, tracez une zone rectangulaire ou polygonale (à plusieurs côtés) :

   * **Zone**
cliquable rectangulaireSélectionnez l’outil Zone cliquable rectangulaire et faites glisser le curseur sur la page pour créer le rectangle.

   * **Zone cliquable polygonaleSélectionnez l’outil Zone cliquable polygonale et cliquez autant de fois que nécessaire autour du périmètre de l’image.**
Lorsque vous cliquez, Dynamic Media Classic trace les bordures de la zone cliquable.
   Après avoir tracé une zone cliquable, Dynamic Media Classic lui attribue un nom dans la liste Zone cliquable. Pour former le nom, Dynamic Media Classic ajoute un numéro d’ordre au nom de la page de catalogue électronique dans laquelle vous travaillez.

1. (Facultatif) Dans la liste des zones cliquables, dans la colonne Nom, saisissez un nouveau nom pour la zone cliquable. N’insérez pas d’espaces dans le nom que vous saisissez.
1. Vous pouvez permettre aux utilisateurs d’afficher une nouvelle page Web lorsqu’ils cliquent sur la zone cliquable. Dans le panneau de la liste des zones cliquables, saisissez l’URL de la page Web dans la colonne URL.

   Cliquez sur **[!UICONTROL Modifier]** et saisissez un modèle pour faciliter la saisie des URL (modèles Href).

   Voir [Utilisation d’un modèle pour entrer du code JavaScript™ et des URL](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. (Facultatif) Dans la liste déroulante Afficher, cliquez sur **[!UICONTROL Texte de survol]**, puis entrez le texte que les utilisateurs doivent voir à l’écran lorsqu’ils déplacent leur pointeur sur la zone cliquable.
1. (Facultatif) Dans la liste déroulante Afficher, cliquez sur **[!UICONTROL Autres actions]**, puis saisissez un attribut pour déclencher un flou ou une action de sélection lorsque les utilisateurs placent leur pointeur sur une zone cliquable.

   (voir [Définition d’autres actions relatives aux zones cliquables](creating-image-maps.md#defining_other_actions_for_image_maps)).

1. Cliquez sur **[!UICONTROL Enregistrer]**.
1. (Facultatif) Cliquez sur **[!UICONTROL Prévisualisation]** pour vue du catalogue électronique avec le paramètre prédéfini de visionneuse de catalogue électronique par défaut.

Pour supprimer une zone cliquable, sélectionnez son nom dans la liste de zone cliquable, puis cliquez sur **[!UICONTROL Supprimer]**. Pour désactiver temporairement une zone cliquable sur une page sans supprimer la zone cliquable, désélectionnez l’option Oui de la zone cliquable dans le panneau de la liste des zones cliquables.

## Intégration de médias enrichis dans un catalogue électronique  {#embedding-rich-media-in-an-ecatalog}

Vous pouvez utiliser l’option Média enrichis du catalogue électronique pour ajouter des vidéos de format MP4 ou des visionneuses à 360° aux zones cliquables que vous avez ajoutées dans un catalogue électronique. Lorsqu’un utilisateur clique sur la région de la zone cliquable dans le catalogue électronique, la vidéo ou la visionneuse à 360° associée s’affiche. Cette fonctionnalité est particulièrement utile si vous souhaitez que les clients puissent voir un élément en cours d’utilisation ou le voir sous d’autres angles et perspectives.

Vous pouvez également afficher du texte d’info-bulle lorsque les clients placent leur pointeur sur la zone cliquable pour savoir ce sur quoi ils cliquent.

**Intégration de médias enrichis dans un catalogue électronique**

1. Tracez une zone cliquable dans un catalogue électronique.

   Voir [Traçage de zones cliquables dans un catalogue électronique](creating-ecatalog-image-maps.md#drawing_ecatalog_image_maps).

1. Dans la liste déroulante Afficher, sélectionnez Médias enrichis.
1. Dans le panneau d’ajout de fichiers sur la gauche, accédez à un dossier contenant le fichier de la visionneuse à 360° ou de vidéo (format MP4) à intégrer.
1. Faites glisser le fichier sur la zone cliquable.
1. (Facultatif) Dans le panneau de la liste des zones cliquables, dans la colonne Info-bulle, saisissez le texte que les utilisateurs doivent voir s’afficher lorsqu’ils placent le pointeur sur la zone cliquable.
1. Cliquez sur **[!UICONTROL Enregistrer]**.

## Edition des zones cliquables d’un catalogue électronique {#editing-ecatalog-image-maps}

En commençant par l’onglet Pages de zones de l’écran Catalogue électronique, utilisez ces techniques pour éditer les zones cliquables d’un catalogue électronique :

* **Ajustement de la**
positionSélectionnez l&#39;outil Panoramique et déplacez le pointeur à proximité de la bordure de la carte, mais pas dessus. Lorsque le pointeur prend la forme d’une flèche à quatre pointes, faites glisser la zone de l’image entière vers un nouvel emplacement.

   Voir [Ajustement de la position, de la forme et de la taille des zones cliquables](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

* **Modification de la forme et de la**
taillePour redimensionner une zone cliquable rectangulaire, sélectionnez l’outil Panorama. Puis déplacez le pointeur au-dessus d’une ligne de bordure ou d’un coin, et lorsque vous voyez apparaître l’icône en forme de flèche à deux pointes, faites glisser. Pour redimensionner une zone cliquable polygonale, faites glisser une poignée de sélection carrée. Pour créer une poignée de sélection, cliquez sur la bordure de la zone cliquable et faites glisser.

   Voir [Ajustement de la position, de la forme et de la taille des zones cliquables](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

* **Suppression de**
zones cliquablesSélectionnez l’outil Panorama, cliquez sur la zone cliquable pour la sélectionner, puis cliquez sur  **[!UICONTROL Supprimer]**.

   Pour supprimer toutes les zones cliquables d’un catalogue électronique, cliquez sur l’onglet **[!UICONTROL Ordre des pages]**, puis sur **[!UICONTROL Effacer les zones cliquables]**.

* **Gestion des zones cliquables se chevauchantFaites glisser le pointeur pour modifier l’ordre des zones cliquables sur la liste de zones cliquables.**


   Voir [Gestion des zones cliquables superposées](creating-image-maps.md#handling_overlapping_image_maps).

* **Copie de zones cliquables vers d’autres**
pagesSélectionnez le bouton Copier les zones cliquables vers (assurez-vous que l’onglet Pages de zones est actif). Dans l’écran Sélectionner les images, sélectionnez la ou les pages sur lesquelles vous souhaitez copier les zones cliquables, puis cliquez sur le bouton **[!UICONTROL Sélectionner]**.

   Voir [Copie de zones cliquables vers d’autres images](creating-image-maps.md#copying_image_maps).

>[!NOTE]
>
>Outre la copie de zones cliquables sur différentes pages d’un catalogue électronique, vous pouvez copier toutes les zones cliquables d’un catalogue électronique dans un autre catalogue électronique. Voir [Copie de zones cliquables entre catalogues électroniques](creating-ecatalog-image-maps.md#copying_image_maps_between_ecatalogs).

## Vérification et importation des données de zone cliquable  {#reviewing-and-importing-image-map-data}

L’écran de résumé de zone cliquable fournit des métadonnées concernant votre catalogue électronique. Il permet également l’importation par lots des données de zone cliquable pour votre catalogue électronique. Cette méthode d’importation des données facilite la saisie des URL et du texte de survol des zones cliquables.

Pour afficher l’écran Résumé de zone cliquable, dans l’onglet Pages de zones de l’écran Catalogue électronique, cliquez sur Résumé.

### Vérification du résumé des données de zone cliquable  {#review-image-map-data-summary}

1. Dans l’écran Pages de zones, cliquez sur **[!UICONTROL Résumé]**.

   L’écran Résumé de zone cliquable indique le nombre de zones cliquables, d’URL, de descriptions de texte de survol et autres actions définies dans votre catalogue électronique.

1. En cas d&#39;erreur de texte de survol, cliquez sur l&#39;erreur dans la colonne Erreur de clé de survol pour voir ce qui doit être modifié dans votre feuille de calcul pour corriger l&#39;erreur. Vous pouvez sélectionner et copier le texte contenu dans ce message et le coller dans la feuille de calcul.
1. Cliquez sur **[!UICONTROL Prévisualisation]** pour examiner une page dans la visionneuse de catalogue électronique, cliquez sur le X pour fermer l’écran Résumé et revenir à l’écran Pages de zones ou sur **[!UICONTROL Fermer]** pour revenir à **[!UICONTROL Parcourir]**.

### Importation des données de zone cliquable {#import-image-map-data}

Plutôt que de saisir les données de zone cliquable sur chacune des pages, vous avez la possibilité d’importer les données de l’ensemble de votre catalogue électronique dans l’écran de résumé de zone cliquable. Vous importez les données de zone cliquable sous la forme d’un fichier délimité par des tabulations ou d’un fichier DTD XML. Les champs du fichier doivent être dans l’ordre indiqué sur l’écran de résumé de zone cliquable : Nom, Etiquettes de table des matières, Zones, URL, Texte de survol, Autres actions et Chaînes de recherche. Vous évitez ainsi d’avoir à saisir les données dans la liste de zones cliquables au fur et à mesure que vous créez ces dernières.

>[!NOTE]
>
>vous devez avoir créé les zones cliquables avant d’importer les données correspondantes.

Depuis l’écran de résumé de zone cliquable, procédez comme suit pour importer les données des zones cliquables que vous avez créées :

1. Cliquez sur **[!UICONTROL Importer les données de mappage]**.
1. Dans la boîte de dialogue Importer les métadonnées, cliquez sur **[!UICONTROL Parcourir]**.
1. Sélectionnez le fichier délimité par des tabulations ou le fichier DTD XML.
1. Dans le champ Nom de la tâche, saisissez le nom du fichier (en veillant à bien indiquer l’extension).
1. Cliquez sur **[!UICONTROL Télécharger]**.

## Copie de zones cliquables entre catalogues électroniques {#copying-image-maps-between-ecatalogs}

Vous pouvez copier toutes les zones cliquables d’un catalogue électronique dans un autre catalogue électronique. Il s’agit d’une méthode pratique de copie de zones cliquables entre les traductions en langues étrangères du même catalogue électronique. Pour que la copie soit réussie, Dynamic Media Classic recommande la copie entre catalogues électroniques avec le même nombre de pages et les mêmes images.

>[!NOTE]
>
>si le catalogue électronique dans lequel vous copiez des zones cliquables contient déjà des zones cliquables, celles-ci sont supprimées lors de la copie.

Pour copier toutes les zones cliquables d’un catalogue électronique vers un autre, procédez comme suit :

1. Sélectionnez le catalogue électronique contenant les zones cliquables à copier, puis cliquez sur le bouton de survol **[!UICONTROL Modifier]** du catalogue électronique.
1. Dans l’onglet Ordre des pages, cliquez sur **[!UICONTROL Copier les zones]**.
1. Dans la boîte de dialogue Sélectionner un fichier, sélectionnez le catalogue électronique dans lequel vous souhaitez copier les zones cliquables, puis cliquez sur **[!UICONTROL Sélectionner]**.

Dynamic Media Classic affiche un message d’avertissement si le catalogue électronique de cible (le catalogue électronique dans lequel vous copiez des zones cliquables) comporte un nombre différent de pages ou d’images de taille différente. Vous pouvez cliquer sur **[!UICONTROL Continuer]** pour copier les zones cliquables malgré l’avertissement.
