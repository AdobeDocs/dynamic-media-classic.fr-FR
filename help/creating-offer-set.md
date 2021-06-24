---
title: Création d’une visionneuse d’offres
description: Découvrez comment créer un ensemble d’offres.
uuid: 6d6a4af9-70c0-4cfa-9a8f-855d6adfcc8f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 59b6437d-c21e-4929-9291-3032dbb34565
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
exl-id: 05f2cce0-72bf-4933-87ab-c9003c848e35
source-git-commit: 7456226cf6469f40e66ff327475d4c605b6d6e13
workflow-type: tm+mt
source-wordcount: '1223'
ht-degree: 52%

---

# Création d’une visionneuse d’offres{#creating-an-offer-set}

Vous pouvez créer un des types suivants de visionneuses d’offres :

* Vidéo
* Modèle paramétré
* Image

Pour les modèles, cliquez sur **[!UICONTROL Ajouter et prévisualiser]**, puis définissez les paramètres de votre choix. Les autres types de visionneuses d’offres n’incluent pas les paramètres, mais vous pouvez toujours les personnaliser en cliquant sur **[!UICONTROL Prévisualiser]** et en modifiant les paramètres prédéfinis disponibles.

Dynamic Media Classic propose des outils de modification et de création de visionneuses d’offres.

