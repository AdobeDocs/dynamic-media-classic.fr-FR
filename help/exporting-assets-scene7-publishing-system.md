---
title: Exportation de fichiers à partir de Scene7 Publishing System
seo-title: Exportation de fichiers à partir de Scene7 Publishing System
description: 'null'
seo-description: Découvrez comment exporter des fichiers à partir de Scene 7 Publishing System.
uuid: d 42 b 7 a 73-80 c 0-4 a 9 a-a 04 e -7 ef 53 e 6 fcf 22
contentOwner: admin
content-type: référence
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/managing_ assets
discoiquuid: eb 850 ec 7-a 669-41 ea-b 2 b 0-4 c 9178 e 34 f 95
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Exportation de fichiers à partir de Scene7 Publishing System{#exporting-assets-from-scene-publishing-system}

Vous pouvez enregistrer des fichiers que vous avez édités dans Scene7 Publishing System sur un lecteur réseau local. Les fichiers exportés sont compressés dans un fichier ZIP pour le téléchargement ou l’envoi par courrier électronique.

La taille du fichier zip compressé ne doit pas dépasser 1 Go pour la tâche d’exportation. En outre, chaque tâche d’exportation ne peut contenir que 500 fichiers au maximum.

Dynamic Media Classic conserve un enregistrement des tâches d'exportation dans l'écran Tâches.

**Pour exporter des fichiers à partir de Scene7 Publishing System**

1. Sélectionnez les fichiers à exporter, puis cliquez sur **Fichier** &gt; **Exporter**.
1. Dans la fenêtre Exporter les fichiers sélectionnés, cliquez sur **Options d’image**, puis spécifiez une ou plusieurs options parmi les suivantes (les administrateurs déterminent quelles options sont disponibles pour les utilisateurs) :

   **Paramètres prédéfinis** Si vous le souhaitez, choisissez un paramètre d'image prédéfini pour le formater lors de son exportation. Si vous choisissez un paramètre d’image prédéfini, les autres options de formatage ne sont pas disponibles, car le fichier adopte les formats définis par ce paramètre d’image prédéfini.

   **Conversion** Convertissez le fichier ou l'image d'origine.

   **Taille** Vous pouvez sélectionner une taille standard. Ou, vous pouvez cliquer sur Autres dans la liste déroulante Taille, choisir l’unité de mesure souhaitée, puis spécifier la largeur et la hauteur.

   Voir aussi [Définition d’options d’exportation disponibles pour les utilisateurs du portail multimédia](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

   **Format** Choisissez un format d'image.

   **Couleur** Choisissez RVB, CMJN ou Gris.

   **Résolution** : 72, 150 ou 300 ppp.

   **Nom de la tâche** Vous pouvez affecter un nom de tâche à l'exportation.

   **Envoyer un courriel à** éventuellement, saisissez une adresse e-mail pour envoyer les fichiers par e-mail. Le message e-mail indique l’URL à laquelle le destinataire peut accéder pour télécharger les fichiers.

1. Cliquez sur **Exporter**.

Trois actions d’exportation de base sont prises en charge :

* Fichier d’origine (exporte le fichier d’origine)
* Conversion avec un paramètre prédéfini (utilise un paramètre prédéfini d’image pour formater le fichier)
* Conversion sans paramètre prédéfini) (utilise la boîte de dialogue d’exportation pour spécifier les modificateurs d’image)

Il est impossible d’exporter les types de fichier suivants (pour tous les autres types de fichier, l’exportation est possible) :

* Visionneuses d’images
* Visionneuses de rendus
* Visionneuses à 360°
* Visionneuses de supports
* Visionneuses à débit binaire multiple
* Catalogues électroniques

Par ailleurs, les modèles ne peuvent être exportés en tant que « fichier d’origine ».

Pour exporter les types de fichier suivants, utilisez la conversion :

* Images
* Modèles
* Images modifiées
* PDF (génère des pages converties)
* Postscript

Le chargement de nombreux types de fichier divers dans l’outil d’exportation entraîne les comportements suivants :

* Tous les types de fichier qu’il est impossible d’exporter sont supprimés de la liste avant que la tâche soit soumise.
* Si une conversion est demandée, tous les types de fichier pouvant être convertis le sont, et tous les autres sont exportés en tant que fichier d’origine.

