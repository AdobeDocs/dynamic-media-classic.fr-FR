---
title: Affichage, ajout et exportation de métadonnées
seo-title: Affichage, ajout et exportation de métadonnées
description: 'null'
seo-description: Découvrez comment afficher, ajouter et exporter des métadonnées.
uuid: a5254c51-9e04-45ae-8236-3eab2925e5fc
contentOwner: admin
content-type: référence
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 5414b4f5-6e05-468c-8725-385423596342
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Affichage, ajout et exportation de métadonnées{#viewing-adding-and-exporting-metadata}

Vous pouvez stocker des informations spécifiques aux fichiers que vous utilisez dans Scene7 Publishing System ; ces informations s’appellent des *métadonnées*. Vous pouvez utiliser des métadonnées dans Dynamic Media Classic pour organiser, rechercher, filtrer et trier vos fichiers.

Les métadonnées s’affichent en mode Affichage des détails avec les informations générées par Dynamic Media Classic, telles que la date de création du fichier, la date de publication et les mots-clés. Pour afficher les métadonnées, ouvrez le fichier en mode Affichage des détails et sélectionnez le panneau Métadonnées. Ensuite, saisissez ou modifier les métadonnées.

Certaines métadonnées sont intégrées directement dans un fichier. Si un fichier contient ces métadonnées, Dynamic Media Classic les télécharge automatiquement avec le fichier. Vous pouvez incorporer des métadonnées dans des fichiers source dans Adobe Photoshop, InDesign, Illustrator et d’autres applications ; Dynamic Media Classic reconnaît ces métadonnées. Vous pouvez aussi ajouter des métadonnées à des fichiers individuels dans le panneau Métadonnées en mode Affichage des détails. Pour assurer la cohérence entre fichiers, les administrateurs créent des modèles de métadonnées qui fournissent les champs de métadonnées à remplir.

For more information about embedded metadata, see [www.adobe.com/go/learn_s7_xmp_en](https://www.adobe.com/go/learn_s7_xmp_en).

## Affichage des métadonnées {#view-metadata}

Pour afficher les métadonnées d’un fichier, ouvrez le fichier en question en mode Affichage des détails, puis cliquez dans le panneau Métadonnées. Choisissez alors une option dans le menu Vues des métadonnées pour sélectionner un jeu de champs de métadonnées. Dynamic Media Classic propose les vues de métadonnées suivantes :

* **Affichage réduit** Liste de valeurs de base.

* **IPTC** Valeurs définies par le Conseil international des télécommunications de la presse.

* **Valeurs XMP** définies par la plate-forme de métadonnées extensible.

Les administrateurs peuvent créer des vues de métadonnées qui apparaissent également dans le menu Vues des métadonnées. Pour plus d’informations sur la création de vues de métadonnées, voir [Vues des métadonnées](application-setup.md#metadata_views).

## Saisie manuelle de métadonnées pour un fichier {#manually-enter-metadata-for-an-asset}

1. Ouvrez le fichier en mode Affichage des détails.
1. Ouvrez le panneau Métadonnées et effectuez une ou les deux opérations suivantes :

   * Choisissez une vue de métadonnées pour déterminer les champs de métadonnées qui apparaissent dans le panneau.
   * Choisissez une valeur prédéfinie et cliquez sur Appliquer pour remplir les champs de métadonnées avec des valeurs prédéfinies. Les administrateurs d’entreprise créent ces valeurs prédéfinies.

1. Entrez les valeurs dans le panneau Métadonnées.

>[!NOTE]
>
>Pour modifier les métadonnées de plusieurs fichiers en une seule fois, sélectionnez les fichiers en question, puis choisissez Fichier &gt; Modifier les infos. Les modifications apportées aux métadonnées dans la fenêtre Modifier les infos s’appliquent à tous les fichiers sélectionnés.

## Ajout ou modification de mots-clés {#add-or-edit-keywords}

En plus des métadonnées, vous pouvez utiliser des mots-clés pour faciliter la recherche et la gestion des fichiers.

Si vous avez ajouté des mots-clés à d’autres fichiers au cours de la session actuelle ou si vous avez supprimé des mots-clés de votre liste, ils figurent dans le tableau Suggestions de mots-clés.

1. Ouvrez le fichier en mode Affichage des détails.
1. Cliquez sur Mots-clés.
1. Pour ajouter des mots-clés, utilisez l’une des méthodes suivantes :

   * Saisissez un mot-clé dans la zone de texte, puis cliquez sur Ajouter.
   * Cliquez sur un mot-clé dans le tableau Suggestions de mots-clés.

1. Pour supprimer un mot-clé, sélectionnez-le et cliquez sur Supprimer. Le mot-clé est placé dans le tableau Suggestions de mots-clés.

>[!NOTE]
Vous pouvez ajouter des mots-clés aux fichiers au fur et à mesure que vous les téléchargez vers Dynamic Media Classic. Dans la boîte de dialogue Télécharger les options de la tâche, sélectionnez l’option Métadonnées supplémentaires, puis saisissez les mots-clés. Voir [Options de téléchargement](uploading-files.md#upload_options).

## Importation de métadonnées {#import-metadata}

Au lieu de saisir manuellement les métadonnées fichier par fichier, vous pouvez les importer pour plusieurs fichiers à partir d’un fichier délimité par des tabulations ou d’un fichier XML. Il est plus rapide de taper les métadonnées dans un fichier délimité par des tabulations ou un fichier XML que vous importez ensuite que de les saisir dans chaque fichier concerné. Sur la première ligne du fichier délimité par des tabulations, saisissez l’identifiant et le nom des champs pour lesquels vous souhaitez enregistrer des métadonnées. Sur chaque ligne suivante, saisissez l’identifiant d’un fichier suivi des valeurs de métadonnées. Les champs qui ne font pas partie du fichier délimité par des tabulations ou du fichier XML ne sont pas modifiés. Pour importer des métadonnées à partir d’un fichier XML, veillez à respecter les définitions DTD.

>[!NOTE]
vous pouvez créer un modèle de saisie des métadonnées afin d’importer les informations correctes dans Scene7 Publishing System. Une fois le modèle défini, vous pouvez y entrer les métadonnées (voir [Création d’un modèle de saisie des métadonnées à télécharger](viewing-adding-exporting-metadata.md#create_a_template_for_entering_metadata_to_upload)).

Pour plus d’informations sur les propriétés normalisées, voir : https://www.adobe.com/devnet/xmp.html

1. Dans le panneau de navigation, sélectionnez les images auxquelles vous souhaitez ajouter des métadonnées à partir du fichier délimité par des tabulations ou du fichier XML.
1. Cliquez sur **Fichier** &gt; **Importer les métadonnées**.
1. Dans la boîte de dialogue **Télécharger les métadonnées**, cliquez sur **Parcourir**.
1. Dans la boîte de dialogue **Sélectionnez les fichiers à télécharger**, sélectionnez le fichier XML ou délimité par des tabulations contenant les métadonnées.
1. Entrez un nom de tâche.
1. Cliquez sur **Télécharger**.

**Identification des différents types de métadonnées dans l’importation**

Gardez cela à l’esprit lors de l’identification des différents types de métadonnées à importer :

* Les champs définis par l’utilisateur sont identifiés par le nom qui leur a été attribué lors de la création dans Configuration &gt; Configuration de l’application &gt; Métadonnées &gt; Champs définis par l’utilisateur. Utilisez la fonctionnalité Générer un fichier pour obtenir une liste de tous les champs définis par l’utilisateur au format d’importation correct.
* Les propriétés des métadonnées XMP doivent avoir le préfixe XMP associé avant le nom (property-). Le symbole deux-points sépare le préfixe du nom. Le préfixe XMP se trouve dans Configuration &gt; Configuration de l’application &gt; Métadonnées &gt; Editeur de schéma de métadonnées. Les noms techniques se trouvent dans la documentation du schéma XMP associé. Notez que les noms des propriétés XMP n’apparaissent pas dans la fonction Générer un fichier.
* Les propriétés de schéma des métadonnées doivent avoir le préfixe associé avant le nom (property-). Le symbole deux-points sépare le préfixe du nom. Le préfixe et les noms de propriété sont définis dans l’Editeur de schéma de métadonnées. Notez que les noms des propriétés de schéma de métadonnées n’apparaissent pas dans la fonction Générer un fichier.

Par exemple : la propriété XMP pour les mots-clés est le schéma XMP « Dublin Core » avec le préfixe « dc » et « subject » est le nom XMP technique. Le préfixe et le nom XMP technique sont combinés en un nom complet de propriété « dc:subject ». Dans le format d’importation des métadonnées XML, « dc:subject » doit représenter le nom de la propriété. Dans le format d’importation délimité par tabulation, il doit représenter l’en-tête de la colonne.

**Importation de mots-clés**

Les mots-clés peuvent être importés en tant que liste séparée par des virgules. Si une virgule apparaît dans l’une des valeurs individuelles, elle doit absolument être ignorée par une barre oblique inverse (\). Une barre oblique inverse littérale est l’habituelle double-barre oblique inverse (\\).

Par exemple, un fichier d’importation de métadonnées contenant la valeur «Hello\, World!,back\\slash,foo » pour « dc:subject » définit trois mots-clés XMP sur le fichier : « Hello, World! », « back\slash » et « foo ».

**Importation de fichiers XMP de métadonnées et de schémas de métadonnées**

L’importation XML n’accepte que les fichiers XML valides. Lors de l’importation de champs XMP ou de schéma de métadonnées, le préfixe d’espace de noms est ajouté et se comporte comme un espace de noms XMP. Cet espace de noms doit être déclaré, par ex. dans la balise de niveau supérieur.

Par exemple :

```as3
<ips> 
    <ghw_object vc_objectname="img_001" dc:subject="word1,word2" 
</ips>
```

**Importation de fichiers délimités par des tabulations de métadonnées et de schémas de métadonnées**

Le préfixe doit être ajouté à l’en-tête de colonne associé du champ d’importation.

## Importation de métadonnées (via FTP) {#import-metadata-via-ftp}

Pour importer les métadonnées de plusieurs fichiers, saisissez les métadonnées dans un fichier délimité par des tabulations ou dans un fichier XML, puis sélectionnez l’option Traiter les fichiers de métadonnées sur l’écran de téléchargement (via FTP).

Vérifiez que les données contenues dans le fichier délimité par des tabulations ou le fichier XML sont enregistrées au bon format. Sur la première ligne, saisissez le champ de l’identifiant, suivi du nom des champs de métadonnées à modifier. Sur chaque ligne suivante, saisissez l’identifiant d’un fichier suivi des valeurs de métadonnées. Les champs qui ne font pas partie du fichier délimité par des tabulations ou du fichier XML ne sont pas modifiés.

Dans la barre de navigation globale, cliquez sur le bouton Télécharger. Ensuite, dans l’écran Tâches, activez l’onglet Via FTP pour importer les métadonnées. Cliquez ensuite sur Options tâche. Dans la boîte de dialogue Télécharger les options de la tâche, choisissez Traiter les fichiers de métadonnées.

## Attribution d’un nouveau nom aux ID par lots à l’aide de métadonnées {#batch-rename-ids-using-metadata}

Vous pouvez renommer des identifiants Scene7 Publishing System au moyen de métadonnées importées à partir d’un fichier délimité par des tabulations ou d’un fichier XML. Les métadonnées importées sont appliquées uniquement aux images spécifiées dans le fichier de métadonnées. Il n’est pas important que les images soient sélectionnées dans le panneau de navigation.

To rename an image’s Scene7 Publishing System ID, add a column labeled *newipsid* to the tab-delimited file, or add a field called* new_vc_objectname* to the XML data.

Par exemple :

| ipsid | newipsid |
|--- |--- |
| testjacket_1 | Jacket_test_1 |
| testjacket_blue | Jacket_test_2 |


Le rapport de la tâche concernant les métadonnées indique les ID qui ont été renommés et ceux qui ne l’ont pas été.

## Création d’un modèle de saisie des métadonnées à télécharger {#create-a-template-for-entering-metadata-to-upload}

Dynamic Media Classic propose une commande permettant de créer un modèle d’enregistrement des métadonnées. L’utilisation d’un modèle permet de s’assurer que les métadonnées sont enregistrées au bon format et qu’elles peuvent être téléchargées sans problème sur Scene7 Publishing System. Pour créer un modèle destiné à l’enregistrement et à l’importation de métadonnées vers Scene7 Publishing System, procédez comme suit :

1. Sélectionnez les fichiers d’image comportant les champs de métadonnées à insérer dans le modèle.
1. Choisissez Fichier &gt; Importer les métadonnées.
1. Sélectionnez Image pour le type de propriétés du fichier.
1. Dans le menu Générer un fichier, sélectionnez Modèle délimité par des onglets, Métadonnées XML du fichier ou DTD XML.
1. Cliquez sur Générer.
1. Dans la boîte de dialogue qui s’affiche, copiez les données. Elles vous serviront à créer le modèle.

## Utilisation des schémas de métadonnées {#working-with-metadata-schemas}

Un administrateur de la société peut afficher une liste de tous les schémas disponibles. Ouvrez Configuration de l’application &gt; Métadonnées &gt; Schéma de métadonnées.

Initialement, la liste des schémas standard globaux tels que XMP est masquée. Elle peut être affichée en utilisant la case située au bas de la liste.

L’administrateur de la société peut créer un nouveau schéma personnalisé ou modifier un schéma personnalisé existant.

Vous pouvez utiliser l’Editeur de schéma de métadonnées pour exécuter les actions suivantes :

| Action | Description |
|--- |--- |
| Ajouter | Ajoute une nouvelle propriété au schéma. Une boîte de dialogue modale collecte les informations : ID, Etiquette, Structure et Type des données. |
| Ajouter une valeur de choix | Ajoute un nouveau choix sélectionnable à une propriété avec la structure Choix ouvert ou Choix fermé. Toutes les valeurs de choix présentent le même type. Vous devez sélectionner la propriété elle-même pour activer le bouton. |
| Edition | Modifiez l’étiquette d’une propriété ou d’une valeur de choix. Vous pouvez uniquement modifier l’étiquette. L’ID et les informations de type sont immuables. |
| Déplacer vers le haut / Déplacer vers le bas | L’ordre du schéma est reflété dans l’interface utilisateur. Pour modifier l’ordre, sélectionnez une propriété ou une valeur de choix et déplacez-la avec les boutons. L’opération glisser-déposer n’est pas prise en charge pour le moment. |
| Suppression | Supprime une propriété ou une valeur de choix du schéma. Cette opération ne supprime pas les valeurs du bloc XMP ou de la base de données. La propriété n’est plus disponible pour les Vues des métadonnées et est supprimée du mode Affichage des détails du fichier. Si la propriété a été publiée sur le serveur de métadonnées, effectuez une publication de force pour supprimer les données du serveur de métadonnées accessible au public. |

Le système génère automatiquement un schéma personnalisé pour les champs définis par l’utilisateur avec le préfixe « s7udf ». Il s’agit des champs définis par l’utilisateur existants et ceux-ci peuvent être modifiés dans leur propre section de configuration.

>[!NOTE]
les modifications apportées au schéma ne modifient jamais les métadonnées de l’élément lui-même. Cependant, elles ne sont pas visibles pour tous les SPS et la fonctionnalité Serveur de métadonnées et ne sont plus accessibles après avoir été modifiées. De même, s’il existe des métadonnées pour un fichier, la création du schéma correspondant rend les métadonnées utilisables dans le SPS et le serveur de métadonnées.

L’Editeur de schéma de métadonnées offre une interface graphique pour ajouter ou modifier un schéma personnalisé dans SPS. Un schéma est défini par un préfixe, un espace de noms et une liste de propriétés.

* Nom

   Nom d’IU pour le schéma. Utilisé pour identifier les propriétés dans les Vues des métadonnées et dans la Recherche avancée. Similaire aux sections XMP telles que Basic, IPTC, PDF.

* Préfixe

   Identificateur unique technique pour le schéma. Limité à des lettres (a-z et A-Z). Le préfixe n’est pas visible dans l’interface utilisateur de SPS, mais il est utilisé lorsque des métadonnées pour un fichier sont stockées dans le bloc XMP et dans notre base de données. Le préfixe est utilisé pour identifier de manière unique les champs de métadonnées dans les recherches de métadonnées sur le serveur de métadonnées ou lors de l’importation.

* Espace de noms

   Identifiant unique technique du schéma, généralement une URL dans le formulaire `https://your.company.com/name/version/`. Consultez la liste des schémas standard pour obtenir des exemples. L’espace de noms n’est pas visible dans l’interface utilisateur de SPS, mais est utilisé pour stocker les métadonnées dans le bloc XMP.

* Description

   Description libre du schéma.

>[!NOTE]
le préfixe et l’espace de noms ne peuvent pas être modifiés. Pour modifier ces propriétés, vous devez supprimer et recréer le schéma.

Les propriétés décrivent les métadonnées pouvant être stockées avec ce schéma dans le bloc XMP. Une propriété se compose des éléments suivants :

| Propriété | Description |
|--- |--- |
| ID | Identificateur technique pour cette propriété. L’ID n’est pas visible dans l’interface utilisateur de SPS, mais est utilisé lorsque des métadonnées pour un fichier sont stockées dans le bloc XMP et dans notre base de données. L’ID est utilisé pour créer des requêtes de recherche sur le Serveur de métadonnées. L’ID est soumis à certaines restrictions telles que : <ul><li>Aucun espace</li><li>Pas de ".", ":", "$"</li><li>Pas de nombre en premier caractère</li><li>Il est conseillé d’utiliser une lettre a-z ou A-Z comme premier caractère</li></ul> <br>Une fois créé, l’ID ne peut pas être modifié. |
| Etiquette | Nom d’IU pour cette propriété. |
| Structure | Détermine le type de la propriété ainsi que le type de données. La structure peut avoir l’une des valeurs suivantes :<ul><li>Type simple : valeur unique de type de données</li><li>Séquence : une liste de valeurs du même type de données</li><li>Choix ouvert : sélectionnez un élément à partir d’une liste de valeurs prédéfinies, ou saisissez du texte libre. Peut uniquement être de type Chaîne ou Entier</li><li>Choix fermé : sélectionnez un élément dans une liste de valeurs prédéfinies (une fenêtre contextuelle ou une zone combinée)</li></ul> |
| Type de données | Sélectionnez parmi ces types disponibles : <ul><li>Chaîne</li><li>Entier</li><li>Flottante</li><li>Oui/Non (valeur booléenne)</li><li>Date</li></ul> |


Lorsque la propriété présente la structure Choix ouvert ou Choix fermé, vous devez fournir au moins une valeur de choix. Le choix ouvert peut être modifié. Le choix fermé ne peut pas être modifié. Toutes les valeurs de choix présentent le même type de données que la propriété.

| Propriété | Description |
|--- |--- |
| ID | Identificateur technique pour cette valeur. L’ID n’est pas visible dans l’interface utilisateur de SPS, mais est utilisé lorsque des métadonnées pour un fichier sont stockées dans le bloc XMP et dans la base de données. L’ID est utilisé dans les requêtes de recherche sur le Serveur de métadonnées. L’ID ne doit pas contenir d’espace. Une fois créé, l’ID ne peut pas être modifié. |
| Etiquette | Nom d’IU pour cette valeur. |

>[!MORELIKETHIS]
* [Paramètres prédéfinis de la visionneuse](application-setup.md#viewer_presets)
* [Paramètres prédéfinis des métadonnées](application-setup.md#metadata_presets)

