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
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '958'
ht-degree: 44%

---

# Création d’une visionneuse à 360°{#creating-a-spin-set}

Pour créer une visionneuse panoramique efficace, assurez-vous que les clichés soient pris correctement. Vous pouvez créer une visionneuse à 360° dans Adobe Dynamic Media Classic en sélectionnant le bouton Créer et en choisissant Visionneuses à 360°. Modifiez les visionneuses à 360° dans l’écran correspondant.

>[!NOTE]
>
>Les versions précédentes d’Adobe Dynamic Media Classic ne fournissaient pas de visionneuses à 360° bidimensionnelles. Si vous avez créé une visionneuse à 360° dans une version précédente d’Adobe Dynamic Media Classic, vous ne pouvez pas enregistrer votre visionneuse à 360° unidimensionnelle sans l’enregistrer au préalable sous un autre nom. Sélectionner **[!UICONTROL Enregistrer sous]** dans l’écran Visionneuse à 360° et saisissez un nouveau nom afin de pouvoir le modifier dans Adobe Dynamic Media Classic.

## Instructions pour prendre des clichés d’images de la visionneuse à 360° {#guidelines-for-shooting-spin-set-images}

En règle générale, plus vous avez d’images dans une visionneuse à 360°, plus l’effet de rotation d’images est important. Cependant, un nombre élevé d’images dans la visionneuse augmente la durée de chargement des images. Adobe Dynamic Media Classic recommande les instructions suivantes pour le tournage d’images à utiliser dans les visionneuses à 360° :

* Au minimum, utilisez 8 à 12 images dans une visionneuse à 360° unidimensionnelle et 16 à 24 images dans une visionneuse à 360° bidimensionnelle.
* Utilisez un format d’image sans perte (formats TIFF et PNG recommandés). 
* Masquez toutes les images pour faire apparaître l’objet sur un fond blanc ou fortement contrasté. Ajoutez éventuellement des ombres.
* Assurez-vous que les détails du produit sont bien éclairés et que leur mise au point est nette.
* Prenez des clichés de vêtements de prêt-à-porter avec un mannequin ou un modèle. Souvent, le mannequin est masqué (à l’aide d’un mannequin en verre) ou un mannequin stylisé est présenté dans l’image. Vous pouvez créer une visionneuse à 360° de modèle en définissant le nombre d’angles. Marquez chaque angle avec du ruban adhésif sur le sol afin que vous puissiez guider le modèle pour qu’il marche et regarde dans la direction de chaque prise de vue.

## Création d’une visionneuse à 360° {#create}

L’ordre dans lequel la visionneuse à 360° est créée ou créée dans Adobe Dynamic Media Classic est important. Selon la manière dont vous organisez les ressources lorsque vous faites glisser des images dans la grille de la page Visionneuse à 360°, la visionneuse à 360° tourne dans une certaine direction. Par conséquent, l’ordre dans lequel elle est visuellement affichée dans le créateur est la manière dont la ressource est déclenchée lorsqu’un utilisateur déplace le pointeur de la souris ou le doigt, de gauche à droite.

Lorsque vous créez une visionneuse, l’option **[!UICONTROL Publish after save]** (« Publier après l’enregistrement ») affecte la visionneuse et ses membres comme suit :

| **[!UICONTROL Publier après enregistrement]** l’option sélectionnée avant l’enregistrement ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
| --- | --- | --- |
| Oui | Publié | Publié |
| Non | Non publié | Les membres de la visionneuse conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually-publishing-assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually-unpublishing-assets) (« Annulation manuelle de la publication des fichiers »).

Lorsque vous créez une visionneuse à 360°, Adobe recommande les bonnes pratiques suivantes et applique la limite suivante :

| Type de limite de visionneuse à 360° | Pratique recommandée | Limite imposée |
| --- | --- | --- |
| Nombre maximal de lignes/colonnes par jeu 2D | 12 à 18 images par visionneuse | 1 000 |

Voir aussi [Limites de Dynamic Media](/help/using/limitations.md).

Lorsque vous enregistrez une visionneuse à 360°, vous pouvez ensuite utiliser la fonction Prévisualiser dans la page Créer : Visionneuse à 360° pour voir comment s’affiche votre visionneuse à 360° dans la visionneuse par défaut.

