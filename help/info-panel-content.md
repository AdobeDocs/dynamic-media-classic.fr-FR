---
title: Gestion du contenu du panneau Informations dans les catalogues électroniques
description: Découvrez comment gérer le contenu du panneau d’informations dans les catalogues électroniques.
uuid: 5aa634f9-0874-4bb5-a3d9-8ce4d5577941
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: be277831-77cc-4011-ae30-e75c18eec99b
feature: Dynamic Media Classic,Visionneuses,Catalogue électronique
role: Business Practitioner
exl-id: bfb9c5a4-5068-4adb-9fe2-a4ead8656289
source-git-commit: 27d9a9b9f158846b54e4318119aec9e4dc9c4c0d
workflow-type: tm+mt
source-wordcount: '862'
ht-degree: 67%

---

# Gestion du contenu du panneau Informations dans les catalogues électroniques{#managing-info-panel-content-in-ecatalogs}

Outre l’utilisation de texte de zone cliquable pour vos survols dans les catalogues électroniques, vous pouvez utiliser un panneau d’informations pour ajouter de plus grandes quantités de texte de survol, y compris des liens. Vous pouvez également gérer le panneau d’informations en utilisant la mise en cache temporisée et en planifiant des mises à jour du contenu.

Vous pouvez gérer la configuration et les données du panneau d’informations à l’aide des fonctionnalités suivantes de Dynamic Media Classic :

* Le panneau Configuration du panneau d’informations vous permet de définir le modèle utilisé pour afficher le texte du panneau, une réponse par défaut aux erreurs, ainsi que la période de mise en cache (en heures) des informations. Par ailleurs, vous pouvez préciser si les catalogues électroniques sont automatiquement publiés.
* Le panneau Source de données du panneau d’informations vous permet de spécifier un fichier CSV contenant le texte que vous souhaitez afficher dans le texte de survol du panneau d’informations, ainsi que de planifier les heures de mise à jour des informations.
* La boîte de dialogue Importer les métadonnées (accessible à partir de la vue Pages de zones) vous permet d’importer un fichier TXT délimité par des tabulations contenant les informations sur le texte de survol. Vous pouvez utiliser cette option TXT ou le panneau de source de données avec l’option de fichier CSV pour votre texte de survol.
* La vue Pages de zones propose une option permettant de prévisualiser le code XML affiché pour des zones cliquables spécifiques.

## Configuration d’un modèle de réponse pour les catalogues électroniques {#set-up-a-response-template-for-ecatalogs}

Vous pouvez sélectionner l’un des trois modèles de réponse prédéfinis pour afficher du texte dans un panneau d’informations. Ces modèles de réponse prédéfinis déterminent le mode de présentation de vos informations dans le panneau d’informations : nombre de colonnes et de lignes, police et corps de caractères, etc. Vous pouvez sélectionner un modèle prédéfini existant ou en créer un nouveau.

