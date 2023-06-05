---
title: Création et gestion des groupes Media Portal
description: Découvrez comment créer et gérer des groupes Media Portal dans Adobe Dynamic Media Classic.
uuid: 23f360e1-ddcb-491b-ab9f-428f3ac9c316
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 91524d36-b77a-4dc4-acba-a7bd85297e98
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: 0deb7133-b895-4c3f-8e5e-8604a6f2d16b
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 56%

---

# Création et gestion des groupes Media Portal{#creating-and-managing-media-portal-groups}

Les *groupes* sont conçus pour vous aider à administrer les utilisateurs du portail multimédia. Pour accéder à un fichier, un utilisateur doit appartenir au minimum à un groupe autorisé à accéder à ce fichier. Lorsque vous ajoutez un utilisateur, vous l’affectez à un ou plusieurs groupes. Ce faisant, vous lui accordez un accès aux dossiers attribués au groupe auquel il appartient. Vous pouvez également choisir les paramètres d’image prédéfinis qui sont disponibles pour un groupe.

## Utilisation de groupes pour restreindre l’accès aux dossiers, aux ressources et aux paramètres d’image prédéfinis {#using-groups-to-restrict-access-to-folders-assets-and-image-presets}

Pour accorder des autorisations d’accès à différents niveaux, vous créez des groupes. Pour chaque groupe, vous définissez des autorisations d’accès en lecture, en écriture et en suppression à des dossiers et à leur contenu. Vous déterminez également les paramètres d’image prédéfinis qui sont disponibles pour le groupe. Vous affectez ensuite les utilisateurs à des groupes. Un utilisateur peut appartenir à plusieurs groupes. Le concept de groupe vous offre la possibilité de donner accès à un nombre limité de contenus par rapport au contenu total.

Si vous n’accordez pas spécifiquement l’autorisation à un groupe à une ressource ou à un dossier, cette ressource ou ce dossier hérite des autorisations que vous avez attribuées à son dossier parent (le dossier situé au-dessus dans la hiérarchie de dossiers). Pour vous assurer que tous les dossiers enfants d’un dossier particulier héritent d’autorisations identiques, accordez les autorisations au dossier parent.

>[!NOTE]
>
>les utilisateurs peuvent appartenir à plusieurs groupes. Lorsqu’un utilisateur appartient à deux groupes ayant des autorisations d’accès différentes à un dossier, cet utilisateur est doté du niveau d’accès le plus élevé.

## Ajout d’un groupe {#adding-a-group}

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de Media Portal]** > **[!UICONTROL Groupes]**.
1. Sélectionner **[!UICONTROL Ajouter]**.
1. Dans la boîte de dialogue Ajouter un groupe, saisissez le nom du groupe dans la zone Nom du groupe, puis sélectionnez **[!UICONTROL Ajouter un groupe]**.
1. Le cas échéant, vous pouvez cocher les cases situées en regard des noms des utilisateurs à ajouter au nouveau groupe.
1. Si vous souhaitez définir les autorisations d’accès maintenant, sélectionnez l’option **[!UICONTROL Autorisations d’accès aux ressources]** puis spécifiez les options de votre choix.

   Voir [Définition des autorisations d’accès aux fichiers pour un groupe](creating-media-portal-groups.md#establishing_asset_access_permissions_for_a_group).

1. Si vous souhaitez choisir les paramètres d’image prédéfinis qui sont disponibles pour le groupe, sélectionnez la variable **[!UICONTROL Autorisations d’accès aux paramètres d’image prédéfinis]** et sélectionnez Paramètres d’image prédéfinis que le groupe peut utiliser.

   Voir [Choix des autorisations d’accès de paramètres d’image prédéfinis pour un groupe](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group).

1. Sélectionner **[!UICONTROL Fermer]**.

## Définition des autorisations d’accès aux fichiers pour un groupe {#establishing-asset-access-permissions-for-a-group}

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de Media Portal]** > **[!UICONTROL Groupes]**.
1. Dans la page de liste des Groupes, effectuez l’une de ces actions :

   * Pour ajouter un groupe et définir des autorisations, sélectionnez **[!UICONTROL Ajouter]**. Dans la boîte de dialogue Ajouter un groupe, saisissez le nom du groupe, puis sélectionnez **[!UICONTROL Ajouter un groupe]**, puis ajoutez des utilisateurs au groupe.
   * Pour modifier les autorisations d’un groupe, sélectionnez-le, puis choisissez **[!UICONTROL Modifier]**.

