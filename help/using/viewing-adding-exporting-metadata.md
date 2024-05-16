---
title: Affichage, ajout et exportation de métadonnées
description: Découvrez comment afficher, ajouter et exporter des métadonnées dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management,Metadata
role: User
exl-id: 2be50cc7-9a8b-4f7b-8ebf-18a3208654f2
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '2225'
ht-degree: 34%

---

# Affichage, ajout et exportation de métadonnées{#viewing-adding-and-exporting-metadata}

Vous pouvez stocker des informations spécifiques aux fichiers que vous utilisez dans Adobe Dynamic Media Classic ; ces informations sont appelées *metadata*. Vous pouvez utiliser des métadonnées dans Adobe Dynamic Media Classic pour organiser, rechercher, filtrer et trier vos ressources.

Les métadonnées s’affichent dans la vue Détails. Il s’affiche avec les informations générées par Adobe Dynamic Media Classic. Par exemple, la date de création du fichier, la date de publication et les mots-clés. Pour afficher les métadonnées, ouvrez la ressource en mode Affichage des détails, puis sélectionnez le panneau Métadonnées. Vous pouvez saisir et modifier des métadonnées dans la vue Détails.

Certaines métadonnées sont intégrées directement dans un fichier. Si un fichier contient ces métadonnées, Adobe Dynamic Media Classic les télécharge automatiquement avec le fichier . Vous pouvez incorporer des métadonnées dans des ressources source dans Adobe Photoshop, InDesign, Illustrator et d’autres applications ; Adobe Dynamic Media Classic reconnaît ces métadonnées. Vous pouvez également ajouter des métadonnées à des fichiers individuels dans le panneau Métadonnées en mode Affichage des détails. Pour assurer la cohérence entre fichiers, les administrateurs créent des modèles de métadonnées qui fournissent les champs de métadonnées à remplir.

