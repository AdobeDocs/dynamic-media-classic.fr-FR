---
title: Recherche de ressources Dynamic Media Classic
description: Découvrez comment rechercher des ressources dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 4b3f690c-7dff-4bf0-9366-085ba918fe6b
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '1513'
ht-degree: 17%

---

# Recherche de ressources dans Adobe Dynamic Media Classic{#searching-assets}

Pour localiser des ressources de fichier dans Adobe Dynamic Media Classic, vous pouvez afficher les ressources par type, les trier dans le panneau Parcourir, lancer une recherche simple, lancer une recherche avancée et filtrer les ressources.

>[!NOTE]
>
>La page Configuration personnelle offre des options pour choisir le mode de recherche. Vous pouvez, par exemple, choisir de lancer une recherche par défaut et d’y ajouter éventuellement des champs définis par l’utilisateur. Pour plus d’informations, voir [Configuration personnelle](personal-setup.md#personal_setup).

## Affichage des ressources par type {#viewing-assets-by-type}

Pour afficher uniquement les fichiers d’un certain type au fur et à mesure de votre navigation, dans la bibliothèque de ressources sur le côté gauche, dans la liste déroulante **[!UICONTROL Afficher]** , choisissez un type de fichier. Seules les ressources du type que vous avez choisi d’afficher apparaissent dans la bibliothèque de ressources.

>[!NOTE]
>
>Si le panneau Bibliothèque de ressources ne s’affiche pas sur le côté gauche, cliquez sur la flèche du triangle droit sur le côté gauche, à mi-chemin de la fenêtre Dynamic Media Classic, pour ouvrir la bibliothèque de ressources.

## Tri des fichiers dans le panneau Parcourir {#sorting-files-in-the-browse-panel}

Vous pouvez trier le contenu d’un dossier ou les résultats de recherche qui apparaissent dans le panneau Parcourir à droite. Dans la barre de navigation globale, sélectionnez **[!UICONTROL Trier]**, puis choisissez une option. Les options sont **[!UICONTROL Name]**, **[!UICONTROL Size (KB)]**, **[!UICONTROL Type]**, **[!UICONTROL Date de création]** et **[!UICONTROL Last Modified]**.

Vous pouvez également choisir **[!UICONTROL ascendant]** ou **[!UICONTROL descendant]** pour trier les ressources par ordre croissant ou décroissant selon les critères de votre choix.

En mode Liste, vous pouvez trier en sélectionnant un nom de colonne.

## Recherche simple {#conducting-a-simple-search}

Utilisez le champ Rechercher de la bibliothèque de ressources pour effectuer des recherches simples. Vous pouvez rechercher des objets par nom ou rechercher des objets dont les métadonnées contiennent un mot-clé. 

1. Dans la bibliothèque de ressources, dans le panneau **[!UICONTROL Dossiers]**, sélectionnez le dossier à rechercher dans un dossier particulier et ses sous-dossiers.
1. À gauche du champ Rechercher de la bibliothèque de ressources, sélectionnez l’icône **[!UICONTROL Loupe]** pour ouvrir la liste déroulante.
1. Dans la liste déroulante, sélectionnez une option qui décrit l’étendue de la recherche. Vous pouvez choisir **[!UICONTROL Dans tous les fichiers et dossiers]**, **[!UICONTROL Dans le dossier sélectionné]** ou **[!UICONTROL Dans le dossier et les sous-dossiers sélectionnés]**.
1. Dans le champ Rechercher , saisissez un terme à rechercher.
1. À droite du champ Rechercher, sélectionnez **[!UICONTROL Aller]** ou appuyez sur **[!UICONTROL Entrée]**.

   Les résultats de votre recherche s’affichent dans le panneau Parcourir à droite.

<!-- Does not appear to be working anymore >[!NOTE]
>
>Adobe Dynamic Media Classic tracks searches. To run a search a second time, select **[!UICONTROL Search]** and choose the name of a search at the bottom of the Search menu. -->

## Recherche avancée {#conducting-an-advanced-search}

Dans la bibliothèque de ressources, directement sous le champ Rechercher, sélectionnez **[!UICONTROL Recherche avancée]** pour effectuer une recherche à l’aide de nombreux critères, y compris des valeurs dans les champs de métadonnées.

Spécifiez l’un des critères suivants dans votre recherche avancée :

* **Filtrer par type de ressource** : limitez votre recherche à un seul type de ressource. Sélectionnez un type de ressource dans le menu.

* **Fichiers et dossiers** : choisissez l’emplacement de recherche : **[!UICONTROL Dans tous les fichiers et dossiers]**, **[!UICONTROL Dans le dossier sélectionné]** ou **[!UICONTROL Dans le dossier et les sous-dossiers sélectionnés]**.

* **Tous les états de publication** : recherchez les fichiers marqués comme prêts pour la publication, qui ne sont pas marqués comme prêts pour la publication ou tous les fichiers.

* **Conditions** : si vous spécifiez des critères de métadonnées pour la recherche, indiquez si la recherche doit correspondre à toutes les conditions (une recherche ALL) ou à n’importe quelle condition (une recherche OR).

* **Critères de recherche** : créez un ou plusieurs champs de recherche pour rechercher des métadonnées. Pour créer des champs de recherche :

   1. Dans la recherche avancée, sous l’en-tête **[!UICONTROL Critères de recherche]** et à gauche du menu **[!UICONTROL Ajouter un champ]** ), sélectionnez l’icône de flèche en forme de triangle vers le bas pour ouvrir la liste déroulante. Sélectionnez une vue de métadonnées. Vous pouvez choisir **[!UICONTROL Toutes les propriétés avec des valeurs]**, **[!UICONTROL Affichage compact]**, **[!UICONTROL IPTC]**, **[!UICONTROL Champs Publish du serveur de métadonnées]** ou **[!UICONTROL XMP]**.
   1. Sélectionnez le menu déroulant **[!UICONTROL Ajouter un champ]** et choisissez un nom de champ.
   1. Choisissez une option **[!UICONTROL Contient]** : **[!UICONTROL Contient]**, **[!UICONTROL Ne contient pas]**, **[!UICONTROL Commence par]**, **[!UICONTROL Se termine par]** ou **[!UICONTROL Est égal à]**.
   1. Pour les champs numériques, choisissez une valeur ou entrez une plage de dates personnalisée.
   1. (Facultatif) Recommencez les étapes 1 à 4 pour créer d’autres champs de recherche.

