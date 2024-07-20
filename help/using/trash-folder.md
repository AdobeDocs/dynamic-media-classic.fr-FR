---
title: Gestion du dossier Corbeille
description: Découvrez comment gérer le dossier Corbeille.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: cffeec19-43fd-4a97-bdcc-df81af108ddd
topic: Content Management
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 28%

---

# Gestion du dossier Corbeille{#managing-the-trash-folder}

Les éléments que vous supprimez d’Adobe Dynamic Media Classic sont déplacés dans le dossier Corbeille . Ces éléments supprimés restent dans ce dossier pendant sept jours jusqu’à ce qu’ils soient restaurés ou supprimés définitivement. Vous pouvez examiner les éléments supprimés en sélectionnant l’icône **[!UICONTROL Corbeille]** au bas de la bibliothèque de ressources et en affichant les éléments dans la page du dossier Corbeille.

Tous les utilisateurs peuvent restaurer des objets du dossier Corbeille vers leurs dossiers d’origine. Tous les utilisateurs peuvent également vider le dossier Corbeille de tout son contenu.

La suppression d’éléments du dossier Corbeille supprime définitivement les éléments d’Adobe Dynamic Media Classic ; les éléments supprimés du dossier Corbeille ne peuvent plus être restaurés. Pour plus d’informations sur la configuration de notifications envoyées aux administrateurs d’entreprises lorsque des fichiers sont sur le point d’être supprimés automatiquement du dossier Corbeille, voir [Paramètres généraux de l’application](application-setup.md#general_settings).

>[!NOTE]
>
>Les Assets qui ont été déplacées vers le dossier Corbeille sont toujours enregistrées sur Adobe Dynamic Media Classic. Supposons, par exemple, que vous teniez de charger un fichier portant le même nom qu’un fichier supprimé dans le dossier Corbeille. Adobe Dynamic Media Classic traite la ressource que vous souhaitez charger comme une ressource en double. Dans ce cas, un numéro est ajouté à son nom.

## A propos du dossier Corbeille {#about-the-trash-folder}

Dès que vous supprimez un objet d’un dossier, cet objet est placé dans le dossier Corbeille. Voici ce qui se passe quand vous supprimez un objet et le déplacez vers le dossier Corbeille :

* Bien que l’élément soit supprimé de votre dossier Adobe Dynamic Media Classic, son identifiant ne peut pas être attribué à une autre ressource tant qu’il reste dans le dossier Corbeille. Si vous tentez de charger une ressource portant le même nom qu’un fichier dans le dossier Corbeille, Adobe Dynamic Media Classic ajoute un chiffre au nom de la ressource.
* L’objet ne peut pas être publié. Même si l’objet était marqué pour publication au moment de sa suppression, il ne sera pas publié.
* L’élément reste dans le dossier Corbeille jusqu’à ce qu’il soit restauré, que sept jours s’écoulent ou qu’une personne choisisse la commande **[!UICONTROL Vider la corbeille]** . Au bout de 7 jours, l’objet est définitivement supprimé au cours d’une opération de nettoyage automatique.

## Restauration des ressources à partir du dossier Corbeille {#restoring-assets-from-the-trash-folder}

Il n’est pas nécessaire que la personne ayant supprimé une ressource la restaure ; tout le monde peut restaurer des ressources à partir du dossier Corbeille. Les fichiers restaurés sont placés dans leurs dossiers d’origine. Si ces dossiers n’existent plus, Adobe Dynamic Media Classic les recrée et les ressources restaurées sont placées dans les dossiers recréés.

Pour restaurer des ressources du dossier Corbeille dans les dossiers à partir desquels elles ont été supprimées, procédez comme suit :

1. Au bas du panneau Bibliothèque de ressources, sélectionnez l’icône **[!UICONTROL Corbeille]** pour ouvrir le dossier Corbeille.
1. Sélectionnez la ou les ressources à restaurer.
1. Accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Restaurer à partir de la corbeille]**.

## Suppression définitive de fichiers du dossier Corbeille {#permanently-deleting-assets-in-the-trash-folder}

Lorsque vous supprimez des fichiers du dossier Corbeille, sachez qu’ils sont définitivement supprimés. Les fichiers sont automatiquement supprimés du dossier Corbeille au bout de 7 jours.

Vous pouvez supprimer définitivement des ressources du dossier Corbeille en sélectionnant l’icône **[!UICONTROL Corbeille]** . Sur la page du dossier Corbeille, effectuez l’une des opérations suivantes :

* **Suppression de ressources individuelles** : vous pouvez supprimer des ressources de manière permanente. Sélectionnez les ressources souhaitées, puis cliquez sur **[!UICONTROL Fichier]** > **[!UICONTROL Vide de la corbeille]**.

* **Suppression de toutes les ressources** : accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Corbeille vide]**.

>[!MORELIKETHIS]
>
>* [Suppression de ressources](moving-renaming-deleting-assets.md#delete_assets)