Pour plus d’informations sur les métadonnées incorporées, voir [Plateforme de métadonnées extensible](https://www.adobe.com/products/xmp.html).

## Affichage des métadonnées {#view-metadata}

Pour afficher les métadonnées d’une ressource, ouvrez-la dans l’affichage des détails, puis appuyez sur le panneau Métadonnées. Pour sélectionner un ensemble de champs de métadonnées, choisissez une option dans le menu Affichage des métadonnées . Adobe Dynamic Media Classic propose les vues de métadonnées suivantes :

* **Affichage réduit**: une liste de valeurs de base.

* **IPTC**: valeurs définies par le Conseil international des télécommunications de la presse.

* **XMP**: valeurs définies par le programme de métadonnées extensible.

Les administrateurs peuvent créer des vues de métadonnées Ces vues s’affichent également dans le menu Vues des métadonnées .

Voir [Vues des métadonnées](application-setup.md#metadata_views) pour plus d’informations sur la création de vues de métadonnées.

## Saisie manuelle de métadonnées pour un fichier {#manually-enter-metadata-for-an-asset}

1. Ouvrez la ressource dans la vue Détails.
1. Ouvrez le panneau Métadonnées et effectuez une ou les deux opérations suivantes :

   * Choisissez une vue de métadonnées pour déterminer les champs de métadonnées qui apparaissent dans le panneau.
   * Sélectionnez une valeur prédéfinie, puis cliquez sur **[!UICONTROL Appliquer]** pour remplir les champs de métadonnées avec des valeurs prédéfinies. Les administrateurs d’entreprise créent ces valeurs prédéfinies.

1. Saisissez les valeurs dans le panneau Métadonnées.

>[!NOTE]
>
>Pour modifier les métadonnées de plusieurs ressources à la fois, sélectionnez les ressources et accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Modifier les infos]**. Les modifications que vous avez apportées aux métadonnées dans la fenêtre Modifier les informations s’appliquent à toutes les ressources que vous avez sélectionnées.

## Ajout ou modification de mots-clés {#add-or-edit-keywords}

Outre les métadonnées, vous pouvez utiliser des mots-clés pour faciliter la recherche et la gestion de vos ressources.

Si vous avez ajouté des mots-clés à d’autres fichiers au cours de cette session ou si vous avez supprimé des mots-clés de votre liste, ils apparaissent dans le tableau Suggestions de mots-clés .

1. Ouvrez le fichier en mode Affichage des détails.
1. Sélectionner **[!UICONTROL Mots-clés]**.
1. Pour ajouter des mots-clés, utilisez l’une des méthodes suivantes :

   * Saisissez un mot-clé dans la zone de texte, puis sélectionnez **[!UICONTROL Ajouter]**.
   * Sélectionnez un mot-clé dans le **[!UICONTROL Suggestions de mots-clés]** table.

1. Pour supprimer un mot-clé, sélectionnez-le et sélectionnez **[!UICONTROL Supprimer]**. Le mot-clé est placé dans le tableau Suggestions de mots-clés.

>[!NOTE]
>
>Vous pouvez ajouter des mots-clés aux fichiers lors de leur chargement dans Adobe Dynamic Media Classic. Dans la boîte de dialogue Télécharger les options de la tâche, choisissez **[!UICONTROL Plus de métadonnées]** et saisissez des mots-clés.
>Voir [Options de téléchargement](uploading-files.md#upload_options).

## Importation de métadonnées {#import-metadata}

Au lieu de saisir manuellement les métadonnées fichier par fichier, vous pouvez les importer pour plusieurs fichiers à partir d’un fichier délimité par des tabulations ou d’un fichier XML. Il est plus rapide de taper les métadonnées dans un fichier délimité par des tabulations ou un fichier XML que vous importez ensuite que de les saisir dans chaque fichier concerné. Sur la première ligne du fichier délimité par des tabulations, saisissez l’identifiant et le nom des champs pour lesquels vous souhaitez enregistrer des métadonnées. Sur chaque ligne suivante, saisissez l’identifiant d’un fichier suivi des valeurs de métadonnées. Les champs qui ne font pas partie du fichier délimité par des tabulations ou du fichier XML ne sont pas modifiés. Pour importer des métadonnées à partir d’un fichier XML, veillez à respecter les définitions DTD.

>[!NOTE]
>
>Vous pouvez créer un modèle de saisie des métadonnées afin qu’elles puissent être correctement importées dans Adobe Dynamic Media Classic. Après avoir créé le modèle, vous pouvez l’utiliser pour saisir les métadonnées.
>(voir [Création d’un modèle de saisie des métadonnées à télécharger](viewing-adding-exporting-metadata.md#create_a_template_for_entering_metadata_to_upload)).

Vous trouverez plus d’informations sur les propriétés normalisées à l’adresse [Adobe XMP Centre de développement](https://www.adobe.com/devnet/xmp.html).

1. Dans le panneau Parcourir , sélectionnez les images auxquelles vous souhaitez ajouter des métadonnées à partir du fichier XML ou délimité par des tabulations.
1. Accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Importation de métadonnées]**.
1. Dans le **[!UICONTROL Chargement des métadonnées]** boîte de dialogue, sélectionnez **[!UICONTROL Parcourir]**.
1. Dans la boîte de dialogue **[!UICONTROL Sélectionnez les fichiers à télécharger]**, sélectionnez le fichier XML ou délimité par des tabulations contenant les métadonnées.
1. Entrez un nom de tâche.
1. Sélectionner **[!UICONTROL Télécharger]**.

### Identification des différents types de métadonnées dans l’importation

Gardez cela à l’esprit lors de l’identification des différents types de métadonnées à importer :

* Les noms des champs définis par l’utilisateur sont identifiés comme créés dans **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Métadonnées]** > **[!UICONTROL Champs définis par les utilisateurs]**. Utilisez la variable `Generate file` pour obtenir une liste de tous les champs définis par l’utilisateur dans le format d’importation correct.
* Les propriétés des métadonnées XMP doivent avoir le préfixe XMP associé avant le nom (property-). Le symbole deux-points sépare le préfixe du nom. Le préfixe XMP se trouve dans **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Métadonnées]** > **[!UICONTROL Schéma de métadonnées]** éditeur. Les noms techniques se trouvent dans la documentation du schéma XMP associé. Les noms des propriétés XMP n’apparaissent pas dans la variable `Generate file` fonction .
* Les propriétés de schéma des métadonnées doivent avoir le préfixe associé avant le nom (property-). Le symbole deux-points sépare le préfixe du nom. Le préfixe et les noms des propriétés sont définis dans l’éditeur de schéma de métadonnées. Les noms des propriétés du schéma de métadonnées n’apparaissent pas dans la variable `Generate file` fonction .

Par exemple : la propriété XMP pour les mots-clés est le schéma XMP &quot;Dublin Core&quot; avec le préfixe `dc` et `subject` est le nom de l’XMP technique. Le préfixe et le nom du XMP technique sont combinés dans la variable `dc:subject` nom complet de la propriété. Au format d&#39;import des métadonnées XML, `dc.subject` doit être le nom de la propriété. Dans le format d’importation délimité par des tabulations, il doit s’agir de l’en-tête de colonne.

### Importation de mots-clés

Les mots-clés peuvent être importés sous forme de liste séparée par des virgules. Si une virgule apparaît dans l’une des valeurs individuelles, échappez-la à l’aide d’une barre oblique inverse (\). Une barre oblique inverse littérale est l’habituelle double-barre oblique inverse (\\).

Par exemple, un fichier d’importation de métadonnées contenant la valeur `Hello\, World!,back\\slash,foo` pour `dc:subject` définit trois mots-clés XMP sur la ressource : `Hello, World!,` `back\slash,` et `foo`.

### Importation de fichiers XMP de métadonnées et de schémas de métadonnées

L’importation XML n’accepte que les fichiers XML valides. Lors de l’importation de champs de schéma XMP ou de métadonnées, le préfixe d’espace de noms est ajouté et se comporte ici comme un XMP-espace de noms. Cet espace de noms doit être déclaré. Par exemple, dans la balise de niveau supérieur.

Par exemple :

```as3
<ips> 
    <ghw_object vc_objectname="img_001" dc:subject="word1,word2" 
</ips>
```

### Importation de fichiers XMP et de métadonnées de schéma de métadonnées délimités par des onglets

Le préfixe doit être ajouté à l’en-tête de colonne associé du champ d’importation.

## Importation de métadonnées (via FTP) {#import-metadata-via-ftp}

Vous pouvez importer des métadonnées pour plusieurs fichiers. Vous saisissez les métadonnées dans un fichier XML ou délimité par des tabulations. Sélectionnez ensuite **[!UICONTROL Traitement des fichiers de métadonnées]** sur la page Télécharger les options de la tâche (onglet FTP ).

Vérifiez que les données contenues dans le fichier délimité par des tabulations ou le fichier XML sont enregistrées au bon format. Sur la première ligne, saisissez le champ de l’identifiant, suivi du nom des champs de métadonnées à modifier. Sur chaque ligne suivante, saisissez l’identifiant d’un fichier suivi des valeurs de métadonnées. Les champs qui ne font pas partie du fichier délimité par des tabulations ou du fichier XML ne sont pas modifiés.

Dans la barre de navigation globale, sélectionnez **[!UICONTROL Télécharger]**. Pour importer les métadonnées, sur la page Télécharger , sélectionnez l’option **[!UICONTROL Via FTP]** , puis sélectionnez **[!UICONTROL Options de tâche]**. Dans la boîte de dialogue Télécharger les options de la tâche, sélectionnez **[!UICONTROL Tâche]**, puis sélectionnez la variable **[!UICONTROL Traitement des fichiers de métadonnées]** .

## Attribution d’un nouveau nom aux ID par lots à l’aide de métadonnées {#batch-rename-ids-using-metadata}

Les métadonnées importées depuis un fichier délimité par des tabulations ou un fichier XML vous permettent de renommer les Adobe Dynamic Media Classic ID. Les métadonnées importées sont appliquées uniquement aux images spécifiées dans le fichier de métadonnées. Le fait que les images soient sélectionnées dans le panneau Parcourir importe peu.

Pour renommer l’Adobe Dynamic Media Classic ID d’une image, ajoutez une colonne intitulée *newipsid* dans le fichier délimité par des tabulations ou ajoutez un champ appelé `new_vc_objectname` aux données XML.

Par exemple :

| | newipsid |
| --- | --- |
| testjacket_1 | Jacket_test_1 |
| testjacket_blue | Jacket_test_2 |

Le journal des tâches de la tâche Métadonnées indique quels ID ont été renommés avec succès et lesquels ne l’ont pas été.

## Création d’un modèle de saisie des métadonnées à télécharger {#create-a-template-for-entering-metadata-to-upload}

Adobe Dynamic Media Classic propose une commande pour créer un modèle d’enregistrement des métadonnées. L’utilisation du modèle permet de s’assurer que les métadonnées sont saisies dans le bon format afin qu’elles puissent être correctement chargées dans Adobe Dynamic Media Classic. Pour créer un modèle à utiliser dans l’enregistrement et l’importation de métadonnées dans Adobe Dynamic Media Classic, procédez comme suit :

1. Sélectionnez des ressources d’image avec les champs de métadonnées que vous souhaitez pour votre modèle.
1. Accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Importation de métadonnées]**.
1. Pour le **[!UICONTROL Type de propriété de ressource]**, sélectionnez **[!UICONTROL Image]**.
1. Dans la **[!UICONTROL `Generate File`]** liste déroulante, choisissez **[!UICONTROL Modèle délimité par des tabulations]**, **[!UICONTROL Métadonnées XML de la ressource]**, ou **[!UICONTROL DTD XML]**.
1. Sélectionner **[!UICONTROL Générer]**.
1. Dans la boîte de dialogue qui s’affiche, copiez les données. Elles vous serviront à créer le modèle.

## Utilisation des schémas de métadonnées {#working-with-metadata-schemas}

Un administrateur d’entreprise peut afficher la liste de tous les schémas disponibles. Dans la barre de navigation globale, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Métadonnées]** > **[!UICONTROL Schéma de métadonnées]**.