**Pour créer une visionneuse à 360° :**

1. Sur le **[!UICONTROL Build]** menu déroulant, sélectionnez **[!UICONTROL Visionneuses à 360°]**.
1. Dans la boîte de dialogue Visionneuse à 360°, définissez le nombre de lignes et de cellules.

   Pour une visionneuse à 360° unidimensionnelle, sélectionnez une seule ligne.

   Pour une visionneuse à 360° bidimensionnelle, sélectionnez au moins deux lignes.

1. Sélectionner **[!UICONTROL OK]**.
1. Faites glisser des images vers la grille de l’écran Visionneuse à 360°.
1. Une fois terminé, près de l’angle inférieur droit de la page, vérifiez que l’option **Publish after save** (« Publier après l’enregistrement ») est sélectionnée (valeur par défaut).
1. Sélectionner **[!UICONTROL Enregistrer]**.
1. Dans la boîte de dialogue Enregistrer, sélectionnez le dossier dans lequel conserver la visionneuse à 360°. Dans le champ Nom de fichier, saisissez le nom de la visionneuse à 360°.
1. Sélectionner **[!UICONTROL Enregistrer]**.

## Modification d’une visionneuse à 360° {#editing-a-spin-set}

Si vous modifiez un jeu publié ou non publié, la variable **[!UICONTROL Publier après enregistrement]** L’option affecte les membres de l’ensemble et de l’ensemble comme suit :

| Visionneuse déjà publiée ? | **[!UICONTROL Publier après enregistrement]** sélectionnée avant d’enregistrer votre modification ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
| --- | --- | --- | --- |
| Oui | Oui | Publié | Publié |
| Oui | Non | Publié | Les membres de visionneuse existants conservent leur état publié. Tout nouveau membre de visionneuse que vous ajoutez lors de votre modification conserve son état publié ou non publié. |
| Non | Oui | Publié | Publié |
| Non | Non | Non publié | Les membres de la visionneuse existants, ainsi que tout nouveau membre de la visionneuse que vous ajoutez lors de votre modification conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually-publishing-assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually-unpublishing-assets) (« Annulation manuelle de la publication des fichiers »).

**Pour modifier une visionneuse à 360° :**

1. Sélectionner le survol de la visionneuse à 360° **[!UICONTROL Modifier]** bouton .
1. Utilisez l’une des méthodes suivantes :

   * **Suppression d’images**: sélectionnez l’image, puis **[!UICONTROL Supprimer]**.

   * **Ajouter des images**: faites glisser l’image dans une cellule.

   * **Réorganisation des lignes (visionneuses à 360° en deux dimensions)**: sélectionnez une zone de sélecteur de ligne (à gauche de la ligne), puis sélectionnez **[!UICONTROL Déplacer la ligne vers le bas]** ou **[!UICONTROL Déplacer la ligne vers le haut]**.

   * **Ajout de lignes et de cellules**: saisissez un nombre dans les champs Lignes et Cellules pour déterminer le nombre de lignes et le nombre de cellules dans chaque ligne.

1. Une fois les modifications terminées, près de l’angle inférieur droit de la page, vérifiez que l’option **[!UICONTROL Publish after save]** (« Publier après l’enregistrement ») est sélectionnée (valeur par défaut).
1. Sélectionner **[!UICONTROL Enregistrer]**, sélectionnez un dossier de stockage, saisissez un nom pour la visionneuse, puis sélectionnez **[!UICONTROL Enregistrer]**.

## Suppression d’une visionneuse à 360°

Lorsque vous supprimez une visionneuse, celle-ci est placée dans la corbeille. Cependant, les membres (ou &quot;enfants&quot;) de cet ensemble ne sont pas affectés ; au lieu de cela, ils conservent chacun leur état publié ou non publié existant.

Voir aussi [Manually publishing assets](publishing-files.md#manually-publishing-assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually-unpublishing-assets) (« Annulation manuelle de la publication des fichiers »).

**Pour supprimer une visionneuse à 360° :**

1. En mode Affichage de la grille, Affichage par liste ou Affichage des détails, sélectionnez une ou plusieurs visionneuses à 360°.
1. Dans la barre de navigation globale, accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Supprimer]** > **[!UICONTROL Supprimer]**.
