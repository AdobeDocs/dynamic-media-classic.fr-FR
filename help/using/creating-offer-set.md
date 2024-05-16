---
title: Création d’une visionneuse d’offres
description: Découvrez comment créer une visionneuse d’offres dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 05f2cce0-72bf-4933-87ab-c9003c848e35
topic: Integrations, Development
level: Experienced
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '1236'
ht-degree: 21%

---

# Création d’une visionneuse d’offres {#creating-an-offer-set}

Vous pouvez créer l’un des types suivants de visionneuses d’offres :

* Vidéo
* Modèle paramétré
* Image

Pour les modèles, sélectionnez **[!UICONTROL Ajouter et prévisualiser]**, puis définissez les paramètres de votre choix. D’autres types de visionneuses d’offres n’incluent pas de paramètres, mais vous pouvez toujours les personnaliser en sélectionnant **[!UICONTROL Aperçu]** et de modifier les paramètres prédéfinis disponibles.

Adobe Dynamic Media Classic propose des outils de modification et de création de visionneuses d’offres.

>[!NOTE]
>
>Avant de créer une visionneuse d’offres, veillez à publier toutes les ressources que vous prévoyez d’utiliser pour la visionneuse dans Adobe Dynamic Media Classic. Voir [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

## Types de visionneuses d’offres {#types-of-offer-sets}

Créez une visionneuse d’offres à partir des types suivants de visionneuses d’offres :

* **Images**: vous pouvez assembler des images pour une visionneuse d’offres. Chaque image comprend une offre différente dans la visionneuse.

* **Modèle d’image**: vous pouvez paramétrer des modèles d’image dans Adobe Dynamic Media Classic avec le **[!UICONTROL Build]** > Concepts de base des modèles, commande. Grâce aux paramètres, aux composants du modèle, au texte des cadres de texte et aux différentes images, il est possible de permuter et de personnaliser le texte. Pour une visionneuse d’offres, vous pouvez utiliser des paramètres de modèle pour créer des variations sur la même image de la visionneuse d’offres, par exemple. Pour plus d’informations sur la création et le paramétrage des modèles d’image, voir [Créer des paramètres de modèle](creating-template-parameters.md#creating_template_parameters).

Voir aussi [Concepts de base des modèles](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) vidéo de formation.

* **Vidéo**: vous pouvez assembler une vidéo pour une visionneuse d’offres. Chaque vidéo est une offre différente dans la visionneuse.

## Création d’une visionneuse d’offres avec un modèle paramétré {#creating-an-offer-set-with-a-parameterized-template}

Lorsque vous créez une visionneuse d’offres, la variable **[!UICONTROL Publier après un enregistrement]** L’option affecte les membres de l’ensemble et de l’ensemble comme suit :

| **[!UICONTROL Publier après un enregistrement]** l’option sélectionnée avant l’enregistrement ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
| --- | --- | --- |
| Oui | Publié | Publié |
| Non | Non publié | Les membres de la visionneuse conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour créer une visionneuse d’offres avec un modèle paramétré :**

1. Sélectionnez le modèle ou la bannière.
1. Accédez à **[!UICONTROL Build]** > **[!UICONTROL Jeu d’offres Test&amp;Target]**.

   La page Jeu d’offres Test&amp;Target répertorie les offres du jeu d’offres. Le premier élément de la liste est l’objet.

1. Sélectionnez l’objet et sélectionnez **[!UICONTROL Ajouter et prévisualiser]**.

   Dans la partie gauche de cette page, les paramètres du modèle ainsi que leurs valeurs sont répertoriés.

1. Modifiez les valeurs de paramètres pour créer l’offre. Par exemple, saisissez un texte différent dans un champ de texte, modifiez la taille d’un calque, changez d’image ou choisissez un autre paramètre prédéfini de visionneuse.
1. Sélectionner **[!UICONTROL Enregistrer]** ou **[!UICONTROL Enregistrer sous**]** pour enregistrer l’offre dans le cadre de la visionneuse d’offres.

   La page Jeu d’offres Test&amp;Target répertorie les offres que vous avez créées.

1. Répétez les étapes 3 à 5 pour créer d’autres offres pour la visionneuse.
1. Lorsque vous avez terminé, près du coin inférieur droit de la page, assurez-vous que **[!UICONTROL Publier après un enregistrement*]** est sélectionné (par défaut).
1. Sélectionner **[!UICONTROL Fermer]**, saisissez un nom pour la visionneuse d’offres, puis sélectionnez **[!UICONTROL Enregistrer]**.

Avant de fermer la page du jeu d’offres Test&amp;Target, placez le jeu d’offres sur Adobe Target Standard/Premium. Voir [Jeux d’offres push sur Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Création d’une visionneuse d’offres avec des images ou des vidéos {#creating-an-offer-set-with-images-or-videos}

Lorsque vous créez une visionneuse d’offres, la variable **[!UICONTROL Publier après un enregistrement]** L’option affecte les membres de l’ensemble et de l’ensemble comme suit :

| **[!UICONTROL Publier après un enregistrement]** l’option sélectionnée avant l’enregistrement ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
| --- | --- | --- |
| Oui | Publié | Publié |
| Non | Non publié | Les membres de la visionneuse conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour créer une visionneuse d’offres avec des images ou des vidéos :**

1. Assemblez des images ou des vidéos pour la visionneuse d’offres. Commencez dans l’écran Visionneuse d’offres Test&amp;Target ou en mode Grille ou Liste, puis utilisez l’une des méthodes suivantes :

   * **Écran Jeu d’offres Test&amp;Target**: accédez à **[!UICONTROL Build]** > **[!UICONTROL Jeu d’offres Test&amp;Target]**. Faites glisser les images ou les vidéos sur l’écran. Pour créer des vidéos ou des images de tailles diverses, faites glisser plusieurs copies de l’image ou de la vidéo et définissez chaque taille séparément.

   * **Mode Grille ou Mode Liste**: sélectionnez les images ou les vidéos, puis accédez à **[!UICONTROL Build]** > **[!UICONTROL Jeu d’offres Test&amp;Target]**.

1. Vous pouvez également sélectionner une image ou une vidéo et sélectionner **[!UICONTROL Aperçu]**. Sur la page Aperçu des offres , vous pouvez modifier la taille et l’aspect de l’image ou de la vidéo que vous avez sélectionnée. Vous pouvez également modifier toutes les images ou vidéos de la visionneuse d’offres.

   * Sélectionnez un paramètre prédéfini pour modifier l’aspect et la taille de l’image ou de la vidéo.
   * Pour appliquer le paramètre prédéfini que vous avez choisi à toutes les offres de la visionneuse, sélectionnez le **[!UICONTROL Sélectionner Paramètres prédéfinis pour tous]** .

   Sélectionner **[!UICONTROL Enregistrer]** pour enregistrer vos modifications dans l’offre d’image ou de vidéo. Sélectionnez **[!UICONTROL Fermer]** pour revenir à la page du jeu d’offres Test&amp;Target.

1. Une fois que vous avez créé des offres pour la visionneuse d’offres et choisi des paramètres d’image prédéfinis pour différentes images, assurez-vous que **[!UICONTROL Publier après un enregistrement]** est sélectionné (par défaut).
1. Sélectionner **[!UICONTROL Enregistrer]** et saisissez un nom pour la visionneuse d’offres, puis sélectionnez **[!UICONTROL Enregistrer]**.

Avant de fermer la page du jeu d’offres Test&amp;Target, placez le jeu d’offres sur Adobe Target Standard/Premium. Voir [Jeux d’offres push sur Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Modification d’une visionneuse d’offres {#editing-an-offer-set}

Si vous modifiez un jeu publié ou non publié, la variable **[!UICONTROL Publier après un enregistrement]** L’option affecte les membres de l’ensemble et de l’ensemble comme suit :

| Visionneuse déjà publiée ? | **[!UICONTROL Publier après un enregistrement]** sélectionnée avant d’enregistrer votre modification ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
| --- | --- | --- | --- |
| Oui | Oui | Publié | Publié |
| Oui | Non | Publié | Les membres de visionneuse existants conservent leur état publié. Tout nouveau membre de visionneuse que vous ajoutez lors de votre modification conserve son état publié ou non publié. |
| Non | Oui | Publié | Publié |
| Non | Non | Non publié | Les membres de la visionneuse existants, ainsi que tout nouveau membre de la visionneuse que vous ajoutez lors de votre modification conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour modifier une visionneuse d’offres :**

1. Pour modifier une visionneuse d’offres, affichez-la en mode Grille ou Liste, puis sélectionnez-la. **[!UICONTROL Modifier]** bouton de survol.
1. Sur la page du jeu d’offres Test&amp;Target, effectuez l’une des opérations suivantes :

   * **Supprimer une offre**: sélectionnez l’offre, puis **[!UICONTROL Supprimer]** pour supprimer une offre du jeu.
   * **Ajouter une offre**: la manière dont vous ajoutez une offre dépend du type de visionneuse d’offres que vous utilisez :
      * **Modèles**: sélectionnez **[!UICONTROL Ajouter et prévisualiser]**, puis sur la page Ajouter et prévisualiser des offres , créez une autre offre.
      * **Images et vidéos**: faites glisser une image ou une vidéo sur la page de la visionneuse d’offres Test&amp;Target.

   >[!NOTE]
   >
   >Vous ne pouvez pas supprimer une visionneuse d’offres associée à une campagne. Pour supprimer une visionneuse d’offres associée à une campagne, connectez-vous à Adobe Target Standard/Premium et supprimez d’abord les associations de campagne. Même après dissociation d’une campagne, la ressource ne peut être supprimée que d’Adobe Dynamic Media Classic, ce qui nécessite une connexion à Adobe Target Standard/Premium, et non d’Adobe Target Standard/Premium.

1. Lorsque vous avez terminé les modifications, près du coin inférieur droit de la page, assurez-vous que **[!UICONTROL Publier après un enregistrement]** est sélectionné (par défaut).
1. Sélectionner **[!UICONTROL Enregistrer]**, sélectionnez un dossier de stockage, saisissez un nom pour la visionneuse, puis sélectionnez **[!UICONTROL Enregistrer]**.

## Suppression d’une visionneuse d’offres {#delet-an-offer-set}

Lorsque vous supprimez une visionneuse d’offres, celle-ci est placée dans la corbeille. Cependant, les membres (ou &quot;enfants&quot;) de cet ensemble ne sont pas affectés ; au lieu de cela, ils conservent chacun leur état publié ou non publié existant.

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour supprimer une visionneuse d’offres :**

1. En mode Grille, Liste ou Détails, sélectionnez une visionneuse d’offres ou plus.
1. Dans la barre de navigation globale, accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Supprimer]** > **Supprimer**.

>[!MORELIKETHIS]
>
>* [Création de paramètres de modèle](creating-template-parameters.md#creating_template_parameters)
