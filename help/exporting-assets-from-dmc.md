---
title: Exportation de ressources à partir d’Adobe Dynamic Media Classic
description: Découvrez comment exporter des ressources à partir d’Adobe Dynamic Media Classic.
uuid: d42b7a73-80c0-4a9a-a04e-7ef53e6fcf22
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: eb850ec7-a669-41ea-b2b0-4c9178e34f95
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 5e3b0002-5ae2-4437-862f-caa098b04362
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 51%

---

# Exportation de ressources à partir d’Adobe Dynamic Media Classic{#exporting-assets-from-dmc}

Vous pouvez enregistrer les ressources que vous avez modifiées dans Adobe Dynamic Media Classic sur un lecteur réseau local. Les fichiers exportés sont compressés dans un fichier ZIP pour le téléchargement ou l’envoi par courrier électronique.

La taille du fichier zip compressé ne doit pas dépasser 1 Go pour la tâche d’exportation. En outre, un maximum de 500 ressources par tâche d’exportation est autorisé.

Adobe Dynamic Media Classic conserve un enregistrement des tâches d’exportation dans l’écran Tâches .

**Pour exporter des ressources à partir d’Adobe Dynamic Media Classic :**

1. Sélectionnez les ressources à exporter, puis accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Exporter]**.
1. Dans la fenêtre Exporter les fichiers sélectionnés, cliquez sur **[!UICONTROL Options d’image]**, puis spécifiez une ou plusieurs options parmi les suivantes (les administrateurs déterminent quelles options sont disponibles pour les utilisateurs) :

   * **[!UICONTROL Paramètres prédéfinis]** - Vous pouvez éventuellement choisir un paramètre d’image prédéfini pour formater la ressource lorsque vous l’exportez. Si vous choisissez un paramètre d’image prédéfini, les autres options de formatage ne sont pas disponibles, car le fichier adopte les formats définis par ce paramètre d’image prédéfini.

   * **[!UICONTROL Conversion]** - Convertissez le fichier de ressource ou l’image d’origine.

   * **[!UICONTROL Taille]** - Vous pouvez sélectionner une taille standard. Vous pouvez également sélectionner **[!UICONTROL Autre]** de la **[!UICONTROL Taille]** , choisissez l’unité de mesure souhaitée, puis définissez la largeur et la hauteur.

      Voir aussi [Définition des options d’exportation disponibles pour les utilisateurs de Media Portal](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

   * **[!UICONTROL Format]** - Choisissez un format d’image.

   * **[!UICONTROL Couleur]** - Choisissez RGB, CMJN ou Gris.

   * **[!UICONTROL Résolution]** - Choisissez 72 ppp, 150 ppp ou 300 ppp.

   * **[!UICONTROL Nom de la tâche]** - Vous pouvez attribuer un nom de tâche à l’exportation.

   * **[!UICONTROL Envoyer un courrier électronique à]** - Vous pouvez éventuellement saisir une adresse électronique si vous envisagez d’envoyer les ressources par courrier électronique. Le message e-mail indique l’URL à laquelle le destinataire peut accéder pour télécharger les fichiers.

1. Sélectionner **[!UICONTROL Exporter]**.

Trois actions d’exportation de base sont prises en charge :

* Fichier d’origine (exporte le fichier d’origine)
* Conversion avec un paramètre prédéfini (utilise un paramètre prédéfini d’image pour formater le fichier)
* Conversion sans paramètre prédéfini) (utilise la boîte de dialogue d’exportation pour spécifier les modificateurs d’image)

Il est impossible d’exporter les types de fichier suivants Tous les autres génèrent une exportation.

* Visionneuses d’images
* Visionneuses de rendus
* Visionneuses à 360°
* Visionneuses de supports
* Visionneuses à débit multiple
* Catalogues électroniques

Par ailleurs, les modèles ne peuvent être exportés en tant que « fichier d’origine ».

Pour exporter les types de fichier suivants, utilisez la conversion :

* Images
* Modèles
* Images modifiées
* PDF (génère des pages converties)
* Postscript®

Le chargement de nombreux types de fichier divers dans l’outil d’exportation entraîne les comportements suivants :

* Tous les types de fichier qu’il est impossible d’exporter sont supprimés de la liste avant que la tâche soit soumise.
* Si une conversion est demandée, tous les types de fichier pouvant être convertis le sont, et tous les autres sont exportés en tant que fichier d’origine.
