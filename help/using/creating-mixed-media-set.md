---
title: Création d’une visionneuse de supports variés
description: Découvrez comment créer une visionneuse de médias mixtes dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: 18669c65-a1c4-4012-8587-cd5095f4bd4e
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 56%

---

# Création d’une visionneuse de supports variés{#creating-a-mixed-media-set}

Vous pouvez créer une visionneuse de supports variés pour associer plusieurs types de visionneuses dans une même présentation. Veillez à ce que vos fichiers, visionneuses d’images, séries d’échantillons et visionneuses à 360° soient prêts pour la publication avant de les ajouter à la visionneuse de supports variés.

![Visionneuse de médias mixtes](/help/using/assets/mm_mixed_media_set.png)

## Création d’une visionneuse de supports variés {#create-a-mixed-media-set}

Lorsque vous créez une visionneuse, l’option **Publish after a save** affecte la visionneuse et les membres de la façon suivante :

| Option &quot;Publish après un enregistrement&quot; sélectionnée avant l’enregistrement ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
| --- | --- | --- |
| Oui | Publié | Publié |
| Non | Non publié | Les membres de la visionneuse conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour créer une visionneuse de médias mixtes :**

1. Accédez à **[!UICONTROL Build]** > **[!UICONTROL Mixed Media Sets]**.
1. Faites glisser les vidéos, visionneuses d’images, visionneuses à 360° et échantillons depuis la bibliothèque de fichiers vers l’écran Visionneuse de supports variés.

   >[!NOTE]
   >
   >Une visionneuse de médias mixtes ne prend pas en charge les ressources dont le nom de fichier contient les caractères suivants : `( ) { }`.

1. Utilisez l’une des méthodes suivantes :

   * Pour ajouter une bande sonore, faites glisser un fichier audio depuis la bibliothèque de fichiers vers la zone Bande sonore. La bande sonore est lue pendant l’affichage des images. Elle s’arrête lors de la lecture d’une vidéo.
   * Pour changer l’ordre des visionneuses, faites-les glisser à l’emplacement de votre choix sur l’écran Visionneuse de supports variés. L’ordre des visionneuses à l’écran détermine l’ordre (de gauche à droite) dans lequel les utilisateurs les visualisent dans la visionneuse de supports variés.
   * (Optionnel) Pour ajouter une miniature personnalisée représentant une vidéo dans la visionneuse, faites glisser un fichier d’image depuis la bibliothèque de fichiers vers l’emplacement réservé à la miniature.

1. Près du coin inférieur droit de la page, assurez-vous que **[!UICONTROL Publish after a save]** est sélectionné (par défaut).
1. Sélectionnez **[!UICONTROL Enregistrer]**.
1. Sélectionnez un dossier pour le stockage de votre visionneuse de médias mixtes, puis saisissez un nom pour la visionneuse.
1. Sélectionnez **[!UICONTROL Enregistrer]**.

   Pour voir à quoi ressemble votre visionneuse d’images combinée dans une visionneuse d’images, sélectionnez **[!UICONTROL Aperçu]**.

## Modification d’une visionneuse de supports variés {#edit-a-mixed-media-set}

Vous pouvez modifier une visionneuse de supports variés. Pour modifier une visionneuse contenue dans une visionneuse de supports variés, ouvrez-la séparément, modifiez-la, puis enregistrez-la. Les modifications s’affichent dans la visionneuse de médias mixtes.

Que vous modifiiez un jeu publié ou non publié, l’option **[!UICONTROL Publish after a save]** affecte l’ensemble et définit ses membres de la manière suivante :

| Visionneuse déjà publiée ? | **[!UICONTROL Publish après un enregistrement]** sélectionné avant d&#39;enregistrer votre modification ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
| --- |--- |--- |--- |
| Oui | Oui | Publié | Publié |
| Oui | Non | Publié | Les membres de visionneuse existants conservent leur état publié. Tout nouveau membre de visionneuse que vous ajoutez lors de votre modification conserve son état publié ou non publié. |
| Non | Oui | Publié | Publié |
| Non | Non | Non publié | Les membres de la visionneuse existants, ainsi que tout nouveau membre de la visionneuse que vous ajoutez lors de votre modification conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour modifier une visionneuse de médias mixtes :**

1. Sélectionnez le bouton de survol **[!UICONTROL Modifier]** de la visionneuse de médias mixtes.
1. Utilisez l’une des méthodes suivantes :

   * Pour supprimer des éléments, sélectionnez-les et sélectionnez **[!UICONTROL Supprimer]**.
   * Pour réorganiser des objets, faites-les glisser vers leur nouvel emplacement.

1. Lorsque vous avez terminé de modifier la visionneuse, près du coin inférieur droit de la page, assurez-vous que **[!UICONTROL Publish after a save]** est sélectionné (par défaut).
1. Sélectionnez **[!UICONTROL Enregistrer]** ou **[!UICONTROL Enregistrer sous]**.

## Suppression d’une visionneuse de médias mixtes

Lorsque vous supprimez une visionneuse, celle-ci est placée dans la corbeille. Cependant, les membres (ou &quot;enfants&quot;) de cet ensemble ne sont pas affectés ; au lieu de cela, ils conservent chacun leur état publié ou non publié existant.

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour supprimer une visionneuse de médias mixtes :**

1. En mode Affichage de la grille, Affichage par liste ou Affichage des détails, sélectionnez une ou plusieurs visionneuses de supports variés.
1. Dans la barre de navigation globale, accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Supprimer]** > **[!UICONTROL Supprimer]**.