Au départ, la liste des schémas standard globaux tels que XMP est masquée. Elle peut être affichée en utilisant la case située au bas de la liste.

L’administrateur d’entreprise peut créer un schéma personnalisé ou modifier un schéma personnalisé existant.

Vous pouvez utiliser l’Editeur de schéma de métadonnées pour exécuter les actions suivantes :

| Action | Description |
| --- | --- |
| Ajouter | Ajoute une propriété au schéma. Une boîte de dialogue modale collecte les informations : ID, Libellé, Structure et Type de données. |
| Ajouter une valeur de choix | Ajoute un nouveau choix sélectionnable à une propriété avec la structure Choix ouvert ou Choix fermé. Toutes les valeurs de choix présentent le même type. Sélectionnez la propriété elle-même pour activer le bouton. |
| Edition | Modifiez l’étiquette d’une propriété ou d’une valeur de choix. Vous pouvez uniquement modifier l’étiquette. L’ID et les informations de type sont immuables. |
| Déplacer vers le haut/Déplacer vers le bas | L’ordre du schéma est reflété dans l’interface utilisateur. Pour modifier l’ordre, sélectionnez une propriété ou une valeur de choix et déplacez-la avec les boutons. Le glisser-déposer n’est actuellement pas pris en charge. |
| Suppression | Supprime une propriété ou une valeur de choix du schéma. Il ne supprime pas les valeurs du bloc XMP ni de la base de données. La propriété n’est plus disponible pour les vues de métadonnées et est supprimée de la vue Détails de la ressource. Si la propriété a été publiée sur le serveur de métadonnées, effectuez une publication forcée pour supprimer les données du serveur de métadonnées destiné au public. |

