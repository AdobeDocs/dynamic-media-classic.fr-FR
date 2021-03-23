---
title: Affichage, ajout et exportation de métadonnées
description: Découvrez comment vue, ajouter et exporter des métadonnées.
uuid: a5254c51-9e04-45ae-8236-3eab2925e5fc
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 5414b4f5-6e05-468c-8725-385423596342
feature: Dynamic Media Classic,Gestion des ressources,Métadonnées
role: Professionnel
translation-type: tm+mt
source-git-commit: 3def4a02eda8dc36f2811b3d4f0e870fff1994e4
workflow-type: tm+mt
source-wordcount: '2250'
ht-degree: 63%

---


# Affichage, ajout et exportation de métadonnées{#viewing-adding-and-exporting-metadata}

Vous pouvez stocker des informations spécifiques aux fichiers que vous utilisez dans Dynamic Media Classic ; ces informations sont appelées *métadonnées*. Vous pouvez utiliser des métadonnées dans Dynamic Media Classic pour organiser, rechercher, filtrer et trier vos fichiers.

Les métadonnées s’affichent dans la vue de détails, ainsi que les informations générées par Dynamic Media Classic, telles que la date de création du fichier, la date de publication et les mots-clés. Pour afficher les métadonnées, ouvrez le fichier en mode Affichage des détails et sélectionnez le panneau Métadonnées. Ensuite, saisissez ou modifier les métadonnées.

Certaines métadonnées sont intégrées directement dans un fichier. Si un fichier contient ces métadonnées, Dynamic Media Classic les télécharge automatiquement avec le fichier. Vous pouvez incorporer des métadonnées dans des fichiers source en Adobe Photoshop, InDesign, Illustrator et dans d’autres applications ; Dynamic Media Classic reconnaît ces métadonnées. Vous pouvez aussi ajouter des métadonnées à des fichiers individuels dans le panneau Métadonnées en mode Affichage des détails. Pour assurer la cohérence entre fichiers, les administrateurs créent des modèles de métadonnées qui fournissent les champs de métadonnées à remplir.

