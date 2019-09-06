---
title: Gestion du contenu du panneau d'informations dans les catalogues électroniques
seo-title: Gestion du contenu du panneau d'informations dans les catalogues électroniques
description: 'null'
seo-description: Découvrez comment gérer le contenu du panneau d'informations dans les catalogues électroniques.
uuid: 5 aa 634 f 9-0874-4 bb 5-a 3 d 9-8 ce 4 d 5577941
contentOwner: admin
content-type: référence
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/ecatalogs
discoiquuid: be 277831-77 cc -4011-ae 30-e 75 c 18 eec 99 b
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Gestion du contenu du panneau d'informations dans les catalogues électroniques{#managing-info-panel-content-in-ecatalogs}

Outre l’utilisation de texte de zone cliquable pour vos survols dans les catalogues électroniques, vous pouvez utiliser un panneau d’informations pour ajouter de plus grandes quantités de texte de survol, y compris des liens. Vous pouvez également gérer le panneau d’informations en utilisant la mise en cache temporisée et en planifiant des mises à jour du contenu.

Vous pouvez gérer la configuration et les données de votre panneau d'informations à l'aide des fonctionnalités suivantes de Dynamic Media Classic :

* Le panneau Configuration du panneau d’informations vous permet de définir le modèle utilisé pour afficher le texte du panneau, une réponse par défaut aux erreurs, ainsi que la période de mise en cache (en heures) des informations. Par ailleurs, vous pouvez préciser si les catalogues électroniques sont automatiquement publiés.
* Le panneau Source de données du panneau d’informations vous permet d’indiquer un fichier CSV contenant le texte à afficher comme texte de survol du panneau d’informations, ainsi que les heures de planification de la mise à jour des informations.
* La boîte de dialogue Importer les métadonnées (accessible à partir de la vue Pages de zones) vous permet d’importer un fichier TXT délimité par des tabulations contenant les informations sur le texte de survol. Vous pouvez utiliser cette option TXT ou le panneau de source de données avec l’option de fichier CSV pour votre texte de survol.
* La vue Pages de zones propose une option permettant de prévisualiser le code XML affiché pour des zones cliquables spécifiques.

## Configuration d'un modèle de réponse pour les catalogues électroniques {#set-up-a-response-template-for-ecatalogs}

Vous pouvez sélectionner l’un des trois modèles de réponse prédéfinis pour afficher du texte dans un panneau d’informations. Ces modèles de réponse prédéfinis déterminent le mode de présentation de vos informations dans le panneau d’informations : nombre de colonnes et de lignes, police et corps de caractères, etc. Vous pouvez sélectionner un modèle prédéfini existant ou en créer un nouveau.

>[!NOTE]
>
>vous pouvez également configurer le modèle de réponse dans le paramètre prédéfini de la visionneuse. To use the Response Template in the Viewer Preset instead, add `fmt=1` to the end of the Information Server URL in the Viewer Preset.
>
>(Voir [Configuration des paramètres prédéfinis de la visionneuse de catalogue électronique](setting-ecatalog-viewer-presets.md#setting_up_ecatalog_viewer_presets).)

1. Cliquez deux fois sur votre catalogue électronique pour l’ouvrir en mode Affichage des détails.
1. Cliquez sur le panneau Configuration du panneau d’informations pour l’ouvrir.
1. Sélectionnez un modèle de réponse :

   * Sélectionnez un paramètre prédéfini dans le menu Modèle de réponse. Le code XML de la conception du modèle s’affiche dans le champ Modèle utilisateur.
   * Sélectionnez Personnalisé pour créer votre propre modèle de réponse. Entrez la définition XML du modèle dans le champ Modèle utilisateur. Vous pouvez vous inspirer des modèles prédéfinis pour créer le vôtre. 

1. (Facultatif) Dans la zone Réponse par défaut, saisissez le texte que vous souhaitez afficher si Dynamic Media Classic rencontre une erreur lors de la récupération d'informations pour une zone cliquable. Par exemple, si le système reçoit un nom d’entreprise et un nom de catalogue électronique, mais pas d’identificateur de survol, ce message est affiché à l’intention de l’utilisateur.
1. Dans le champ Réponse TTL, entrez le nombre d’heures d’attente avant la mise en cache des données :

   * Optez pour une valeur faible si de nombreuses mises à jour des données sont effectuées quotidiennement.
   * Optez pour une valeur élevée si les données sont relativement stables et ne nécessitent pas de mises à jour fréquentes. La valeur par défaut est de 10 heures.

1. Click **Publish**.

## Import source content for the Info Panel in eCatalogs {#import-source-content-for-the-info-panel-in-ecatalogs}

Vous pouvez utiliser un fichier CSV (valeurs délimitées par des virgules) ou TXT (valeurs délimitées par des tabulations) pour le texte source d’un panneau d’informations de catalogue électronique. Les fichiers délimités par des tabulations doivent utiliser l’encodage UTF16 (Unicode). La méthode d’importation utilisée dépend du type de fichier.

Lorsque vous effectuez la mise en forme du contenu source, n’oubliez pas les points suivants :

* Assurez-vous que les données délimitées par des virgules et des tabulations contiennent autant de colonnes que nécessaire pour le modèle de survol.
* Assurez-vous que le premier objet ou la première colonne de données correspond bien à l’identificateur de survol (associé à la valeur rollover_key des URL de zone cliquable).
* Assurez-vous que chaque objet délimité par des virgules ou des tabulations situé après l’identificateur est bien celui que vous souhaitez remplacer dans le modèle de réponse (la première colonne est donc remplacée par $1$, la deuxième par $2$, et ainsi de suite).

### Import CSV content into eCatalogs from an externally hosted location {#import-csv-content-into-ecatalogs-from-an-externally-hosted-location}

1. Cliquez deux fois sur le catalogue électronique pour l’ouvrir en mode Affichage des détails.
1. Cliquez sur le panneau Source de données du panneau d’informations pour l’ouvrir.
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
1. Cliquez sur le panneau Configuration du panneau d’informations pour l’ouvrir.
1. **Cliquez sur Télécharger le contenu S 7 Info**.
1. Click **Browse**, select the tab-delimited TXT file, CSV or SSV file you want to use, and click **Open**.
1. Cliquez sur **Télécharger**.

Dynamic Media Classic vous envoie un message électronique vous indiquant si le transfert a réussi ou non.

## Prévisualisation du texte de survol pour une zone cliquable {#preview-rollover-key-text-for-an-image-map}

L’écran Pages de zones vous permet de visualiser, en un tournemain, le texte du panneau d’informations pour les zones cliquables sur une page spécifique de votre catalogue électronique.

1. Cliquez sur le bouton de survol Modifier du catalogue électronique.
1. Cliquez sur Pages de zones.
1. Sélectionnez Panneau d’informations dans le menu Afficher situé dans la partie supérieure du tableau à droite de l’écran.

   Le texte de survol apparaît en regard de chaque zone cliquable contenant le texte du panneau d’informations.