Le système génère automatiquement un schéma personnalisé pour les champs définis par l’utilisateur avec le préfixe . `s7udf`. Le schéma se compose de champs définis par l’utilisateur existants et modifiés dans leur propre section Configuration .

>[!NOTE]
>
>les modifications apportées au schéma ne modifient jamais les métadonnées de l’élément lui-même. Toutefois, elles ne sont pas visibles pour toutes les fonctionnalités d’Adobe Dynamic Media Classic et du serveur de métadonnées et ne sont pas accessibles après avoir été modifiées. De même, s’il existe des métadonnées pour une ressource, la création du schéma correspondant rend les métadonnées utilisables dans Adobe Dynamic Media Classic et le serveur de métadonnées.

L’éditeur de schéma de métadonnées offre un moyen graphique d’ajouter ou de modifier un schéma d’entreprise personnalisé dans Adobe Dynamic Media Classic. Un préfixe, un espace de noms et une liste de propriétés définissent un schéma.

* **[!UICONTROL Nom]**: nom d’interface utilisateur du schéma. Utilisé pour identifier les propriétés dans les Vues des métadonnées et dans la Recherche avancée. Similaire aux sections XMP telles que Basic, IPTC, PDF.

* **[!UICONTROL Préfixe]**: identifiant unique technique du schéma. Limité aux lettres a-z et A-Z. Le préfixe n’est pas visible dans l’interface utilisateur d’Adobe Dynamic Media Classic, mais il est utilisé lorsque les métadonnées d’une ressource sont stockées dans le bloc XMP et dans la base de données. Le préfixe identifie de manière unique les champs de métadonnées dans les requêtes de recherche de métadonnées sur le serveur de métadonnées ou l’importation.

