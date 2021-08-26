---
title: Affichage, ajout et exportation de métadonnées
description: Découvrez comment afficher, ajouter et exporter des métadonnées.
uuid: a5254c51-9e04-45ae-8236-3eab2925e5fc
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 5414b4f5-6e05-468c-8725-385423596342
feature: Dynamic Media Classic,Asset Management,Metadata
role: User
exl-id: 2be50cc7-9a8b-4f7b-8ebf-18a3208654f2
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '2268'
ht-degree: 47%

---

# Affichage, ajout et exportation de métadonnées{#viewing-adding-and-exporting-metadata}

Vous pouvez stocker des informations spécifiques aux fichiers que vous utilisez dans Adobe Dynamic Media Classic ; ces informations sont appelées *metadata*. Vous pouvez utiliser des métadonnées dans Adobe Dynamic Media Classic pour organiser, rechercher, filtrer et trier vos ressources.

Les métadonnées s’affichent dans la vue Détails avec les informations générées par Adobe Dynamic Media Classic, telles que la date de création du fichier, la date de publication et les mots-clés. Pour afficher les métadonnées, ouvrez la ressource en mode Affichage des détails, puis sélectionnez le panneau Métadonnées. Vous pouvez saisir et modifier des métadonnées en mode Affichage des détails.

Certaines métadonnées sont intégrées directement dans un fichier. Si un fichier contient ces métadonnées, Adobe Dynamic Media Classic les télécharge automatiquement avec le fichier . Vous pouvez incorporer des métadonnées dans des ressources source dans Adobe Photoshop, InDesign, Illustrator et d’autres applications. Adobe Dynamic Media Classic reconnaît ces métadonnées. Vous pouvez également ajouter des métadonnées à des fichiers individuels dans le panneau Métadonnées en mode Affichage des détails. Pour assurer la cohérence entre fichiers, les administrateurs créent des modèles de métadonnées qui fournissent les champs de métadonnées à remplir.

