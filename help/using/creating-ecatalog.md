---
title: Création d’un catalogue électronique
description: Découvrez comment créer un catalogue électronique dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 51d411b2-b4bc-4cf6-afca-dd0ed0d219a1
topic: Integrations, Development
level: Experienced
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '984'
ht-degree: 30%

---

# Création d’un catalogue électronique {#creating-an-ecatalog}

La création d’un catalogue électronique implique de classer les pages, de choisir la mise en page et de lier les pages en dessinant des zones cliquables. Elle nécessite également la saisie des données de survol et de lien hypertexte. Accessoirement, vous pouvez personnaliser la table des matières afin que les utilisateurs puissent voir le nom des pages plutôt que leur numéro dans la visionneuse de catalogue électronique.

## Création d’un catalogue électronique {#create}

Vous pouvez inclure des fichiers image et des fichiers PDF dans votre catalogue électronique.

Lorsque vous créez un catalogue électronique, l’option **[!UICONTROL Publier après un enregistrement]** affecte les membres de visionneuse et de visionneuse des manières suivantes :

| L’option « Publier après un enregistrement » est-elle sélectionnée avant l’enregistrement ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
| --- | --- | --- |
| Oui | Publié | Publié |
| Non | Non publié | Les membres de la visionneuse conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour créer un catalogue électronique, procédez comme suit**

1. Utilisez l’une des méthodes suivantes pour commencer à créer votre catalogue électronique :

   * **Sélectionnez d’abord les fichiers** : dans le panneau de navigation, sélectionnez les fichiers, puis accédez à **[!UICONTROL Créer]** > **[!UICONTROL Catalogues électroniques]**.

   * **À partir de l’écran Catalogue électronique** accédez à **[!UICONTROL Créer]** > **[!UICONTROL Catalogues électroniques]**. Sélectionnez un dossier dans la bibliothèque de ressources. Faites glisser des fichiers du dossier vers l’onglet Pages de commande de la page du catalogue électronique.

     >[!NOTE]
     >
     >pour visualiser les éléments de la bibliothèque de fichiers par nom plutôt que par miniature, sélectionnez l’option Nom pour l’affichage par défaut de la bibliothèque de fichiers dans l’écran Configuration personnelle.

1. Sélectionnez la disposition globale de votre catalogue électronique. Sélectionnez **[!UICONTROL 1 vers le haut]** pour les pages simples, **[!UICONTROL 2 vers le haut]** pour les pages doubles ou **[!UICONTROL Personnalisé]** pour les pages de plus de deux pages. Dans la boîte de dialogue **[!UICONTROL Modifier la disposition du catalogue électronique]**, sélectionnez les options **[!UICONTROL Toutes les planches]** et sélectionnez **[!UICONTROL OK]**.
1. Vous pouvez éventuellement modifier la disposition de pages individuelles ou de planches à pages en les sélectionnant, puis en cliquant sur le bouton **[!UICONTROL 1 vers le haut]**, **[!UICONTROL 2 vers le haut]** ou **[!UICONTROL Personnalisé]**. Dans la boîte de dialogue **[!UICONTROL Modifier la disposition du catalogue électronique]**, sélectionnez les options **[!UICONTROL Plages de disques sélectionnées]** puis **[!UICONTROL OK]**.
1. Réorganisez les pages selon vos besoins en utilisant l’une des méthodes suivantes :

   * **Glisser** : faites glisser une page ou une planche de page vers un nouvel emplacement. La barre verticale indique le nouvel emplacement de la page.

   * **Bouton Déplacer vers** : sélectionnez une page ou une planche de page, puis sélectionnez **[!UICONTROL Déplacer vers]** et choisissez la page dans le menu qui doit précéder la page.

   * **Séquence n°** : dans la vue Liste, saisissez les numéros de page dans les champs de la séquence n°.

1. Lorsque vous avez terminé, en bas à droite de la page, assurez-vous que l’option **[!UICONTROL Publier après un enregistrement]** est sélectionnée (par défaut).
1. Sélectionnez **[!UICONTROL Enregistrer]**.
1. Dans la boîte de dialogue Enregistrer, sélectionnez le dossier dans lequel conserver le catalogue électronique. Dans le champ Nom de fichier, saisissez le nom de la visionneuse à 360°.
1. Sélectionnez **[!UICONTROL Enregistrer]**.

   Une fois enregistré, vous pouvez prévisualiser votre catalogue électronique en sélectionnant **[!UICONTROL Aperçu]**.

## Modification d’un catalogue électronique {#editing-an-ecatalog}

Que vous modifiiez une visionneuse publiée ou une visionneuse dépubliée, l’option **[!UICONTROL Publier après un enregistrement]** affecte la visionneuse et les membres de la visionneuse des manières suivantes :