* **[!UICONTROL Espace de noms]**: identifiant unique technique du schéma, généralement une URL dans le formulaire. `https://your.company.com/name/version/`. Consultez la liste des schémas standard pour obtenir des exemples. L’espace de noms n’est pas visible dans l’interface utilisateur d’Adobe Dynamic Media Classic, mais est utilisé pour stocker les métadonnées dans le bloc XMP.

* **[!UICONTROL Description]**: description de forme libre du schéma.

>[!NOTE]
>
>le préfixe et l’espace de noms ne peuvent pas être modifiés. Pour modifier ces propriétés, vous devez supprimer et recréer le schéma.

Les propriétés décrivent les métadonnées pouvant être stockées avec ce schéma dans le bloc XMP. Une propriété se compose des éléments suivants :

| Propriété | Description |
| --- | --- |
| ID | Identificateur technique pour cette propriété. L’ID n’est pas visible dans l’interface utilisateur d’Adobe Dynamic Media Classic, mais il est utilisé lorsque les métadonnées d’une ressource sont stockées dans le bloc XMP et dans la base de données. L’ID est utilisé pour créer des requêtes de recherche sur le serveur de métadonnées. L’ID comporte certaines restrictions, telles que : `<ul><li>No spaces</li><li>No ".", ":", "$"</li><li>No number as first character</li><li>Best practice is to use a-z or A-Z as first character</li></ul>` <br>Une fois créé, l’ID ne peut plus être modifié. |
| Etiquette | Nom d’IU pour cette propriété. |
| Structure | Détermine le type de la propriété ainsi que le type de données. La structure peut avoir l’une des valeurs suivantes :<ul><li>Type simple : valeur unique de type de données</li><li>Séquence : une liste de valeurs du même type de données</li><li>Choix ouvert : sélectionnez un élément dans une liste de valeurs prédéfinies ou saisissez du texte. Il ne peut être de type de données que Chaîne ou Entier.</li><li>Choix fermé : sélectionnez un élément dans une liste de valeurs prédéfinies (une fenêtre contextuelle ou une zone combinée)</li></ul> |
| Type de données | Sélectionnez parmi ces types disponibles : <ul><li>Chaîne</li><li>Entier</li><li>Flottante</li><li>Oui/Non (valeur booléenne)</li><li>Date</li></ul> |

Lorsque la propriété a la structure Choix ouvert ou Choix fermé, vous devez fournir au moins une valeur de choix. Le choix ouvert peut être modifié. Le choix fermé ne peut pas être modifié. Toutes les valeurs de choix ont le type de données de la propriété .

| Propriété | Description |
| --- | --- |
| ID | Identificateur technique pour cette valeur. L’ID n’est pas visible dans l’interface utilisateur d’Adobe Dynamic Media Classic, mais il est utilisé lorsque les métadonnées d’une ressource sont stockées dans le bloc XMP et dans la base de données. L’ID est utilisé dans les requêtes de recherche sur le Serveur de métadonnées. L’ID ne doit pas contenir d’espace. Une fois créé, l’ID ne peut pas être modifié. |
| Etiquette | Nom d’IU pour cette valeur. |

>[!MORELIKETHIS]
>
>* [Paramètres prédéfinis de la visionneuse](application-setup.md#viewer_presets)
>* [Paramètres prédéfinis des métadonnées](application-setup.md#metadata_presets)
