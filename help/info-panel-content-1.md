---
title: Gestion du contenu du panneau d’informations dans les visionneuses d’images
seo-title: Gestion du contenu du panneau d’informations dans les visionneuses d’images
description: 'null'
seo-description: Découvrez comment gérer le contenu du panneau d’informations dans les visionneuses d’images.
uuid: ed7b4344-f180-41fc-a95a-62a9767dc056
contentOwner: rbrough
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
content-type: reference
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: ba5d1fb1-af54-471c-a471-853ace7f72fd
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 73%

---


# Gestion du contenu du panneau d’informations dans les visionneuses d’images{#managing-info-panel-content-in-image-sets}

Outre l’utilisation de texte de zone cliquable pour vos survols dans les visionneuses d’images, vous pouvez utiliser un panneau d’informations pour ajouter de plus grandes quantités de texte de survol, y compris des liens. Vous pouvez également gérer le panneau d’informations en utilisant la mise en cache temporisée et en planifiant des mises à jour du contenu.

Vous pouvez gérer la configuration et les données de votre panneau d’informations à l’aide des fonctionnalités suivantes de Dynamic Media Classic :

* Le panneau Configuration du panneau d’informations vous permet de définir le modèle utilisé pour afficher le texte du panneau, une réponse par défaut aux erreurs, ainsi que la période de mise en cache (en heures) des informations. Par ailleurs, vous pouvez préciser si la visionneuse d’image est automatiquement publiée.
* Le panneau Source de données du panneau d’informations vous permet d’indiquer un fichier CSV contenant le texte à afficher comme texte de survol du panneau d’informations, ainsi que les heures de planification de la mise à jour des informations.
* La boîte de dialogue Importer les métadonnées vous permet d’importer un fichier TXT délimité par des tabulations contenant les informations sur le texte de survol. Vous pouvez utiliser cette option TXT ou le panneau de source de données du panneau d’informations avec l’option de fichier CSV pour votre texte de survol.

## Configuration d’un modèle de réponse pour les visionneuses d’images {#set-up-a-response-template-for-image-sets}

Vous pouvez sélectionner l’un des trois modèles de réponse prédéfinis pour afficher du texte dans un panneau d’informations. Ces modèles de réponse prédéfinis déterminent le mode de présentation de vos informations dans le panneau d’informations : nombre de colonnes et de lignes, police et corps de caractères, etc. Vous pouvez sélectionner un modèle prédéfini existant ou en créer un nouveau.

**Pour configurer un modèle de réponse**

1. Cliquez deux fois sur votre visionneuse d’image pour l’ouvrir en mode Affichage des détails.
1. Click **InfoPanel Setup** to unfold the panel.
1. Dans la liste déroulante Modèle de réponse, procédez de l’une des façons suivantes :

   * Sélectionnez Par défaut pour utiliser la réponse par défaut. Le code XML de la conception du modèle s’affiche, grisé, dans la zone de texte Modèle utilisateur.
   * Sélectionnez Personnalisé pour créer votre propre modèle de réponse. Dans la zone de texte Modèle utilisateur, entrez la définition du modèle XML. Vous pouvez utiliser le modèle par défaut qui est déjà défini dans la zone de texte comme base pour votre propre réponse.

1. (Facultatif) Dans la zone Réponse par défaut, saisissez le texte à afficher si Dynamic Media Classic rencontre une erreur lors de la récupération des informations d’une zone cliquable. Par exemple, si le système reçoit un nom d’entreprise et un nom de visionneuse d’image, mais pas d’identificateur de survol, ce message est affiché à l’intention de l’utilisateur.
1. Dans le champ Réponse TTL, entrez le nombre d’heures d’attente avant la mise en cache des données.

   * Optez pour une valeur faible si de nombreuses mises à jour des données sont effectuées quotidiennement.
   * Optez pour une valeur élevée si les données sont relativement stables et ne nécessitent pas de mises à jour fréquentes. La valeur par défaut est de 10 heures.

1. Click **Upload** to upload info panel content, based on the rollover_key values, to s7info.
1. In the S7Info Upload dialog box, browse to the file that you want to use, and then click **Upload**.

   Les formats de fichiers pris en charge sont les fichiers délimités par des tabulations avec un encodage UTF-16, ou au format CSV avec un encodage ASCII. Pour les fichiers CSV, les caractères non ASCII doivent être encodés au format HTML.

1. In the InfoPanel Setup panel, click **Publish**.

## Importation de contenu source pour le panneau d’informations dans les visionneuses d’images {#import-source-content-for-the-info-panel-in-image-sets}

Vous pouvez utiliser un fichier CSV (valeurs séparées par des virgules) avec un encodage ASCII (les caractères non ASCII doivent être encodés au format HTML) ou un fichier délimité par des tabulations pour le texte source d’un panneau d’informations, pour une visionneuse d’image. Les fichiers délimités par des tabulations doivent utiliser l’encodage UTF-16 (Unicode). La méthode d’importation utilisée dépend du type de fichier.

Lorsque vous effectuez la mise en forme du contenu source, n’oubliez pas les points suivants :

* Les données délimitées par des virgules et des tabulations doivent contenir autant de colonnes que nécessaire pour le modèle de survol.
* Le premier objet ou la première colonne de données doit correspondre à l’identificateur de survol (associé à la valeur rollover_key des URL de zone cliquable).
* Assurez-vous que chaque objet délimité par des virgules ou des tabulations situé après l’identificateur est bien celui que vous souhaitez remplacer dans le modèle de réponse (la première colonne est donc remplacée par $1$, la deuxième par $2$, et ainsi de suite).

### Importation de contenu CSV dans des visionneuses d’images à partir d’un emplacement hébergé en externe {#import-csv-content-into-image-sets-from-an-externally-hosted-location}

1. Cliquez deux fois sur la visionneuse d’image pour l’ouvrir en mode Affichage des détails.
1. Click **InfoPanel Datafeed** to unfold the panel.
1. Dans le champ de l’emplacement du fichier CSV hébergé en externe (HTTP), entrez l’URL du fichier CSV.
1. (Optional) In the Schedule Update fields, specify a time to update the content, and then click **Add**.

   Vous pouvez sélectionner plusieurs heures. Chaque heure de mise à jour apparaît dans la zone Mettre à jour les durées. To remove a scheduled time, select it, and then click **Delete**.

1. (Optional) Click **Run Update** to immediately update the content.

