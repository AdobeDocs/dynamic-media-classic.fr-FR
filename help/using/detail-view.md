---
title: Vue détaillée du travail
description: Découvrez comment utiliser la vue détaillée dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 618ae6a4-6f60-4a80-b197-a9d35b3c47af
topic: Content Management
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 20%

---

# Vue détaillée du travail{#working-in-detail-view}

Vous pouvez travailler avec une ressource et en savoir plus à son sujet en l’ouvrant dans l’affichage des détails. Dans la vue Détail, vous pouvez voir la taille de la ressource, les attributs, les dérivés et les métadonnées. Vous pouvez également voir si et quand la ressource a été publiée et vous pouvez obtenir l’URL des ressources publiées. En fonction du type de fichier, vous pouvez le prévisualiser selon différentes tailles, effectuer un zoom avant et exécuter une accentuation, un recadrage ou d’autres opérations de mise en forme.

<!-- 

Comment Type: remark
Last Modified By: Rick Brough (rbrough@adobe.com)
Last Modified Date: 2018-06-14T13:52:46.623-0400

<p>as_detail_view_popup.png found in Downloads on local in folder "scene7-images"</p>

 -->

![Affichage des détails](/help/using/assets/image_0.img.png)
*Affichage des détails avec le panneau Bibliothèque de ressources masqué de la vue sur le côté gauche.*

>[!NOTE]
>
>Pour ouvrir le dossier dans lequel la ressource est stockée, vous pouvez sélectionner le chemin d’accès au dossier dans la partie supérieure du panneau Informations .

## Ouverture d’une ressource dans la vue détaillée {#open-an-asset-in-detail-view}

Vous pouvez afficher une ressource dans la vue détaillée afin de pouvoir l’examiner, la prévisualiser ou l’exploiter.

1. Dans le panneau de navigation, effectuez l’une des opérations suivantes :

   * Sélectionnez la ressource. Dans le coin supérieur droit d’Adobe Dynamic Media Classic, sélectionnez l’icône **[!UICONTROL Affichage des détails]**.
   * Cliquez deux fois sur le fichier.
   * Sélectionnez la ressource, puis accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Détails]**.

>[!NOTE]
>
>Vous pouvez paginer d’une ressource à l’autre dans le même dossier dans le mode Détails. Il vous suffit de cliquer sur **[!UICONTROL Ressource précédente]** ou **[!UICONTROL Ressource suivante]**. Ces boutons se trouvent dans le coin supérieur droit de la vue Détail.

## Obtenir des informations dans la vue détaillée {#getting-information-in-detail-view}

L’Affichage des détails fournit des informations sur une ressource ou un fichier. Ces informations s’affichent à propos d’un élément : le dossier dans lequel il est stocké, son nom de fichier, la date à laquelle l’élément a été chargé dans Adobe Dynamic Media Classic et son historique de publication. Vous pouvez également afficher et modifier des métadonnées et ajouter des mots-clés pour une ressource dans l’affichage des détails.

Vous pouvez obtenir une URL de ressource dans la vue détaillée. Toutefois, l’URL n’est pas active tant que vous n’avez pas publié la ressource. Pour les images, l’affichage des détails fournit également une liste des ressources et des métadonnées créées et dérivées, telles que les cibles de zoom et les visionneuses d’images.

## Utilisation des ressources dans la vue détaillée {#working-with-assets-in-detail-view}

Le mode Détail propose des outils permettant d’utiliser la ressource que vous avez ouverte. Les outils disponibles dépendent du type de ressource que vous utilisez, mais l’affichage des détails offre toujours les fonctions suivantes :

* **éléments à publier** : sélectionnez l’icône **[!UICONTROL `Publish`]** à gauche du nom ou accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Publier]** ou **[!UICONTROL Fichier]** > **[!UICONTROL Dépublier]**.

* **Renommer la ressource** : sélectionnez le nom et saisissez un nouveau nom.

* **Modifier et ajouter des métadonnées** : sélectionnez le panneau Métadonnées et apportez les modifications souhaitées. Voir [Affichage, ajout et exportation de métadonnées](/help/using/viewing-adding-exporting-metadata.md).

* **Modifier et ajouter des mots-clés** : sélectionnez les mots-clés et ajoutez ou supprimez-les selon vos besoins. (voir [Ajout ou modification de mots-clés](/help/using/viewing-adding-exporting-metadata.md)).

* **Supprimer la ressource** : accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Supprimer]**.

Pour les fichiers discrets (images, visionneuses d’images et polices, par exemple), vous pouvez afficher l’historique de publication et de modification, et vérifier les détails de la tâche dans la vue Détail.

Ce tableau montre les autres options disponibles avec différents types de ressources dans l’affichage des détails.

| Type de fichier | Edition/Modification | Prévisualisation |
| --- | --- | --- |
| Images | Ajout de zones cliquables<br>Ajout de cibles de zoom<br>Recadrage<br>Accentuation<br>Création de vues ajustées | Oui : zoom et paramètres d’image prédéfinis |
| Images de meuble et de garnitures de fenêtre | Non | Miniature |
| Catalogues électroniques | Edition | Le panneau Oui<br>Info est également disponible |
| Polices | Edition des informations de polices | Non |
| Fichiers FXG | Edition | Oui |
| Profils ICC | Edition des informations de profil | Non |
| Fichiers Illustrator | Non (sauf conversion au format FXG) | Non |
| Visionneuses d’images | Edition | Oui |
| Fichiers InDesign | Non (sauf conversion au format FXG) | Non |
| Fichiers PDF | Non | Non |
| Fichiers PSD | Oui pour les calques individuels | Oui pour les calques individuels |
| Visionneuses à 360° | Edition | Oui |
| Fichiers SVG | Non | Non |
| Modèles | Edition | Oui |
| Vidéos | Non | Oui |
| Vignettes et rendus de vignette | Non | L’image s’affiche<br> Vous pouvez afficher le contenu et la structure des éléments rendus de la vignette au format XML |
| Fichiers XML | Non | Le contenu est affiché. |
| Fichiers ZIP | Non | Le contenu n’est pas affiché. |

>[!MORELIKETHIS]
>
>* [Affichage, ajout et exportation de métadonnées](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
