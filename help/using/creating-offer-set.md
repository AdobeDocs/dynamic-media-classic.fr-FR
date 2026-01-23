---
title: Création d’un ensemble d’offres
description: Découvrez comment créer un jeu d’offres dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 05f2cce0-72bf-4933-87ab-c9003c848e35
topic: Integrations, Development
level: Experienced
source-git-commit: c4613c78347c4bda3d84747a72146617158c03b6
workflow-type: tm+mt
source-wordcount: '1232'
ht-degree: 21%

---

# Création d’un ensemble d’offres {#creating-an-offer-set}

Vous pouvez créer l’un des types d’ensembles d’offres suivants :

* Vidéo
* Modèle paramétré
* Image

Pour les modèles, sélectionnez **[!UICONTROL Ajouter et prévisualiser]**, puis définissez les paramètres de votre choix. Les autres types de jeux d’offres n’incluent pas de paramètres, mais vous pouvez toujours les personnaliser en sélectionnant **[!UICONTROL Prévisualisation]** et en modifiant les paramètres prédéfinis disponibles.

Adobe Dynamic Media Classic propose des outils permettant de modifier et de créer des ensembles d’offres.

>[!NOTE]
>
>Avant de créer un ensemble d’offres, veillez à publier dans Adobe Dynamic Media Classic toutes les ressources que vous avez l’intention d’utiliser pour l’ensemble. Voir [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

## Types d’ensembles d’offres {#types-of-offer-sets}

Créez un jeu d’offres à partir des types de jeux d’offres suivants :

* **Images** : vous pouvez assembler des images pour un ensemble d’offres. Chaque image inclut une offre différente dans la visionneuse.

* **Modèle d’image** : vous pouvez paramétrer les modèles d’image dans Adobe Dynamic Media Classic à l’aide de la commande **[!UICONTROL Créer]** > Principes de base des modèles. Grâce aux paramètres, les composants du modèle, le texte dans les cadres de texte, les différentes images, peuvent être changés et personnalisés. Pour un ensemble d’offres, vous pouvez utiliser des paramètres de modèle pour créer des variations sur la même image de votre ensemble d’offres, par exemple. Pour plus d’informations sur la création et le paramétrage des modèles d’image, voir [Créer des paramètres de modèle](creating-template-parameters.md#creating_template_parameters).

Consultez également la vidéo de formation [Principes de base des modèles](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS).

* **Vidéo** : vous pouvez assembler une vidéo pour un ensemble d’offres. Chaque vidéo est une offre différente dans la visionneuse.

## Création d’un jeu d’offres avec un modèle paramétré {#creating-an-offer-set-with-a-parameterized-template}

Lorsque vous créez un jeu d&#39;offres, l&#39;option **[!UICONTROL Publier après un enregistrement]** affecte le jeu et les membres du jeu de la manière suivante :

| L’option **[!UICONTROL Publier après un enregistrement]** est-elle sélectionnée avant l’enregistrement ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
| --- | --- | --- |
| Oui | Publié | Publié |
| Non | Non publié | Les membres de la visionneuse conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour créer un jeu d&#39;offres avec un modèle paramétré, procédez comme suit**

1. Sélectionnez le modèle ou la bannière.
1. Accédez à **[!UICONTROL Créer]** > **[!UICONTROL Jeu d’offres Test&amp;Target]**.

   La page Jeu d’offres Test&amp;Target répertorie les offres du jeu d’offres. Le premier élément de la liste est l’objet.

1. Sélectionnez l’objet et sélectionnez **[!UICONTROL Ajouter et prévisualiser]**.

   Dans la partie gauche de cette page, les paramètres du modèle ainsi que leurs valeurs sont répertoriés.

1. Modifiez les valeurs de paramètres pour créer l’offre. Par exemple, saisissez un texte différent dans un champ de texte, modifiez la taille d’un calque, remplacez une image par une autre ou choisissez un autre paramètre prédéfini de visionneuse.
1. Sélectionnez **[!UICONTROL Enregistrer]** ou **[!UICONTROL Enregistrer sous**]** pour enregistrer l’offre dans le jeu d’offres.

   La page Jeu d’offres Test&amp;Target répertorie les offres que vous avez créées.

1. Répétez les étapes 3 à 5 pour créer d’autres offres pour la visionneuse.
1. Lorsque vous avez terminé, en bas à droite de la page, assurez-vous que l’option **[!UICONTROL Publier après un enregistrement*]** est sélectionnée (par défaut).
1. Sélectionnez **[!UICONTROL Fermer]**, saisissez un nom pour le jeu d&#39;offres, puis sélectionnez **[!UICONTROL Enregistrer]**.

Avant de fermer la page Jeu d’offres Test&amp;Target, poussez le jeu d’offres vers Adobe Target Standard/Premium. Voir [ Envoi d’ensembles d’offres vers Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Création d’un ensemble d’offres avec des images ou des vidéos {#creating-an-offer-set-with-images-or-videos}

Lorsque vous créez un jeu d&#39;offres, l&#39;option **[!UICONTROL Publier après un enregistrement]** affecte le jeu et les membres du jeu de la manière suivante :

| L’option **[!UICONTROL Publier après un enregistrement]** est-elle sélectionnée avant l’enregistrement ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
| --- | --- | --- |
| Oui | Publié | Publié |
| Non | Non publié | Les membres de la visionneuse conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour créer un ensemble d’offres avec des images ou des vidéos, procédez comme suit**

1. Assemblez des images ou des vidéos pour le jeu d’offres. Commencez dans l’écran Jeu d’offres Test&amp;Target ou dans la vue Grille ou Liste et utilisez l’une des méthodes suivantes :

   * **Écran du jeu d’offres Test&amp;Target** : accédez à **[!UICONTROL Créer]** > **[!UICONTROL Jeu d’offres Test&amp;Target]**. Faites glisser les images ou les vidéos sur l’écran. Pour créer des vidéos ou des images de tailles diverses, faites glisser plusieurs copies de l’image ou de la vidéo et définissez chaque taille séparément.

   * **Vue Grille ou Vue Liste** : sélectionnez les images ou les vidéos, puis accédez à **[!UICONTROL Créer]** > **[!UICONTROL Jeu d’offres Test&amp;Target]**.

1. Vous pouvez également sélectionner une image ou une vidéo, puis sélectionner **[!UICONTROL Aperçu]**. Sur la page Aperçu des offres , vous pouvez modifier la taille et l’aspect de l’image ou de la vidéo que vous avez sélectionnée. Vous pouvez également modifier toutes les images ou vidéos du jeu d’offres.

   * Sélectionnez un paramètre prédéfini pour modifier l’aspect et la taille de l’image ou de la vidéo.
   * Pour appliquer le paramètre prédéfini que vous avez choisi à toutes les offres du jeu d’offres, cochez la case **`Select Presets to All`** .

   Sélectionnez **[!UICONTROL Enregistrer]** pour enregistrer les modifications apportées à l’offre image ou vidéo. Sélectionnez ensuite **[!UICONTROL Fermer]** pour revenir à la page Jeu d’offres Test&amp;Target.

1. Une fois que vous avez terminé de créer des offres pour le jeu d’offres et de choisir des paramètres d’image prédéfinis pour différentes images, assurez-vous que l’option **[!UICONTROL Publier après un enregistrement]** est sélectionnée (par défaut).
1. Sélectionnez **[!UICONTROL Enregistrer]** saisissez un nom pour le jeu d&#39;offres, puis sélectionnez **[!UICONTROL Enregistrer]**.

Avant de fermer la page Jeu d’offres Test&amp;Target, poussez le jeu d’offres vers Adobe Target Standard/Premium. Voir [ Envoi d’ensembles d’offres vers Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Modification d’un ensemble d’offres {#editing-an-offer-set}

Que vous modifiiez une visionneuse publiée ou une visionneuse dépubliée, l’option **[!UICONTROL Publier après un enregistrement]** affecte la visionneuse et les membres de la visionneuse des manières suivantes :

| Visionneuse déjà publiée ? | L’option **[!UICONTROL Publier après un enregistrement]** est-elle sélectionnée avant d’enregistrer votre modification ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
| --- | --- | --- | --- |
| Oui | Oui | Publié | Publié |
| Oui | Non | Publié | Les membres d’ensemble existants conservent leur statut publié. Tout nouveau membre de visionneuse que vous ajoutez lors de votre modification conserve son état publié ou non publié. |
| Non | Oui | Publié | Publié |
| Non | Non | Non publié | Les membres de la visionneuse existants, ainsi que tout nouveau membre de la visionneuse que vous ajoutez lors de votre modification conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour modifier un jeu d&#39;offres, procédez comme suit**

1. Pour modifier un jeu d’offres, affichez-le dans la vue Grille ou Liste, puis cliquez sur son bouton de survol **[!UICONTROL Modifier]**.
1. Dans la page Jeu d’offres Test&amp;Target, effectuez l’une des opérations suivantes :

   * **Suppression d’une offre** : sélectionnez l’offre, puis sélectionnez **[!UICONTROL Supprimer]** pour supprimer une offre de la visionneuse.
   * **Ajout d’une offre** : la manière dont vous ajoutez une offre dépend du type de jeu d’offres utilisé :
      * **Modèles** : sélectionnez **[!UICONTROL Ajouter et prévisualiser]**, puis sur la page Ajouter et prévisualiser des offres , créez une autre offre.
      * **Images et vidéos** : faites glisser une image ou une vidéo sur la page Jeu d’offres Test&amp;Target.

   >[!NOTE]
   >
   >Vous ne pouvez pas supprimer un ensemble d’offres associé à une campagne. Pour supprimer un ensemble d’offres associé à une campagne, connectez-vous à Adobe Target Standard/Premium et supprimez d’abord les associations de campagnes. Même après la désassociation d’une campagne, la ressource ne peut être supprimée d’Adobe Dynamic Media Classic que si vous vous connectez à Adobe Target Standard/Premium, et non dans Adobe Target Standard/Premium.

1. Lorsque vous avez terminé la modification, en bas à droite de la page, assurez-vous que l’option **[!UICONTROL Publier après un enregistrement]** est sélectionnée (par défaut).
1. Sélectionnez **[!UICONTROL Enregistrer]**, sélectionnez un dossier de stockage, saisissez un nom pour la visionneuse, puis sélectionnez **[!UICONTROL Enregistrer]**.

## Suppression d’un ensemble d’offres {#delet-an-offer-set}

Lorsque vous supprimez une visionneuse d’offres, celle-ci est placée dans la corbeille. Toutefois, les membres (ou « enfants ») de cet ensemble ne sont pas affectés. Ils conservent chacun leur état publié ou dépublié existant.

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour supprimer un jeu d’offres, procédez comme suit**

1. Dans la vue Grille, Liste ou Détails, sélectionnez un ou plusieurs jeux d&#39;offres.
1. Sur la barre de navigation globale, accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Supprimer]** > **Supprimer**.

>[!MORELIKETHIS]
>
>* [Création de paramètres de modèle](creating-template-parameters.md#creating_template_parameters)
