---
title: Création d’une visionneuse d’images
description: Découvrez comment créer une visionneuse d’images dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
feature: Dynamic Media Classic,Viewers,Image Sets,Spin Sets
role: User
exl-id: c18bb98c-b087-45d0-a4c9-44f58a3b514f
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 38%

---

# Création d’une visionneuse d’images{#creating-an-image-set}

Pour créer une visionneuse d’images avec des vues multiples, vos images doivent montrer un objet selon différentes perspectives ou montrer différents aspects d’un même article. L’objectif est de présenter aux utilisateurs des images d’un objet qui leur permettent de s’en faire une idée précise.

## Création d’une visionneuse d’images {#create}

Lorsque vous créez une visionneuse, l’option **[!UICONTROL Publier après un enregistrement]** affecte la visionneuse et les membres de la visionneuse des manières suivantes :

| **[!UICONTROL `Publish after a save`]** option sélectionnée avant l’enregistrement ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
| --- | --- | --- |
| Oui | Publié | Publié |
| Non | Non publié | Les membres de la visionneuse conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

Lorsque vous créez une visionneuse d’images, Adobe recommande les bonnes pratiques suivantes et applique les limites suivantes :

| Type de limite | Pratique recommandée | Limite imposée |
| --- | --- | --- |
| Nombre de ressources en double par visionneuse | Aucun doublon | 20 ‡ |
| Nombre maximal d’images par visionneuse | 5 à 10 images par ensemble | 1 000 |

‡ Il est recommandé de ne pas avoir de ressources en double dans un ensemble. La limite est de 20 doublons pour une seule ressource. Si, dans l’ensemble, vous ajoutez un autre doublon pour cette ressource, la requête renvoie une erreur ou ignore le doublon.

Voir aussi [Limites de Dynamic Media](/help/using/limitations.md).

**Création d’une visionneuse d’images:**

1. Effectuez l’une des opérations suivantes :

   * **Sélectionnez d’abord les images** : dans le panneau Parcourir , sélectionnez les images à utiliser pour votre visionneuse d’images, puis accédez à **[!UICONTROL Créer]** > **[!UICONTROL Visionneuses d’images]**.

   * **À partir de l’écran de la visionneuse d’images** : accédez à **[!UICONTROL Créer]** > **[!UICONTROL Visionneuses d’images]**. L’écran Visionneuse d’images s’affiche. Sélectionnez un dossier dans la bibliothèque de fichiers, puis faites glisser les images de la visionneuse sur l’écran Visionneuse d’images.

1. Pour changer l’ordre des images, faites-les glisser vers leur nouvel emplacement.
1. Près du coin inférieur droit de la page, assurez-vous que l’option **[!UICONTROL Publier après un enregistrement]** est sélectionnée (par défaut).
1. Sélectionnez **[!UICONTROL Enregistrer]**, sélectionnez un dossier pour stocker votre visionneuse d’images, saisissez un nom pour la visionneuse, puis sélectionnez **[!UICONTROL Enregistrer]**.
1. Pour afficher la visionneuse d’images dans la visionneuse d’images, sélectionnez **[!UICONTROL Aperçu]** dans l’écran de la visionneuse d’images. Vous pouvez sélectionner des miniatures d’échantillon dans la visionneuse d’images pour voir comment elles se comportent.

## Modification d’une visionneuse d’images {#editing-an-image-set}

Que vous modifiiez une visionneuse publiée ou dépubliée, l’option **[!UICONTROL Publier après un enregistrement]** affecte la visionneuse et les membres de la visionneuse des manières suivantes :

| Visionneuse déjà publiée ? | **[!UICONTROL `Publish after a save`]** option sélectionnée avant d’enregistrer votre modification ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
| --- | --- | --- | --- |
| Oui | Oui | Publié | Publié |
| Oui | Non | Publié | Les membres d’ensemble existants conservent leur statut publié. Tout nouveau membre de visionneuse que vous ajoutez lors de votre modification conserve son état publié ou non publié. |
| Non | Oui | Publié | Publié |
| Non | Non | Non publié | Les membres de la visionneuse existants, ainsi que tout nouveau membre de la visionneuse que vous ajoutez lors de votre modification conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour modifier une visionneuse d’images :**

1. Dans la vue Grille, accédez à une visionneuse d’images, puis, sous l’image, sélectionnez **[!UICONTROL Modifier]**.
1. Utilisez l’une des méthodes suivantes :

   * Pour ajouter une image (publiée ou dépubliée), faites-la glisser d’un dossier dans Ajouter Assets vers la page **[!UICONTROL Vues]** de la visionneuse d’images.
   * Pour supprimer une image, sélectionnez-la, puis sélectionnez **[!UICONTROL Supprimer]** dans la barre d’outils.
   * Pour réorganiser des images, faites glisser l’image de votre choix vers sa nouvelle position.

1. Lorsque vous avez terminé de modifier la visionneuse, près du coin inférieur droit de la page, assurez-vous que l’option **[!UICONTROL Publier après un enregistrement]** est sélectionnée (par défaut).
1. Sélectionnez **[!UICONTROL Enregistrer]**, sélectionnez un dossier de stockage pour votre visionneuse, saisissez un nom pour la visionneuse, puis sélectionnez **[!UICONTROL Enregistrer]**.

## Suppression d’une visionneuse d’images

Lorsque vous supprimez une visionneuse, celle-ci est placée dans la corbeille. Toutefois, les membres (ou « enfants ») de cet ensemble ne sont pas affectés. Ils conservent chacun leur état publié ou dépublié existant.

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour supprimer une visionneuse d’images :**

1. Dans la vue Grille, Liste ou Détails, sélectionnez une visionneuse d’images ou plusieurs.
1. Sur la barre de navigation globale, accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Supprimer]** > **[!UICONTROL Supprimer]**.
