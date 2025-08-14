---
title: Gestion du contenu du panneau Informations dans les visionneuses d’images
description: Découvrez comment gérer le contenu du panneau Informations dans les visionneuses d’images d’Adobe Dynamic Media Classic.
contentOwner: rbrough
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
content-type: reference
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: 09fafdb4-51e2-4719-83b6-056f79d1ba9e
topic: Content Management
level: Intermediate
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 34%

---

# Gestion du contenu du panneau Informations dans les visionneuses d’images{#managing-info-panel-content-in-image-sets}

Outre l’utilisation de texte de zone cliquable pour les survols dans les visionneuses d’images, vous pouvez utiliser un panneau d’informations pour ajouter de plus grandes quantités de texte de survol, y compris des liens. Vous pouvez également gérer l’InfoPanel à l’aide de la mise en cache temporelle et de la planification des mises à jour de contenu.

Vous pouvez gérer la configuration et les données de votre InfoPanel à l’aide des fonctionnalités suivantes d’Adobe Dynamic Media Classic :

* Le panneau Configuration du panneau Informations vous permet de spécifier le modèle utilisé pour afficher le texte du panneau Informations, une réponse par défaut pour les erreurs et le nombre d’heures pendant lesquelles les informations sont mises en cache. Par ailleurs, vous pouvez préciser si la visionneuse d’image est automatiquement publiée.
* Le panneau Flux de données du panneau Informations vous permet de spécifier un fichier CSV contenant le texte à afficher dans le texte de remplacement du panneau Informations et de planifier les heures de mise à jour des informations.
* La boîte de dialogue Importer des métadonnées vous permet d’importer un fichier TXT délimité par des tabulations contenant les informations de texte de survol. Vous pouvez utiliser cette option TXT ou le panneau Flux de données InfoPanel avec l’option Fichier CSV pour votre texte de survol.

## Configurer un modèle de réponse pour les visionneuses d’images {#set-up-a-response-template-for-image-sets}

Vous pouvez sélectionner l’un des trois modèles de réponse prédéfinis pour afficher du texte dans un panneau d’informations. Ces modèles de réponse prédéfinis déterminent le mode de présentation de vos informations dans le panneau d’informations : nombre de colonnes et de lignes, police et corps de caractères, etc. Vous pouvez sélectionner un modèle prédéfini existant ou en créer un nouveau.

**Pour configurer un modèle de réponse pour les visionneuses d’images :**

1. Double-cliquez sur la visionneuse d’images pour l’ouvrir dans l’affichage des détails.
1. Sélectionnez **[!UICONTROL Configuration du panneau Informations]**.
1. Dans la liste déroulante Modèle de réponse, procédez de l’une des façons suivantes :

   * Pour utiliser la réponse par défaut, sélectionnez **[!UICONTROL Par défaut]**. Le code XML de la conception du modèle s’affiche, grisé, dans la zone de texte Modèle utilisateur.
   * Pour créer votre propre modèle de réponse, sélectionnez **[!UICONTROL Personnalisé]**. Dans la zone de texte Modèle utilisateur, entrez la définition du modèle XML. Vous pouvez utiliser le modèle par défaut qui est déjà défini dans la zone de texte comme base pour votre propre réponse.

1. (Facultatif) Dans la zone Réponse par défaut, saisissez le texte à afficher si Adobe Dynamic Media Classic rencontre une erreur lors de la récupération des informations d’une zone cliquable. Par exemple, si le système reçoit un nom d’entreprise et un nom de visionneuse d’image, mais pas d’identificateur de survol, ce message est affiché à l’intention de l’utilisateur.
1. Dans le champ Réponse TTL, entrez le nombre d’heures d’attente avant la mise en cache des données.

   * Optez pour une valeur faible si de nombreuses mises à jour des données sont effectuées quotidiennement.
   * Optez pour une valeur élevée si les données sont relativement stables et ne nécessitent pas de mises à jour fréquentes. La valeur par défaut est de 10 heures.

1. Sélectionnez **[!UICONTROL Charger]** pour charger le contenu du panneau Informations, en fonction de la valeur rollover_key, dans s7info.
1. Dans la boîte de dialogue de chargement S7Info, recherchez le fichier que vous souhaitez utiliser, puis sélectionnez **[!UICONTROL Charger]**.

   Les formats de fichiers pris en charge sont des fichiers délimités par des tabulations avec un codage UTF-16 et des fichiers CSV avec un codage ASCII. Pour les fichiers CSV, les caractères non ASCII doivent être encodés au format HTML.

1. Dans le panneau Configuration de l’InfoPanel, sélectionnez **[!UICONTROL Publier]**.

## Importation du contenu source pour le panneau Informations dans les visionneuses d’images {#import-source-content-for-the-info-panel-in-image-sets}

Vous pouvez utiliser un fichier CSV (valeurs séparées par des virgules) avec un codage ASCII (les caractères non-ASCII doivent être codés en HTML) ou un fichier délimité par des tabulations pour le texte source d’un panneau d’informations d’une visionneuse d’images. Les fichiers délimités par des tabulations doivent utiliser l’encodage UTF-16 (Unicode). Vous pouvez importer les différents types de fichiers à l’aide de différentes méthodes.

Lorsque vous effectuez la mise en forme du contenu source, n’oubliez pas les points suivants :

* Les données délimitées par des tabulations et des virgules peuvent contenir autant de colonnes que nécessaire pour le modèle de survol.
* Le premier élément ou la première colonne de données est l’identifiant de survol (associé à la valeur rollover_key des URL de la zone cliquable).
* Assurez-vous que chaque élément délimité par des tabulations ou des virgules après l’identifiant est l’élément que vous souhaitez remplacer dans le modèle de réponse. Ainsi, la première colonne est remplacée par $1$, la deuxième par $2$, et ainsi de suite).

### Importer du contenu CSV dans des visionneuses d’images à partir d’un emplacement hébergé en externe {#import-csv-content-into-image-sets-from-an-externally-hosted-location}

1. Double-cliquez sur la visionneuse d’images pour l’ouvrir en mode Détail.
1. Sélectionnez **[!UICONTROL Flux de données InfoPanel]**.
1. Dans le champ de l’emplacement du fichier CSV hébergé en externe (HTTP), entrez l’URL du fichier CSV.
1. (Facultatif) Dans le champ Planifier la mise à jour , spécifiez une heure pour mettre à jour le contenu, puis sélectionnez **[!UICONTROL Ajouter]**.

   Vous pouvez sélectionner plusieurs heures. Chaque heure de mise à jour apparaît dans la zone Mettre à jour les durées. Pour supprimer une heure planifiée, sélectionnez-la, puis sélectionnez **[!UICONTROL Supprimer]**.

1. (Facultatif) Sélectionnez **[!UICONTROL Exécuter la mise à jour]** pour pouvoir mettre immédiatement à jour le contenu.
