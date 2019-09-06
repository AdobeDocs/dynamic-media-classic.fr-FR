---
title: Création d’une visionneuse de supports variés
seo-title: Création d’une visionneuse de supports variés
description: 'null'
seo-description: Découvrez comment créer une visionneuse de supports variés.
uuid: a 0 c 6 e 5 fa -7 a 85-4376-b 9 a 3-b 72 ae 63 d 3 d 95
contentOwner: admin
content-type: référence
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
discoiquuid: 0 ff 9 e 763-897 c -4 ba 5-b 606-a 95 d 5 e 45 f 35 e
translation-type: tm+mt
source-git-commit: 2f99190eb0c346b87402e69c4067e94365042339

---


# Création d’une visionneuse de supports variés{#creating-a-mixed-media-set}

Vous pouvez créer une visionneuse de supports variés pour associer plusieurs types de visionneuses dans une même présentation. Veillez à ce que vos fichiers, visionneuses d’images, séries d’échantillons et visionneuses à 360° soient prêts pour la publication avant de les ajouter à la visionneuse de supports variés.

![Visionneuse de supports variés](/help/assets/mm_mixed_media_set.png)

## Création d’une visionneuse de supports variés {#create-a-mixed-media-set}

Lorsque vous créez une visionneuse, l’option **Publish after save** (« Publier après l’enregistrement ») affecte la visionneuse et ses membres comme suit :

| L’option « Publish after save » (« Publier après l’enregistrement ») est-elle sélectionnée avant l’enregistrement ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
|--- |--- |--- |
| Oui | Publié | Publié |
| Non | Non publié | Les membres de la visionneuse conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Création d’une visionneuse de supports variés**

1. Cliquez sur **Créer** &gt; **Visionneuses de supports variés**.
1. Faites glisser les vidéos, visionneuses d’images, visionneuses à 360° et échantillons depuis la bibliothèque de fichiers vers l’écran Visionneuse de supports variés.

   >[!NOTE]
   >
   >les visionneuses de supports variés ne prennent pas en charge les éléments dont le nom de fichier comporte l’un des caractères suivants : ( ) { }.

1. Utilisez l’une des méthodes suivantes :

   * Pour ajouter une bande sonore, faites glisser un fichier audio depuis la bibliothèque de fichiers vers la zone Bande sonore. La bande sonore est lue pendant l’affichage des images. Elle s’arrête dès que la lecture de la vidéo commence.
   * Pour changer l’ordre des visionneuses, faites-les glisser à l’emplacement de votre choix sur l’écran Visionneuse de supports variés. L’ordre des visionneuses à l’écran détermine l’ordre (de gauche à droite) dans lequel les utilisateurs les visualisent dans la visionneuse de supports variés.
   * (Optionnel) Pour ajouter une miniature personnalisée représentant une vidéo dans la visionneuse, faites glisser un fichier d’image depuis la bibliothèque de fichiers vers l’emplacement réservé à la miniature.

1. Près de l’angle inférieur droit de la page, assurez-vous que l’option **Publish after save** (« Publier après l’enregistrement ») est sélectionnée (valeur par défaut).
1. Cliquez sur **Enregistrer**, sélectionnez un dossier pour y stocker votre visionneuse de supports variés, attribuez un nom à la visionneuse, puis cliquez sur **Enregistrer**.

   Cliquez sur **Aperçu** pour voir à quoi ressemble votre visionneuse combinée dans une visionneuse d’images.

## Modification d’une visionneuse de supports variés {#edit-a-mixed-media-set}

Vous pouvez modifier une visionneuse de supports variés. Pour modifier une visionneuse contenue dans une visionneuse de supports variés, ouvrez-la séparément, modifiez-la, puis enregistrez-la. Les modifications s’affichent dans la visionneuse de supports variés.

Selon que vous modifiez une visionneuse publiée ou non publiée, l’option **Publish after save** (« Publier après l’enregistrement ») affecte la visionneuse et ses membres comme suit :

| Visionneuse déjà publiée ? | L’option « Publish after save » (« Publier après l’enregistrement ») est-elle sélectionnée avant l’enregistrement de votre modification ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
|--- |--- |--- |--- |
| Oui | Oui | Publié | Publié |
| Oui | Non | Publié | Les membres de visionneuse existants conservent leur état publié. Tous les nouveaux membres de la visionneuse ajoutés lors de la modification conservent leur état publié ou non publié. |
| Non | Oui | Publié | Publié |
| Non | Non | Non publié | Les membres de la visionneuse existants, ainsi que tout nouveau membre de la visionneuse que vous ajoutez lors de votre modification conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour modifier une visionneuse de supports variés**

1. Cliquez sur le bouton de **modification** en survol de la visionneuse de supports variés. 
1. Utilisez l’une des méthodes suivantes :

   * Pour supprimer des objets, sélectionnez-les, puis cliquez sur **Supprimer**.
   * Pour réorganiser des objets, faites-les glisser vers leur nouvel emplacement.

1. Lorsque vous avez terminé de modifier la visionneuse, près de l’angle inférieur droit de la page, vérifiez que l’option **Publish after save** (« Publier après l’enregistrement ») est sélectionnée (valeur par défaut).
1. Cliquez sur **Enregistrer** ou sur **Enregistrer sous**.

## Suppression d’une visionneuse de supports variés {#deleting-a-mixed-media-set}

Lorsque vous supprimez une visionneuse, celle-ci est placée dans la corbeille. Toutefois, les membres (ou « enfants ») de cette visionneuse ne sont pas affectés : ils conservent en fait leur état existant publié ou non publié.

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (Annulation manuelle de la publication des fichiers »).

**Pour supprimer une visionneuse de supports variés**

1. En mode Affichage de la grille, Affichage par liste ou Affichage des détails, sélectionnez une ou plusieurs visionneuses de supports variés.
1. Sur la barre de navigation globale, cliquez sur **Fichier** &gt; **Supprimer** &gt; **Supprimer**.

