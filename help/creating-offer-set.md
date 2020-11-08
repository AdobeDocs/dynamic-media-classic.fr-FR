---
title: Création d’une visionneuse d’offres
seo-title: Création d’une visionneuse d’offres
description: 'null'
seo-description: Découvrez comment créer un jeu d’offres.
uuid: 6d6a4af9-70c0-4cfa-9a8f-855d6adfcc8f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 59b6437d-c21e-4929-9291-3032dbb34565
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '1220'
ht-degree: 57%

---


# Création d’une visionneuse d’offres{#creating-an-offer-set}

Vous pouvez créer un des types suivants de visionneuses d’offres :

* Vidéo
* Modèle paramétré
* Image

For templates, click **Add and Preview**, then set the parameters you choose. Les autres types de visionneuses d’offres n’incluent pas les paramètres, mais vous pouvez toujours les personnaliser en cliquant sur **Prévisualiser** et en modifiant les paramètres prédéfinis disponibles.

Outils d’offres Dynamic Media Classic pour la modification et la création de jeux d’offres.

>[!NOTE]
>
>Avant de créer une visionneuse d’offres, veillez à publier tous les fichiers que vous prévoyez d’utiliser pour la visionneuse sur Contenu multimédia dynamique classique. Voir [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

## Types de visionneuses d’offres {#types-of-offer-sets}

Créez une visionneuse d’offres à partir des types suivants :

* **Images** Vous pouvez assembler des images pour une visionneuse d’offres. Chaque image comporte une offre différente dans la visionneuse.

* **Modèle** d’image Vous pouvez paramétrer des modèles d’image dans Dynamic Media Classic à l’aide de la commande Créer > Concepts de base des modèles. A travers les paramètres, les composants du modèle (le texte des cadres textuels, les différentes images) peuvent être modifiés et personnalisés. Pour une visionneuse d’offres, vous pouvez utiliser les paramètres de modèles afin de créer des variantes de la même image dans votre visionneuse d’offres, par exemple. Pour plus d’informations sur la création et le paramétrage des modèles d’images, voir Création de paramètres de modèle.

* **Vidéo** Vous pouvez assembler de la vidéo pour une visionneuse d’offres. Chaque vidéo est une offre différente dans la visionneuse.

## Création d’un jeu d’offres à l’aide d’un modèle paramétré {#creating-an-offer-set-with-a-parameterized-template}

Lorsque vous créez une visionneuse d’offres, l’option **Publish after save** (« Publier après l’enregistrement ») affecte la visionneuse et ses membres comme suit :

| L’option « Publish after save » (« Publier après l’enregistrement ») est-elle sélectionnée avant l’enregistrement ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
|--- |--- |--- |
| Oui | Publié | Publié |
| Non | Non publié | Les membres de la visionneuse conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour créer un jeu d’offres avec un modèle paramétré**

1. Sélectionnez le modèle ou la bannière.
1. Cliquez sur **Créer** > **Visionneuse d’offres Test&amp;Target**.

   La page Jeu d’Offres Test&amp;Cible liste les offres du jeu d’offres. Le premier élément de la liste est l’objet.

1. Sélectionnez l’objet, puis cliquez sur **Ajouter et prévisualiser**.

   Dans la partie gauche de cette page, les paramètres du modèle ainsi que leurs valeurs sont répertoriés.

1. Modifiez les valeurs de paramètres pour créer l’offre. Par exemple, entrez du texte différent dans un champ de texte, modifiez la taille d’un calque, remplacez une image par une autre ou choisissez un autre paramètre prédéfini de visionneuse.
1. Cliquez sur **Enregistrer** ou **Enregistrer sous** pour enregistrer l’offre dans le cadre de la visionneuse d’offres.

   La page Jeu d&#39;Offres Test&amp;Cible liste les offres que vous avez créées.

1. Répétez les étapes 3 à 5 pour créer d’autres offres pour la visionneuse.
1. When you finish, near the lower-right corner of the page, ensure that **Publish after save** is selected (default).
1. Click **Close**, enter a name for the offer set, and then click **Save**.

Avant de fermer la page Jeu d’Offres Test&amp;Cible, poussez le jeu d’offres sur Target Standard/Premium. Voir [Promotion de visionneuses d’offres sur Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target). 

## Creating an offer set with images or videos {#creating-an-offer-set-with-images-or-videos}

Lorsque vous créez une visionneuse d’offres, l’option **Publish after save** (« Publier après l’enregistrement ») affecte la visionneuse et ses membres comme suit :

| L’option « Publish after save » (« Publier après l’enregistrement ») est-elle sélectionnée avant l’enregistrement ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
|--- |--- |--- |
| Oui | Publié | Publié |
| Non | Non publié | Les membres de la visionneuse conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour créer une visionneuse d’offres avec des images ou des vidéos**

1. Assemblage d’images ou de vidéos pour la visionneuse d’offres. Début dans l’écran Visionneuse d’Offres Test&amp;Cible ou dans la Vue de grille ou la Vue de Liste et utilisez l’une des méthodes suivantes :

   * **Ecran** Visionneuse d’Offres Test&amp;Cible, cliquez sur **[!UICONTROL Créer > Visionneuse]** d’Offres Test&amp;Cible. Faites glisser les images ou les vidéos sur l’écran. Pour créer des vidéos ou des images de tailles diverses, faites glisser plusieurs copies de l’image ou de la vidéo et définissez chaque taille séparément.

   * **Vue** de grille ou de Liste Sélectionnez les images ou les vidéos, puis cliquez sur **[!UICONTROL Créer > Visionneuse]** d’Offres Test&amp;Cible.

1. (Facultatif) Sélectionnez une image ou une vidéo et cliquez sur **Aperçu**. Sur la page Offres de Prévisualisation, vous pouvez modifier la taille et l’aspect de l’image ou de la vidéo que vous avez sélectionnée. Vous pouvez également modifier toutes les images ou vidéos de la visionneuse d’offres.

   * Sélectionnez un paramètre prédéfini pour modifier l’aspect et la taille de l’image ou de la vidéo.
   * Cochez la case de sélection des paramètres prédéfinis applicables à toutes les offres afin d’appliquer le paramètre prédéfini à toutes les offres de la visionneuse.

   Cliquez sur **Enregistrer** pour enregistrer les modifications dans l’offre d’images ou de vidéos. Cliquez ensuite sur **Fermer** pour retourner à la page Visionneuse d’offres Test&amp;Target.

1. After you finish creating offers for the offer set and choosing Image Presets for different images, ensure that **Publish after save** is selected (default).
1. Cliquez sur **Fermer** et entrez un nom pour la visionneuse d’offres, puis cliquez sur **Enregistrer**.

Avant de fermer la page Jeu d’Offres Test&amp;Cible, poussez le jeu d’offres sur Target Standard/Premium. Voir [Promotion de visionneuses d’offres sur Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target). 

## Modification d’une visionneuse d’offres {#editing-an-offer-set}

Selon que vous modifiez une visionneuse publiée ou non publiée, l’option **Publish after save** (« Publier après l’enregistrement ») affecte la visionneuse et ses membres comme suit :

| Visionneuse déjà publiée ? | L’option « Publish after save » (« Publier après l’enregistrement ») est-elle sélectionnée avant l’enregistrement de votre modification ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
|--- |--- |--- |--- |
| Oui | Oui | Publié | Publié |
| Oui | Non | Publié | Les membres de visionneuse existants conservent leur état publié. Tous les nouveaux membres de visionneuse que vous avez ajoutés pendant votre modification conservent leur état publié ou non publié. |
| Non | Oui | Publié | Publié |
| Non | Non | Non publié | Les membres de la visionneuse existants, ainsi que tout nouveau membre de la visionneuse que vous ajoutez lors de votre modification conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour modifier une visionneuse d’offres**

1. To edit an offer set, display the offer set in Grid view or List view, and then click its **Edit** rollover button.
1. Dans la page Jeu d’Offres de Test&amp;Cible, effectuez l’une des opérations suivantes :

   * **Suppression d&#39;une offre** Sélectionnez l&#39;offre, puis cliquez sur 
**Supprimer** pour supprimer une offre de la visionneuse.
   * **Ajouter une offre** La façon dont vous ajoutez une offre dépend du type de jeu d’offres sur lequel vous travaillez :
   * **Modèles** Click 
**Ajoute et Prévisualisation**, et sur la page Ajouter et Offres de Prévisualisation, créez une autre offre.
   * **Images et vidéos** Faites glisser une image ou une vidéo sur la page Visionneuse d’Offres Test&amp;Cible.
   >[!NOTE]
   >
   >il n’est pas possible de supprimer une visionneuse d’offres associée à une campagne. Pour supprimer un jeu d’offres associé à une campagne, connectez-vous à Target Standard/Premium et supprimez d’abord les associations de campagne. Même après avoir été dissocié d’une campagne, le fichier peut uniquement être supprimé de Dyanonic Media Classic, ce qui nécessite une connexion à Target Standard/Premium et non à partir de Target Standard/Premium.

1. When you finish editing, near the lower-right corner of the page, ensure that **Publish after save** is selected (default).
1. Cliquez sur **Enregistrer**, sélectionnez un dossier de stockage, attribuez un nom à la visionneuse, puis cliquez sur **Enregistrer**.

## Suppression d’une visionneuse d’offres {#deleting-an-offer-set}

Lorsque vous supprimez une visionneuse d’offres, celle-ci est placée dans la corbeille. Toutefois, les membres (ou « enfants ») de cette visionneuse ne sont pas affectés : ils conservent en fait leur état existant publié ou non publié.

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour supprimer une visionneuse d’offres**

1. En mode Affichage de la grille, Affichage par liste ou Affichage des détails, sélectionnez une ou plusieurs visionneuses d’offres.
1. Sur la barre de navigation globale, cliquez sur **Fichier** > **Supprimer** > **Supprimer**.

>[!MORELIKETHIS]
>
>* [Création de paramètres de modèle](creating-template-parameters.md#creating_template_parameters)

