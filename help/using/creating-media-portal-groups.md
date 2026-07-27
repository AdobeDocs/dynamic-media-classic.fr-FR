---
title: Créer et gérer des groupes de portail multimédia
description: Découvrez comment créer et gérer des groupes du portail multimédia dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: 0deb7133-b895-4c3f-8e5e-8604a6f2d16b
topic: Administration, Collaboration
level: Intermediate
autotag-review: '2026-05-13T17:41:54.576Z'
TQID: 'https://experienceleague.adobe.com/If0j5hWmxTOGGYshsqh2sa0iM3S2SvG57iPO2rtG1lY'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 9e8d28c53d9bcc90cbbbb09b038833136fc96ad7
workflow-type: tm+mt
source-wordcount: 843
ht-degree: 39%

---

# Création et gestion de groupes du portail multimédia{#creating-and-managing-media-portal-groups}

Les groupes sont conçus pour vous aider à administrer les utilisateurs du portail multimédia. Pour accéder à un fichier, un utilisateur doit appartenir au minimum à un groupe autorisé à accéder à ce fichier. Lorsque vous ajoutez un utilisateur, vous l’affectez à un ou plusieurs groupes. Ce faisant, vous accordez à l’utilisateur l’accès aux dossiers auxquels le groupe a été affecté. Vous pouvez également choisir les paramètres d’image prédéfinis qui sont disponibles pour un groupe.

## Utilisez des groupes pour restreindre l’accès aux dossiers, ressources et paramètres d’image prédéfinis {#using-groups-to-restrict-access-to-folders-assets-and-image-presets}

Pour accorder des autorisations d’accès à différents niveaux, vous créez des groupes. Pour chaque groupe, vous définissez des autorisations d’accès en lecture, en écriture et en suppression à des dossiers et à leur contenu. En outre, vous décidez des paramètres d’image prédéfinis disponibles pour le groupe. Vous affectez ensuite les utilisateurs à des groupes. Un utilisateur peut appartenir à plusieurs groupes. La fonction de groupe offre la possibilité d’attribuer l’accès à des ensembles limités de contenu total.

Si vous n’accordez pas spécifiquement l’autorisation de groupe à une ressource ou à un dossier, cette ressource ou ce dossier hérite des autorisations que vous avez attribuées à son dossier parent (le dossier situé au-dessus dans la hiérarchie des dossiers). Octroyez des autorisations sur un dossier parent. Effectuez cette opération pour vous assurer que tous ses dossiers enfants héritent des mêmes autorisations.

>[!NOTE]
>
>les utilisateurs peuvent appartenir à plusieurs groupes. Lorsqu’un utilisateur appartient à deux groupes avec des autorisations d’accès différentes à un dossier, l’accès le plus permissif lui est accordé.

## Ajout d’un groupe {#adding-a-group}

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration du portail multimédia]** > **[!UICONTROL Groupes]**.
1. Sélectionnez **[!UICONTROL Ajouter]**.
1. Dans la boîte de dialogue Ajouter un groupe, saisissez un nom pour le groupe dans la zone Nom du groupe, puis sélectionnez **[!UICONTROL Ajouter un groupe]**.
1. Le cas échéant, vous pouvez cocher les cases situées en regard des noms des utilisateurs à ajouter au nouveau groupe.
1. Si vous souhaitez spécifier des autorisations d’accès maintenant, sélectionnez l’onglet **[!UICONTROL Autorisations d’accès aux ressources]**, puis spécifiez les options de votre choix.

   Voir [Définition des autorisations d’accès aux fichiers pour un groupe](creating-media-portal-groups.md#establishing_asset_access_permissions_for_a_group).

1. Vous pouvez choisir les paramètres d’image prédéfinis disponibles pour le groupe. Cliquez sur l’onglet **[!UICONTROL Autorisations d’accès aux paramètres d’image prédéfinis]** et sélectionnez Paramètres d’image prédéfinis que le groupe peut utiliser.

   Voir [Choix des autorisations d’accès de paramètres d’image prédéfinis pour un groupe](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group).

1. Sélectionnez **[!UICONTROL Fermer]**.

## Définition des autorisations d’accès aux fichiers pour un groupe {#establishing-asset-access-permissions-for-a-group}

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration du portail multimédia]** > **[!UICONTROL Groupes]**.
1. Dans la page de liste des Groupes, effectuez l’une de ces actions :

   * Pour ajouter un groupe et spécifier des autorisations, sélectionnez **[!UICONTROL Ajouter]**. Dans la boîte de dialogue Ajouter un groupe, saisissez un nom pour le groupe, sélectionnez **[!UICONTROL Ajouter un groupe]** et ajoutez des utilisateurs au groupe.
   * Pour modifier les autorisations d’un groupe, sélectionnez-le, puis sélectionnez **[!UICONTROL Modifier]**.

