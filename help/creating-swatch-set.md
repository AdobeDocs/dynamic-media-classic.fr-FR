---
title: Création d’une série d’échantillons
description: Découvrez comment créer une série d’échantillons.
uuid: 250b3525-310d-4481-b0bc-f9057e823e0b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/swatch_sets
discoiquuid: 631d2b2d-9e69-4b96-8392-17e00a1a8de0
feature: Dynamic Media Classic,Viewers
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '707'
ht-degree: 84%

---


# Création d’une série d’échantillons{#creating-a-swatch-set}

Une série d’échantillons permet à l’utilisateur de visualiser un objet dans une couleur, un motif ou un fini différent. Pour créer une série d’échantillons avec des nuances, vous devez disposer d’une image pour chaque couleur, motif ou fini que vous souhaitez présenter aux utilisateurs. Vous avez également besoin d’un échantillon pour chaque couleur, motif ou fini. 

Par exemple, si vous souhaitez présenter des casquettes avec des visières de couleurs différentes (rouge, vert et bleu), vous avez besoin de trois prises de vue de la même casquette : une première vue avec une visière rouge, une autre avec une visière verte et une dernière avec une visière bleue. Vous avez également besoin d’une nuance rouge, verte et bleue. Les nuances servent de miniatures sur lesquelles les utilisateurs cliquent dans la visionneuse de série d’échantillons pour visualiser les casquettes avec visière rouge, verte et bleue.

## Création d’une série d’échantillons  {#create}

Lorsque vous créez une visionneuse, l’option **Publier après l’enregistrement** affecte la visionneuse et ses membres comme suit :
| L&#39;option &quot;Publier après l&#39;enregistrement&quot; est sélectionnée avant l&#39;enregistrement ?|Etat de la visionneuse après l&#39;enregistrement|Etat des membres de la visionneuse après l&#39;enregistrement|
|— |— |— |
|Oui|Publié|Publié|
|Non|Non publié|Les membres de la visionneuse conservent leur état publié ou non publié.|

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour créer une série d’échantillons**

1. Effectuez l’une des opérations suivantes :

   **Sélectionnez d’** abord les images dans le panneau de navigation, sélectionnez les images, puis cliquez sur Créer > Séries d’échantillons.

   **Début de l’** écran Série d’échantillonsCliquez sur Créer > Séries d’échantillons. Sélectionnez un dossier dans la bibliothèque des fichiers, puis faites glisser les images sur la section Vues de la page Série d’échantillons.

1. Faites glisser des nuances, des motifs ou des finis sur l’emplacement réservé Echantillons de la page Série d’échantillons.

   Assurez-vous que l’échantillon de la couleur, du motif ou du fini que vous faites glisser sur chaque emplacement réservé correspond à celui de l’image adjacente.

1. Pour changer l’ordre des images dans votre série d’échantillons, faites-les glisser vers leur nouvel emplacement.
1. Près de l’angle inférieur droit de la page, vérifiez que l’option **Publish after save** (« Publier après l’enregistrement ») est sélectionnée (valeur par défaut).
1. Cliquez sur **Enregistrer**, sélectionnez un dossier pour y stocker votre série d’échantillons, attribuez un nom à la série, puis cliquez sur Envoyer.
1. Pour afficher votre série d’échantillons dans sa visionneuse, cliquez sur **Prévisualiser** dans l’écran Série d’échantillons. Vous pouvez cliquer sur des miniatures d’échantillon dans la visionneuse de série d’échantillons afin d’examiner leur comportement.

## Modification d’une série d’échantillons  {#editing-a-swatch-set}

Selon que vous modifiez une visionneuse publiée ou non publiée, l’option **Publish after save** (« Publier après l’enregistrement ») affecte la visionneuse et ses membres comme suit :

| Visionneuse déjà publiée ? | L’option « Publish after save » (« Publier après l’enregistrement ») est-elle sélectionnée avant l’enregistrement de votre modification ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
|--- |--- |--- |--- |
| Oui | Oui | Publié | Publié |
| Oui | Non | Publié | Les membres de visionneuse existants conservent leur état publié. Tous les nouveaux membres de visionneuse que vous avez ajoutés pendant votre modification conservent leur état publié ou non publié. |
| Non | Oui | Publié | Publié |
| Non | Non | Non publié | Les membres de la visionneuse existants, ainsi que tout nouveau membre de la visionneuse que vous ajoutez lors de votre modification conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour modifier une série d’échantillons**

1. En mode Grille, recherchez un SwatchSet (série d’échantillons), puis au-dessous de l’image, cliquez sur **Modifier**.
1. Utilisez l’une des méthodes suivantes :

   * Pour ajouter une image (publiée ou non publiée), faites-la glisser d’un dossier du panneau d’ajout des fichiers sur la page **des vues** de la série d’échantillons.
   * Pour supprimer une image, sélectionnez-la, puis cliquez sur **Supprimer** dans la barre d’outils.
   * Pour réorganiser des images, faites glisser l’image de votre choix vers sa nouvelle position.

1. Lorsque vous avez terminé de modifier la visionneuse, près de l’angle inférieur droit de la page, assurez-vous que l’option **Publish after save** (« Publier après l’enregistrement ») est sélectionnée (valeur par défaut).
1. Cliquez sur **Enregistrer**, sélectionnez un dossier de stockage, attribuez un nom à la visionneuse, puis cliquez sur **Enregistrer**.

## Suppression d’une série d’échantillons  {#deleting-a-swatch-set}

Lorsque vous supprimez une visionneuse, celle-ci est placée dans la corbeille. Toutefois, les membres (ou « enfants ») de cette visionneuse ne sont pas affectés : ils conservent en fait leur état existant publié ou non publié.

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour supprimer une série d’échantillons**

1. En mode Affichage de la grille, Affichage par liste ou Affichage des détails, sélectionnez une ou plusieurs séries d’échantillons.
1. Sur la barre de navigation globale, cliquez sur **Fichier** > **Supprimer** > **Supprimer**.

