---
title: 'Utilisation de la vue Détails '
description: Découvrez comment travailler dans la vue de détails.
uuid: cb62f765-9b7f-4a53-8206-99afae2fb80d
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: eaa214ff-d1ef-4691-9148-d01bf243c810
feature: Dynamic Media Classic,Gestion des ressources
role: Business Practitioner
exl-id: 618ae6a4-6f60-4a80-b197-a9d35b3c47af
translation-type: tm+mt
source-git-commit: eb37440a2917094aae8f32e9337b4c187ec6c1c2
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 65%

---

# Utilisation de la vue Détails {#working-in-detail-view}

Le mode Affichage des détails permet d’utiliser un fichier et d’en savoir plus à son sujet. En mode Affichage des détails, la taille, les attributs, les dérivés, ainsi que les métadonnées du fichier sont visibles. Vous obtenez également des indications sur la publication ou non du fichier, la date de sa publication et l’URL du fichier publié. En fonction du type de fichier, vous pouvez le prévisualiser selon différentes tailles, effectuer un zoom avant et exécuter une accentuation, un recadrage ou d’autres opérations de mise en forme.

<!-- 

Comment Type: remark
Last Modified By: Rick Brough (rbrough@adobe.com)
Last Modified Date: 2018-06-14T13:52:46.623-0400

<p>as_detail_view_popup.png found in Downloads on local in folder "scene7-images"</p>

 -->

![Affichage des détails ](/help/assets/image_0.img.png)
*VueDétails avec le panneau Bibliothèque de fichiers masqué de la vue sur le côté gauche.*

>[!NOTE]
>
>Pour ouvrir le dossier dans lequel le fichier est stocké, vous pouvez cliquer sur le chemin du dossier indiqué en haut du panneau Informations.

## Ouverture d’une ressource dans la vue Détails {#open-an-asset-in-detail-view}

Pour examiner en détail un fichier, le prévisualiser ou l’utiliser, choisissez l’option Affichage des détails. 

1. Dans le panneau de navigation, effectuez l’une des opérations suivantes :

   * Sélectionnez le fichier. Près du coin supérieur droit de Dynamic Media Classic, cliquez sur l’icône **[!UICONTROL Vue de détails]** .
   * Cliquez deux fois sur le fichier.
   * Sélectionnez le fichier, puis cliquez sur **[!UICONTROL Fichier]** > **[!UICONTROL Détails]**.

>[!NOTE]
>
>En mode Affichage des détails, vous pouvez passer d’un fichier à l’autre dans le même dossier en sélectionnant le bouton Fichier précédent ou Fichier suivant. Ces boutons se trouvent dans le coin supérieur droit de la vue de détails.

## Obtention d’informations dans la vue Détails {#getting-information-in-detail-view}

L’affichage des détails permet d’obtenir des informations sur un fichier. Il affiche les informations suivantes sur un élément : le dossier dans lequel il est stocké, son nom de fichier, la date de téléchargement de l’élément vers Dynamic Media Classic et son historique de publication. Vous pouvez également afficher et modifier des métadonnées et ajouter des mots-clés à un fichier en mode Affichage des détails.

Vous pouvez obtenir une URL de fichier en mode Affichage des détails ; cependant, l’URL n’est activée qu’une fois l’objet publié. Pour les images, l’affichage des détails fournit également une liste des fichiers et métadonnées créés et dérivés, comme les cibles de zoom et les visionneuses d’images.

## Utilisation de ressources dans la vue Détails {#working-with-assets-in-detail-view}

L’affichage des détails donne accès à des outils utilisables avec le fichier que vous avez ouvert. La nature des outils disponibles dépend du type de fichier que vous utilisez, mais l’affichage des détails propose les fonctions suivantes :

* **éléments pour publication**  - Cliquez sur la  **** publication à gauche du nom ou sur  **[!UICONTROL Fichier >]** Fichier de publication  **[!UICONTROL > Annuler la publication]**.

* **Attribution d&#39;un nouveau nom au fichier**  : sélectionnez le nom et saisissez-en un nouveau.

* **Modification et ajout de métadonnées**  - Sélectionnez le panneau Métadonnées et modifiez-le selon vos besoins. (voir [Affichage, ajout et exportation de métadonnées](/help/viewing-adding-exporting-metadata.md)).

* **Modification et ajout de mots-clés**  - Sélectionnez Mots-clés et ajoutez ou supprimez-les selon vos besoins. (voir [Ajout ou modification de mots-clés](/help/viewing-adding-exporting-metadata.md)).

* **Suppression de la ressource**  - Cliquez sur  **[!UICONTROL Fichier]**  >  **[!UICONTROL Supprimer]**.

Pour les fichiers discrets (images, visionneuses d’images et polices, par exemple), vous pouvez visualiser l’historique de publication et d’édition, et vérifier les détails de la tâche, en mode Affichage des détails.

Ce tableau présente les autres options disponibles avec différents types de fichiers dans la vue de détails.

| Type de fichier | Edition/Modification | Prévisualisation |
|--- |--- |--- |
| Images | Ajout de zones cliquables<br>Ajouter des <br><br><br>cibles de zoomCropSharpenCréer des vues ajustées | Oui : zoom et paramètres d’image prédéfinis |
| Images de meuble et de garnitures de fenêtre | Non | Miniature |
| Catalogues électroniques | Edition | Oui<br>Le panneau d’informations est également disponible |
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
| Vignettes et rendus de vignette | Non | L’image s’affiche <br>Vous pouvez vue le contenu et la structure des éléments du rendu de la vignette au format XML. |
| Fichiers XML | Non | Le contenu est affiché. |
| Fichiers ZIP | Non | Le contenu n’est pas affiché |

>[!MORELIKETHIS]
>
>* [Affichage, ajout et exportation de métadonnées](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)

