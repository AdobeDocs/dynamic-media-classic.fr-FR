---
title: Création d’un catalogue électronique
seo-title: Création d’un catalogue électronique
description: 'null'
seo-description: Découvrez comment créer un catalogue électronique.
uuid: 2aff05c2-7052-426c-b61d-7f9091f7ace8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 28889c60-596a-40d2-85d4-f48a4f86b932
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '1005'
ht-degree: 78%

---


# Création d’un catalogue électronique{#creating-an-ecatalog}

Dans le cadre de la création d’un catalogue électronique, il convient de définir l’ordre des pages et leur disposition, puis de les lier en traçant des zones cliquables et en saisissant des données de lien hypertexte et de survol. Accessoirement, vous pouvez personnaliser la table des matières afin que les utilisateurs puissent voir le nom des pages plutôt que leur numéro dans la visionneuse de catalogue électronique.

## Création d’un catalogue électronique {#create}

Vous pouvez inclure des fichiers d’images ainsi que des fichiers PDF dans votre catalogue électronique. 

Lorsque vous créez un catalogue électronique, l’option **Publish after save** (« Publier après l’enregistrement ») affecte la visionneuse et ses membres comme suit :

| L’option « Publish after save » (« Publier après l’enregistrement ») est-elle sélectionnée avant l’enregistrement ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
|--- |--- |--- |
| Oui | Publié | Publié |
| Non | Non publié | Les membres de la visionneuse conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour créer un catalogue électronique**

1. Utilisez l’une des méthodes suivantes pour commencer à créer votre catalogue électronique :

   **Sélectionnez d’abord** les fichiers Dans le panneau de navigation, sélectionnez les fichiers, puis cliquez sur Créer > Catalogues électroniques.

   **Début de l’écran** Catalogue électronique Cliquez sur Créer > Catalogues électroniques. Sélectionnez un dossier dans la bibliothèque de fichiers, puis faites glisser son contenu vers l’onglet Ordre des pages de la page Catalogue électronique.

   ***note**: To view the items in the Asset Library by name instead of thumbnail, select the Name option for Default Asset Library View in Personal Setup. *

1. Sélectionnez la disposition globale de votre catalogue électronique. Cliquez sur le bouton 1 vignette pour des pages simples, 2 vignettes pour des planches en double page ou Personnalisé pour des planches de plus de deux pages. La boîte de dialogue Modifier la disposition du catalogue électronique s’affiche. Select the All Spreads options and click **OK**.
1. Le cas échéant, vous pouvez changer la disposition des pages individuelles ou des planches en les sélectionnant, puis en cliquant sur le bouton 1 vignette (1 haut), 2 vignettes (2 haut) ou Personnalisé. La boîte de dialogue Modifier la disposition du catalogue électronique s’affiche. Select the Selected Spreads options and click **OK**.
1. Réorganisez les pages selon vos besoins en utilisant l’une des méthodes suivantes :

   **Glissement** Faites glisser une page ou une planche vers un nouvel emplacement. La barre verticale indique le nouvel emplacement de la page.

   **Bouton** Déplacer vers : sélectionnez une page ou une planche, cliquez sur le bouton Déplacer vers, puis choisissez la page du menu qui doit précéder la page.

   **Séquence #** Dans la Vue de Liste, saisissez les numéros de page dans les champs Séquence #.

1. Une fois terminé, près de l’angle inférieur droit de la page, vérifiez que l’option **Publish after save** (« Publier après l’enregistrement ») est sélectionnée (valeur par défaut).
1. Cliquez sur **Enregistrer**.
1. Dans la boîte de dialogue Enregistrer, sélectionnez le dossier dans lequel conserver le catalogue électronique. Dans le champ Nom de fichier, saisissez le nom de la visionneuse à 360°.
1. Cliquez sur **Enregistrer**.

   Vous pouvez prévisualiser votre catalogue électronique, après l’avoir enregistré, en cliquant sur **Prévisualiser**.

## Modification d’un catalogue électronique {#editing-an-ecatalog}

Selon que vous modifiez une visionneuse publiée ou non publiée, l’option **Publish after save** (« Publier après l’enregistrement ») affecte la visionneuse et ses membres comme suit :

| Visionneuse déjà publiée ? | L’option « Publish after save » (« Publier après l’enregistrement ») est-elle sélectionnée avant l’enregistrement de votre modification ? | Etat de la visionneuse après enregistrement | Etat des membres de la visionneuse après enregistrement |
|--- |--- |--- |--- |
| Oui | Oui | Publié | Publié |
| Oui | Non | Publié | Les membres de visionneuse existants conservent leur état publié. Tous les nouveaux membres de visionneuse que vous avez ajoutés pendant votre modification conservent leur état publié ou non publié. |
| Non | Oui | Publié | Publié |
| Non | Non | Non publié | Les membres de la visionneuse existants, ainsi que tout nouveau membre de la visionneuse que vous ajoutez lors de votre modification conservent leur état publié ou non publié. |

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour modifier un catalogue électronique**

