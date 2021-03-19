---
title: Création d’une visionneuse d’images
description: Découvrez comment créer une visionneuse d’images.
uuid: 689fdc14-4f51-4c94-8515-cd8551e101d8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: 3f356410-b30e-4870-ad95-6e5a9dc126c8
feature: Dynamic Media Classic, Visionneuses, Visionneuses d’images
role: Professionnel
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '589'
ht-degree: 88%

---


# Création d’une visionneuse d’images{#creating-an-image-set}

Pour créer une visionneuse d’images avec des vues multiples, vos images doivent montrer un objet selon différentes perspectives ou montrer différents aspects d’un même article. L’objectif est de présenter aux utilisateurs des images d’un objet qui leur permettent de s’en faire une idée précise.

## Création d’une visionneuse d’images  {#create}

Lorsque vous créez une visionneuse, l’option **Publish after save** (« Publier après l’enregistrement ») affecte la visionneuse et ses membres comme suit :

| L’option « Publish after save » (« Publier après l’enregistrement ») est-elle sélectionnée avant l’enregistrement ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
|:--- |:--- |:--- |
| Oui | Publié | Publié |
| Non | Non publié | Les membres de la visionneuse conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour créer une visionneuse d’images**

1. Effectuez l’une des opérations suivantes :

   **Sélectionnez** d’abord les imagesDans le panneau de navigation, sélectionnez les images de votre visionneuse, cliquez sur Créer > Visionneuses d’images.

   **Début de l’** écran Visionneuse d’imagesCliquez sur Créer > Visionneuses d’images. L’écran Visionneuse d’images s’affiche. Sélectionnez un dossier dans la bibliothèque de fichiers, puis faites glisser les images de la visionneuse sur l’écran Visionneuse d’images.

1. Pour changer l’ordre des images, faites-les glisser vers leur nouvel emplacement.
1. Près de l’angle inférieur droit de la page, vérifiez que l’option **Publish after save** (« Publier après l’enregistrement ») est sélectionnée (valeur par défaut).
1. Cliquez sur **Enregistrer**, sélectionnez un dossier pour y stocker la visionneuse d’images, attribuez un nom à la visionneuse, puis cliquez sur **Enregistrer**.
1. Pour afficher vos images dans la visionneuse, cliquez sur **Prévisualiser** dans l’écran Visionneuse d’images. Vous pouvez cliquer sur des miniatures d’échantillon dans la visionneuse d’images afin d’examiner leur comportement.

## Modification d’une visionneuse d’images  {#editing-an-image-set}

Selon que vous modifiez une visionneuse publiée ou non publiée, l’option **Publish after save** (« Publier après l’enregistrement ») affecte la visionneuse et ses membres comme suit :

| Visionneuse déjà publiée ? | L’option « Publish after save » (« Publier après l’enregistrement ») est-elle sélectionnée avant l’enregistrement de votre modification ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
|--- |--- |--- |--- |
| Oui | Oui | Publié | Publié |
| Oui | Non | Publié | Les membres de visionneuse existants conservent leur état publié. Tous les nouveaux membres de visionneuse que vous avez ajoutés pendant votre modification conservent leur état publié ou non publié. |
| Non | Oui | Publié | Publié |
| Non | Non | Non publié | Les membres de la visionneuse existants, ainsi que tout nouveau membre de la visionneuse que vous ajoutez lors de votre modification conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour modifier une visionneuse d’images**

1. En mode Grille, recherchez un ImageSet (visionneuse d’images), puis au-dessous de l’image, cliquez sur **Modifier**.
1. Utilisez l’une des méthodes suivantes :

   * Pour ajouter une image (publiée ou non publiée), faites-la glisser d’un dossier du panneau d’ajout de fichiers sur la page **des vues** de la visionneuse d’images.
   * Pour supprimer une image, sélectionnez-la, puis cliquez sur **Supprimer** dans la barre d’outils.
   * Pour réorganiser des images, faites glisser l’image de votre choix vers sa nouvelle position.

1. Lorsque vous avez terminé de modifier la visionneuse, près de l’angle inférieur droit de la page, assurez-vous que l’option **Publish after save** (« Publier après l’enregistrement ») est sélectionnée (valeur par défaut).
1. Cliquez sur **Enregistrer**, sélectionnez un dossier pour y stocker la visionneuse, attribuez un nom à celle-ci, puis cliquez sur **Enregistrer**.

## Suppression d’une visionneuse d’images  {#deleting-an-image-set}

Lorsque vous supprimez une visionneuse, celle-ci est placée dans la corbeille. Toutefois, les membres (ou « enfants ») de cette visionneuse ne sont pas affectés : ils conservent en fait leur état existant publié ou non publié.

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour supprimer une visionneuse d’images**

1. En mode Affichage de la grille, Affichage par liste ou Affichage des détails, sélectionnez une ou plusieurs visionneuses d’images.
1. Sur la barre de navigation globale, cliquez sur **Fichier** > **Supprimer** > **Supprimer**.