1. Dans la boîte de dialogue Ajouter un groupe ou Modifier le groupe , sélectionnez l’onglet **[!UICONTROL Autorisations d’accès aux ressources]**. Dans la partie droite de l’onglet, des cases permettent de définir les autorisations en lecture, en écriture et en suppression sur les dossiers et les fichiers. Vous pouvez développer et réduire les dossiers et sous-dossiers dans le volet gauche.
1. Pour attribuer des droits sur des dossiers ou des fichiers individuels, sélectionnez le dossier dans le volet gauche. Le contenu du dossier s’affiche dans le volet droit. Attribuez ensuite des droits au groupe en cochant les cases des fichiers correspondants. Vous pouvez également sélectionner les dossiers dans le volet de droite.

   Ce tableau présente la correspondance entre différentes tâches et les autorisations de lecture, d’écriture et de suppression associées.

   | Tâche | Lecture | Ecriture | Suppression |
   | --- | --- | --- | --- |
   | Parcourir dossiers et fichiers | X | | |
   | Modifier des fichiers (recadrage, accentuation, modification) | | X | |
   | Modifier les noms de fichiers | | X | |
   | Déplacer des fichiers vers des dossiers différents | | X | |
   | Renommer des fichiers | | X | |
   | Supprimer des fichiers | | | X |

1. Sélectionnez **[!UICONTROL Fermer]**.

>[!NOTE]
>
>les droits d’accès sont établis lorsque vous sélectionnez une zone de texte. Lorsque vous accordez des droits sur un dossier, ses sous-dossiers ainsi que tous les fichiers qu’il contient obtiennent les mêmes droits que le dossier parent. Toutefois, vous pouvez définir des droits différents pour des sous-dossiers et des fichiers individuels.

## Choix des autorisations d’accès de paramètres d’image prédéfinis pour un groupe

Sélectionnez Autorisations d’accès aux paramètres prédéfinis d’image pour un groupe. Utilisez cette option pour spécifier les paramètres d’image prédéfinis disponibles pour les membres du groupe. Utilisez cette option lorsqu’ils exportent des ressources avec Media Portal.

Voir aussi [Définition des options d’exportation disponibles pour les utilisateurs du portail multimédia](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

**Pour choisir les autorisations d’accès des paramètres prédéfinis d’image pour un groupe :**

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration du portail multimédia]** > **[!UICONTROL Groupes]**.
1. Dans la page de liste des Groupes, effectuez l’une de ces actions :

   * Pour ajouter un groupe et spécifier les paramètres d’image prédéfinis disponibles, sélectionnez **[!UICONTROL Ajouter]**. Dans la boîte de dialogue Ajouter un groupe, saisissez un nom pour le groupe, sélectionnez **[!UICONTROL Ajouter un groupe]** et ajoutez des utilisateurs au groupe.
   * Pour modifier les options de paramètre prédéfini d’image d’un groupe, sélectionnez le groupe, puis sélectionnez **[!UICONTROL Modifier]**.

1. Dans la boîte de dialogue Ajouter un groupe ou Modifier le groupe , sélectionnez l’onglet **[!UICONTROL Autorisations d’accès aux paramètres prédéfinis d’image]**.
1. Pour spécifier les paramètres prédéfinis disponibles pour les utilisateurs du portail multimédia lorsqu’ils exportent des ressources, sélectionnez ou désélectionnez Paramètres d’image prédéfinis.
1. Sélectionnez **[!UICONTROL Fermer]**.

## Modification et suppression de groupes {#edit-and-delete-groups}

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration du portail multimédia]** > **[!UICONTROL Groupes]**.
1. Sur la page de liste des groupes, sélectionnez un groupe et modifiez ou supprimez-le.

   **Modifier un groupe** : sélectionnez **[!UICONTROL Modifier]**, puis choisissez les options de la boîte de dialogue Modifier le groupe.

   **Supprimer un groupe** : sélectionnez **[!UICONTROL Supprimer]**.
