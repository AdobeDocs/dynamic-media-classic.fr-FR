---
title: Création d’une visionneuse à 360°
description: Découvrez comment créer une visionneuse à 360° dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 35e8e7fc-5b3c-441a-959c-df2e39ea0d4b
topic: Content Management
level: Intermediate
source-git-commit: c4613c78347c4bda3d84747a72146617158c03b6
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 32%

---

# Création d’une visionneuse à 360°{#creating-a-spin-set}

Pour créer une visionneuse panoramique efficace, assurez-vous que les clichés soient pris correctement. Vous pouvez créer une visionneuse à 360° dans Adobe Dynamic Media Classic en cliquant sur le bouton Créer et en choisissant Visionneuses à 360°. Modifiez les visionneuses à 360° dans l’écran correspondant.

>[!NOTE]
>
>Les versions précédentes d’Adobe Dynamic Media Classic ne proposaient pas de visionneuses à 360° bidimensionnelles. Si vous avez créé une visionneuse à 360° dans une version précédente d’Adobe Dynamic Media Classic, enregistrez-la sous un autre nom. Vous pouvez alors enregistrer votre visionneuse à 360° unidimensionnelle. Sélectionnez **[!UICONTROL Enregistrer sous]** dans l’écran Visionneuse à 360° et saisissez un nouveau nom pour pouvoir le modifier dans Adobe Dynamic Media Classic.

## Instructions pour prendre des clichés d’images de la visionneuse à 360° {#guidelines-for-shooting-spin-set-images}

En règle générale, plus il y a d’images dans une visionneuse à 360°, meilleur est l’effet de rotation des images. Cependant, un nombre élevé d’images dans la visionneuse augmente la durée de chargement des images. Adobe Dynamic Media Classic recommande de suivre les instructions suivantes pour les prises de vue à utiliser dans les visionneuses à 360° :

* Utilisez au minimum 8 à 12 images dans une visionneuse à 360° unidimensionnelle et 16 à 24 images dans une visionneuse à 360° bidimensionnelle.
* Utilisez un format d’image sans perte (formats TIFF et PNG recommandés). 
* Masquez toutes les images pour faire apparaître l’objet sur un fond blanc ou fortement contrasté. Ajoutez éventuellement des ombres.
* Assurez-vous que les détails du produit sont bien éclairés et que leur mise au point est nette.
* Prenez des clichés de vêtements de prêt-à-porter avec un mannequin ou un modèle. Souvent, le mannequin est masqué (en utilisant un mannequin transparent) ou un mannequin stylisé est présenté dans l’image. Vous pouvez créer une visionneuse à 360° sur modèle en définissant le nombre d’angles. Marquez chaque angle avec du ruban adhésif sur le sol afin de guider le modèle à regarder dans la direction de chaque prise de vue.

## Création d’une visionneuse à 360° {#create}

L’ordre dans lequel la visionneuse à 360° est créée dans Adobe Dynamic Media Classic est important. Selon la manière dont vous ordonnez les ressources lorsque vous faites glisser et déposez des images dans la grille de la page de la visionneuse à 360°, celle-ci pivote dans une certaine direction. Par conséquent, l’ordre dans lequel elle s’affiche visuellement dans le créateur correspond à la manière dont la ressource est tournée lorsqu’un utilisateur déplace le pointeur de la souris ou le doigt, de gauche à droite.

Lorsque vous créez une visionneuse, l’option **[!UICONTROL Publier après un enregistrement]** affecte la visionneuse et les membres de la visionneuse des manières suivantes :

| L’option **[!UICONTROL Publier après un enregistrement]** est-elle sélectionnée avant l’enregistrement ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
| --- | --- | --- |
| Oui | Publié | Publié |
| Non | Non publié | Les membres de la visionneuse conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually-publishing-assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually-unpublishing-assets) (« Annulation manuelle de la publication des fichiers »).

Lorsque vous créez une visionneuse à 360°, Adobe recommande les bonnes pratiques suivantes et applique la limite suivante :

| Type de limite de visionneuse à 360° | Pratique recommandée | Limite imposée |
| --- | --- | --- |
| Nombre maximal de lignes/colonnes par ensemble 2D | 12 à 18 images par ensemble | 1 000 |

Voir aussi [Limites de Dynamic Media](/help/using/limitations.md).

