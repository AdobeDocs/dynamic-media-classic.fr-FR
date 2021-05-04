---
title: Gestion du dossier Corbeille
description: Découvrez comment gérer le dossier Corbeille.
uuid: 3992a5b8-1919-4924-b07d-7fb25565effd
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 553c95fc-0a41-4f06-af50-a62bc1438149
feature: Dynamic Media Classic,Gestion des ressources
role: Business Practitioner
exl-id: cffeec19-43fd-4a97-bdcc-df81af108ddd
translation-type: tm+mt
source-git-commit: 1beb30b9eda4487dcd549034906079dee0b3149a
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 39%

---

# Gestion du dossier Corbeille{#managing-the-trash-folder}

Les éléments que vous supprimez de Dynamic Media Classic sont déplacés dans le dossier Corbeille. Les éléments supprimés restent dans ce dossier pendant sept jours jusqu’à ce qu’ils soient restaurés ou définitivement supprimés. Vous pouvez examiner les éléments supprimés en cliquant sur l’icône **[!UICONTROL Corbeille]** au bas de la bibliothèque de fichiers et en affichant les éléments dans la page du dossier Corbeille.

Tous les utilisateurs peuvent restaurer des objets du dossier Corbeille vers leurs dossiers d’origine. Tous les utilisateurs peuvent également vider le dossier Corbeille de tout son contenu.

La suppression d’éléments du dossier Corbeille supprime définitivement les éléments de Dynamic Media Classic ; les éléments supprimés du dossier Corbeille ne peuvent plus être restaurés. Pour plus d’informations sur la configuration de notifications envoyées aux administrateurs d’entreprises lorsque des fichiers sont sur le point d’être supprimés automatiquement du dossier Corbeille, voir [Paramètres généraux de l’application](application-setup.md#general_settings).

>[!NOTE]
>
>Les fichiers qui ont été déplacés dans le dossier Corbeille sont toujours enregistrés dans Dynamic Media Classic. Si vous tentez de télécharger un fichier portant le même nom qu’un fichier supprimé dans le dossier Corbeille, Dynamic Media Classic traite le fichier à télécharger comme un fichier duplicata. A ce titre, un numéro sera ajouté à son nom.

## A propos du dossier Corbeille {#about-the-trash-folder}

Dès que vous supprimez un objet d’un dossier, cet objet est placé dans le dossier Corbeille. Voici ce qui se passe quand vous supprimez un objet et le déplacez vers le dossier Corbeille :

* Bien que l’élément ait été supprimé de vos dossiers Dynamic Media Classic, son ID ne peut pas être affecté à un autre fichier tant qu’il reste dans le dossier Corbeille. Si vous tentez de télécharger un fichier portant le même nom qu’un fichier dans le dossier Corbeille, Dynamic Media Classic ajoute un numéro au nom du fichier.
* L’objet ne peut pas être publié. Même si l’objet était marqué pour publication au moment de sa suppression, il ne sera pas publié.
* L’élément reste dans le dossier Corbeille jusqu’à ce qu’il soit restauré, que sept jours s’écoulent ou que quelqu’un choisisse la commande **[!UICONTROL Vider la corbeille]**. Au bout de 7 jours, l’objet est définitivement supprimé au cours d’une opération de nettoyage automatique.

## Restauration de fichiers à partir du dossier Corbeille  {#restoring-assets-from-the-trash-folder}

N’importe quelle personne est autorisée à restaurer des fichiers du dossier Corbeille. Les fichiers restaurés sont placés dans leurs dossiers d’origine. Si ces dossiers n’existent plus, Dynamic Media Classic les recrée et les fichiers restaurés sont placés dans les dossiers recréés.

Pour restaurer des fichiers du dossier Corbeille vers les dossiers à partir desquels ils ont été supprimés, procédez comme suit :

1. Au bas du panneau Bibliothèque de fichiers, cliquez sur l’icône **[!UICONTROL Corbeille]** pour ouvrir le dossier Corbeille.
1. Sélectionnez le ou les fichiers à restaurer.
1. Cliquez sur **[!UICONTROL Fichier]** > **[!UICONTROL Restaurer à partir de la corbeille]**.

## Suppression définitive de fichiers du dossier Corbeille {#permanently-deleting-assets-in-the-trash-folder}

Lorsque vous supprimez des fichiers du dossier Corbeille, sachez qu’ils sont définitivement supprimés. Les fichiers sont automatiquement supprimés du dossier Corbeille au bout de 7 jours.

Pour supprimer définitivement des fichiers du dossier Corbeille, cliquez sur l’icône **[!UICONTROL Corbeille]**. Sur la page du dossier Corbeille, effectuez l’une des opérations suivantes :

* **Suppression de fichiers**  individuels : sélectionnez les fichiers à supprimer définitivement, puis cliquez sur  **[!UICONTROL Fichier]**  >  **[!UICONTROL Supprimer de la corbeille]**.

* **Suppression de tous les fichiers**  - Cliquez sur  **[!UICONTROL Fichier]**  >  **[!UICONTROL Vider la corbeille]**.

>[!MORELIKETHIS]
>
>* [Suppression de fichiers](moving-renaming-deleting-assets.md#delete_assets)

