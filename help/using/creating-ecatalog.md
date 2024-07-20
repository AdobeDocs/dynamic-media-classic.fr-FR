---
title: Créer un catalogue électronique
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

La création d’un catalogue électronique implique de classer les pages, de choisir la mise en page et de lier les pages en dessinant des zones cliquables. Elle requiert également la saisie de données de lien de survol et hypertexte. Accessoirement, vous pouvez personnaliser la table des matières afin que les utilisateurs puissent voir le nom des pages plutôt que leur numéro dans la visionneuse de catalogue électronique.

## Créer un catalogue électronique {#create}

Vous pouvez inclure des fichiers image et PDF dans votre catalogue électronique.

Lorsque vous créez un catalogue électronique, l’option **[!UICONTROL Publish après un enregistrement]** affecte l’ensemble et définit les membres de la manière suivante :

| Option &quot;Publish après un enregistrement&quot; sélectionnée avant l’enregistrement ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
| --- | --- | --- |
| Oui | Publié | Publié |
| Non | Non publié | Les membres de la visionneuse conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour créer un catalogue électronique :**

1. Utilisez l’une des méthodes suivantes pour commencer à créer votre catalogue électronique :

   * **Sélectionnez d’abord les fichiers** : dans le panneau Parcourir, sélectionnez les fichiers, puis accédez à **[!UICONTROL Build]** > **[!UICONTROL eCatalogs]**.

   * **Démarrer à partir de l’écran de catalogue électronique** : accédez à **[!UICONTROL Build]** > **[!UICONTROL eCatalogs]**. Sélectionnez un dossier dans la bibliothèque de ressources. Faites glisser des fichiers du dossier vers l’onglet Ordre des pages de la page Catalogue électronique.

     >[!NOTE]
     >
     >pour visualiser les éléments de la bibliothèque de fichiers par nom plutôt que par miniature, sélectionnez l’option Nom pour l’affichage par défaut de la bibliothèque de fichiers dans l’écran Configuration personnelle.

1. Sélectionnez la disposition globale de votre catalogue électronique. Sélectionnez **[!UICONTROL 1 Up]** pour les pages simples, **[!UICONTROL 2 Up]** pour les planches à deux pages ou **[!UICONTROL Custom]** pour les planches de plus de deux pages. Dans la boîte de dialogue **[!UICONTROL Modifier la mise en page du catalogue électronique]**, sélectionnez les options **[!UICONTROL Toutes les plages]** et sélectionnez **[!UICONTROL OK]**.
1. Vous pouvez éventuellement modifier la mise en page de pages individuelles ou de planches en les sélectionnant, puis en choisissant le bouton **[!UICONTROL 1 Up]**, **[!UICONTROL 2 Up]** ou **[!UICONTROL Custom]** . Dans la boîte de dialogue **[!UICONTROL Modifier la mise en page du catalogue électronique]**, sélectionnez les options **[!UICONTROL Diffusions sélectionnées]** et sélectionnez **[!UICONTROL OK]**.
1. Réorganisez les pages selon vos besoins en utilisant l’une des méthodes suivantes :

   * **Glissement de page** : faites glisser une page ou une page vers un nouvel emplacement. La barre verticale indique le nouvel emplacement de la page.

   * **Bouton Déplacer vers** : sélectionnez une page ou une étendue de page, sélectionnez **[!UICONTROL Déplacer vers]**, puis choisissez la page du menu avant lequel vous souhaitez que votre page apparaisse.

   * **Séquence #** : en mode Liste, saisissez les numéros de page dans les champs de la séquence #.

1. Lorsque vous avez terminé, près du coin inférieur droit de la page, assurez-vous que **[!UICONTROL Publish after a save]** est sélectionné (par défaut).
1. Sélectionnez **[!UICONTROL Enregistrer]**.
1. Dans la boîte de dialogue Enregistrer, sélectionnez le dossier dans lequel conserver le catalogue électronique. Dans le champ Nom du fichier , saisissez le nom de la visionneuse à 360°.
1. Sélectionnez **[!UICONTROL Enregistrer]**.

   Vous pouvez prévisualiser votre catalogue électronique, après l’avoir enregistré, en sélectionnant **[!UICONTROL Aperçu]**.

## Modifier un catalogue électronique {#editing-an-ecatalog}

Que vous modifiiez un jeu publié ou non publié, l’option **[!UICONTROL Publish after a save]** affecte l’ensemble et définit ses membres de la manière suivante :