Pour plus d’informations sur les métadonnées incorporées, voir [www.adobe.com/go/learn_s7_xmp_en](https://www.adobe.com/go/learn_s7_xmp_en).

## Affichage des métadonnées {#view-metadata}

Pour vue des métadonnées d’un fichier, ouvrez le fichier dans la vue de détails, puis appuyez sur le panneau Métadonnées. Pour sélectionner un ensemble de champs de métadonnées, choisissez une option dans le menu Vue de métadonnées. Dynamic Media Classic offre ces Vues de métadonnées :

* **Affichage compact**
liste de base des valeurs.

* ****
IPTCValues telles que définies par l&#39;International Press Telecommunications Council.

* ****
XMPValues telles que définies par la plate-forme de métadonnées extensible.

Les administrateurs peuvent créer des vues de métadonnées qui apparaissent également dans le menu Vues des métadonnées. Pour plus d’informations sur la création de vues de métadonnées, voir [Vues des métadonnées](application-setup.md#metadata_views).

## Saisie manuelle de métadonnées pour un fichier  {#manually-enter-metadata-for-an-asset}

1. Ouvrez le fichier en mode Affichage des détails.
1. Ouvrez le panneau Métadonnées et effectuez une ou les deux opérations suivantes :

   * Choisissez une vue de métadonnées pour déterminer les champs de métadonnées qui apparaissent dans le panneau.
   * Choisissez une valeur prédéfinie et cliquez sur Appliquer pour remplir les champs de métadonnées avec des valeurs prédéfinies. Les administrateurs d’entreprise créent ces valeurs prédéfinies.

1. Entrez les valeurs dans le panneau Métadonnées.

>[!NOTE]
>
>Pour modifier les métadonnées de plusieurs fichiers en une seule fois, sélectionnez les fichiers en question, puis choisissez Fichier > Modifier les infos. Les modifications apportées aux métadonnées dans la fenêtre Modifier les infos s’appliquent à tous les fichiers sélectionnés.

## Ajout ou modification de mots-clés  {#add-or-edit-keywords}

Outre les métadonnées, vous pouvez utiliser des mots-clés pour faciliter la recherche et la gestion de vos fichiers.

Si vous avez ajouté des mots-clés à d’autres fichiers au cours de la session actuelle ou si vous avez supprimé des mots-clés de votre liste, ils figurent dans le tableau Suggestions de mots-clés.

1. Ouvrez le fichier en mode Affichage des détails.
1. Cliquez sur Mots-clés.
1. Pour ajouter des mots-clés, utilisez l’une des méthodes suivantes :

   * Saisissez un mot-clé dans la zone de texte, puis cliquez sur Ajouter.
   * Cliquez sur un mot-clé dans le tableau Suggestions de mots-clés.

1. Pour supprimer un mot-clé, sélectionnez-le et cliquez sur Supprimer. Le mot-clé est placé dans le tableau Suggestions de mots-clés.

>[!NOTE]
>
>Vous pouvez ajouter des mots-clés aux fichiers au fur et à mesure que vous les téléchargez vers Dynamic Media Classic. Dans la boîte de dialogue Télécharger les options de la tâche, sélectionnez l’option Métadonnées supplémentaires, puis saisissez les mots-clés. Voir [Options de téléchargement](uploading-files.md#upload_options).

## Importation de métadonnées  {#import-metadata}

Au lieu de saisir manuellement les métadonnées fichier par fichier, vous pouvez les importer pour plusieurs fichiers à partir d’un fichier délimité par des tabulations ou d’un fichier XML. Il est plus rapide de taper les métadonnées dans un fichier délimité par des tabulations ou un fichier XML que vous importez ensuite que de les saisir dans chaque fichier concerné. Sur la première ligne du fichier délimité par des tabulations, saisissez l’identifiant et le nom des champs pour lesquels vous souhaitez enregistrer des métadonnées. Sur chaque ligne suivante, saisissez l’identifiant d’un fichier suivi des valeurs de métadonnées. Les champs qui ne font pas partie du fichier délimité par des tabulations ou du fichier XML ne sont pas modifiés. Pour importer des métadonnées à partir d’un fichier XML, veillez à respecter les définitions DTD.

>[!NOTE]
>
>Vous pouvez créer un modèle de saisie des métadonnées afin de pouvoir les importer correctement dans Dynamic Media Classic. Une fois le modèle défini, vous pouvez y entrer les métadonnées (voir [Création d’un modèle de saisie des métadonnées à télécharger](viewing-adding-exporting-metadata.md#create_a_template_for_entering_metadata_to_upload)).

Vous trouverez plus d’informations sur les propriétés normalisées à l’adresse : https://www.adobe.com/devnet/xmp.html

1. Dans le panneau de navigation, sélectionnez les images auxquelles vous souhaitez ajouter des métadonnées à partir du fichier délimité par des tabulations ou du fichier XML.
1. Cliquez sur **Fichier** > **Importer les métadonnées**.
1. Dans la boîte de dialogue **Télécharger les métadonnées**, cliquez sur **Parcourir**.
1. Dans la boîte de dialogue **Sélectionnez les fichiers à télécharger**, sélectionnez le fichier XML ou délimité par des tabulations contenant les métadonnées.
1. Entrez un nom de tâche.
1. Cliquez sur **Télécharger**.

**Identification des différents types de métadonnées dans l’importation**

Gardez cela à l’esprit lors de l’identification des différents types de métadonnées à importer :

* Les champs définis par l’utilisateur sont identifiés par leur nom tel qu’ils ont été créés dans Configuration > Configuration de l’application > Métadonnées > Champs définis par l’utilisateur. Utilisez la fonctionnalité Générer un fichier pour obtenir une liste de tous les champs définis par l’utilisateur au format d’importation correct.
* Les propriétés des métadonnées XMP doivent avoir le préfixe XMP associé avant le nom (property-). Le symbole deux-points sépare le préfixe du nom. Le préfixe XMP se trouve dans Configuration > Configuration de l’application > Métadonnées > Editeur de schéma de métadonnées. Les noms techniques se trouvent dans la documentation du schéma XMP associé. XMP noms de propriétés n’apparaissent pas dans la fonction Générer un fichier.
* Les propriétés de schéma des métadonnées doivent avoir le préfixe associé avant le nom (property-). Le symbole deux-points sépare le préfixe du nom. Le préfixe et les noms de propriété sont définis dans l’Editeur de schéma de métadonnées. Les noms des propriétés du Schéma de métadonnées n’apparaissent pas dans la fonction Générer un fichier.

Par exemple : la propriété XMP pour les mots-clés est le schéma XMP « Dublin Core » avec le préfixe « dc » et « subject » est le nom XMP technique. Le préfixe et le nom XMP technique sont combinés en un nom complet de propriété « dc:subject ». Dans le format d’importation des métadonnées XML, « dc:subject » doit représenter le nom de la propriété. Dans le format d’importation délimité par des tabulations, il doit s’agir de l’en-tête de colonne.

**Importation de mots-clés**

Les mots-clés peuvent être importés en tant que liste séparée par des virgules. Si une virgule apparaît dans l’une des valeurs individuelles, elle doit être précédée d’une barre oblique inverse (\). Une barre oblique inverse littérale est l’habituelle double-barre oblique inverse (\\).

Par exemple, un fichier d’importation de métadonnées contenant la valeur «Hello\, World!,back\\slash,foo » pour « dc:subject » définit trois mots-clés XMP sur le fichier : « Hello, World! », « back\slash » et « foo ».

**Importation de fichiers XMP de métadonnées et de schémas de métadonnées**

L’importation XML n’accepte que les fichiers XML valides. Lors de l’importation de champs de Schéma de XMP ou de métadonnées, le préfixe d’espace de nommage est ajouté et se comporte ici comme un XMP-espace de nommage. Cet espace de nommage doit être déclaré. Par exemple, dans la balise de niveau supérieur.

Par exemple :

```as3
<ips> 
    <ghw_object vc_objectname="img_001" dc:subject="word1,word2" 
</ips>
```

**Importation de fichiers délimités par des tabulations de métadonnées et de schémas de métadonnées**

Le préfixe doit être ajouté à l’en-tête de colonne associé du champ d’importation.

## Importation de métadonnées (via FTP)  {#import-metadata-via-ftp}

Pour importer les métadonnées de plusieurs fichiers, saisissez les métadonnées dans un fichier délimité par des tabulations ou dans un fichier XML, puis sélectionnez l’option Traiter les fichiers de métadonnées sur l’écran de téléchargement (via FTP).

Vérifiez que les données contenues dans le fichier délimité par des tabulations ou le fichier XML sont enregistrées au bon format. Sur la première ligne, saisissez le champ de l’identifiant, suivi du nom des champs de métadonnées à modifier. Sur chaque ligne suivante, saisissez l’identifiant d’un fichier suivi des valeurs de métadonnées. Les champs qui ne font pas partie du fichier délimité par des tabulations ou du fichier XML ne sont pas modifiés.

Cliquez sur le bouton Télécharger de la barre de navigation globale. Pour importer les métadonnées, dans l’écran Tâches, sélectionnez l’onglet **[!UICONTROL Via FTP]**, puis cliquez sur **[!UICONTROL Options tâche]**. Dans la boîte de dialogue Télécharger les options de la tâche, choisissez Traiter les fichiers de métadonnées.

## Attribution d’un nouveau nom aux ID par lots à l’aide de métadonnées {#batch-rename-ids-using-metadata}

A l’aide de métadonnées importées à partir d’un fichier délimité par des tabulations ou d’un fichier XML, vous pouvez renommer les identifiants Dynamic Media Classic. Les métadonnées importées sont appliquées uniquement aux images spécifiées dans le fichier de métadonnées. Il n’est pas important que les images soient sélectionnées dans le panneau de navigation.

Pour renommer l’identifiant Dynamic Media Classic d’une image, ajoutez une colonne intitulée *newipsid* au fichier délimité par des tabulations ou ajoutez un champ appelé* new_vc_objectname* aux données XML.

Par exemple :

| ipsid | newipsid |
|--- |--- |
| testjacket_1 | Jacket_test_1 |
| testjacket_blue | Jacket_test_2 |

Le journal des tâches de la tâche de métadonnées indique les ID qui ont été renommés avec succès et ceux qui n’ont pas été renommés.

## Création d’un modèle de saisie des métadonnées à télécharger {#create-a-template-for-entering-metadata-to-upload}

Dynamic Media Classic offre une commande permettant de créer un modèle pour l’enregistrement des métadonnées. L’utilisation du modèle permet de s’assurer que les métadonnées sont enregistrées au bon format afin de pouvoir être téléchargées correctement dans Dynamic Media Classic. Pour créer un modèle à utiliser pour l’enregistrement et l’importation de métadonnées vers Dynamic Media Classic, procédez comme suit :

1. Sélectionnez les fichiers d’image comportant les champs de métadonnées à insérer dans le modèle.
1. Choisissez Fichier > Importer les métadonnées.
1. Sélectionnez Image pour le type de propriétés du fichier.
1. Dans le menu Générer un fichier, sélectionnez Modèle délimité par des onglets, Métadonnées XML du fichier ou DTD XML.
1. Cliquez sur Générer.
1. Dans la boîte de dialogue qui s’affiche, copiez les données. Elles vous serviront à créer le modèle.

## Utilisation des schémas de métadonnées {#working-with-metadata-schemas}

Un administrateur de la société peut afficher une liste de tous les schémas disponibles. Ouvrez Configuration de l’application > Métadonnées > Schéma de métadonnées.

Au départ, la liste des schémas standard globaux tels que XMP est masquée. Elle peut être affichée en utilisant la case située au bas de la liste.

L’administrateur de société peut créer un schéma personnalisé ou modifier un schéma personnalisé existant.

Vous pouvez utiliser l’Editeur de schéma de métadonnées pour exécuter les actions suivantes :

| Action | Description |
|--- |--- |
| Ajouter | Ajoute une propriété au schéma. Une boîte de dialogue modale collecte les informations suivantes : ID, libellé, structure et type de données. |
| Ajouter une valeur de choix | Ajoute un nouveau choix sélectionnable à une propriété avec la structure Choix ouvert ou Choix fermé. Toutes les valeurs de choix présentent le même type. Sélectionnez la propriété elle-même pour activer le bouton. |
| Edition | Modifiez l’étiquette d’une propriété ou d’une valeur de choix. Vous pouvez uniquement modifier l’étiquette. L’ID et les informations de type sont immuables. |
| Déplacer vers le haut / Déplacer vers le bas | L’ordre du schéma est reflété dans l’interface utilisateur. Pour modifier l’ordre, sélectionnez une propriété ou une valeur de choix et déplacez-la avec les boutons. Le glisser-déposer n’est pas pris en charge actuellement. |
| Suppression | Supprime une propriété ou une valeur de choix du schéma. Il ne supprime pas les valeurs du bloc XMP ou de la base de données. La propriété n’est plus disponible pour les Vues de métadonnées et est supprimée de la Vue Détails du fichier. Si la propriété a été publiée sur le serveur de métadonnées, effectuez une publication forcée pour supprimer les données du serveur de métadonnées destiné au public. |

Le système génère automatiquement un schéma personnalisé pour les champs définis par l’utilisateur avec le préfixe « s7udf ». Il s’agit de champs définis par l’utilisateur existants et ils sont modifiés dans leur propre section Configuration.

>[!NOTE]
>
>les modifications apportées au schéma ne modifient jamais les métadonnées de l’élément lui-même. Toutefois, elles ne sont pas visibles pour toutes les fonctionnalités Dynamic Media Classic et Serveur de métadonnées et ne peuvent pas être consultées après avoir été modifiées. De même, s’il existe des métadonnées pour un fichier, la création du schéma correspondant rend les métadonnées utilisables dans Dynamic Media Classic et le serveur de métadonnées.

L’éditeur de Schéma de métadonnées offre une méthode graphique pour ajouter ou modifier un schéma de société personnalisé dans Dynamic Media Classic. Un schéma est défini par un préfixe, un espace de noms et une liste de propriétés.

* Nom

   Nom d’IU pour le schéma. Utilisé pour identifier les propriétés dans les Vues des métadonnées et dans la Recherche avancée. Similaire aux sections XMP telles que Basic, IPTC, PDF.

* Préfixe

   Identificateur unique technique pour le schéma. Limité aux lettres a-z et A-Z. Le préfixe n’est pas visible dans l’interface utilisateur de Dynamic Media Classic, mais il est utilisé lorsque les métadonnées d’un fichier sont stockées dans le bloc XMP et la base de données. Le préfixe est utilisé pour identifier de manière unique les champs de métadonnées dans les recherches de métadonnées sur le serveur de métadonnées ou lors de l’importation.

* Espace de noms

   Identificateur unique technique du schéma, généralement une URL sous la forme `https://your.company.com/name/version/`. Consultez la liste des schémas standard pour obtenir des exemples. L’espace de nommage n’est pas visible dans l’interface utilisateur de Dynamic Media Classic, mais il est utilisé pour stocker les métadonnées dans le bloc XMP.

* Description

   Description libre du schéma.

>[!NOTE]
>
>le préfixe et l’espace de noms ne peuvent pas être modifiés. Pour modifier ces propriétés, vous devez supprimer et recréer le schéma.

Les propriétés décrivent les métadonnées pouvant être stockées avec ce schéma dans le bloc XMP. Une propriété se compose des éléments suivants :

| Propriété | Description |
|--- |--- |
| ID | Identificateur technique pour cette propriété. L’ID n’est pas visible dans l’interface utilisateur de Dynamic Media Classic, mais il est utilisé lorsque les métadonnées d’un fichier sont stockées dans le bloc XMP et la base de données. L’ID est utilisé pour créer des requêtes de recherche sur le Serveur de métadonnées. L’ID est soumis à certaines restrictions telles que : <ul><li>Aucun espace</li><li>Pas de &quot;.&quot;, &quot;:&quot;, &quot;$&quot;</li><li>Pas de nombre en premier caractère</li><li>Il est conseillé d’utiliser une lettre a-z ou A-Z comme premier caractère</li></ul> <br>Une fois créé, l’ID ne peut pas être modifié. |
| Etiquette | Nom d’IU pour cette propriété. |
| Structure | Détermine le type de la propriété ainsi que le type de données. La structure peut avoir l’une des valeurs suivantes :<ul><li>Type simple : valeur unique de type de données</li><li>Séquence : une liste de valeurs du même type de données</li><li>Choix ouvert : sélectionnez un élément à partir d’une liste de valeurs prédéfinies, ou saisissez du texte libre. Peut uniquement être de type Chaîne ou Entier</li><li>Choix fermé : sélectionnez un élément dans une liste de valeurs prédéfinies (une fenêtre contextuelle ou une zone combinée)</li></ul> |
| Type de données | Sélectionnez parmi ces types disponibles : <ul><li>Chaîne</li><li>Entier</li><li>Flottante</li><li>Oui/Non (valeur booléenne)</li><li>Date</li></ul> |


Lorsque la propriété présente la structure Choix ouvert ou Choix fermé, vous devez fournir au moins une valeur de choix. Le choix ouvert peut être modifié. Le choix fermé ne peut pas être modifié. Toutes les valeurs de choix présentent le même type de données que la propriété.

| Propriété | Description |
|--- |--- |
| ID | Identificateur technique pour cette valeur. L’ID n’est pas visible dans l’interface utilisateur de Dynamic Media Classic, mais il est utilisé lorsque les métadonnées d’un fichier sont stockées dans le bloc XMP et la base de données. L’ID est utilisé dans les requêtes de recherche sur le Serveur de métadonnées. L’ID ne doit pas contenir d’espace. Une fois créé, l’ID ne peut pas être modifié. |
| Etiquette | Nom d’IU pour cette valeur. |

>[!MORELIKETHIS]
>
>* [Paramètres prédéfinis de la visionneuse](application-setup.md#viewer_presets)
>* [Paramètres prédéfinis des métadonnées](application-setup.md#metadata_presets)