1. Cliquez sur le bouton de survol **Modifier** du catalogue électronique.
1. Apportez les modifications de votre choix.
1. Une fois les modifications terminées, près de l’angle inférieur droit de la page, vérifiez que l’option **Publish after save** (« Publier après l’enregistrement ») est sélectionnée (valeur par défaut).
1. Cliquez sur **Enregistrer**, sélectionnez un dossier de stockage, attribuez un nom à la visionneuse, puis cliquez sur **Enregistrer**.

## Suppression d’un catalogue électronique {#deleting-an-ecatalog}

Lorsque vous supprimez une visionneuse, celle-ci est placée dans la corbeille. Toutefois, les membres (ou « enfants ») de cette visionneuse ne sont pas affectés : ils conservent en fait leur état existant publié ou non publié.

Voir aussi [Manually publishing assets](publishing-files.md#manually_publishing_assets) (« Publication manuelle des fichiers ») et [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets) (« Annulation manuelle de la publication des fichiers »).

**Pour supprimer un catalogue électronique**

1. En mode Affichage de la grille, Affichage par liste ou Affichage des détails, sélectionnez un ou plusieurs catalogues électroniques.
1. Sur la barre de navigation globale, cliquez sur **Fichier** > **Supprimer** > **Supprimer**.

## Personnalisation de la table des matières {#customizing-the-table-of-contents-toc}

Dynamic Media Classic fournit les numéros de page par défaut dans votre catalogue électronique sous l’onglet Ordre des pages de l’écran Catalogue électronique. Pour utiliser des noms de page personnalisés, libre à vous de modifier les étiquettes de page qui composent la table des matières. Il est recommandé de renommer les pages de couverture recto (avant) et verso (arrière). Par exemple, la page de couverture recto peut lire &quot;Couverture&quot; au lieu de &quot;Page 0-1&quot;.

Vous pouvez créer une table des matières personnalisée pour votre catalogue électronique, manuellement ou en important le nom des pages à partir d’un fichier CSV (Mac uniquement) ou XML.

>[!NOTE]
>
>pour restaurer les titres des pages par défaut, sous l’onglet Ordre des pages, cliquez sur le bouton Etiquettes de la table des matières, puis choisissez Restaurer paramètres par défaut (tous).

### Saisie manuelle des noms de pages {#manually-entering-page-names}

Pour entrer manuellement les noms de page un par un, activez l’onglet Ordre des pages de l’écran Catalogue électronique. Cliquez ensuite dans le champ de numérotation des pages, puis entrez un nom pour chacune des pages à nommer.

### Importation des noms de page {#importing-page-names}

Il est recommandé d’utiliser la méthode d’importation des noms de page si le catalogue électronique contient de nombreuses pages. Vous pouvez importer les noms à partir d’un fichier délimité par des tabulations ou d’un fichier XML.

Le libellé de la table des matières est stocké dans le champ Données utilisateur d’une image ; formater ces données en tant que liste de `name=<value>`` pairs separated by two question marks “??” `. Par exemple, pour définir une étiquette pour un champ de table des matières nommé tocEN &quot;, définissez les données utilisateur de l’image sur :

tocEN=&lt;EN_étiquette_de_page>

Pour définir des étiquettes distinctes pour les champs des tables de matières tocEN et tocFR :

tocEN=&lt;EN_étiquette_de_page>??tocFR=&lt;FR_étiquette_de_page>

Pour importer le champ Données utilisateur dans un fichier délimité par des tabulations, ajoutez le champ userdata :

| IPSID | Userdata |
|--- |--- |
| `<image_IPS_ID>` | tocEN=&lt;EN_étiquette_de_page>??tocFR=&lt;FR_étiquette_de_page> |

Pour importer le champ Données utilisateur dans un fichier XML, ajoutez l’attribut `vc_userdata`:

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

Pour importer les noms de page à partir d’un fichier délimité par des tabulations ou d’un fichier XML, cliquez sur le bouton Etiq. tab. mat., puis choisissez Importer. La boîte de dialogue Télécharger les métadonnées s’affiche. Cliquez sur le bouton Parcourir, puis importez le fichier CSV (Mac uniquement) ou XML qui associe chaque page à un nom de page. 
