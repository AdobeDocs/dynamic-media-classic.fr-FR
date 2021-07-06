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
role: User
exl-id: cffeec19-43fd-4a97-bdcc-df81af108ddd
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 39%

---

# Gestion du dossier Corbeille{#managing-the-trash-folder}

Les éléments que vous supprimez de Dynamic Media Classic sont déplacés dans le dossier Corbeille . Les éléments supprimés restent dans ce dossier pendant sept jours jusqu’à ce qu’ils soient restaurés ou supprimés définitivement. Vous pouvez examiner les éléments supprimés en cliquant sur l’icône **[!UICONTROL Corbeille]** au bas de la bibliothèque de ressources et en affichant les éléments dans la page du dossier Corbeille.

Tous les utilisateurs peuvent restaurer des objets du dossier Corbeille vers leurs dossiers d’origine. Tous les utilisateurs peuvent également vider le dossier Corbeille de tout son contenu.

La suppression d’éléments du dossier Corbeille supprime définitivement les éléments de Dynamic Media Classic ; les éléments supprimés du dossier Corbeille ne peuvent plus être restaurés. Pour plus d’informations sur la configuration de notifications envoyées aux administrateurs d’entreprises lorsque des fichiers sont sur le point d’être supprimés automatiquement du dossier Corbeille, voir [Paramètres généraux de l’application](application-setup.md#general_settings).

>[!NOTE]
>
>Les ressources qui ont été déplacées dans le dossier Corbeille sont toujours enregistrées dans Dynamic Media Classic. Si vous essayez de charger un fichier portant le même nom qu’un fichier supprimé dans le dossier Corbeille, Dynamic Media Classic traite la ressource que vous souhaitez charger comme ressource en double. A ce titre, un numéro sera ajouté à son nom.

## A propos du dossier Corbeille {#about-the-trash-folder}

Dès que vous supprimez un objet d’un dossier, cet objet est placé dans le dossier Corbeille. Voici ce qui se passe quand vous supprimez un objet et le déplacez vers le dossier Corbeille :

* Bien que l’élément ait été supprimé de vos dossiers Dynamic Media Classic, son identifiant ne peut pas être attribué à une autre ressource tant qu’il reste dans le dossier Corbeille. Si vous essayez de charger une ressource portant le même nom qu’un fichier dans le dossier Corbeille, Dynamic Media Classic ajoute un chiffre au nom de la ressource.
* L’objet ne peut pas être publié. Même si l’objet était marqué pour publication au moment de sa suppression, il ne sera pas publié.
* L’élément reste dans le dossier Corbeille jusqu’à ce qu’il soit restauré, que sept jours s’écoulent ou qu’une personne choisisse la commande **[!UICONTROL Vider la corbeille]** . Au bout de 7 jours, l’objet est définitivement supprimé au cours d’une opération de nettoyage automatique.

## Restauration de fichiers à partir du dossier Corbeille {#restoring-assets-from-the-trash-folder}

N’importe quelle personne est autorisée à restaurer des fichiers du dossier Corbeille. Les fichiers restaurés sont placés dans leurs dossiers d’origine. Si ces dossiers n’existent plus, Dynamic Media Classic les recrée et les ressources restaurées sont placées dans les dossiers recréés.

Pour restaurer des ressources du dossier Corbeille dans les dossiers à partir desquels elles ont été supprimées, procédez comme suit :

1. Au bas du panneau Bibliothèque de ressources, cliquez sur l’icône **[!UICONTROL Corbeille]** pour ouvrir le dossier Corbeille.
1. Sélectionnez le ou les fichiers à restaurer.
1. Cliquez sur **[!UICONTROL Fichier]** > **[!UICONTROL Restaurer à partir de la corbeille]**.

## Suppression définitive de fichiers du dossier Corbeille {#permanently-deleting-assets-in-the-trash-folder}

Lorsque vous supprimez des fichiers du dossier Corbeille, sachez qu’ils sont définitivement supprimés. Les fichiers sont automatiquement supprimés du dossier Corbeille au bout de 7 jours.

Pour supprimer définitivement des ressources du dossier Corbeille, cliquez sur l’icône **[!UICONTROL Corbeille]**. Sur la page du dossier Corbeille, effectuez l’une des opérations suivantes :

* **Suppression de ressources individuelles**  : sélectionnez les ressources à supprimer définitivement, puis cliquez sur  **[!UICONTROL Fichier]**  >  **[!UICONTROL Vider de la corbeille]**.

* **Suppression de toutes les ressources**  - Cliquez sur  **[!UICONTROL Fichier]**  >  **[!UICONTROL Corbeille vide]**.

>[!MORELIKETHIS]
>
>* [Suppression de fichiers](moving-renaming-deleting-assets.md#delete_assets)

