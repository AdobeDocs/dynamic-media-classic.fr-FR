---
title: Gestion du contenu du panneau Informations dans les visionneuses d’images
description: Découvrez comment gérer le contenu du panneau d’informations dans les visionneuses d’images.
uuid: ed7b4344-f180-41fc-a95a-62a9767dc056
contentOwner: rbrough
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
content-type: reference
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: ba5d1fb1-af54-471c-a471-853ace7f72fd
feature: Dynamic Media Classic,Visionneuses,Visionneuses d’images
role: User
exl-id: 09fafdb4-51e2-4719-83b6-056f79d1ba9e
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '763'
ht-degree: 54%

---

# Gestion du contenu du panneau Informations dans les visionneuses d’images{#managing-info-panel-content-in-image-sets}

Outre l’utilisation de texte de zone cliquable pour vos survols dans les visionneuses d’images, vous pouvez utiliser un panneau d’informations pour ajouter de plus grandes quantités de texte de survol, y compris des liens. Vous pouvez également gérer le panneau d’informations en utilisant la mise en cache temporisée et en planifiant des mises à jour du contenu.

Vous pouvez gérer la configuration et les données du panneau d’informations à l’aide des fonctionnalités suivantes de Dynamic Media Classic :

* Le panneau Configuration du panneau d’informations vous permet de définir le modèle utilisé pour afficher le texte du panneau, une réponse par défaut aux erreurs, ainsi que la période de mise en cache (en heures) des informations. Par ailleurs, vous pouvez préciser si la visionneuse d’image est automatiquement publiée.
* Le panneau Source de données du panneau d’informations vous permet de spécifier un fichier CSV contenant le texte que vous souhaitez afficher dans le texte de survol du panneau d’informations et de planifier les heures de mise à jour des informations.
* La boîte de dialogue Importer les métadonnées vous permet d’importer un fichier TXT délimité par des tabulations contenant les informations sur le texte de survol. Vous pouvez utiliser cette option TXT ou le panneau de flux de données du panneau d’informations avec l’option de fichier CSV pour votre texte de survol.

## Configuration d’un modèle de réponse pour les visionneuses d’images {#set-up-a-response-template-for-image-sets}

Vous pouvez sélectionner l’un des trois modèles de réponse prédéfinis pour afficher du texte dans un panneau d’informations. Ces modèles de réponse prédéfinis déterminent le mode de présentation de vos informations dans le panneau d’informations : nombre de colonnes et de lignes, police et corps de caractères, etc. Vous pouvez sélectionner un modèle prédéfini existant ou en créer un nouveau.

**Pour configurer un modèle de réponse :**

1. Cliquez deux fois sur votre visionneuse d’image pour l’ouvrir en mode Affichage des détails.
1. Cliquez sur **[!UICONTROL Configuration du panneau d’informations]**.
1. Dans la liste déroulante Modèle de réponse, procédez de l’une des façons suivantes :

   * Pour utiliser la réponse par défaut, sélectionnez **[!UICONTROL Default]**. Le code XML de la conception du modèle s’affiche, grisé, dans la zone de texte Modèle utilisateur.
   * Pour créer votre propre modèle de réponse, sélectionnez **[!UICONTROL Personnalisé]**. Dans la zone de texte Modèle utilisateur, entrez la définition du modèle XML. Vous pouvez utiliser le modèle par défaut qui est déjà défini dans la zone de texte comme base pour votre propre réponse.

1. (Facultatif) Dans la zone Réponse par défaut, saisissez le texte que vous souhaitez afficher si Dynamic Media Classic rencontre une erreur lors de la récupération des informations pour une zone cliquable. Par exemple, si le système reçoit un nom d’entreprise et un nom de visionneuse d’image, mais pas d’identificateur de survol, ce message est affiché à l’intention de l’utilisateur.
1. Dans le champ Réponse TTL, entrez le nombre d’heures d’attente avant la mise en cache des données.

   * Optez pour une valeur faible si de nombreuses mises à jour des données sont effectuées quotidiennement.
   * Optez pour une valeur élevée si les données sont relativement stables et ne nécessitent pas de mises à jour fréquentes. La valeur par défaut est de 10 heures.

1. Cliquez sur **[!UICONTROL Télécharger]** pour charger le contenu du panneau d’informations, en fonction des valeurs rollover_key, dans s7info.
1. Dans la boîte de dialogue S7Info Upload, accédez au fichier que vous souhaitez utiliser, puis cliquez sur **[!UICONTROL Télécharger]**.

   Les formats de fichiers pris en charge sont des fichiers délimités par des tabulations avec codage UTF-16 et des fichiers CSV avec codage ASCII. Pour les fichiers CSV, les caractères non ASCII doivent être encodés au format HTML.

1. Dans le panneau Configuration du panneau d’informations, cliquez sur **[!UICONTROL Publier]**.

## Importation du contenu source pour le panneau Informations dans les visionneuses d’images {#import-source-content-for-the-info-panel-in-image-sets}

Vous pouvez utiliser un fichier CSV (valeurs séparées par des virgules) avec un encodage ASCII (les caractères non ASCII doivent être encodés au format HTML) ou un fichier délimité par des tabulations pour le texte source d’un panneau d’informations, pour une visionneuse d’image. Les fichiers délimités par des tabulations doivent utiliser l’encodage UTF-16 (Unicode). La méthode d’importation utilisée dépend du type de fichier.

Lorsque vous effectuez la mise en forme du contenu source, n’oubliez pas les points suivants :

* Les données délimitées par des virgules et des tabulations peuvent contenir autant de colonnes que nécessaire pour le modèle de survol.
* Le premier élément ou la première colonne de données est l’identifiant de survol (associé à la valeur rollover_key des URL de zone cliquable).
* Assurez-vous que chaque élément délimité par des tabulations ou des virgules après l’identifiant est l’élément que vous souhaitez remplacer dans le modèle de réponse. Ainsi, la première colonne est remplacée par $1$, la deuxième par $2$, etc.).

### Importation de contenu CSV dans les visionneuses d’images à partir d’un emplacement hébergé en externe {#import-csv-content-into-image-sets-from-an-externally-hosted-location}

1. Cliquez deux fois sur la visionneuse d’image pour l’ouvrir en mode Affichage des détails.
1. Cliquez sur **[!UICONTROL InfoPanel Datafeed]**.
1. Dans le champ de l’emplacement du fichier CSV hébergé en externe (HTTP), entrez l’URL du fichier CSV.
1. (Facultatif) Dans les champs Mise à jour du planning , indiquez l’heure de mise à jour du contenu, puis cliquez sur **[!UICONTROL Ajouter]**.

   Vous pouvez sélectionner plusieurs heures. Chaque heure de mise à jour apparaît dans la zone Mettre à jour les durées. Pour supprimer une heure planifiée, sélectionnez-la, puis cliquez sur **[!UICONTROL Supprimer]**.

1. (Facultatif) Cliquez sur **[!UICONTROL Exécuter la mise à jour]** pour mettre immédiatement à jour le contenu.
