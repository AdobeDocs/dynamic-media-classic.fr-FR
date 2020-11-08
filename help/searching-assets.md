---
title: Recherche de fichiers
seo-title: Recherche de fichiers
description: 'null'
seo-description: Découvrez comment rechercher des ressources.
uuid: 058209bc-bac4-4d5c-8261-e242a543beaf
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: effef4e7-37c5-42e2-9266-ecd026cad628
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '1407'
ht-degree: 77%

---


# Recherche de fichiers{#searching-assets}

Pour localiser des fichiers dans Dynamic Media Classic, vous pouvez vue les fichiers par type, les trier dans le panneau de navigation, lancer une recherche simple, lancer une recherche avancée et filtrer les fichiers.

>[!NOTE]
>
>L’écran Configuration personnelle contient des options de recherche. Vous pouvez, par exemple, choisir de lancer une recherche par défaut et d’y ajouter éventuellement des champs définis par l’utilisateur. Pour plus d’informations, voir [Configuration personnelle](personal-setup.md#personal_setup).

## Affichage des fichiers par type {#viewing-assets-by-type}

Pour afficher uniquement un certain type de fichiers, ouvrez le menu déroulant Afficher dans la bibliothèque de fichiers, puis choisissez un type de fichier. Seuls les fichiers du type choisi apparaissent dans la bibliothèque de fichiers.

## Tri de fichiers dans le panneau de navigation {#sorting-files-in-the-browse-panel}

Pour trier le contenu d’un dossier ou les résultats d’une recherche dans le panneau de navigation, sélectionnez le menu Tri, puis choisissez l’une des options suivantes : Nom, Taille, Type, Date de création ou Dernière modification.

Vous pouvez choisir l’option Croissant ou Décroissant pour trier les fichiers par ordre croissant ou décroissant selon les critères choisis.

En mode Affichage par liste, vous pouvez trier les fichiers en cliquant sur le nom d’une colonne.

## Recherche simple {#conducting-a-simple-search}

Utilisez le champ de recherche pour effectuer une recherche simple. Vous pouvez rechercher des objets par nom ou rechercher des objets dont les métadonnées contiennent un mot-clé. 

Pour mener une recherche simple :

1. Sélectionnez le dossier en question dans la bibliothèque de fichiers pour effectuer une recherche dans un dossier spécifique et ses sous-dossiers.
1. Cliquez sur  dans la bibliothèque de fichiers, puis choisissez une option qui décrit l’étendue de la recherche. Choisissez l’option Dans tous les fichiers et dossiers, Dans le dossier sélectionné ou Dans dossier et sous-doss. sélect.
1. Spécifiez le terme à rechercher.
1. Cliquez sur Ok ou appuyez sur Entrée.

   Les résultats de la recherche s’affichent dans le panneau de navigation. 

>[!NOTE]
>
>Dynamic Media Classic effectue le suivi des recherches. Pour lancer une seconde fois une recherche, cliquez sur le bouton Rechercher, puis choisissez le nom d’une recherche dans la partie inférieure du menu de recherche.

## Recherche avancée {#conducting-an-advanced-search}

Cliquez sur Recherche avancée dans la bibliothèque de fichiers pour effectuer une recherche à l’aide de plusieurs critères, notamment des valeurs dans les champs de métadonnées.

Configurez un ou plusieurs des critères de recherche suivants :

**Filtrer par type** de fichier Limitez votre recherche à un seul type de fichier en choisissant un type de fichier dans le menu.

**Fichiers et dossiers** Choisissez l&#39;emplacement de recherche : Dans tous les fichiers et dossiers, Dans le dossier sélectionné ou Dans dossier et sous-dossiers sélectionnés.

**Tous les états** de publication Recherchez les fichiers marqués pour publication, non marqués pour publication ou tous les fichiers.

**Conditions** Si vous spécifiez des critères de métadonnées pour la recherche, indiquez si la recherche doit correspondre à toutes les conditions (recherche TOUT) ou à toute condition (recherche OU).

**Spécifier les critères** de recherche de métadonnées Créez un ou plusieurs champs de recherche pour rechercher des métadonnées. Pour créer des champs de recherche :

1. Déroulez le menu Vues des métadonnées (situé à gauche du menu Ajouter un champ) et choisissez un type d’affichage des métadonnées. Vous pouvez choisir un affichage compact, IPTC, XMP ou tel que défini par l’administrateur.
1. Sélectionnez le menu Ajouter un champ et choisissez un nom de champ dans la liste déroulante.
1. Choisissez une option sous Contient (Contient, Ne contient pas, Commence par, Se termine par ou Est égal à).
1. Pour les champs numériques, choisissez une valeur ou entrez une plage de dates personnalisée.
1. (Facultatif) Répétez les étapes 1 à 4 pour créer d’autres champs de recherche.

Pour supprimer un champ de recherche, cliquez sur le bouton Supprimer le champ de recherche.

Cliquez sur Rechercher pour lancer la recherche. Les résultats de la recherche s’affichent dans le panneau de navigation. Vous pouvez modifier n’importe quel critère de recherche puis cliquer sur Rechercher pour lancer une nouvelle recherche.

Cliquez sur Effacer pour effacer les critères de recherche et lancer une nouvelle recherche. Lorsque vos recherches sont terminées, cliquez sur Fermer pour fermer le volet de recherche.

## Filtrage des fichiers à l’aide de métadonnées {#filter-assets-using-metadata}

Vous pouvez filtrer les fichiers dans l’onglet Filtres de la bibliothèque de fichiers. Pour ce faire, vous pouvez utiliser les métadonnées comme critères de filtre. Après sélection d’un champ de métadonnées, l’onglet Filtres répertorie toutes les valeurs de métadonnées saisies dans le champ sélectionné et le nombre de fichiers attribués à chaque valeur. Par exemple, dans une opération de filtre portant sur le champ de métadonnées Créateur, l’onglet Filtres répertorie tous les noms de tous les fichiers qui ont été saisis dans le champ de métadonnées Créateur, et pour chaque nom, le nombre de fichiers pour lesquels ce nom est utilisé. Cliquez ensuite sur une valeur de métadonnées pour afficher tous les fichiers pour lesquels cette valeur a été utilisée. Dans cet exemple, cliquez sur la valeur de métadonnées Jimmy pour afficher tous les fichiers pour lesquels Jimmy a été saisi dans le champ de métadonnées Créateur. Le filtrage par métadonnées peut porter sur plusieurs critères de filtre.

Les opérations de filtre peuvent être enregistrées afin d’être réutilisées plusieurs fois.

>[!NOTE]
>
>seuls les champs de métadonnées de la vue de métadonnées par défaut sont utilisables pour les opérations de filtre. L’écran Vues des métadonnées affiche le nom de la vue de données par défaut. 

Voir [Vues des métadonnées](application-setup.md#metadata_views).

### Exécution d’une opération de filtre {#running-a-filter-operation}

Procédez comme suit pour trouver des fichiers en filtrant leurs valeurs de métadonnées :

1. Cliquez sur l’onglet Filtres dans la bibliothèque de fichiers.

   Les critères de votre opération de filtrage précédente apparaissent dans le panneau Filtres. Chaque volet du panneau Filtres représente un champ de métadonnées. Utilisez les volets du panneau pour choisir les champs de métadonnées, et dans chaque champ, choisissez une valeur de métadonnées à utiliser pour l’opération de filtrage.

   Pour exécuter une opération de filtrage enregistrée, cliquez sur le bouton Sélectionner le paramètre prédéfini, puis choisissez le nom de l’opération à exécuter dans le menu.

   Voir [Enregistrement, réexécution et suppression d’opérations de filtrage](searching-assets.md#saving_repeating_and_deleting_filter_operations).

1. Après avoir cliqué sur le bouton Champ  d’un panneau, suivez ces instructions pour afficher le menu de filtrage et exécuter une opération de filtrage :

   **Sélectionner un champ** de métadonnées Sélectionnez le nom du champ dans le menu de filtrage.

   ***remarque **: Seuls les noms des champs de métadonnées de la Vue de métadonnées par défaut apparaissent dans le menu de filtrage.*

   Voir [Vues des métadonnées](application-setup.md#metadata_views).

   **Ajouter un champ** de métadonnées Choisissez Ajouter un panneau. Lorsque le volet apparaît dans le panneau Filtres, cliquez sur le bouton Champ et sélectionnez le nom d’un champ de métadonnées dans le menu de filtre.

   **Suppression d’un champ** de métadonnées Choisissez Supprimer ce panneau dans le menu de filtrage.

   Lorsque vous choisissez un champ de métadonnées, son panneau répertorie :

   * toutes les valeurs de métadonnées saisies dans le champ,
   * pour chaque valeur de métadonnées, le nombre de fichiers portant cette valeur.

1. Répétez l’étape 2 autant de fois que nécessaire pour répertorier tous les champs de métadonnées pour l’opération de filtre sur les panneaux.
1. Dans chaque panneau, sélectionnez une valeur de métadonnées à filtrer (pas plus d’une par panneau).

   Les fichiers qui correspondent à toutes les valeurs sélectionnées s’affichent dans le panneau de navigation.

   >[!NOTE]
   >
   >Pour ignorer temporairement un champ de l’opération de filtrage, cliquez sur l’option Tout désélectionner. Cette option se trouve en haut de chaque panneau, au-dessus des valeurs de métadonnées.

1. (Facultatif) Pour enregistrer une opération de filtre afin de l’exécuter ultérieurement, cliquez sur le bouton Sélectionner le paramètre prédéfini, choisissez l’option Enregistrer l’élément actuel en tant que nouveau paramètre prédéfini, puis saisissez un nom dans la boîte de dialogue Enregistrer.

### Enregistrement, réexécution et suppression d’opérations de filtrage {#saving-repeating-and-deleting-filter-operations}

Suivez les instructions affichées sur l’onglet Filtres pour enregistrer, réexécuter et supprimer des opérations de filtrage :

**Enregistrement d’une opération** de filtrage Cliquez sur le bouton Sélectionner le paramètre prédéfini, choisissez l’option Enregistrer l’élément actuel en tant que nouveau paramètre prédéfini, puis saisissez un nom dans la boîte de dialogue Enregistrer.

**Répétition d’une opération** de filtrage Cliquez sur le bouton Sélectionner un paramètre prédéfini et choisissez le nom d’une opération de filtrage dans le menu. Le menu répertorie les opérations de filtrage que vous avez enregistrées.

**Suppression d’une opération de filtrage à partir du menu Sélectionner le paramètre prédéfini** Exécutez l’opération de filtrage. Cliquez ensuite sur le bouton Sélectionner le paramètre prédéfini, puis choisissez l’option Supprimer le paramètre prédéfini dans le menu.

## Utilisation du serveur de métadonnées {#using-the-metadata-server}

Le serveur de métadonnées est une API publique qui permet de rechercher des fichiers par métadonnées, via des requêtes HTTP.

Pour configurer le serveur de métadonnées, cliquez sur Configuration > Configuration de l’application > Configuration de la publication > Serveur de métadonnées.

L’écran Publication sur le serveur de métadonnées apparaît. Cet écran vous permet de définir les options suivantes :

**Publication instantanée** Entraîne automatiquement toute modification des métadonnées lorsqu’elle est effectuée, y compris les nouveaux fichiers, les modifications de mots-clés, etc.

**XMP Packet** publie le XMP Packet. Ce paquet n’est pas pris en compte dans la recherche mais fournit des informations XMP à jour.

**Mots-clés** Publie vos mots-clés sur le serveur de métadonnées pour les utiliser dans les recherches.

**Champs** de publication du serveur de métadonnées Sélectionnez les champs à inclure dans les métadonnées. Cela vous permet de déterminer la quantité d’informations relatives à vos fichiers qui est accessible au public. Ces champs sont également affichés dans les vues des métadonnées, mais ils peuvent uniquement être modifiés dans le serveur de métadonnées.

Click **Publish Now** to start the job. Un message de confirmation, vous indiquant que la tâche a démarré, apparaît.

>[!MORELIKETHIS]
>
>* [Navigation - Notions élémentaires](navigation-basics.md#navigation_basics)
>* [Affichage, ajout et exportation de métadonnées](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)