| Visionneuse déjà publiée ? | L’option « Publier après un enregistrement » est-elle sélectionnée avant d’enregistrer vos modifications ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
| --- | --- | --- | --- |
| Oui | Oui | Publié | Publié |
| Oui | Non | Publié | Les membres d’ensemble existants conservent leur statut publié. Tout nouveau membre de visionneuse que vous ajoutez lors de votre modification conserve son état publié ou non publié. |
| Non | Oui | Publié | Publié |
| Non | Non | Non publié | Les membres de la visionneuse existants, ainsi que tout nouveau membre de la visionneuse que vous ajoutez lors de votre modification conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour modifier un catalogue électronique, procédez comme suit**

1. Sélectionnez le bouton de substitution du catalogue électronique **[!UICONTROL Modifier]**.
1. Apportez les modifications de votre choix.
1. Lorsque vous avez terminé la modification, en bas à droite de la page, assurez-vous que l’option **[!UICONTROL Publier après un enregistrement]** est sélectionnée (par défaut).
1. Sélectionnez **[!UICONTROL Enregistrer]**, sélectionnez un dossier de stockage, saisissez un nom pour la visionneuse, puis sélectionnez **[!UICONTROL Enregistrer]**.

## Suppression d’un catalogue électronique

Lorsque vous supprimez une visionneuse, celle-ci est placée dans la corbeille. Toutefois, les membres (ou « enfants ») de cet ensemble ne sont pas affectés. Ils conservent chacun leur état publié ou dépublié existant.

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour supprimer un catalogue électronique, procédez comme suit**

1. En mode Affichage de la grille, Affichage par liste ou Affichage des détails, sélectionnez un ou plusieurs catalogues électroniques.
1. Sur la barre de navigation globale, accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Supprimer]** > **[!UICONTROL Supprimer]**.

## Personnalisation de la table des matières {#customizing-the-table-of-contents-toc}

Adobe Dynamic Media Classic fournit les numéros de page par défaut dans votre catalogue électronique dans l’onglet Commander des pages de l’écran Catalogue électronique. Pour utiliser des noms de page personnalisés, libre à vous de modifier les étiquettes de page qui composent la table des matières. Il est recommandé de renommer les pages de couverture recto (avant) et verso (arrière). Par exemple, la page de garde peut indiquer « Couverture » au lieu de « Page 0-1 ».

Vous pouvez créer manuellement une table des matières personnalisée pour votre catalogue électronique. Vous pouvez également importer les noms de page à partir d’un fichier CSV (Mac uniquement) ou XML.

>[!NOTE]
>
>Pour restaurer les titres de page par défaut, dans l’onglet **[!UICONTROL Classer les pages]**, sélectionnez **[!UICONTROL Libellés de la table des matières]**, puis sélectionnez **[!UICONTROL Restaurer les valeurs par défaut (tous)]**.

### Saisie manuelle des noms de pages {#manually-entering-page-names}

Saisissez manuellement les noms de page un par un en accédant à l’onglet Commander des pages de l’écran Catalogue électronique. Ensuite, dans le champ numéro de page, saisissez un nom pour chaque page que vous souhaitez nommer.

### Importer les noms de page {#importing-page-names}

Il est recommandé d’utiliser la méthode d’importation des noms de page si le catalogue électronique contient de nombreuses pages. Vous pouvez importer les noms à partir d’un fichier délimité par des tabulations ou d’un fichier XML.

Le libellé de la table des matières est stocké dans le champ de données utilisateur d’une image. Mettez en forme ces données sous la forme d’une liste de `name=<value>` ` pairs separated by two question marks "??" `. Par exemple, pour définir un libellé pour un champ de table des matières nommé `tocEN`, définissez les données utilisateur de l’image sur :

`tocEN=&lt;EN_page_label>`

Pour définir des libellés distincts pour les champs de la table des matières nommés `tocEN` et `tocFR` :

`tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label>`

Pour importer le champ Données utilisateur dans un fichier délimité par des tabulations, incluez les données utilisateur du champ :

| IPSID | Données utilisateur |
| --- | --- |
| `<image_IPS_ID>` | `tocEN=<EN_page_label>??tocFR=<FR_page_label>` |

Pour importer le champ Données utilisateur dans un fichier XML, incluez l’attribut `vc_userdata` :

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

Pour importer des noms de page à partir d’un fichier XML ou délimité par des tabulations, cliquez sur le bouton **[!UICONTROL Libellés de table des matières]** puis sélectionnez **[!UICONTROL Importer]**. Dans la boîte de dialogue Charger les métadonnées, sélectionnez **[!UICONTROL Parcourir]**, puis importez le fichier CSV (Mac uniquement) ou le fichier XML qui associe chaque page à un nom de page.
