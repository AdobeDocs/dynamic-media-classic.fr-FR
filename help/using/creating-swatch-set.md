---
title: Création de la série d’échantillons
description: Découvrez comment créer un ensemble d’échantillons dans Adobe Dynamic Media Classic.
uuid: 250b3525-310d-4481-b0bc-f9057e823e0b
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/swatch_sets
discoiquuid: 631d2b2d-9e69-4b96-8392-17e00a1a8de0
feature: Dynamic Media Classic,Viewers
role: User
exl-id: 426b6e6b-daed-4ca6-b095-99bb06604b07
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 67%

---

# Création de la série d’échantillons{#creating-a-swatch-set}

Une série d’échantillons permet à l’utilisateur de visualiser un objet dans une couleur, un motif ou un fini différent. Pour créer une série d’échantillons avec des nuances, vous devez disposer d’une image pour chaque couleur, motif ou fini que vous souhaitez présenter aux utilisateurs. Vous avez également besoin d’un échantillon pour chaque couleur, motif ou fini. 

Par exemple, si vous souhaitez présenter des casquettes avec des visières de couleurs différentes (rouge, vert et bleu), vous avez besoin de trois prises de vue de la même casquette : une première vue avec une visière rouge, une autre avec une visière verte et une dernière avec une visière bleue. Vous avez également besoin d’une nuance rouge, verte et bleue. Les échantillons de couleurs servent de miniatures que les utilisateurs sélectionnent dans la visionneuse de séries d’échantillons pour afficher les visionneuses rouge, verte ou bleue.

## Création de la série d’échantillons {#create}

Lorsque vous créez une visionneuse, l’option **Publish after save** (« Publier après l’enregistrement ») affecte la visionneuse et ses membres comme suit :

| **[!UICONTROL Publier après l’enregistrement]** l’option sélectionnée avant l’enregistrement ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
| --- | --- | --- |
| Oui | Publié | publié |
| Non | Non publié | Les membres de la visionneuse conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour créer une série d’échantillons:**

1. Effectuez l’une des opérations suivantes :

   * **Sélectionner les images en premier** - Dans le panneau de navigation, sélectionnez les images, puis accédez à **[!UICONTROL Build]** > **[!UICONTROL Séries d’échantillons]**.

   * **Démarrage à partir de l’écran Série d’échantillons** - Accédez à **[!UICONTROL Build]** > **[!UICONTROL Séries d’échantillons]**. Sélectionnez un dossier dans la bibliothèque des fichiers, puis faites glisser les images sur la section Vues de la page Série d’échantillons.

1. Faites glisser des nuances, des motifs ou des finis sur l’emplacement réservé Echantillons de la page Série d’échantillons.

   Assurez-vous que l’échantillon de la couleur, du motif ou du fini que vous faites glisser sur chaque emplacement réservé correspond à celui de l’image adjacente.

1. Pour changer l’ordre des images dans votre série d’échantillons, faites-les glisser vers leur nouvel emplacement.
1. Près de l’angle inférieur droit de la page, vérifiez que l’option **[!UICONTROL Publish after save]** (« Publier après l’enregistrement ») est sélectionnée (valeur par défaut).
1. Sélectionner **[!UICONTROL Enregistrer]**, sélectionnez un dossier pour le stockage de la série d’échantillons de couleurs, saisissez un nom pour la série, puis sélectionnez **[!UICONTROL Envoyer]**.
1. Pour afficher votre série d’échantillons dans la visionneuse, sélectionnez **[!UICONTROL Aperçu]** sur l’écran Série d’échantillons . Vous pouvez sélectionner des miniatures d’échantillon dans la visionneuse de séries d’échantillons pour voir comment elles se comportent.

## Modification d’une série d’échantillons {#editing-a-swatch-set}

Si vous modifiez un jeu publié ou non publié, la variable **[!UICONTROL Publier après l’enregistrement]** L’option affecte les membres de l’ensemble et de l’ensemble comme suit :

| Visionneuse déjà publiée ? | **[!UICONTROL Publier après]** option d’enregistrement sélectionnée avant d’enregistrer votre modification ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
|--- |--- |--- |--- |
| Oui | Oui | Publié | Publié |
| Oui | Non | Publié | Les membres de visionneuse existants conservent leur état publié. Tout nouveau membre de visionneuse que vous ajoutez lors de votre modification conserve son état publié ou non publié. |
| Non | Oui | Publié | Publié |
| Non | Non | Non publié | Les membres de la visionneuse existants, ainsi que tout nouveau membre de la visionneuse que vous ajoutez lors de votre modification conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour modifier une série d’échantillons:**

1. En mode d’affichage Grille, accédez à un SwatchSet, puis sous l’image, sélectionnez **[!UICONTROL Modifier]**.
1. Utilisez l’une des méthodes suivantes :

   * Pour ajouter une image (publiée ou non publiée), faites-la glisser d’un dossier du panneau d’ajout des fichiers sur la page **[!UICONTROL des vues]** de la série d’échantillons.
   * Pour supprimer une image, sélectionnez-la, puis sélectionnez **[!UICONTROL Supprimer]** dans la barre d’outils.
   * Pour réorganiser des images, faites glisser l’image de votre choix vers sa nouvelle position.

1. Lorsque vous avez terminé de modifier la visionneuse, près de l’angle inférieur droit de la page, assurez-vous que l’option **[!UICONTROL Publish after save]** (« Publier après l’enregistrement ») est sélectionnée (valeur par défaut).
1. Sélectionner **[!UICONTROL Enregistrer]**, sélectionnez un dossier de stockage, saisissez un nom pour la visionneuse, puis sélectionnez **[!UICONTROL Enregistrer]**.

## Suppression d’une série d’échantillons {#deleting-a-swatch-set}

Lorsque vous supprimez une visionneuse, celle-ci est placée dans la corbeille. Toutefois, les membres (ou « enfants ») de cette visionneuse ne sont pas affectés : ils conservent en fait leur état existant publié ou non publié.

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour supprimer une série d’échantillons:**

1. En mode Grille, Liste ou Détails, sélectionnez une série d’échantillons ou plus.
1. Dans la barre de navigation globale, accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Supprimer]** > **[!UICONTROL Supprimer]**.