Lorsque vous enregistrez une visionneuse à 360°, vous pouvez ensuite utiliser la fonction Prévisualiser dans la page Créer : Visionneuse à 360° pour voir comment s’affiche votre visionneuse à 360° dans la visionneuse par défaut.

**Pour créer une visionneuse à 360°, procédez comme suit**

1. Dans le menu déroulant **[!UICONTROL Créer]**, sélectionnez **[!UICONTROL Visionneuse à 360°]**.
1. Dans la boîte de dialogue Visionneuse à 360°, définissez le nombre de lignes et de cellules.

   Pour créer une visionneuse à 360° unidimensionnelle, sélectionnez une seule ligne.

   Pour une visionneuse à 360° bidimensionnelle, sélectionnez au moins deux lignes.

1. Sélectionnez **[!UICONTROL OK]**.
1. Faites glisser des images vers la grille de l’écran Visionneuse à 360°.
1. Lorsque vous avez terminé, en bas à droite de la page, assurez-vous que l’option **Publier après un enregistrement** est sélectionnée (par défaut).
1. Sélectionnez **[!UICONTROL Enregistrer]**.
1. Dans la boîte de dialogue Enregistrer , sélectionnez un dossier pour stocker la visionneuse à 360°. Dans le champ Nom de fichier, saisissez le nom de la visionneuse à 360°.
1. Sélectionnez **[!UICONTROL Enregistrer]**.

## Modification d’une visionneuse à 360° {#editing-a-spin-set}

Que vous modifiiez une visionneuse publiée ou une visionneuse dépubliée, l’option **[!UICONTROL Publier après un enregistrement]** affecte la visionneuse et les membres de la visionneuse des manières suivantes :

| Visionneuse déjà publiée ? | L’option **[!UICONTROL Publier après un enregistrement]** est-elle sélectionnée avant d’enregistrer votre modification ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
| --- | --- | --- | --- |
| Oui | Oui | Publié | Publié |
| Oui | Non | Publié | Les membres d’ensemble existants conservent leur statut publié. Tout nouveau membre de visionneuse que vous ajoutez lors de votre modification conserve son état publié ou non publié. |
| Non | Oui | Publié | Publié |
| Non | Non | Non publié | Les membres de la visionneuse existants, ainsi que tout nouveau membre de la visionneuse que vous ajoutez lors de votre modification conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually-publishing-assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually-unpublishing-assets) (« Annulation manuelle de la publication des fichiers »).

**Pour modifier une visionneuse à 360°, procédez comme suit**

1. Sélectionnez le bouton de survol de la visionneuse à 360° **[!UICONTROL Modifier]**.
1. Utilisez l’une des méthodes suivantes :

   * **Suppression des images** : sélectionnez l’image, puis sélectionnez **[!UICONTROL Supprimer]**.

   * **Ajouter des images** : faites glisser l’image dans une cellule.

   * **Réorganisation des lignes (visionneuse à 360° bidimensionnelle)** : sélectionnez une zone de sélecteur de ligne (à gauche de la ligne), puis sélectionnez **[!UICONTROL Déplacer la ligne vers le bas]** ou **[!UICONTROL Déplacer la ligne vers le haut]**.

   * **Ajout de lignes et de cellules** : saisissez un nombre dans les zones Lignes et Cellules pour déterminer le nombre de lignes et de cellules dans chaque ligne.

1. Lorsque vous avez terminé la modification, en bas à droite de la page, assurez-vous que l’option **[!UICONTROL Publier après un enregistrement]** est sélectionnée (par défaut).
1. Sélectionnez **[!UICONTROL Enregistrer]**, sélectionnez un dossier de stockage, saisissez un nom pour la visionneuse, puis sélectionnez **[!UICONTROL Enregistrer]**.

## Suppression d’une visionneuse à 360°

Lorsque vous supprimez une visionneuse, celle-ci est placée dans la corbeille. Toutefois, les membres (ou « enfants ») de cet ensemble ne sont pas affectés. Ils conservent chacun leur état publié ou dépublié existant.

Voir aussi [Manually publishing assets](publishing-files.md#manually-publishing-assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually-unpublishing-assets) (« Annulation manuelle de la publication des fichiers »).

**Pour supprimer une visionneuse à 360°, procédez comme suit**

1. En mode Affichage de la grille, Affichage par liste ou Affichage des détails, sélectionnez une ou plusieurs visionneuses à 360°.
1. Sur la barre de navigation globale, accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Supprimer]** > **[!UICONTROL Supprimer]**.