Pour plus d’informations sur les métadonnées incorporées, voir [www.adobe.com/go/learn_s7_xmp_en](https://www.adobe.com/go/learn_s7_xmp_en).

## Affichage des métadonnées {#view-metadata}

Pour afficher les métadonnées d’une ressource, ouvrez-la dans l’affichage des détails, puis appuyez sur le panneau Métadonnées. Pour sélectionner un ensemble de champs de métadonnées, choisissez une option dans le menu Affichage des métadonnées . Adobe Dynamic Media Classic offre les vues de métadonnées suivantes :

* **Affichage réduit**  : liste de valeurs de base.

* **IPTC**  : valeurs définies par le Conseil international des télécommunications de la presse.

* **XMP**  : valeurs définies par le programme de métadonnées extensible.

Les administrateurs peuvent créer des vues de métadonnées qui apparaissent également dans le menu Vues des métadonnées.

Voir [Vues des métadonnées](application-setup.md#metadata_views) pour plus d’informations sur la création de vues de métadonnées.

## Saisie manuelle de métadonnées pour un fichier {#manually-enter-metadata-for-an-asset}

1. Ouvrez la ressource dans la vue Détails.
1. Ouvrez le panneau Métadonnées et effectuez une ou les deux opérations suivantes :

   * Choisissez une vue de métadonnées pour déterminer les champs de métadonnées qui apparaissent dans le panneau.
   * Sélectionnez une valeur prédéfinie, puis cliquez sur **[!UICONTROL Appliquer]** pour remplir les champs de métadonnées avec des valeurs prédéfinies. Les administrateurs d’entreprise créent ces valeurs prédéfinies.

1. Entrez les valeurs dans le panneau Métadonnées.

>[!NOTE]
>
>Pour modifier les métadonnées de plusieurs ressources à la fois, sélectionnez les ressources et cliquez sur **[!UICONTROL Fichier]** > **[!UICONTROL Modifier les informations]**. Les modifications apportées aux métadonnées dans la fenêtre Modifier les infos s’appliquent à tous les fichiers sélectionnés.

## Ajout ou modification de mots-clés {#add-or-edit-keywords}

Outre les métadonnées, vous pouvez utiliser des mots-clés pour faciliter la recherche et la gestion de vos ressources.

Si vous avez ajouté des mots-clés à d’autres fichiers au cours de cette session ou si vous avez supprimé des mots-clés de votre liste, ils apparaissent dans le tableau Suggestions de mots-clés .

1. Ouvrez le fichier en mode Affichage des détails.
1. Cliquez sur **[!UICONTROL Mots-clés]**.
1. Pour ajouter des mots-clés, utilisez l’une des méthodes suivantes :

   * Saisissez un mot-clé dans la zone de texte, puis cliquez sur **[!UICONTROL Ajouter]**.
   * Cliquez sur un mot-clé dans le tableau **[!UICONTROL Suggestions de mots-clés]** .

1. Pour supprimer un mot-clé, sélectionnez-le et cliquez sur **[!UICONTROL Supprimer]**. Le mot-clé est placé dans le tableau Suggestions de mots-clés.

>[!NOTE]
>
>Vous pouvez ajouter des mots-clés aux fichiers lors de leur chargement dans Adobe Dynamic Media Classic. Dans la boîte de dialogue Télécharger les options de la tâche, sélectionnez **[!UICONTROL Métadonnées supplémentaires]** et saisissez des mots-clés.
>Voir [Options de téléchargement](uploading-files.md#upload_options).

## Importation de métadonnées {#import-metadata}

Au lieu de saisir manuellement les métadonnées fichier par fichier, vous pouvez les importer pour plusieurs fichiers à partir d’un fichier délimité par des tabulations ou d’un fichier XML. Il est plus rapide de taper les métadonnées dans un fichier délimité par des tabulations ou un fichier XML que vous importez ensuite que de les saisir dans chaque fichier concerné. Sur la première ligne du fichier délimité par des tabulations, saisissez l’identifiant et le nom des champs pour lesquels vous souhaitez enregistrer des métadonnées. Sur chaque ligne suivante, saisissez l’identifiant d’un fichier suivi des valeurs de métadonnées. Les champs qui ne font pas partie du fichier délimité par des tabulations ou du fichier XML ne sont pas modifiés. Pour importer des métadonnées à partir d’un fichier XML, veillez à respecter les définitions DTD.

>[!NOTE]
>
>Vous pouvez créer un modèle pour saisir des métadonnées afin qu’elles puissent être correctement importées dans Adobe Dynamic Media Classic. Une fois le modèle défini, vous pouvez y entrer les métadonnées 
>(voir [Création d’un modèle de saisie des métadonnées à télécharger](viewing-adding-exporting-metadata.md#create_a_template_for_entering_metadata_to_upload)).

Vous trouverez plus d’informations sur les propriétés normalisées à l’adresse [Adobe XMP Centre de développement](https://www.adobe.com/devnet/xmp.html).

1. Dans le panneau de navigation, sélectionnez les images auxquelles vous souhaitez ajouter des métadonnées à partir du fichier délimité par des tabulations ou du fichier XML.
1. Cliquez sur **[!UICONTROL Fichier]** > **[!UICONTROL Importer les métadonnées]**.
1. Dans la boîte de dialogue **[!UICONTROL Télécharger les métadonnées]**, cliquez sur **[!UICONTROL Parcourir]**.
1. Dans la boîte de dialogue **[!UICONTROL Sélectionnez les fichiers à télécharger]**, sélectionnez le fichier XML ou délimité par des tabulations contenant les métadonnées.
1. Entrez un nom de tâche.
1. Cliquez sur **[!UICONTROL Télécharger]**.

### Identification des différents types de métadonnées dans l’importation

Gardez cela à l’esprit lors de l’identification des différents types de métadonnées à importer :

* Les champs définis par l’utilisateur sont identifiés par leur nom comme créés dans **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Métadonnées]** > **[!UICONTROL Champs définis par l’utilisateur]**. Utilisez la fonctionnalité Générer un fichier pour obtenir une liste de tous les champs définis par l’utilisateur au format d’importation correct.
* Les propriétés des métadonnées XMP doivent avoir le préfixe XMP associé avant le nom (property-). Le symbole deux-points sépare le préfixe du nom. Le préfixe XMP se trouve dans **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Métadonnées]** > **[!UICONTROL Schéma de métadonnées]** éditeur. Les noms techniques se trouvent dans la documentation du schéma XMP associé. Les noms des propriétés XMP n’apparaissent pas dans la fonction Générer un fichier .
* Les propriétés de schéma des métadonnées doivent avoir le préfixe associé avant le nom (property-). Le symbole deux-points sépare le préfixe du nom. Le préfixe et les noms de propriété sont définis dans l’Editeur de schéma de métadonnées. Les noms des propriétés du schéma de métadonnées n’apparaissent pas dans la fonction Générer le fichier .

Par exemple : La propriété XMP pour les mots-clés est le schéma XMP &quot;Dublin Core&quot; avec le préfixe `dc` et `subject` est le nom de la XMP technique. Le préfixe et le nom du XMP technique sont combinés dans le nom complet de la propriété `dc:subject`. Dans le format d’importation des métadonnées XML, `dc.subject` doit être le nom de la propriété. Dans le format d’importation délimité par des tabulations, il doit s’agir de l’en-tête de colonne.

### Importation de mots-clés

Les mots-clés peuvent être importés sous forme de liste séparée par des virgules. Si une virgule apparaît dans l’une des valeurs individuelles, elle doit être précédée d’une barre oblique inverse (\). Une barre oblique inverse littérale est l’habituelle double-barre oblique inverse (\\).

Par exemple, un fichier d’importation de métadonnées contenant la valeur &quot;Hello\, World!,back\\slash,foo&quot; pour `dc:subject` définit trois mots-XMP sur la ressource : &quot;Bonjour, monde !&quot; &quot;back\slash&quot; et &quot;foo&quot;.

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

Vous pouvez importer des métadonnées pour plusieurs fichiers en saisissant les métadonnées dans un fichier XML ou délimité par des tabulations et en sélectionnant **[!UICONTROL Traiter les fichiers de métadonnées]** sur la page Télécharger les options de la tâche (via l’onglet FTP).

Vérifiez que les données contenues dans le fichier délimité par des tabulations ou le fichier XML sont enregistrées au bon format. Sur la première ligne, saisissez le champ de l’identifiant, suivi du nom des champs de métadonnées à modifier. Sur chaque ligne suivante, saisissez l’identifiant d’un fichier suivi des valeurs de métadonnées. Les champs qui ne font pas partie du fichier délimité par des tabulations ou du fichier XML ne sont pas modifiés.

Sur la barre de navigation globale, cliquez sur **[!UICONTROL Télécharger]**. Pour importer les métadonnées, sur la page Télécharger, cliquez sur l’onglet **[!UICONTROL Via FTP]**, puis sur **[!UICONTROL Options de tâche]**. Dans la boîte de dialogue Télécharger les options de la tâche, cliquez sur **[!UICONTROL Traitement]**, puis cochez la case **[!UICONTROL Traiter les fichiers de métadonnées]** .

## Attribution d’un nouveau nom aux ID par lots à l’aide de métadonnées {#batch-rename-ids-using-metadata}

À l’aide de métadonnées importées à partir d’un fichier délimité par des tabulations ou d’un fichier XML, vous pouvez renommer les Dynamic Media Classic ID Adobe. Les métadonnées importées sont appliquées uniquement aux images spécifiées dans le fichier de métadonnées. Peu importe que les images soient sélectionnées dans le panneau de navigation.

Pour renommer l’identifiant Dynamic Media Classic Adobe d’une image, ajoutez une colonne intitulée *newipsid* au fichier délimité par des tabulations ou ajoutez un champ appelé `new_vc_objectname` aux données XML.

Par exemple :

| ipsid | newipsid |
|--- |--- |
| testjacket_1 | Jacket_test_1 |
| testjacket_blue | Jacket_test_2 |

Le journal des tâches de la tâche Métadonnées indique quels ID ont été renommés avec succès et lesquels ne l’ont pas été.

## Création d’un modèle de saisie des métadonnées à télécharger {#create-a-template-for-entering-metadata-to-upload}

Adobe Dynamic Media Classic propose une commande pour créer un modèle d’enregistrement des métadonnées. L’utilisation du modèle permet de s’assurer que les métadonnées sont entrées dans le bon format afin qu’elles puissent être chargées correctement dans Adobe Dynamic Media Classic. Pour créer un modèle à utiliser dans l’enregistrement et l’importation de métadonnées dans Adobe Dynamic Media Classic, procédez comme suit :

1. Sélectionnez les fichiers d’image comportant les champs de métadonnées à insérer dans le modèle.
1. Cliquez sur **[!UICONTROL Fichier]** > **[!UICONTROL Importer les métadonnées]**.
1. Pour **[!UICONTROL Type de propriétés de ressource]**, sélectionnez **[!UICONTROL Image]**.
1. Dans la liste déroulante **[!UICONTROL Générer le fichier]**, sélectionnez **[!UICONTROL Modèle délimité par des tabulations]**, **[!UICONTROL Métadonnées XML de la ressource]** ou **[!UICONTROL DTD XML]**.
1. Cliquez sur **[!UICONTROL Générer]**.
1. Dans la boîte de dialogue qui s’affiche, copiez les données. Elles vous serviront à créer le modèle.

## Utilisation des schémas de métadonnées {#working-with-metadata-schemas}

Un administrateur de la société peut afficher une liste de tous les schémas disponibles. Dans la barre de navigation globale, cliquez sur **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Métadonnées]** > **[!UICONTROL Schéma de métadonnées]**.

Au départ, la liste des schémas standard globaux tels que XMP est masquée. Elle peut être affichée en utilisant la case située au bas de la liste.

L’administrateur de l’entreprise peut créer un schéma personnalisé ou modifier un schéma personnalisé existant.

Vous pouvez utiliser l’Editeur de schéma de métadonnées pour exécuter les actions suivantes :

| Action | Description |
|--- |--- |
| Ajouter | Ajoute une propriété au schéma. Une boîte de dialogue modale collecte les informations suivantes : ID, libellé, structure et type de données. |
| Ajouter une valeur de choix | Ajoute un nouveau choix sélectionnable à une propriété avec la structure Choix ouvert ou Choix fermé. Toutes les valeurs de choix présentent le même type. Sélectionnez la propriété elle-même pour activer le bouton. |
| Edition | Modifiez l’étiquette d’une propriété ou d’une valeur de choix. Vous pouvez uniquement modifier l’étiquette. L’ID et les informations de type sont immuables. |
| Déplacer vers le haut / Déplacer vers le bas | L’ordre du schéma est reflété dans l’interface utilisateur. Pour modifier l’ordre, sélectionnez une propriété ou une valeur de choix et déplacez-la avec les boutons. Le glisser-déposer n’est actuellement pas pris en charge. |
| Suppression | Supprime une propriété ou une valeur de choix du schéma. Il ne supprime pas les valeurs du bloc XMP ni de la base de données. La propriété n’est plus disponible pour les vues de métadonnées et est supprimée de la vue Détails de la ressource. Si la propriété a été publiée sur le serveur de métadonnées, effectuez une publication forcée pour supprimer les données du serveur de métadonnées destiné au public. |

Le système génère automatiquement un schéma personnalisé pour les champs définis par l’utilisateur avec le préfixe `s7udf`. Il s’agit de champs définis par l’utilisateur existants et ils sont modifiés dans leur propre section Configuration.

>[!NOTE]
>
>les modifications apportées au schéma ne modifient jamais les métadonnées de l’élément lui-même. Toutefois, elles ne sont pas visibles pour toutes les fonctionnalités Adobe Dynamic Media Classic et Serveur de métadonnées et ne sont pas accessibles après avoir été modifiées. De même, s’il existe des métadonnées pour une ressource, la création du schéma correspondant rend les métadonnées utilisables dans Adobe Dynamic Media Classic et le serveur de métadonnées.

L’éditeur de schéma de métadonnées offre un moyen graphique d’ajouter ou de modifier un schéma d’entreprise personnalisé dans Adobe Dynamic Media Classic. Un schéma est défini par un préfixe, un espace de noms et une liste de propriétés.

* **Nom**  - Nom d’interface utilisateur du schéma. Utilisé pour identifier les propriétés dans les Vues des métadonnées et dans la Recherche avancée. Similaire aux sections XMP telles que Basic, IPTC, PDF.

* **Préfixe**  : identifiant unique technique du schéma. Limité aux lettres a-z et A-Z. Le préfixe n’est pas visible dans l’interface utilisateur d’Adobe Dynamic Media Classic, mais il est utilisé lorsque les métadonnées d’une ressource sont stockées dans le bloc XMP et dans la base de données. Le préfixe est utilisé pour identifier de manière unique les champs de métadonnées dans les recherches de métadonnées sur le serveur de métadonnées ou lors de l’importation.

* **Espace de noms**  : identifiant unique technique du schéma, généralement une URL dans le formulaire  `https://your.company.com/name/version/`. Consultez la liste des schémas standard pour obtenir des exemples. L’espace de noms n’est pas visible dans l’interface utilisateur d’Adobe Dynamic Media Classic, mais est utilisé pour stocker les métadonnées dans le bloc XMP.

* **Description**  : description libre du schéma.

>[!NOTE]
>
>le préfixe et l’espace de noms ne peuvent pas être modifiés. Pour modifier ces propriétés, vous devez supprimer et recréer le schéma.

Les propriétés décrivent les métadonnées pouvant être stockées avec ce schéma dans le bloc XMP. Une propriété se compose des éléments suivants :

| Propriété | Description |
|--- |--- |
| ID | Identificateur technique pour cette propriété. L’ID n’est pas visible dans l’interface utilisateur d’Adobe Dynamic Media Classic, mais il est utilisé lorsque les métadonnées d’une ressource sont stockées dans le bloc XMP et dans la base de données. L’ID est utilisé pour créer des requêtes de recherche sur le Serveur de métadonnées. L’ID est soumis à certaines restrictions telles que : <ul><li>Aucun espace</li><li>Pas de &quot;.&quot;, &quot;:&quot;, &quot;$&quot;</li><li>Pas de nombre en premier caractère</li><li>Il est conseillé d’utiliser une lettre a-z ou A-Z comme premier caractère</li></ul> <br>Une fois créé, l’ID ne peut pas être modifié. |
| Etiquette | Nom d’IU pour cette propriété. |
| Structure | Détermine le type de la propriété ainsi que le type de données. La structure peut avoir l’une des valeurs suivantes :<ul><li>Type simple : valeur unique de type de données</li><li>Séquence : une liste de valeurs du même type de données</li><li>Choix ouvert : sélectionnez un élément à partir d’une liste de valeurs prédéfinies, ou saisissez du texte libre. Peut uniquement être de type Chaîne ou Entier</li><li>Choix fermé : sélectionnez un élément dans une liste de valeurs prédéfinies (une fenêtre contextuelle ou une zone combinée)</li></ul> |
| Type de données | Sélectionnez parmi ces types disponibles : <ul><li>Chaîne</li><li>Entier</li><li>Flottante</li><li>Oui/Non (valeur booléenne)</li><li>Date</li></ul> |

Lorsque la propriété présente la structure Choix ouvert ou Choix fermé, vous devez fournir au moins une valeur de choix. Le choix ouvert peut être modifié. Le choix fermé ne peut pas être modifié. Toutes les valeurs de choix présentent le même type de données que la propriété.

| Propriété | Description |
|--- |--- |
| ID | Identificateur technique pour cette valeur. L’ID n’est pas visible dans l’interface utilisateur d’Adobe Dynamic Media Classic, mais il est utilisé lorsque les métadonnées d’une ressource sont stockées dans le bloc XMP et dans la base de données. L’ID est utilisé dans les requêtes de recherche sur le Serveur de métadonnées. L’ID ne doit pas contenir d’espace. Une fois créé, l’ID ne peut pas être modifié. |
| Etiquette | Nom d’IU pour cette valeur. |

>[!MORELIKETHIS]
>
>* [Paramètres prédéfinis de la visionneuse](application-setup.md#viewer_presets)
>* [Paramètres prédéfinis des métadonnées](application-setup.md#metadata_presets)