1. Dans la boîte de dialogue Ajouter un groupe ou Modifier le groupe , sélectionnez le **[!UICONTROL Autorisations d’accès aux ressources]** . Dans la partie droite de l’onglet, des cases permettent de définir les autorisations en lecture, en écriture et en suppression sur les dossiers et les fichiers. Vous pouvez développer et réduire les dossiers et sous-dossiers dans le volet gauche.
1. Pour attribuer des droits sur des dossiers ou des fichiers individuels, sélectionnez le dossier dans le volet gauche. Le contenu du dossier s’affiche dans le volet droit. Attribuez ensuite des droits au groupe en cochant les cases des dossiers ou fichiers correspondants dans le volet droit.

   Ce tableau présente la correspondance entre différentes tâches et les autorisations de lecture, d’écriture et de suppression associées.

   | Tâche | Lecture | Ecriture | Suppression |
   | --- | --- | --- | --- |
   | Parcourir dossiers et fichiers | X |  |  |
   | Modifier des fichiers (recadrage, accentuation, modification) |  | X |  |
   | Modifier les noms de fichiers |  | X |  |
   | Déplacer des fichiers vers des dossiers différents |  | X |  |
   | Renommer des fichiers |  | X |  |
   | Supprimer des fichiers |  |  | X |

1. Sélectionner **[!UICONTROL Fermer]**.

>[!NOTE]
>
>les droits d’accès sont établis lorsque vous sélectionnez une zone de texte. Lorsque vous accordez des droits sur un dossier, ses sous-dossiers ainsi que tous les fichiers qu’il contient obtiennent les mêmes droits que le dossier parent. Toutefois, vous pouvez définir des droits différents pour des sous-dossiers et des fichiers individuels.

## Choix des autorisations d’accès de paramètres d’image prédéfinis pour un groupe {#choosing-image-preset-access-permissions-for-a-group}

Choisissez les autorisations d’accès de paramètres d’image prédéfinis si vous souhaitez indiquer quels paramètres d’image prédéfinis sont disponibles pour les membres du groupes lorsqu’ils exportent des fichiers avec le portail multimédia.

Voir aussi [Définition des options d’exportation disponibles pour les utilisateurs de Media Portal](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

**Pour choisir les autorisations d’accès aux paramètres d’image prédéfinis pour un groupe :**

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de Media Portal]** > **[!UICONTROL Groupes]**.
1. Dans la page de liste des Groupes, effectuez l’une de ces actions :

   * Pour ajouter un groupe et spécifier les paramètres d’image prédéfinis qui lui sont disponibles, sélectionnez **[!UICONTROL Ajouter]**. Dans la boîte de dialogue Ajouter un groupe, saisissez le nom du groupe, puis sélectionnez **[!UICONTROL Ajouter un groupe]**, puis ajoutez des utilisateurs au groupe.
   * Pour modifier les options de paramètre d’image prédéfini d’un groupe, sélectionnez le groupe, puis sélectionnez **[!UICONTROL Modifier]**.

1. Dans la boîte de dialogue Ajouter un groupe ou Modifier le groupe , sélectionnez le **[!UICONTROL Autorisations d’accès aux paramètres d’image prédéfinis]** .
1. Pour spécifier les paramètres prédéfinis qui sont disponibles pour les utilisateurs du portail multimédia lorsqu’ils exportent des ressources, sélectionnez ou désélectionnez Paramètres d’image prédéfinis.
1. Sélectionner **[!UICONTROL Fermer]**.

## Modification et suppression de groupes {#edit-and-delete-groups}

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de Media Portal]** > **[!UICONTROL Groupes]**.
1. Sur la page de liste des groupes, sélectionnez un groupe et modifiez ou supprimez-le.

   **Modification d’un groupe** - Sélectionner **[!UICONTROL Modifier]**, puis sélectionnez des options dans la boîte de dialogue Modifier le groupe .

   **Suppression d’un groupe** - Sélectionner **[!UICONTROL Supprimer]**.
