---
title: Déplacement, suppression et changement de nom de fichier
description: Découvrez comment déplacer, renommer et supprimer des fichiers.
uuid: deff6521-0ad0-4db9-b4e0-e3211ff97740
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 1c9e29f0-3083-4d22-a439-2a01faf59683
feature: Dynamic Media Classic,Gestion des ressources
role: Professionnel
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '574'
ht-degree: 65%

---


# Déplacement, suppression et changement de nom de fichier{#moving-renaming-and-deleting-assets}

Vous pouvez déplacer, renommer et supprimer des fichiers à partir du panneau de navigation. Vous pouvez également supprimer plusieurs fichiers simultanément à l’aide d’un fichier texte.

## Déplacement des fichiers {#move-assets}

Vous pouvez déplacer des fichiers dans d’autres dossiers du panneau de navigation.

1. Pour ce faire, sélectionnez le ou les fichiers dans le panneau de navigation, puis utilisez l’une des méthodes suivantes :

   * Affichez le dossier vers lequel vous souhaitez déplacer les fichiers dans la bibliothèque de fichiers, puis faites glisser les fichiers vers le dossier en question.
   * Choisissez Fichier > Déplacer, sélectionnez un dossier dans la fenêtre Déplacer les fichiers, puis cliquez sur Déplacer.

## Attribution d’un nouveau nom à un fichier  {#rename-assets}

Pour renommer un fichier :

1. Sélectionnez le fichier dans le panneau de navigation, puis utilisez l’une des méthodes suivantes :

   * Sélectionnez le nom, saisissez un nouveau nom, puis appuyez sur Entrée ou cliquez en dehors du nom.
   * Choisissez Fichier > Renommer. Le nom du fichier est mis en surbrillance. Saisissez un nouveau nom, puis appuyez sur la touche Entrée.

Veillez à ne pas saisir le nom d’une ressource Dynamic Media Classic existante.

## Suppression de fichiers {#delete-assets}

Vous pouvez supprimer des fichiers sélectionnés dans le panneau de navigation ainsi que des dossiers entiers. Les fichiers et les dossiers supprimés sont déplacés vers le dossier Corbeille, où ils sont conservés pendant sept jours avant d’être définitivement supprimés.

Lorsque vous supprimez un fichier, tous les fichiers dérivés de ce fichier sont supprimés en même temps. Par exemple, la suppression d’une image pour laquelle vous avez créé des cibles de zoom entraîne la suppression simultanée des cibles de zoom.

>[!NOTE]
>
>les cibles de zoom, les attributs d’image et les entrées d’historique sont supprimés définitivement lorsque vous supprimez les fichiers d’où ils proviennent. Ils ne sont pas déplacés simultanément avec le fichier vers le dossier Corbeille ; ils ne peuvent pas non plus être restaurés depuis la Corbeille.

1. Utilisez l’une des méthodes suivantes :

   * Pour supprimer un ou plusieurs fichiers, sélectionnez-les dans le panneau de navigation et appuyez sur la touche Suppr ou choisissez Fichier > Supprimer.
   * Pour supprimer un dossier, sélectionnez-le dans la bibliothèque de fichiers, puis cliquez sur **Supprimer un dossier**.

      La suppression d’un dossier supprime tous les fichiers qu’il contient ainsi que tous les fichiers de ses sous-dossiers.

>[!NOTE]
>
>Dynamic Media Classic recommande d’écraser les fichiers plutôt que de les supprimer si vous souhaitez remplacer un fichier par un autre fichier portant le même nom.

## Suppression de plusieurs fichiers à l’aide d’un fichier texte {#delete-multiple-assets-with-a-text-file}

Pour supprimer plusieurs fichiers à la fois dans la bibliothèque de fichiers, vous pouvez liste les fichiers à supprimer dans un fichier texte et envoyer la liste à Dynamic Media Classic.

Créez la liste des identifiants Dynamic Media Classic et enregistrez-la dans un fichier texte (.txt). Chaque identifiant Dynamic Media Classic doit se trouver sur sa propre ligne (suivi d’un retour à la ligne forcé).

Pour supprimer des fichiers à l’aide de cette liste créée, procédez comme suit :

1. Choisissez Fichier > Supprimer une liste de fichiers.
1. Dans la boîte de dialogue Supprimer une liste de fichiers, parcourez les dossiers ou tapez le chemin de l’emplacement du fichier texte comportant la liste des fichiers à supprimer.
1. Cliquez sur le bouton Supprimer.

Lorsque vous supprimez des fichiers à l’aide d’un fichier texte, si un identifiant Dynamic Media Classic ne figure pas sur la liste, un message s’affiche vous informant que Dynamic Media Classic est &quot;Impossible de valider ces entrées dans votre liste :&quot; avec la liste des entrées. Cependant, Dynamic Media Classic ne génère pas d’erreur sur l’écran Tâches.

>[!MORELIKETHIS]
>
>* [Sélection de fichiers dans le panneau de navigation](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [Préparation du téléchargement des fichiers et dossiers](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [Restauration de fichiers à partir du dossier Corbeille](trash-folder.md#restoring_assets_from_the_trash_folder)

