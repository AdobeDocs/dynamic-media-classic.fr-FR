---
title: Exportation de fichiers à partir de Dynamic Media Classic
description: Découvrez comment exporter des fichiers à partir de Dynamic Media Classic.
uuid: d42b7a73-80c0-4a9a-a04e-7ef53e6fcf22
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: eb850ec7-a669-41ea-b2b0-4c9178e34f95
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 70%

---


# Exportation d’actifs à partir de Dynamic Media Classic{#exporting-assets-from-dmc}

Vous pouvez enregistrer des fichiers que vous avez modifiés dans Dynamic Media Classic sur un lecteur réseau local. Les fichiers exportés sont compressés dans un fichier ZIP pour le téléchargement ou l’envoi par courrier électronique.

La taille du fichier zip compressé ne doit pas dépasser 1 Go pour la tâche d’exportation. En outre, chaque tâche d’exportation ne peut contenir que 500 fichiers au maximum.

Dynamic Media Classic conserve un enregistrement des tâches d’exportation dans l’écran Tâches.

**Pour exporter des fichiers à partir de Dynamic Media Classic**

1. Sélectionnez les fichiers à exporter, puis cliquez sur **Fichier** > **Exporter**.
1. Dans la fenêtre Exporter les fichiers sélectionnés, cliquez sur **Options d’image**, puis spécifiez une ou plusieurs options parmi les suivantes (les administrateurs déterminent quelles options sont disponibles pour les utilisateurs) :

   * ****
Paramètres prédéfinis (facultatif), choisissez un paramètre d’image prédéfini pour formater le fichier lorsque vous l’exportez. Si vous choisissez un paramètre d’image prédéfini, les autres options de formatage ne sont pas disponibles, car le fichier adopte les formats définis par ce paramètre d’image prédéfini.

   * ****
ConversionConvertissez le fichier ou l’image d’origine.

   * ****
TailleVous pouvez sélectionner une taille standard. Ou, vous pouvez cliquer sur Autres dans la liste déroulante Taille, choisir l’unité de mesure souhaitée, puis spécifier la largeur et la hauteur.

      Voir aussi [Définition d’options d’exportation disponibles pour les utilisateurs du portail multimédia](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

   * ****
FormatChoisissez un format d&#39;image.

   * ****
CouleurChoisissez RVB, CMJN ou Gris.

   * ****
RésolutionChoisissez 72, 150 ou 300 ppp.

   * **Nom de la tâcheVous pouvez attribuer un nom de tâche à l&#39;exportation.**


   * **Envoyer un courrier électronique**
àSi vous le souhaitez, entrez une adresse électronique pour envoyer les fichiers par courrier électronique. Le message e-mail indique l’URL à laquelle le destinataire peut accéder pour télécharger les fichiers.

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