| Visionneuse déjà publiée ? | Option &quot;Publish après un enregistrement&quot; sélectionnée avant d’enregistrer votre modification ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
| --- | --- | --- | --- |
| Oui | Oui | Publié | Publié |
| Oui | Non | Publié | Les membres de visionneuse existants conservent leur état publié. Tout nouveau membre de visionneuse que vous ajoutez lors de votre modification conserve son état publié ou non publié. |
| Non | Oui | Publié | Publié |
| Non | Non | Non publié | Les membres de la visionneuse existants, ainsi que tout nouveau membre de la visionneuse que vous ajoutez lors de votre modification conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour modifier un catalogue électronique :**

1. Sélectionnez le bouton de survol **[!UICONTROL Modifier]** du catalogue électronique.
1. Apportez les modifications de votre choix.
1. Lorsque vous avez terminé les modifications, près du coin inférieur droit de la page, assurez-vous que **[!UICONTROL Publish after a save]** est sélectionné (par défaut).
1. Sélectionnez **[!UICONTROL Enregistrer]**, sélectionnez un dossier de stockage, saisissez un nom pour la visionneuse, puis sélectionnez **[!UICONTROL Enregistrer]**.

## Supprimer un catalogue électronique

Lorsque vous supprimez une visionneuse, celle-ci est placée dans la corbeille. Cependant, les membres (ou &quot;enfants&quot;) de cet ensemble ne sont pas affectés ; au lieu de cela, ils conservent chacun leur état publié ou non publié existant.

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour supprimer un catalogue électronique :**

1. En mode Affichage de la grille, Affichage par liste ou Affichage des détails, sélectionnez un ou plusieurs catalogues électroniques.
1. Dans la barre de navigation globale, accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Supprimer]** > **[!UICONTROL Supprimer]**.

## Personnalisation de la table des matières {#customizing-the-table-of-contents-toc}

Adobe Dynamic Media Classic fournit les numéros de page par défaut dans votre catalogue électronique, sous l’onglet Ordre des pages de l’écran Catalogue électronique. Pour utiliser des noms de page personnalisés, libre à vous de modifier les étiquettes de page qui composent la table des matières. Il est recommandé de renommer les pages de couverture recto (avant) et verso (arrière). Par exemple, la page de couverture frontale peut lire &quot;Couverture&quot; au lieu de &quot;Page 0-1&quot;.

Vous pouvez créer manuellement une table des matières personnalisée pour votre catalogue électronique. Vous pouvez également importer les noms de page à partir d’un fichier CSV (Mac uniquement) ou XML.

>[!NOTE]
>
>Pour restaurer les titres de page par défaut, dans l’onglet **[!UICONTROL Classer les pages]**, sélectionnez **[!UICONTROL Étiquettes de table des matières]**, puis sélectionnez **[!UICONTROL Restaurer les valeurs par défaut (toutes)]**.

### Saisie manuelle des noms de pages {#manually-entering-page-names}

Saisissez manuellement les noms de page un par un en accédant à l’onglet Ordre des pages de l’écran Catalogue électronique. Ensuite, dans le champ du numéro de page, saisissez le nom de chaque page que vous souhaitez nommer.

### Importer les noms de page {#importing-page-names}

Il est recommandé d’utiliser la méthode d’importation des noms de page si le catalogue électronique contient de nombreuses pages. Vous pouvez importer les noms à partir d’un fichier délimité par des tabulations ou d’un fichier XML.

Le libellé de la table des matières est stocké dans le champ Données utilisateur d’une image. Formatez ces données en tant que liste de `name=<value>` ` pairs separated by two question marks "??" `. Par exemple, pour définir un libellé pour un champ de table des matières nommé `tocEN`, définissez les Données utilisateur de l’image sur :

`tocEN=&lt;EN_page_label>`

Pour définir des libellés distincts pour les champs de table des matières nommés `tocEN` et `tocFR` :

`tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label>`

Pour importer le champ Données utilisateur dans un fichier délimité par des tabulations, incluez les données utilisateur du champ :

| IPSID | Données utilisateur |
| --- | --- |
| `<image_IPS_ID>` | `tocEN=<EN_page_label>??tocFR=<FR_page_label>` |

Pour importer le champ User Data dans un fichier XML, incluez l’attribut `vc_userdata` :

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

Pour importer les noms de page à partir d’un fichier XML ou délimité par des tabulations, cliquez sur le bouton **[!UICONTROL Étiquettes TOC]** et sélectionnez **[!UICONTROL Importer]**. Dans la boîte de dialogue Télécharger les métadonnées, sélectionnez **[!UICONTROL Parcourir]**, puis importez le fichier CSV (Mac uniquement) ou XML qui associe chaque page à un nom de page.