>[!NOTE]
>
>vous pouvez également configurer le modèle de réponse dans le paramètre prédéfini de la visionneuse. Pour utiliser le modèle de réponse dans le paramètre prédéfini de la visionneuse, ajoutez `fmt=1` à la fin de l’URL du serveur d’informations dans le paramètre prédéfini de la visionneuse.
>
>(Voir [Configuration des paramètres prédéfinis de la visionneuse de catalogue électronique](setting-ecatalog-viewer-presets.md#setting_up_ecatalog_viewer_presets).)

1. Cliquez deux fois sur votre catalogue électronique pour l’ouvrir en mode Affichage des détails.
1. Cliquez sur le panneau Configuration du panneau d’informations.
1. Sélectionnez un modèle de réponse :

   * Sélectionnez un paramètre prédéfini dans le menu Modèle de réponse. Le code XML de la conception du modèle s’affiche dans le champ Modèle utilisateur.
   * Pour créer votre propre modèle de réponse, sélectionnez **[!UICONTROL Personnalisé]**. Entrez la définition XML du modèle dans le champ Modèle utilisateur. Vous pouvez vous inspirer des modèles prédéfinis pour créer le vôtre. 

1. (Facultatif) Dans la zone Réponse par défaut, saisissez le texte que vous souhaitez afficher si Dynamic Media Classic rencontre une erreur lors de la récupération des informations pour une zone cliquable. Par exemple, si le système reçoit un nom d’entreprise et un nom de catalogue électronique, mais pas d’identificateur de survol, ce message est affiché à l’intention de l’utilisateur.
1. Dans le champ Réponse TTL, entrez le nombre d’heures d’attente avant la mise en cache des données :

   * Optez pour une valeur faible si de nombreuses mises à jour des données sont effectuées quotidiennement.
   * Optez pour une valeur élevée si les données sont relativement stables et ne nécessitent pas de mises à jour fréquentes. La valeur par défaut est de 10 heures.

1. Cliquez sur **[!UICONTROL Publier]**.

## Importation du contenu source pour le panneau Informations dans les catalogues électroniques {#import-source-content-for-the-info-panel-in-ecatalogs}

Vous pouvez utiliser un fichier CSV (valeurs délimitées par des virgules) ou TXT (valeurs délimitées par des tabulations) pour le texte source d’un panneau d’informations de catalogue électronique. Les fichiers délimités par des tabulations doivent utiliser l’encodage UTF16 (Unicode). La méthode d’importation utilisée dépend du type de fichier.

Lorsque vous effectuez la mise en forme du contenu source, n’oubliez pas les points suivants :

* Assurez-vous que les données délimitées par des virgules et des tabulations contiennent autant de colonnes que nécessaire pour le modèle de survol.
* Assurez-vous que le premier objet ou la première colonne de données correspond bien à l’identificateur de survol (associé à la valeur rollover_key des URL de zone cliquable).
* Assurez-vous que chaque élément délimité par des tabulations ou des virgules après l’identifiant est l’élément que vous souhaitez remplacer dans le modèle de réponse. Ainsi, la première colonne est remplacée par $1$, la deuxième par $2$, etc.

### Importation de contenu CSV dans des catalogues électroniques à partir d’un emplacement hébergé en externe {#import-csv-content-into-ecatalogs-from-an-externally-hosted-location}

1. Cliquez deux fois sur le catalogue électronique pour l’ouvrir en mode Affichage des détails.
1. Cliquez sur le panneau InfoPanel Datafeed .
1. Dans la zone Emplacement du fichier CSV hébergé en externe (HTTP), saisissez l’URL associée au fichier CSV. Vous pouvez coller l’URL dans ce champ ou la saisir directement.
1. (Facultatif) Indiquez l’heure de mise à jour du contenu à l’aide des menus Planifier une mise à jour, puis cliquez sur Ajouter. Vous pouvez sélectionner plusieurs heures. Chaque heure de mise à jour apparaît dans la zone Mettre à jour les durées. (Pour supprimer une heure, sélectionnez-la, puis cliquez sur Supprimer.)
1. (Facultatif) Cliquez sur M. à jour maintenant pour procéder à une mise à jour immédiate du contenu.

### Importation d’un fichier CSV ou délimité par des tabulations {#import-a-tab-delimited-or-csv-file}

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>SR changed this section 10/23/2012</p>

 -->

1. Cliquez deux fois sur le catalogue électronique pour l’ouvrir en mode Affichage des détails.
1. Cliquez sur le panneau Configuration du panneau d’informations.
1. Cliquez sur **[!UICONTROL Télécharger le contenu S7Info]**.
1. Cliquez sur **[!UICONTROL Parcourir]**, sélectionnez le fichier TXT délimité par des tabulations, le fichier CSV ou le fichier SSV que vous souhaitez utiliser, puis cliquez sur **[!UICONTROL Ouvrir]**.
1. Cliquez sur **[!UICONTROL Télécharger]**.

Dynamic Media Classic vous envoie un message électronique vous informant de la réussite ou de l’échec du transfert.

## Prévisualisation du texte de survol pour une zone cliquable {#preview-rollover-key-text-for-an-image-map}

L’écran Pages de zones vous permet de visualiser, en un tournemain, le texte du panneau d’informations pour les zones cliquables sur une page spécifique de votre catalogue électronique.

1. Cliquez sur le bouton de survol **[!UICONTROL Modifier]** du catalogue.
1. Cliquez sur **[!UICONTROL Faire correspondre les pages]**.
1. En haut du tableau sur le côté droit de l’écran, sélectionnez **[!UICONTROL Panneau d’informations]** dans le menu Afficher.

   Le texte de survol s’affiche en regard de chaque zone cliquable contenant du texte du panneau Informations.
