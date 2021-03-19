---
title: Création d’une visionneuse à 360°
description: Découvrez comment créer une visionneuse à 360°.
uuid: 697bd78f-5e39-46bf-aa6d-ad8ab99fe40e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 735b5867-e249-4627-a5a5-25c19c2255bf
feature: Dynamic Media Classic, Visionneuses, Visionneuses à 360°
role: Professionnel
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '909'
ht-degree: 73%

---


# Création d’une visionneuse à 360°{#creating-a-spin-set}

Pour créer une visionneuse panoramique efficace, assurez-vous que les clichés soient pris correctement. Vous pouvez créer une visionneuse à 360° dans Dynamic Media Classic en sélectionnant le bouton Créer, puis en choisissant Visionneuses à 360°. Modifiez les visionneuses à 360° dans l’écran correspondant.

>[!NOTE]
>
>Les versions précédentes de Dynamic Media Classic n’offres pas les visionneuses à 360° bidimensionnelles. Si vous avez créé une visionneuse à 360° dans une version précédente de Dynamic Media Classic, vous ne pouvez pas enregistrer votre visionneuse à 360° unidimensionnelle sans l’enregistrer d’abord sous un autre nom. Cliquez sur Enregistrer sous dans l’écran Visionneuse à 360° et saisissez un nouveau nom afin de pouvoir le modifier dans Dynamic Media Classic.

## Instructions pour prendre des clichés d’images de la visionneuse à 360°{#guidelines-for-shooting-spin-set-images}

En règle générale, plus le nombre d’images de la visionneuse est élevé, meilleure est la qualité de l’effet de rotation de l’objet. Cependant, un nombre élevé d’images dans la visionneuse augmente la durée de chargement des images. Dynamic Media Classic recommande les consignes suivantes pour les prises de vue d’images à utiliser dans les visionneuses à 360° :

* Utilisez au minimum 8 à 12 images dans une visionneuse à 360° unidimensionnelle et 16 à 24 images dans une visionneuse à 360° bidimensionnelle.
* Utilisez un format d’image sans perte (formats TIFF et PNG recommandés). 
* Masquez toutes les images pour faire apparaître l’objet sur un fond blanc ou fortement contrasté. Ajoutez éventuellement des ombres.
* Assurez-vous que les détails du produit sont bien éclairés et que leur mise au point est nette.
* Prenez des clichés de vêtements de prêt-à-porter avec un mannequin ou un modèle. Souvent, le mannequin est entièrement masqué (avec un mannequin en verre), ou un mannequin stylé/de couture est visible sur l’image. Vous pouvez créer une visionneuse sur un modèle vivant en définissant le nombre d’angles. Marquez chaque angle avec du ruban adhésif sur le sol pour guider le modèle sur la pose à prendre et indiquer la direction de chaque prise de vue. 

## Création d’une visionneuse à 360°  {#create}

Notez que l’ordre dans lequel la visionneuse à 360° est créée ou créée dans Dynamic Media Classic est important. La rotation de la visionneuse à 360° varie en fonction du classement des fichiers lorsque vous faites glisser et déposer des images dans la grille de la page de la visionneuse à 360°. L’ordre dans lequel elle est affichée dans la zone de création définit sa rotation lorsque l’utilisateur déplace le pointeur de la souris ou ses doigts, de gauche à droite.

Lorsque vous créez une visionneuse, l’option **Publish after save** (« Publier après l’enregistrement ») affecte la visionneuse et ses membres comme suit :

| L’option « Publish after save » (« Publier après l’enregistrement ») est-elle sélectionnée avant l’enregistrement ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
|--- |--- |--- |
| Oui | Publié | Publié |
| Non | Non publié | Les membres de la visionneuse conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually-publishing-assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually-unpublishing-assets) (« Annulation manuelle de la publication des fichiers »).

Lorsque vous enregistrez une visionneuse à 360°, vous pouvez ensuite utiliser la fonction Prévisualiser dans la page Créer : Visionneuse à 360° pour voir comment s’affiche votre visionneuse à 360° dans la visionneuse par défaut.

