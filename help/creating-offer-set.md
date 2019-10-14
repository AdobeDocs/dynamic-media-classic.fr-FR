---
title: Création d’une visionneuse d’offres
seo-title: Création d’une visionneuse d’offres
description: 'null'
seo-description: Découvrez comment créer une visionneuse d’offres.
uuid: 6d6a4af9-70c0-4cfa-9a8f-855d6adfcc8f
contentOwner: admin
content-type: référence
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: 59b6437d-c21e-4929-9291-3032dbb34565
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Création d’une visionneuse d’offres{#creating-an-offer-set}

Vous pouvez créer un des types suivants de visionneuses d’offres :

* Vidéo
* Modèle paramétré
* Image

For templates, click **Add and Preview**, then set the parameters you choose. Les autres types de visionneuses d’offres n’incluent pas les paramètres, mais vous pouvez toujours les personnaliser en cliquant sur **Prévisualiser** et en modifiant les paramètres prédéfinis disponibles.

Dynamic Media Classic propose des outils de modification et de création de visionneuses d’offres.

>[!NOTE]
>
>Avant de créer une visionneuse d’offres, veillez à publier tous les fichiers que vous prévoyez d’utiliser pour la visionneuse sur Scene7 Publishing System. Voir [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

## Types de visionneuses d’offres {#types-of-offer-sets}

Créez une visionneuse d’offres à partir des types suivants :

* **Images** Vous pouvez assembler des images pour une visionneuse d’offres. Chaque image comprend une offre différente dans la visionneuse.

* **Modèle** d’image Vous pouvez paramétrer des modèles d’image dans Dynamic Media Classic à l’aide de la commande Créer &gt; Concepts de base des modèles. A travers les paramètres, les composants du modèle (le texte des cadres textuels, les différentes images) peuvent être modifiés et personnalisés. Pour une visionneuse d’offres, vous pouvez utiliser les paramètres de modèles afin de créer des variantes de la même image dans votre visionneuse d’offres, par exemple. Pour plus d’informations sur la création et le paramétrage des modèles d’images, voir Création de paramètres de modèle.

* **Vidéo** Vous pouvez assembler de la vidéo pour une visionneuse d’offres. Chaque vidéo est une offre différente dans la visionneuse.

## Création d’une visionneuse d’offres à l’aide d’un modèle paramétré {#creating-an-offer-set-with-a-parameterized-template}

Lorsque vous créez une visionneuse d’offres, l’option **Publish after save** (« Publier après l’enregistrement ») affecte la visionneuse et ses membres comme suit :

| L’option « Publish after save » (« Publier après l’enregistrement ») est-elle sélectionnée avant l’enregistrement ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
|--- |--- |--- |
| Oui | Publié | Publié |
| Non | Non publié | Les membres de la visionneuse conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour créer une visionneuse d’offres avec un modèle paramétré**

1. Sélectionnez le modèle ou la bannière.
1. Click **Build** &gt; **Target Classic Offer Set**.

   La page Visionneuse d’offres Target Classic répertorie les offres de la visionneuse d’offres. Le premier élément de la liste est l’objet.

1. Sélectionnez l’objet, puis cliquez sur **Ajouter et prévisualiser**.

   Dans la partie gauche de cette page, les paramètres du modèle ainsi que leurs valeurs sont répertoriés.

1. Modifiez les valeurs de paramètres pour créer l’offre. Par exemple, entrez du texte différent dans un champ de texte, modifiez la taille d’un calque, remplacez une image par une autre ou choisissez un autre paramètre prédéfini de visionneuse.
1. Cliquez sur **Enregistrer** ou **Enregistrer sous** pour enregistrer l’offre dans le cadre de la visionneuse d’offres.

   La page Visionneuse d’offres Target Classic répertorie les offres que vous avez créées.

1. Répétez les étapes 3 à 5 pour créer d’autres offres pour la visionneuse.
1. When you finish, near the lower-right corner of the page, ensure that **Publish after save** is selected (default).
1. Click **Close**, enter a name for the offer set, and then click **Save**.

Avant de fermer la page Visionneuse d’offres Target Classic, poussez la visionneuse d’offres sur Target Classic. See [Pushing offer sets to Target Classic](pushing-offer-sets-target-classic.md#pushing_offer_sets_to_target_classic).

## Creating an offer set with images or videos {#creating-an-offer-set-with-images-or-videos}

Lorsque vous créez une visionneuse d’offres, l’option **Publish after save** (« Publier après l’enregistrement ») affecte la visionneuse et ses membres comme suit :

| L’option « Publish after save » (« Publier après l’enregistrement ») est-elle sélectionnée avant l’enregistrement ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
|--- |--- |--- |
| Oui | Publié | Publié |
| Non | Non publié | Les membres de la visionneuse conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour créer une visionneuse d’offres avec des images ou des vidéos**

1. Assemblez des images ou des vidéos pour la visionneuse d’offres. Commencez dans l’écran Visionneuse d’offres Target Classic ou en mode Affichage de la grille ou Affichage par liste et utilisez l’une des méthodes suivantes :

   * **Ecran** Créer &gt; Visionneuse d’offres Target Classic. Faites glisser les images ou les vidéos sur l’écran. Pour créer des vidéos ou des images de tailles diverses, faites glisser plusieurs copies de l’image ou de la vidéo et définissez chaque taille séparément.

   * **Affichage par grille ou Affichage par liste** Sélectionnez les images ou les vidéos, puis cliquez sur Créer &gt; Visionneuse d’offres Target Classic.

1. (Facultatif) Sélectionnez une image ou une vidéo et cliquez sur **Aperçu**. Sur la page Prévisualiser les offres, vous pouvez modifier la taille et l’aspect de l’image ou de la vidéo sélectionnée. Vous pouvez également modifier toutes les images ou vidéos de la visionneuse d’offres.

   * Sélectionnez un paramètre prédéfini pour modifier l’aspect et la taille de l’image ou de la vidéo.
   * Cochez la case de sélection des paramètres prédéfinis applicables à toutes les offres afin d’appliquer le paramètre prédéfini à toutes les offres de la visionneuse.
   Cliquez sur **Enregistrer** pour enregistrer les modifications dans l’offre d’images ou de vidéos. Then click **Close** to return to the Target Classic Offer Set page.

1. After you finish creating offers for the offer set and choosing Image Presets for different images, ensure that **Publish after save** is selected (default).
1. Cliquez sur **Fermer** et entrez un nom pour la visionneuse d’offres, puis cliquez sur **Enregistrer**.

Avant de fermer la page Visionneuse d’offres Target Classic, poussez la visionneuse d’offres sur Target Classic. See [Pushing offer sets to Target Classic](pushing-offer-sets-target-classic.md#pushing_offer_sets_to_target_classic).

## Modification d’une visionneuse d’offres {#editing-an-offer-set}

Selon que vous modifiez une visionneuse publiée ou non publiée, l’option **Publish after save** (« Publier après l’enregistrement ») affecte la visionneuse et ses membres comme suit :

| Visionneuse déjà publiée ? | L’option « Publish after save » (« Publier après l’enregistrement ») est-elle sélectionnée avant l’enregistrement de votre modification ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
|--- |--- |--- |--- |
| Oui | Oui | Publié | Publié |
| Oui | Non | Publié | Les membres de visionneuse existants conservent leur état publié. Les nouveaux membres de visionneuse que vous avez ajoutés pendant votre modification conservent leur état publié ou non publié. |
| Non | Oui | Publié | Publié |
| Non | Non | Non publié | Les membres de la visionneuse existants, ainsi que tout nouveau membre de la visionneuse que vous ajoutez lors de votre modification conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour modifier une visionneuse d’offres**

1. To edit an offer set, display the offer set in Grid view or List view, and then click its **Edit** rollover button.
1. Dans la page Visionneuse d’offres Target Classic, effectuez l’une des opérations suivantes :

   * **Suppression d’une offre** Sélectionnez l’offre, puis cliquez sur **Supprimer** pour supprimer une offre de la visionneuse.
   * **Ajout d’une offre** La manière dont vous ajoutez une offre dépend du type de visionneuse d’offres sur laquelle vous travaillez :
   * **Modèles** Cliquez sur **Ajouter et prévisualiser**, puis sur la page Ajouter et prévisualiser des offres, créez une autre offre.
   * **Images et vidéos** Faites glisser une image ou une vidéo sur la page Visionneuse d’offres Target Classic.
   >[!NOTE]
   >
   >il n’est pas possible de supprimer une visionneuse d’offres associée à une campagne. Pour supprimer une visionneuse d’offres associée à une campagne, connectez-vous à Target Classic et supprimez d’abord les associations de campagne. Même après la dissociation d’une campagne, le fichier peut uniquement être supprimé de Scene7 Publishing System, ce qui nécessite une connexion à Target Classic et non à Target Classic.

1. When you finish editing, near the lower-right corner of the page, ensure that **Publish after save** is selected (default).
1. Cliquez sur **Enregistrer**, sélectionnez un dossier de stockage, attribuez un nom à la visionneuse, puis cliquez sur **Enregistrer**.

## Suppression d’une visionneuse d’offres {#deleting-an-offer-set}

Lorsque vous supprimez une visionneuse d’offres, celle-ci est placée dans la corbeille. Toutefois, les membres (ou « enfants ») de cette visionneuse ne sont pas affectés : ils conservent en fait leur état existant publié ou non publié.

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour supprimer une visionneuse d’offres**

1. En mode Affichage de la grille, Affichage par liste ou Affichage des détails, sélectionnez une ou plusieurs visionneuses d’offres.
1. Sur la barre de navigation globale, cliquez sur **Fichier** &gt; **Supprimer** &gt; **Supprimer**.

>[!MORELIKETHIS]
>
>* [Création de paramètres de modèle](creating-template-parameters.md#creating_template_parameters)

