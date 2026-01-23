---
title: Déplacement, changement de nom et suppression de ressources
description: Découvrez comment déplacer, renommer et supprimer des ressources dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 391eb7ce-ed89-47a8-a6c6-5adb3e95bf78
topic: Content Management
level: Intermediate
source-git-commit: c4613c78347c4bda3d84747a72146617158c03b6
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 17%

---

# Déplacement, changement de nom et suppression de ressources{#moving-renaming-and-deleting-assets}

Vous pouvez déplacer, renommer et supprimer des ressources à partir du panneau de navigation. Vous pouvez également supprimer plusieurs fichiers simultanément à l’aide d’un fichier texte.

## Déplacement des fichiers {#move-assets}

Vous pouvez déplacer des ressources vers différents dossiers dans le panneau Parcourir .

**Pour déplacer des ressources, procédez comme suit**

1. Sélectionnez la ou les ressources dans le panneau de navigation, puis effectuez l’une des opérations suivantes :

   * Affichez le dossier dans lequel vous souhaitez déplacer les ressources dans la bibliothèque de ressources et faites-les glisser vers le dossier.
   * Accédez à **[!UICONTROL Fichier]** > **`Move`**, sélectionnez un dossier dans la fenêtre `Move Assets`, puis sélectionnez **`Move`**.

## Attribution d’un nouveau nom à un fichier {#rename-assets}

1. Sélectionnez la ressource dans le panneau Parcourir et effectuez l’une des opérations suivantes :

   * Sélectionnez le nom, saisissez un nouveau nom, puis appuyez sur **[!UICONTROL Entrée]** ou sélectionnez un nom différent.
   * Sélectionnez **[!UICONTROL Fichier]** > **[!UICONTROL Renommer]**. Le nom du fichier est mis en surbrillance. Saisissez un nouveau nom et appuyez sur **[!UICONTROL Entrée]**. Veillez à ne pas saisir le nom d’une ressource Adobe Dynamic Media Classic existante.

## Suppression de fichiers {#delete-assets}

Vous pouvez supprimer des ressources sélectionnées dans le panneau de navigation et supprimer des dossiers entiers. Les fichiers et les dossiers supprimés sont déplacés vers le dossier Corbeille, où ils sont conservés pendant sept jours avant d’être définitivement supprimés.

Lorsque vous avez supprimé une ressource, toutes les ressources qui en étaient dérivées sont également supprimées. Par exemple, la suppression d’une image pour laquelle vous avez créé des cibles de zoom supprime les cibles de zoom ainsi que l’image.

les cibles de zoom, les attributs d’image et les entrées d’historique sont supprimés définitivement lorsque vous supprimez les fichiers d’où ils proviennent. Ils ne sont pas déplacés simultanément avec le fichier vers le dossier Corbeille ; ils ne peuvent pas non plus être restaurés depuis la Corbeille.

>[!IMPORTANT]
>
>La suppression en bloc est une opération intensive. Veillez à exécuter les suppressions en bloc de manière séquentielle plutôt que comme des opérations de suppression lourdes simultanées. Adobe vous recommande de limiter les opérations de suppression à 5 000 suppressions de ressources ou moins par heure. Tout nombre supérieur à 5 000 par heure peut entraîner une limitation de débit.

**Pour supprimer des ressources, procédez comme suit**

1. Utilisez l’une des méthodes suivantes :

   * Pour supprimer une ou plusieurs ressources, sélectionnez-les dans le panneau Parcourir et appuyez sur **[!UICONTROL Supprimer]** ou accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Supprimer]**.
   * Pour supprimer un dossier, sélectionnez-le dans la bibliothèque de ressources, puis sélectionnez **[!UICONTROL Supprimer le dossier]**.

     La suppression d’un dossier supprime le dossier, toutes les ressources du dossier et toutes les ressources de ses sous-dossiers.

Adobe Dynamic Media Classic recommande de remplacer les fichiers de ressources plutôt que de les supprimer si la raison de la suppression d’un fichier de ressources est de le remplacer par un autre fichier portant le même nom.

## Suppression de plusieurs fichiers à l’aide d’un fichier texte {#delete-multiple-assets-with-a-text-file}

Pour supprimer plusieurs ressources à la fois dans la bibliothèque de ressources, vous pouvez répertorier les ressources à supprimer dans un fichier texte et envoyer la liste à Adobe Dynamic Media Classic.

Créez la liste des identifiants Adobe Dynamic Media Classic et enregistrez-la en tant que fichier texte (.txt). Chaque Adobe Dynamic Media Classic ID doit se trouver sur sa propre ligne (suivi d’un retour hard).

Pour supprimer des fichiers à l’aide de cette liste créée, procédez comme suit :

1. Accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Supprimer la liste des ressources]**.
1. Dans la boîte de dialogue **[!UICONTROL Liste des ressources supprimées]**, saisissez le chemin d’accès au fichier texte avec la liste des ressources à supprimer.
1. Sélectionnez **[!UICONTROL Supprimer]**.

Lorsque vous supprimez des ressources avec un fichier texte, si un Adobe Dynamic Media Classic ID ne figure pas dans la liste, le message « Impossible de valider ces entrées dans la liste : » s’affiche. La liste des entrées s’affiche également. Toutefois, Adobe Dynamic Media Classic ne génère pas d’erreur sur la page de la tâche.

>[!MORELIKETHIS]
>
>* [Sélection de ressources dans le panneau de navigation](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [Préparation du chargement de vos ressources et dossiers](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [Restaurer des ressources à partir du dossier Corbeille](trash-folder.md#restoring_assets_from_the_trash_folder)