Sélectionnez l’icône **[!UICONTROL Supprimer un champ de recherche]** (cercle avec &quot;X&quot; à l’intérieur) pour supprimer le champ de recherche.

Dans le coin inférieur droit du panneau Recherche avancée, sélectionnez **[!UICONTROL Rechercher]** pour lancer votre recherche. Les résultats de la recherche s’affichent dans le panneau Parcourir à droite. Vous pouvez modifier n’importe quelle condition de recherche et sélectionner **[!UICONTROL Rechercher]** pour lancer à nouveau la recherche.

Sélectionnez **[!UICONTROL Effacer]** si vous souhaitez effacer les critères de recherche et lancer une nouvelle recherche. Sélectionnez **[!UICONTROL Fermer]** lorsque vous avez terminé la recherche pour fermer le panneau Rechercher.

## Filtrage des fichiers à l’aide de métadonnées {#filter-assets-using-metadata}

Vous pouvez filtrer les fichiers dans l’onglet Filtres de la bibliothèque de fichiers. Pour ce faire, vous pouvez utiliser les métadonnées comme critères de filtre. Après avoir choisi un champ de métadonnées sur lequel filtrer les données, l’onglet Filtres répertorie toutes les valeurs de métadonnées saisies dans le champ que vous avez choisi. Il indique également le nombre de ressources auxquelles chaque valeur a été affectée. Par exemple, dans une opération de filtrage sur le champ de métadonnées **[!UICONTROL Créateur]**, l’onglet **[!UICONTROL Filtres]** répertorie tous les noms qui ont été entrés dans le champ de métadonnées **[!UICONTROL Créateur]** pour différentes ressources. Il répertorie également pour chaque nom, le nombre de ressources affectées au nom. Sélectionnez ensuite une valeur de métadonnées pour afficher toutes les ressources auxquelles cette valeur a été affectée. Dans cet exemple, vous sélectionnez la valeur de métadonnées `Prairie Cat` pour afficher toutes les ressources dans lesquelles le nom `Prairie Cat` a été saisi dans le champ de métadonnées **[!UICONTROL Créateur]**. Le filtrage par métadonnées peut porter sur plusieurs critères de filtre.

Vous pouvez enregistrer les opérations de filtrage pour les exécuter plusieurs fois.

>[!NOTE]
>
>seuls les champs de métadonnées de la vue de métadonnées par défaut sont utilisables pour les opérations de filtre. La page Vues des métadonnées affiche le nom de la vue de métadonnées par défaut.

