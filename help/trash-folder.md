---
title: Gestion du dossier Corbeille
seo-title: Gestion du dossier Corbeille
description: 'null'
seo-description: Découvrez comment gérer le dossier Corbeille.
uuid: 3992a5b8-1919-4924-b07d-7fb25565effd
contentOwner: admin
content-type: référence
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 553c95fc-0a41-4f06-af50-a62bc1438149
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Gestion du dossier Corbeille{#managing-the-trash-folder}

Les objets que vous supprimez de Scene7 Publishing System sont déplacés vers le dossier Corbeille. Ils y restent sept jours durant avant d’être restaurés ou définitivement supprimés. Vous pouvez examiner des objets supprimés en sélectionnant l’icône Corbeille  située en bas de la bibliothèque de fichiers.

Tous les utilisateurs peuvent restaurer des objets du dossier Corbeille vers leurs dossiers d’origine. Tous les utilisateurs peuvent également vider le dossier Corbeille de tout son contenu.

La suppression d’objets du dossier Corbeille entraîne la suppression définitive des objets de Scene7 Publishing System ; les objets supprimés du dossier Corbeille ne peuvent plus être restaurés. Pour plus d’informations sur la configuration de notifications envoyées aux administrateurs d’entreprises lorsque des fichiers sont sur le point d’être supprimés automatiquement du dossier Corbeille, voir [Paramètres généraux de l’application](application-setup.md#general_settings).

>[!NOTE]
>
>les fichiers déplacés vers le dossier Corbeille sont toujours enregistrés dans Scene7 Publishing System. Si vous tentez de télécharger un fichier portant le même nom qu’un fichier supprimé dans le dossier Corbeille, Dynamic Media Classic traite le fichier à télécharger comme un fichier en double. A ce titre, un numéro sera ajouté à son nom.

## A propos du dossier Corbeille {#about-the-trash-folder}

Dès que vous supprimez un objet d’un dossier, cet objet est placé dans le dossier Corbeille. Voici ce qui se passe quand vous supprimez un objet et le déplacez vers le dossier Corbeille :

* Bien que l’objet soit supprimé de vos dossiers Scene7 Publishing System, il est impossible d’attribuer son identification à un autre fichier tant qu’il reste dans le dossier Corbeille. Si vous tentez de télécharger un fichier portant le même nom qu’un fichier dans le dossier Corbeille, Dynamic Media Classic ajoute un numéro au nom du fichier.
* L’objet ne peut pas être publié. Même si l’objet était marqué pour publication au moment de sa suppression, il ne sera pas publié.
* L’objet reste dans le dossier Corbeille jusqu’à ce qu’il soit restauré, que 7 jours se soient écoulés ou qu’il soit définitivement supprimé par la commande Vider la corbeille. Au bout de 7 jours, l’objet est définitivement supprimé au cours d’une opération de nettoyage automatique.

## Restauration de fichiers à partir du dossier Corbeille {#restoring-assets-from-the-trash-folder}

N’importe quelle personne est autorisée à restaurer des fichiers du dossier Corbeille. Les fichiers restaurés sont placés dans leurs dossiers d’origine. Si ces dossiers n’existent plus, Scene7 Publishing System les recrée pour les y placer.

Pour restaurer des fichiers du dossier Corbeille vers leurs dossiers d’origine, procédez comme suit :

1. Cliquez sur l’icône Corbeille pour ouvrir le dossier Corbeille.
1. Sélectionnez le ou les fichiers à restaurer.
1. Choisissez Fichier &gt; Restaurer depuis la corbeille.

## Suppression définitive de fichiers du dossier Corbeille {#permanently-deleting-assets-in-the-trash-folder}

Lorsque vous supprimez des fichiers du dossier Corbeille, sachez qu’ils sont définitivement supprimés. Les fichiers sont automatiquement supprimés du dossier Corbeille au bout de 7 jours.

Pour supprimer définitivement des fichiers du dossier Corbeille, sélectionnez l’icône Corbeille  pour ouvrir le dossier correspondant. Ensuite, procédez à la suppression de fichiers individuels ou de tous les fichiers :

* **Suppression de fichiers** individuels Sélectionnez les fichiers à supprimer définitivement, puis cliquez sur **[!UICONTROL Fichier &gt; Vider de la corbeille]**.

* **Pour supprimer tous les fichiers** , cliquez sur **[!UICONTROL Fichier &gt; Corbeille]** vide.

>[!MORELIKETHIS]
>
>* [Suppression de fichiers](moving-renaming-deleting-assets.md#delete_assets)

