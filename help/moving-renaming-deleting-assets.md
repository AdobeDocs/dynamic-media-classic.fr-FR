---
title: Déplacement, suppression et changement de nom de fichier
seo-title: Déplacement, suppression et changement de nom de fichier
description: 'null'
seo-description: Découvrez comment déplacer, renommer et supprimer des fichiers.
uuid: deff 6521-0 ad 0-4 db 9-b 4 e 0-e 3211 ff 97740
contentOwner: admin
content-type: référence
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/managing_ assets
discoiquuid: 1 c 9 e 29 f 0-3083-4 d 22-a 439-2 a 01 faf 59683
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Déplacement, suppression et changement de nom de fichier{#moving-renaming-and-deleting-assets}

Vous pouvez déplacer, renommer et supprimer des fichiers à partir du panneau de navigation. Vous pouvez également supprimer plusieurs fichiers simultanément à l’aide d’un fichier texte.

## Déplacement des fichiers {#move-assets}

Vous pouvez déplacer des fichiers dans d’autres dossiers du panneau de navigation.

1. Pour ce faire, sélectionnez le ou les fichiers dans le panneau de navigation, puis utilisez l’une des méthodes suivantes :

   * Affichez le dossier vers lequel vous souhaitez déplacer les fichiers dans la bibliothèque de fichiers, puis faites glisser les fichiers vers le dossier en question.
   * Choisissez Fichier &gt; Déplacer, sélectionnez un dossier dans la fenêtre Déplacer les fichiers, puis cliquez sur Déplacer.

## Attribution d’un nouveau nom à un fichier {#rename-assets}

Pour renommer un fichier :

1. Sélectionnez le fichier dans le panneau de navigation, puis utilisez l’une des méthodes suivantes :

   * Sélectionnez le nom, saisissez un nouveau nom, puis appuyez sur Entrée ou cliquez en dehors du nom.
   * Choisissez Fichier &gt; Renommer. Le nom du fichier est mis en surbrillance. Saisissez un nouveau nom, puis appuyez sur la touche Entrée.

Vous ne devez pas saisir le nom d’un fichier Scene7 Publishing System existant.

## Suppression de fichiers {#delete-assets}

Vous pouvez supprimer des fichiers sélectionnés dans le panneau de navigation ainsi que des dossiers entiers. Les fichiers et les dossiers supprimés sont déplacés vers le dossier Corbeille, où ils sont conservés pendant sept jours avant d’être définitivement supprimés.

Lorsque vous supprimez un fichier, tous les fichiers dérivés de ce fichier sont supprimés en même temps. Par exemple, la suppression d’une image pour laquelle vous avez créé des cibles de zoom entraîne la suppression simultanée des cibles de zoom.

>[!NOTE]
>
>les cibles de zoom, les attributs d’image et les entrées d’historique sont supprimés définitivement lorsque vous supprimez les fichiers d’où ils proviennent. Ils ne sont pas déplacés simultanément avec le fichier vers le dossier Corbeille ; ils ne peuvent pas non plus être restaurés depuis la Corbeille.

1. Utilisez l’une des méthodes suivantes :

   * Pour supprimer un ou plusieurs fichiers, sélectionnez-les dans le panneau de navigation et appuyez sur la touche Suppr ou choisissez Fichier &gt; Supprimer.
   * To delete a folder, select the folder in the Asset Library, and click **Remove Folder**.

      La suppression d’un dossier supprime tous les fichiers qu’il contient ainsi que tous les fichiers de ses sous-dossiers.

>[!NOTE]
>
>Dynamic Media Classic recommande d'écraser les fichiers plutôt que de les supprimer si votre motif de suppression d'un fichier est de le remplacer par un autre portant le même nom.

## Suppression de plusieurs fichiers à l’aide d’un fichier texte {#delete-multiple-assets-with-a-text-file}

Pour supprimer plusieurs fichiers à la fois dans la bibliothèque de fichiers, vous pouvez répertorier les fichiers à supprimer dans un fichier texte et les envoyer à Dynamic Media Classic.

Créez la liste des identifiants Scene7 Publishing System et enregistrez-la dans un fichier texte (.txt). Chaque identifiant Scene7 Publishing System doit apparaître sur une ligne différente (suivi d’un retour à la ligne forcé).

Pour supprimer des fichiers à l’aide de cette liste créée, procédez comme suit :

1. Choisissez Fichier &gt; Supprimer une liste de fichiers.
1. Dans la boîte de dialogue Supprimer une liste de fichiers, parcourez les dossiers ou tapez le chemin de l’emplacement du fichier texte comportant la liste des fichiers à supprimer.
1. Cliquez sur le bouton Supprimer.

Lorsque vous supprimez des fichiers avec un fichier texte, si un identifiant Scene 7 Publishing System ne figure pas dans la liste, un message s'affiche pour vous informer que Dynamic Media Classic est « Impossible de valider ces entrées dans votre liste :  » avec la liste des entrées. Cependant, Dynamic Media Classic ne génère pas d'erreur sur l'écran Tâches.

>[!MORELIKETHIS]
>
>* [Sélection de fichiers dans le panneau de navigation](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [Préparation du téléchargement des fichiers et dossiers](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [Restauration de fichiers à partir du dossier Corbeille](trash-folder.md#restoring_assets_from_the_trash_folder)

