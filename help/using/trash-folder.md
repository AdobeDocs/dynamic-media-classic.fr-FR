---
title: Gestion du dossier Corbeille
description: Découvrez comment gérer le dossier Corbeille.
uuid: 3992a5b8-1919-4924-b07d-7fb25565effd
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 553c95fc-0a41-4f06-af50-a62bc1438149
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: cffeec19-43fd-4a97-bdcc-df81af108ddd
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 31%

---

# Gestion du dossier Corbeille{#managing-the-trash-folder}

Les éléments que vous supprimez d’Adobe Dynamic Media Classic sont déplacés dans le dossier Corbeille . Les éléments supprimés restent dans ce dossier pendant sept jours jusqu’à ce qu’ils soient restaurés ou supprimés définitivement. Vous pouvez examiner les éléments supprimés en cliquant sur le bouton **[!UICONTROL Corbeille]** au bas de la bibliothèque de ressources et en affichant les éléments sur la page du dossier Corbeille.

Tous les utilisateurs peuvent restaurer des objets du dossier Corbeille vers leurs dossiers d’origine. Tous les utilisateurs peuvent également vider le dossier Corbeille de tout son contenu.

La suppression d’éléments du dossier Corbeille supprime définitivement les éléments d’Adobe Dynamic Media Classic ; les éléments supprimés du dossier Corbeille ne peuvent plus être restaurés. Pour plus d’informations sur la configuration de notifications envoyées aux administrateurs d’entreprises lorsque des fichiers sont sur le point d’être supprimés automatiquement du dossier Corbeille, voir [Paramètres généraux de l’application](application-setup.md#general_settings).

>[!NOTE]
>
>Les ressources qui ont été déplacées vers le dossier Corbeille sont toujours enregistrées sur Adobe Dynamic Media Classic. Si vous essayez de charger un fichier portant le même nom qu’un fichier supprimé dans le dossier Corbeille, Adobe Dynamic Media Classic traite la ressource que vous souhaitez charger comme une ressource en double. A ce titre, un numéro sera ajouté à son nom.

## A propos du dossier Corbeille {#about-the-trash-folder}

Dès que vous supprimez un objet d’un dossier, cet objet est placé dans le dossier Corbeille. Voici ce qui se passe quand vous supprimez un objet et le déplacez vers le dossier Corbeille :

* Bien que l’élément ait été supprimé de vos dossiers Adobe Dynamic Media Classic, son identifiant ne peut pas être attribué à une autre ressource tant qu’il reste dans le dossier Corbeille. Si vous tentez de charger une ressource portant le même nom qu’un fichier dans le dossier Corbeille, Adobe Dynamic Media Classic ajoute un chiffre au nom de la ressource.
* L’objet ne peut pas être publié. Même si l’objet était marqué pour publication au moment de sa suppression, il ne sera pas publié.
* L’élément reste dans le dossier Corbeille jusqu’à ce qu’il soit restauré, que sept jours s’écoulent ou qu’une personne choisisse le **[!UICONTROL Vider la corbeille]** . Au bout de 7 jours, l’objet est définitivement supprimé au cours d’une opération de nettoyage automatique.

## Restauration des ressources à partir du dossier Corbeille {#restoring-assets-from-the-trash-folder}

Il n’est pas nécessaire que la personne ayant supprimé une ressource la restaure ; n’importe qui peut restaurer des ressources à partir du dossier Corbeille . Les fichiers restaurés sont placés dans leurs dossiers d’origine. Si ces dossiers n’existent plus, Adobe Dynamic Media Classic les recrée et les ressources restaurées sont placées dans les dossiers recréés.

Pour restaurer des ressources du dossier Corbeille dans les dossiers à partir desquels elles ont été supprimées, procédez comme suit :

1. Au bas du panneau Bibliothèque de ressources, sélectionnez la variable **[!UICONTROL Corbeille]** pour ouvrir le dossier Corbeille.
1. Sélectionnez la ou les ressources à restaurer.
1. Accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Restaurer à partir de la corbeille]**.

## Suppression définitive de fichiers du dossier Corbeille {#permanently-deleting-assets-in-the-trash-folder}

Lorsque vous supprimez des fichiers du dossier Corbeille, sachez qu’ils sont définitivement supprimés. Les fichiers sont automatiquement supprimés du dossier Corbeille au bout de 7 jours.

Pour supprimer définitivement des ressources du dossier Corbeille, sélectionnez l’option **[!UICONTROL Corbeille]** icône . Sur la page du dossier Corbeille, effectuez l’une des opérations suivantes :

* **Suppression de ressources individuelles** - Sélectionnez les ressources à supprimer définitivement, puis accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Vide De La Corbeille]**.

* **Suppression de toutes les ressources** - Accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Corbeille vide]**.

>[!MORELIKETHIS]
>
>* [Suppression de fichiers](moving-renaming-deleting-assets.md#delete_assets)