Voir [Vues des métadonnées](application-setup.md#metadata_views).

### Exécution d’une opération de filtrage {#running-a-filter-operation}

Pour localiser des ressources en filtrant avec leurs valeurs de métadonnées, procédez comme suit :

1. Dans la bibliothèque de ressources, sélectionnez l’onglet **[!UICONTROL Filtres]** .

   Les critères de votre opération de filtrage précédente apparaissent dans le panneau Filtres. Chaque volet du panneau Filtres représente un champ de métadonnées. Utilisez les volets du panneau pour choisir les champs de métadonnées, et dans chaque champ, choisissez une valeur de métadonnées à utiliser pour l’opération de filtrage.

   Pour exécuter une opération de filtrage que vous avez créée et enregistrée, sélectionnez **[!UICONTROL Sélectionner un paramètre prédéfini]**, puis choisissez le nom de l’opération dans le menu.

   Voir [Enregistrement, répétition et suppression des opérations de filtre](searching-assets.md#saving_repeating_and_deleting_filter_operations).

1. Cliquez sur **[!UICONTROL Champ]** dans un panneau, puis suivez ces instructions pour afficher le menu de filtrage et construire l’opération de filtrage :

   * **Choisir un champ de métadonnées** : sélectionnez le nom du champ dans le menu de filtrage.

     >[!NOTE]
     >
     >seuls les noms des champs de métadonnées contenus dans la vue de métadonnées par défaut s’affichent dans le menu de filtrage. 

     Voir [Vues des métadonnées](application-setup.md#metadata_views).

   * **Ajouter un champ de métadonnées** : sélectionnez **[!UICONTROL Ajouter un panneau]**. Une fois le panneau affiché dans le volet Filtres, sélectionnez le bouton **[!UICONTROL Champ]** et choisissez le nom d’un champ de métadonnées dans le menu de filtrage.

   * **Supprimer un champ de métadonnées** : sélectionnez **[!UICONTROL Supprimer ce panneau]** dans le menu de filtrage.

   Lorsque vous choisissez un champ de métadonnées, son panneau répertorie les éléments suivants :

   * Toutes les valeurs de métadonnées sont renseignées dans le champ .
   * pour chaque valeur de métadonnées, le nombre de fichiers portant cette valeur.

1. Répétez l’étape 2 autant de fois que nécessaire pour répertorier tous les champs de métadonnées pour l’opération de filtre sur les panneaux.
1. Dans chaque panneau, sélectionnez une valeur de métadonnées à filtrer Vous ne pouvez pas sélectionner plusieurs valeurs de métadonnées dans chaque panneau.

   Les Assets qui correspondent à toutes les valeurs que vous avez sélectionnées apparaissent dans le panneau Parcourir.

   >[!NOTE]
   >
   >Supprimez temporairement un champ de l’opération de filtrage en cliquant sur **[!UICONTROL Tout désélectionner]**. Cette option se trouve en haut de chaque panneau, au-dessus des valeurs de métadonnées.

1. (Facultatif) Pour enregistrer l’opération de filtrage et pouvoir l’exécuter ultérieurement, sélectionnez **[!UICONTROL Sélectionner un paramètre prédéfini]** > **[!UICONTROL Enregistrer actuel en tant que nouveaux paramètres prédéfinis]**, puis saisissez un nom dans la boîte de dialogue **[!UICONTROL Enregistrer]**.

### Enregistrement, répétition et suppression des opérations de filtre {#saving-repeating-and-deleting-filter-operations}

Suivez ces instructions dans l’onglet Filtres afin de pouvoir enregistrer, répéter et supprimer des opérations de filtrage :

* **Enregistrer une opération de filtre** : accédez à **[!UICONTROL Sélectionner un paramètre prédéfini]** > **[!UICONTROL Enregistrer actuel en tant que nouveaux paramètres prédéfinis]**, puis saisissez un nom dans la boîte de dialogue **[!UICONTROL Enregistrer]**.

* **Répétez une opération de filtre** : sélectionnez **[!UICONTROL Sélectionner un paramètre prédéfini]** et choisissez le nom d’une opération de filtre dans le menu. Le menu répertorie les opérations de filtrage que vous avez enregistrées.

* **Supprimer une opération de filtre du menu Sélectionner un paramètre prédéfini** : exécutez l’opération de filtrage. Ensuite, accédez à **[!UICONTROL Sélectionner le paramètre prédéfini]** > **[!UICONTROL Supprimer le paramètre prédéfini]** dans le menu.

## Utilisation du serveur de métadonnées {#using-the-metadata-server}

Le serveur de métadonnées est une API publique que vous pouvez utiliser pour rechercher des ressources par métadonnées au moyen de requêtes http.

Pour configurer le serveur de métadonnées, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Configuration de Publish]** > **[!UICONTROL Serveur de métadonnées]**.

La page Publish du serveur de métadonnées vous permet de définir les options suivantes :

* **[!UICONTROL Publish instantané]** : envoie automatiquement toutes les modifications de métadonnées lorsqu’elles sont effectuées, y compris les nouvelles ressources, les modifications de mots-clés, etc.

* **[!UICONTROL XMP Packet]** : publie le XMP Packet. Ce paquet n’est pas utilisé pour la recherche, mais fournit les XMP les plus récents.

* **[!UICONTROL Mots-clés]** : publie vos mots-clés sur le serveur de métadonnées pour les utiliser dans les recherches.

* **[!UICONTROL Champs Publish du serveur de métadonnées]** : sélectionnez les champs à inclure dans les métadonnées. Cette option vous permet de déterminer le volume d’informations disponibles sur vos ressources pour le public. Ces champs sont également affichés dans les vues des métadonnées, mais ils peuvent uniquement être modifiés dans le serveur de métadonnées.

Sélectionnez **[!UICONTROL Publish Now]** pour démarrer la tâche. Un message de confirmation, vous indiquant que la tâche a démarré, apparaît.

>[!MORELIKETHIS]
>
>* [Principes de navigation](navigation-basics.md#navigation_basics)
>* [Affichage, ajout et exportation de métadonnées](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
