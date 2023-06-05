---
title: Création d’une visionneuse d’images
description: Découvrez comment créer une visionneuse d’images dans Adobe Dynamic Media Classic.
uuid: 689fdc14-4f51-4c94-8515-cd8551e101d8
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: 3f356410-b30e-4870-ad95-6e5a9dc126c8
feature: Dynamic Media Classic,Viewers,Image Sets,Spin Sets
role: User
exl-id: c18bb98c-b087-45d0-a4c9-44f58a3b514f
source-git-commit: 38d7f8d6e5888e1c5ba9260ada45b79fb16b338f
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 59%

---

# Création d’une visionneuse d’images{#creating-an-image-set}

Pour créer une visionneuse d’images avec des vues multiples, vos images doivent montrer un objet selon différentes perspectives ou montrer différents aspects d’un même article. L’objectif est de présenter aux utilisateurs des images d’un objet qui leur permettent de s’en faire une idée précise.

## Création d’une visionneuse d’images {#create}

Lorsque vous créez une visionneuse, l’option **[!UICONTROL Publish after save]** (« Publier après l’enregistrement ») affecte la visionneuse et ses membres comme suit :

| **[!UICONTROL Publier après l’enregistrement]** l’option sélectionnée avant l’enregistrement ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
| --- | --- | --- |
| Oui | Publié | Publié |
| Non | Non publié | Les membres de la visionneuse conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

Lorsque vous créez une visionneuse d’images, Adobe recommande les bonnes pratiques suivantes et applique les limites suivantes :

| Type de limite | Pratique recommandée | Limite imposée |
| --- | --- | --- |
| Nombre de ressources en double par ensemble | Aucun doublon | 20 |
| Nombre maximal d’images par visionneuse | 5 à 10 images par visionneuse | 1 000 |

Voir aussi [Limites de Dynamic Media](/help/using/limitations.md).

**Pour créer une visionneuse d’images:**

1. Effectuez l’une des opérations suivantes :

   * **Sélectionner les images en premier** - Dans le panneau de navigation, sélectionnez les images de votre visionneuse d’images, accédez à **[!UICONTROL Build]** > **[!UICONTROL Visionneuses d’images]**.

   * **Démarrage à partir de l’écran Visionneuse d’images** - Accédez à **[!UICONTROL Build]** > **[!UICONTROL Visionneuses d’images]**. L’écran Visionneuse d’images s’affiche. Sélectionnez un dossier dans la bibliothèque de fichiers, puis faites glisser les images de la visionneuse sur l’écran Visionneuse d’images.

1. Pour changer l’ordre des images, faites-les glisser vers leur nouvel emplacement.
1. Près de l’angle inférieur droit de la page, vérifiez que l’option **[!UICONTROL Publish after save]** (« Publier après l’enregistrement ») est sélectionnée (valeur par défaut).
1. Sélectionner **[!UICONTROL Enregistrer]**, sélectionnez un dossier pour le stockage de la visionneuse d’images, saisissez un nom pour la visionneuse, puis sélectionnez **[!UICONTROL Enregistrer]**.
1. Pour afficher votre visionneuse d’images dans la visionneuse, sélectionnez **[!UICONTROL Aperçu]** dans l’écran Visionneuse d’images. Vous pouvez sélectionner des miniatures d’échantillon dans la visionneuse d’images pour voir comment elles se comportent.

## Modification d’une visionneuse d’images {#editing-an-image-set}

Si vous modifiez un jeu publié ou non publié, la variable **[!UICONTROL Publier après l’enregistrement]** L’option affecte les membres de l’ensemble et de l’ensemble comme suit :

| Visionneuse déjà publiée ? | **[!UICONTROL Publier après l’enregistrement]** sélectionnée avant d’enregistrer votre modification ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
| --- | --- | --- | --- |
| Oui | Oui | Publié | Publié |
| Oui | Non | Publié | Les membres de visionneuse existants conservent leur état publié. Tout nouveau membre de visionneuse que vous ajoutez lors de votre modification conserve son état publié ou non publié. |
| Non | Oui | Publié | Publié |
| Non | Non | Non publié | Les membres de la visionneuse existants, ainsi que tout nouveau membre de la visionneuse que vous ajoutez lors de votre modification conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour modifier une visionneuse d’images:**

1. En mode d’affichage Grille, accédez à une visionneuse d’images, puis, sous l’image, sélectionnez **[!UICONTROL Modifier]**.
1. Utilisez l’une des méthodes suivantes :

   * Pour ajouter une image (publiée ou non publiée), faites-la glisser d’un dossier du panneau d’ajout de fichiers sur la page **[!UICONTROL des vues]** de la visionneuse d’images.
   * Pour supprimer une image, sélectionnez-la, puis sélectionnez **[!UICONTROL Supprimer]** dans la barre d’outils.
   * Pour réorganiser des images, faites glisser l’image de votre choix vers sa nouvelle position.

1. Lorsque vous avez terminé de modifier la visionneuse, près de l’angle inférieur droit de la page, assurez-vous que l’option **[!UICONTROL Publish after save]** (« Publier après l’enregistrement ») est sélectionnée (valeur par défaut).
1. Sélectionner **[!UICONTROL Enregistrer]**, sélectionnez un dossier de stockage pour la visionneuse, saisissez un nom pour la visionneuse, puis sélectionnez **[!UICONTROL Enregistrer]**.

## Suppression d’une visionneuse d’images {#deleting-an-image-set}

Lorsque vous supprimez une visionneuse, celle-ci est placée dans la corbeille. Toutefois, les membres (ou « enfants ») de cette visionneuse ne sont pas affectés : ils conservent en fait leur état existant publié ou non publié.

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour supprimer une visionneuse d’images:**

1. En mode Grille, Liste ou Détails, sélectionnez une visionneuse d’images ou plus.
1. Dans la barre de navigation globale, accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Supprimer]** > **[!UICONTROL Supprimer]**.