>[!NOTE]
>
>Avant de créer une visionneuse d’offres, veillez à publier toutes les ressources que vous prévoyez d’utiliser pour la visionneuse sur Dynamic Media Classic. Voir [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

## Types de visionneuses d’offres {#types-of-offer-sets}

Créez une visionneuse d’offres à partir des types suivants :

* **Images**  : vous pouvez assembler des images pour une visionneuse d’offres. Chaque image comprend une offre différente dans la visionneuse.

* **Modèle d’image**  : vous pouvez paramétrer des modèles d’image dans Dynamic Media Classic à l’aide de la commande Créer > Concepts de base des modèles . A travers les paramètres, les composants du modèle (le texte des cadres textuels, les différentes images) peuvent être modifiés et personnalisés. Pour une visionneuse d’offres, vous pouvez utiliser les paramètres de modèles afin de créer des variantes de la même image dans votre visionneuse d’offres, par exemple. Pour plus d’informations sur la création et le paramétrage des modèles d’images, voir Création de paramètres de modèle.

* **Vidéo**  : vous pouvez assembler une vidéo pour une visionneuse d’offres. Chaque vidéo est une offre différente dans la visionneuse.

## Créer un ensemble d&#39;offres avec un modèle paramétré {#creating-an-offer-set-with-a-parameterized-template}

Lorsque vous créez une visionneuse d’offres, l’option **[!UICONTROL Publish after save]** (« Publier après l’enregistrement ») affecte la visionneuse et ses membres comme suit :

| L’option « Publish after save » (« Publier après l’enregistrement ») est-elle sélectionnée avant l’enregistrement ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
|--- |--- |--- |
| Oui | Publié | Publié |
| Non | Non publié | Les membres de la visionneuse conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour créer un ensemble d&#39;offres avec un modèle paramétré :**

1. Sélectionnez le modèle ou la bannière.
1. Cliquez sur **[!UICONTROL Créer]** > **[!UICONTROL Visionneuse d’offres Test&amp;Target]**.

   La page Jeu d’offres Test&amp;Target répertorie les offres du jeu d’offres. Le premier élément de la liste est l’objet.

1. Sélectionnez l’objet, puis cliquez sur **[!UICONTROL Ajouter et prévisualiser]**.

   Dans la partie gauche de cette page, les paramètres du modèle ainsi que leurs valeurs sont répertoriés.

1. Modifiez les valeurs de paramètres pour créer l’offre. Par exemple, entrez du texte différent dans un champ de texte, modifiez la taille d’un calque, remplacez une image par une autre ou choisissez un autre paramètre prédéfini de visionneuse.
1. Cliquez sur **[!UICONTROL **Enregistrer]** ou **[!UICONTROL Enregistrer sous**]** pour enregistrer l’offre dans le cadre du jeu d’offres.

   La page Jeu d’offres Test&amp;Target répertorie les offres que vous avez créées.

1. Répétez les étapes 3 à 5 pour créer d’autres offres pour la visionneuse.
1. Une fois que vous avez terminé, près du coin inférieur droit de la page, assurez-vous que l’option **[!UICONTROL Publier après l’enregistrement*]** est sélectionnée (par défaut).
1. Cliquez sur **[!UICONTROL Fermer]**, saisissez un nom pour le jeu d’offres, puis cliquez sur **[!UICONTROL Enregistrer]**.

Avant de fermer la page du jeu d’offres Test&amp;Target, vous devez envoyer le jeu d’offres vers Adobe Target Standard/Premium. Voir [Promotion de visionneuses d’offres sur Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target). 

## Création d’une visionneuse d’offres à l’aide d’images ou de vidéos {#creating-an-offer-set-with-images-or-videos}

Lorsque vous créez une visionneuse d’offres, l’option **[!UICONTROL Publish after save]** (« Publier après l’enregistrement ») affecte la visionneuse et ses membres comme suit :

| **[!UICONTROL Option Publier après l’]** enregistrement sélectionnée avant l’enregistrement ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
|--- |--- |--- |
| Oui | Publié | Publié |
| Non | Non publié | Les membres de la visionneuse conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour créer une visionneuse d’offres avec des images ou des vidéos:**

1. Assemblez des images ou des vidéos pour la visionneuse d’offres. Commencez dans l’écran Visionneuse d’offres Test&amp;Target ou en mode Grille ou Liste, puis utilisez l’une des méthodes suivantes :

   * **Écran Jeu d’offres Test&amp;Target**  - Cliquez sur  **[!UICONTROL Créer]**  >  **[!UICONTROL Jeu d’offres Test&amp;Target]**. Faites glisser les images ou les vidéos sur l’écran. Pour créer des vidéos ou des images de tailles diverses, faites glisser plusieurs copies de l’image ou de la vidéo et définissez chaque taille séparément.

   * **Mode Affichage de la grille ou Mode Liste**  : sélectionnez les images ou les vidéos, puis cliquez sur  **[!UICONTROL Créer]**  >  **[!UICONTROL Visionneuse d’offres Test&amp;Target]**.

1. (Facultatif) Sélectionnez une image ou une vidéo et cliquez sur **[!UICONTROL Aperçu]**. Sur la page Aperçu des offres , vous pouvez modifier la taille et l’aspect de l’image ou de la vidéo que vous avez sélectionnée. Vous pouvez également modifier toutes les images ou vidéos de la visionneuse d’offres.

   * Sélectionnez un paramètre prédéfini pour modifier l’aspect et la taille de l’image ou de la vidéo.
   * Pour appliquer le paramètre prédéfini que vous avez choisi à toutes les offres du jeu d’offres, cochez la case **[!UICONTROL Sélectionner les paramètres prédéfinis à tous]** .

   Cliquez sur **[!UICONTROL Enregistrer]** pour enregistrer les modifications dans l’offre d’images ou de vidéos. Cliquez ensuite sur **[!UICONTROL Fermer]** pour retourner à la page Visionneuse d’offres Test&amp;Target.

1. Une fois que vous avez créé des offres pour la visionneuse d’offres et choisi Paramètres d’image prédéfinis pour différentes images, assurez-vous que l’option **[!UICONTROL Publier après l’enregistrement]** est sélectionnée (par défaut).
1. Cliquez sur **[!UICONTROL Fermer]** et entrez un nom pour la visionneuse d’offres, puis cliquez sur **[!UICONTROL Enregistrer]**.

Avant de fermer la page du jeu d’offres Test&amp;Target, vous devez envoyer le jeu d’offres vers Adobe Target Standard/Premium. Voir [Promotion de visionneuses d’offres sur Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target). 

## Modification d’une visionneuse d’offres {#editing-an-offer-set}

Que vous modifiiez un jeu publié ou non publié, l’option **[!UICONTROL Publier après l’enregistrement]** affecte le jeu et les membres de la façon suivante :

| Visionneuse déjà publiée ? | **[!UICONTROL l’option Publier après l’]** enregistrement est sélectionnée avant d’enregistrer votre modification ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
|--- |--- |--- |--- |
| Oui | Oui | Publié | Publié |
| Oui | Non | Publié | Les membres de visionneuse existants conservent leur état publié. Tout nouveau membre de visionneuse que vous ajoutez lors de votre modification conserve son état publié ou non publié. |
| Non | Oui | Publié | Publié |
| Non | Non | Non publié | Les membres de la visionneuse existants, ainsi que tout nouveau membre de la visionneuse que vous ajoutez lors de votre modification conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour modifier une visionneuse d’offres:**

1. Pour modifier un ensemble d’offres, affichez-le en mode Grille ou Liste, puis cliquez sur son bouton de survol **[!UICONTROL Modifier]** .
1. Sur la page du jeu d’offres Test&amp;Target, effectuez l’une des opérations suivantes :

   * **Suppression d’une offre**  : sélectionnez l’offre, puis cliquez sur  **** Supprimer pour supprimer une offre de la visionneuse.
   * **Ajout d’une offre**  : la manière dont vous ajoutez une offre dépend du type de jeu d’offres utilisé :
      * **Modèles**  : cliquez sur  **[!UICONTROL Ajouter et prévisualiser]**, puis sur la page Ajouter et prévisualiser des offres, créez une autre offre.
      * **Images et vidéos**  : faites glisser une image ou une vidéo sur la page du jeu d’offres Test&amp;Target.

   >[!NOTE]
   >
   >il n’est pas possible de supprimer une visionneuse d’offres associée à une campagne. Pour supprimer un ensemble d’offres associé à une campagne, connectez-vous à Adobe Target Standard/Premium et supprimez d’abord les associations de campagne. Même après dissociation d’une campagne, la ressource ne peut être supprimée que de Dynamic Media Classic, ce qui nécessite une connexion à Adobe Target Standard/Premium, et non d’Adobe Target Standard/Premium.

1. Une fois les modifications terminées, près du coin inférieur droit de la page, assurez-vous que l’option **[!UICONTROL Publier après l’enregistrement]** est sélectionnée (par défaut).
1. Cliquez sur **[!UICONTROL Enregistrer]**, sélectionnez un dossier de stockage, attribuez un nom à la visionneuse, puis cliquez sur **[!UICONTROL Enregistrer]**.

## Suppression d’une visionneuse d’offres {#deleting-an-offer-set}

Lorsque vous supprimez une visionneuse d’offres, celle-ci est placée dans la corbeille. Toutefois, les membres (ou « enfants ») de cette visionneuse ne sont pas affectés : ils conservent en fait leur état existant publié ou non publié.

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour supprimer une visionneuse d’offres:**

1. En mode Affichage de la grille, Affichage par liste ou Affichage des détails, sélectionnez une ou plusieurs visionneuses d’offres.
1. Sur la barre de navigation globale, cliquez sur **[!UICONTROL Fichier]** > **[!UICONTROL Supprimer]** > **Supprimer**.

>[!MORELIKETHIS]
>
>* [Création de paramètres de modèle](creating-template-parameters.md#creating_template_parameters)