**Pour créer une visionneuse à 360°**

1. Dans le menu déroulant **Créer**, cliquez sur **Visionneuse à 360°**.
1. Dans la boîte de dialogue Visionneuse à 360°, définissez le nombre de lignes et de cellules.

   Pour une visionneuse à 360° unidimensionnelle, sélectionnez une seule ligne.

   Pour une visionneuse à 360° bidimensionnelle, sélectionnez au moins deux lignes.

1. Cliquez sur **OK**.
1. Faites glisser des images vers la grille de l’écran Visionneuse à 360°.
1. Une fois terminé, près de l’angle inférieur droit de la page, vérifiez que l’option **Publish after save** (« Publier après l’enregistrement ») est sélectionnée (valeur par défaut).
1. Cliquez sur **Enregistrer**.
1. Dans la boîte de dialogue Enregistrer, sélectionnez le dossier dans lequel conserver la visionneuse à 360°. Dans le champ Nom de fichier, saisissez le nom de la visionneuse à 360°.
1. Cliquez sur **Enregistrer**.

## Edition d’une visionneuse à 360°  {#editing-a-spin-set}

Selon que vous modifiez une visionneuse publiée ou non publiée, l’option **Publish after save** (« Publier après l’enregistrement ») affecte la visionneuse et ses membres comme suit :

| Visionneuse déjà publiée ? | L’option « Publish after save » (« Publier après l’enregistrement ») est-elle sélectionnée avant l’enregistrement de votre modification ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
|--- |--- |--- |--- |
| Oui | Oui | Publié | Publié |
| Oui | Non | Publié | Les membres de visionneuse existants conservent leur état publié. Tous les nouveaux membres de visionneuse que vous avez ajoutés pendant votre modification conservent leur état publié ou non publié. |
| Non | Oui | Publié | Publié |
| Non | Non | Non publié | Les membres de la visionneuse existants, ainsi que tout nouveau membre de la visionneuse que vous ajoutez lors de votre modification conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually-publishing-assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually-unpublishing-assets) (« Annulation manuelle de la publication des fichiers »).

**Pour modifier une visionneuse à 360°**

1. Cliquez sur le bouton de survol **Modifier** de la visionneuse à 360°.
1. Utilisez l’une des méthodes suivantes :

   * **Suppression d&#39;**
imagesSélectionnez l&#39;image, puis cliquez sur 
**Supprimer**.

   * **Ajouter**
des imagesFaites glisser l&#39;image dans une cellule.

   * **Réorganisation des lignes (visionneuses à 360° bidimensionnelles)**
Cliquez sur une zone de sélection de ligne (à gauche de la ligne), puis cliquez sur 
**Déplacer la rangée** Déplacer la rangée vers le haut ****.

   * **Ajouter des rangées et des**
cellulesEntrez un nombre dans les zones Lignes et Cellules pour déterminer le nombre de rangées et le nombre de cellules dans chaque rangée.

1. Une fois les modifications terminées, près de l’angle inférieur droit de la page, vérifiez que l’option **Publish after save** (« Publier après l’enregistrement ») est sélectionnée (valeur par défaut).
1. Cliquez sur **Enregistrer**, sélectionnez un dossier de stockage, attribuez un nom à la visionneuse, puis cliquez sur **Enregistrer**.

## Suppression d’une visionneuse à 360°  {#deleting-a-spin-set}

Lorsque vous supprimez une visionneuse, celle-ci est placée dans la corbeille. Toutefois, les membres (ou « enfants ») de cette visionneuse ne sont pas affectés : ils conservent en fait leur état existant publié ou non publié.

Voir aussi [Manually publishing assets](publishing-files.md#manually-publishing-assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually-unpublishing-assets) (« Annulation manuelle de la publication des fichiers »).

**Pour supprimer une visionneuse à 360°**

1. En mode Affichage de la grille, Affichage par liste ou Affichage des détails, sélectionnez une ou plusieurs visionneuses à 360°.
1. Sur la barre de navigation globale, cliquez sur **Fichier** > **Supprimer** > **Supprimer**.

