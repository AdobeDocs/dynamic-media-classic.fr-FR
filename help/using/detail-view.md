---
title: Travail en mode Détails
description: Découvrez comment travailler en mode Détails dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 618ae6a4-6f60-4a80-b197-a9d35b3c47af
topic: Content Management
level: Intermediate
source-git-commit: 5b5dcd1199bd51ec987b5673fce75bc86baad55b
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 20%

---

# Travail en mode Détails{#working-in-detail-view}

Vous pouvez utiliser et en savoir plus sur une ressource en l’ouvrant dans l’affichage des détails. En mode d’affichage des détails, la taille, les attributs, les dérivés et les métadonnées des ressources s’affichent. Vous pouvez également déterminer si et quand la ressource a été publiée et obtenir l’URL des ressources publiées. En fonction du type de fichier, vous pouvez le prévisualiser selon différentes tailles, effectuer un zoom avant et exécuter une accentuation, un recadrage ou d’autres opérations de mise en forme.

<!-- 

Comment Type: remark
Last Modified By: Rick Brough (rbrough@adobe.com)
Last Modified Date: 2018-06-14T13:52:46.623-0400

<p>as_detail_view_popup.png found in Downloads on local in folder "scene7-images"</p>

 -->

![Affichage des détails](/help/using/assets/image_0.img.png)
*Affichage des détails avec le panneau Bibliothèque de ressources masqué dans la vue de gauche.*

>[!NOTE]
>
>Pour ouvrir le dossier dans lequel la ressource est stockée, vous pouvez sélectionner le chemin du dossier en haut du panneau Informations.

## Ouverture d’une ressource dans l’affichage des détails {#open-an-asset-in-detail-view}

Pour examiner de plus près, prévisualiser ou travailler sur une ressource, vous pouvez l’afficher dans la vue Détails.

1. Dans le panneau de navigation, effectuez l’une des opérations suivantes :

   * Sélectionnez la ressource. Dans le coin supérieur droit d’Adobe Dynamic Media Classic, sélectionnez la variable **[!UICONTROL Affichage des détails]** icône .
   * Cliquez deux fois sur le fichier.
   * Sélectionnez la ressource, puis accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Détails]**.

>[!NOTE]
>
>Vous pouvez passer d’une ressource à une autre dans le même dossier en mode d’affichage des détails en sélectionnant **[!UICONTROL Ressource précédente]** ou **[!UICONTROL Ressource suivante]**. Ces boutons se trouvent dans le coin supérieur droit de la vue Détails.

## Obtention d’informations dans la vue Détails {#getting-information-in-detail-view}

L’affichage des détails fournit des informations sur une ressource ou un fichier. Ces informations s’affichent sur un élément : son dossier de stockage, son nom de fichier, la date de téléchargement de l’élément dans Adobe Dynamic Media Classic et son historique de publication. Vous pouvez également afficher et modifier des métadonnées et ajouter des mots-clés pour une ressource dans le mode Affichage des détails.

Vous pouvez obtenir une URL de ressource en mode Affichage des détails ; toutefois, l’URL n’est pas active tant que vous n’avez pas publié la ressource. Pour les images, la vue Détails fournit également une liste de ressources et de métadonnées créées et dérivées, telles que les cibles de zoom et les visionneuses d’images.

## Utilisation de ressources dans l’affichage des détails {#working-with-assets-in-detail-view}

Le mode Affichage des détails propose des outils pour travailler avec la ressource que vous avez ouverte. Les outils disponibles dépendent du type de ressource que vous utilisez, mais l’affichage des détails offre toujours les fonctions suivantes :

* **éléments pour publication** - Sélectionnez la variable **[!UICONTROL `Publish`]** à gauche du nom ou accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Publier]** ou **[!UICONTROL Fichier]** > **[!UICONTROL Dépublier]**.

* **Renommer la ressource** - Sélectionnez le nom et saisissez un nouveau nom.

* **Modification et ajout de métadonnées** - Sélectionnez le panneau Métadonnées et modifiez-le selon vos besoins. Voir [Affichage, ajout et exportation de métadonnées](/help/using/viewing-adding-exporting-metadata.md).

* **Modifier et ajouter des mots-clés** - Sélectionnez Mots-clés et ajoutez ou supprimez-les selon vos besoins. (voir [Ajout ou modification de mots-clés](/help/using/viewing-adding-exporting-metadata.md)).

* **Suppression de la ressource** - Accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Supprimer]**.

Pour les fichiers discrets (images, visionneuses d’images et polices, par exemple), vous pouvez afficher l’historique de publication et de modification, ainsi que vérifier les détails de la tâche, en mode Affichage des détails.

Ce tableau indique quelles autres options sont disponibles avec différents types de ressources dans la vue Détails.

| Type de fichier | Edition/Modification | Prévisualisation |
| --- | --- | --- |
| Images | Ajout de zones cliquables<br>Ajout de cibles de zoom<br>Recadrer<br>Accentuer<br>Créer des vues ajustées | Oui : zoom et paramètres d’image prédéfinis |
| Images de meuble et de garnitures de fenêtre | Non | Miniature |
| Catalogues électroniques | Edition | Oui<br>Le panneau Informations est également disponible |
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
| Vignettes et rendus de vignette | Non | L’image s’affiche<br>Vous pouvez visualiser le contenu et la structure des éléments rendables de la vignette au format XML. |
| Fichiers XML | Non | Le contenu est affiché. |
| Fichiers ZIP | Non | Contenu non affiché |

>[!MORELIKETHIS]
>
>* [Affichage, ajout et exportation de métadonnées](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
