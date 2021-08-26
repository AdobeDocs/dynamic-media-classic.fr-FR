---
title: Déplacer, renommer et supprimer des ressources
description: Découvrez comment déplacer, renommer et supprimer des ressources dans Adobe Dynamic Media Classic.
uuid: deff6521-0ad0-4db9-b4e0-e3211ff97740
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 1c9e29f0-3083-4d22-a439-2a01faf59683
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 391eb7ce-ed89-47a8-a6c6-5adb3e95bf78
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 37%

---

# Déplacer, renommer et supprimer des ressources{#moving-renaming-and-deleting-assets}

Vous pouvez déplacer, renommer et supprimer des fichiers à partir du panneau de navigation. Vous pouvez également supprimer plusieurs fichiers simultanément à l’aide d’un fichier texte.

## Déplacement des fichiers {#move-assets}

Vous pouvez déplacer des fichiers dans d’autres dossiers du panneau de navigation.

1. Pour ce faire, sélectionnez le ou les fichiers dans le panneau de navigation, puis utilisez l’une des méthodes suivantes :

   * Affichez le dossier vers lequel vous souhaitez déplacer les fichiers dans la bibliothèque de fichiers, puis faites glisser les fichiers vers le dossier en question.
   * Accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Déplacer]**, sélectionnez un dossier dans la fenêtre Déplacer les ressources, puis sélectionnez **[!UICONTROL Déplacer]**.

## Attribution d’un nouveau nom à un fichier {#rename-assets}

1. Sélectionnez le fichier dans le panneau de navigation, puis utilisez l’une des méthodes suivantes :

   * Sélectionnez le nom, saisissez un nouveau nom, puis appuyez sur **[!UICONTROL Entrée]** ou sélectionnez un nom différent.
   * Accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Renommer]**. Le nom du fichier est mis en surbrillance. Saisissez un nouveau nom et appuyez sur **[!UICONTROL Entrée]**.

Veillez à ne pas saisir le nom d’une ressource Dynamic Media Classic Adobe existante.

## Suppression de fichiers {#delete-assets}

Vous pouvez supprimer des ressources sélectionnées dans le panneau de navigation et supprimer des dossiers entiers. Les fichiers et les dossiers supprimés sont déplacés vers le dossier Corbeille, où ils sont conservés pendant sept jours avant d’être définitivement supprimés.

Lorsque vous supprimez un fichier, tous les fichiers dérivés de ce fichier sont supprimés en même temps. Par exemple, la suppression d’une image pour laquelle vous avez créé des cibles de zoom entraîne la suppression simultanée des cibles de zoom.

>[!NOTE]
>
>les cibles de zoom, les attributs d’image et les entrées d’historique sont supprimés définitivement lorsque vous supprimez les fichiers d’où ils proviennent. Ils ne sont pas déplacés simultanément avec le fichier vers le dossier Corbeille ; ils ne peuvent pas non plus être restaurés depuis la Corbeille.

1. Utilisez l’une des méthodes suivantes :

   * Pour supprimer une ou plusieurs ressources, sélectionnez-les dans le panneau de navigation, puis appuyez sur **[!UICONTROL Supprimer]** ou accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Supprimer]**.
   * Pour supprimer un dossier, sélectionnez-le dans la bibliothèque de ressources, puis sélectionnez **[!UICONTROL Supprimer le dossier]**.

      La suppression d’un dossier supprime le dossier, toutes les ressources qu’il contient, ainsi que toutes les ressources qu’il contient.

>[!NOTE]
>
>Adobe Dynamic Media Classic recommande de remplacer les fichiers de ressources plutôt que de les supprimer si la raison pour laquelle vous supprimez un fichier de ressources est de le remplacer par un autre portant le même nom.

## Suppression de plusieurs fichiers à l’aide d’un fichier texte {#delete-multiple-assets-with-a-text-file}

Pour supprimer de nombreuses ressources à la fois dans la bibliothèque de ressources, vous pouvez répertorier les ressources que vous souhaitez supprimer dans un fichier texte et envoyer la liste à Adobe Dynamic Media Classic.

Créez la liste des identifiants Dynamic Media Classic Adobe et enregistrez-la sous la forme d’un fichier texte (.txt). Chaque identifiant Dynamic Media Classic Adobe doit se trouver sur sa propre ligne (suivie d’un retour forcé).

Pour supprimer des fichiers à l’aide de cette liste créée, procédez comme suit :

1. Accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Supprimer la liste des ressources]**.
1. Dans la boîte de dialogue Supprimer la liste des ressources, recherchez ou saisissez le chemin d’accès au fichier texte avec la liste des ressources à supprimer.
1. Sélectionnez **[!UICONTROL Supprimer]**.

Lorsque vous supprimez des ressources avec un fichier texte, si un identifiant Dynamic Media Classic Adobe n’est pas répertorié dans la liste, le message &quot;Impossible de valider ces entrées dans votre liste :&quot; s’affiche et la liste des entrées s’affiche. Cependant, Adobe Dynamic Media Classic ne génère pas d’erreur sur la page Tâche.

>[!MORELIKETHIS]
>
>* [Sélection de ressources dans le panneau de navigation](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [Préparation du chargement des ressources et des dossiers](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [Restauration des ressources à partir du dossier Corbeille](trash-folder.md#restoring_assets_from_the_trash_folder)

