---
title: Configuration des paramètres d’image prédéfinis
seo-title: Configuration des paramètres d’image prédéfinis
description: 'null'
seo-description: Découvrez comment configurer des paramètres d'image prédéfinis.
uuid: 90530948-dee 9-41 bd-b 39 e -684140446 abc
contentOwner: admin
content-type: référence
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/image_ sizing
discoiquuid: 1 ec 39 fe 5-7 b 2 a -4034-9570-6 b 5595 f 97052
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Configuration des paramètres d’image prédéfinis{#setting-up-image-presets}

Semblable à une macro, un paramètre d’image prédéfini est un ensemble prédéfini de commandes de dimensionnement et de formatage enregistrées sous un nom. Pour comprendre le fonctionnement des paramètres d’image prédéfinis, imaginez que votre site Web nécessite l’affichage de chaque image d’un produit dans deux tailles différentes : 500 x 500 pixels et 150 x 150 pixels. Vous créez deux paramètres d’image prédéfinis, l’un nommé « Agrandissement » pour afficher des images de 500 x 500 pixels et l’autre nommé « Miniature » pour afficher des images de 150 x 150 pixels. Pour fournir des images à la taille « Agrandissement » et « Miniature », un serveur d'images de médias dynamiques recherche la définition du paramètre d'image prédéfini et du paramètre prédéfini de miniature. Ensuite, le serveur génère en mode dynamique une image dont la taille et le format correspondent à chaque type de paramètre prédéfini.

Dynamic Media Classic est fourni avec plusieurs paramètres d'image prédéfinis « recommandés » qui sont déjà configurés. Les administrateurs peuvent également créer des paramètres d'image prédéfinis. Vous pouvez créer un paramètre d’image prédéfini entièrement nouveau ou exploiter un paramètre existant et enregistrer votre création sous un nouveau nom.

Les images de taille réduite, lorsqu’elles sont diffusées dynamiquement à partir d’un serveur, peuvent perdre en netteté et en détail. C’est la raison pour laquelle chaque paramètre d’image prédéfini contient des commandes de formatage permettant d’optimiser l’image lorsqu’elle est diffusée avec une taille particulière. Ces commandes garantissent une image nette et claire au moment de la diffusion vers le site Web ou l’application.

## Création d’un paramètre d’image prédéfini {#creating-an-image-preset}

Si vous avez le statut d’administrateur, vous pouvez créer vos propres paramètres d’image prédéfinis. Vous pouvez créer des paramètres d'image prédéfinis ou commencer par un paramètre d'image prédéfini par défaut fourni par Dynamic Media Classic, le modifier et l'enregistrer sous un nouveau nom.

**Pour créer un paramètre d’image prédéfini**

1. Cliquez sur **Configuration** &gt; **Paramètres d’image prédéfinis**.

   Dans cet écran, vous pouvez sélectionner le nom d’un paramètre d’image prédéfini pour le prévisualiser. Lorsque vous sélectionnez un nom de paramètre d’image prédéfini, l’échantillon d’image de la fenêtre de prévisualisation change de taille et d’apparence.

1. Effectuez l’une des opérations suivantes :

   **Création d'un
paramètre d'image prédéfini** Cliquez sur Ajouter.

   **Modification d'un paramètre d'image prédéfini** Accédez au paramètre d'image prédéfini le plus proche de celui que vous souhaitez créer, puis cliquez sur Modifier.

1. Entrez le nom du paramètre.
1. Complétez les champs Largeur et Hauteur en pixels. Ces mesures déterminent la taille à laquelle les images sont diffusées.
1. Renseignez l’écran Ajouter un paramètre prédéfini ou Modifier le paramètre prédéfini. Pour plus de détails, voir [Options des paramètres d’image prédéfinis](application-setup.md#image_preset_options).

   Dynamic Media Classic recommande de choisir les options recommandées pour démarrer :

   **Format** Choisissez un format JPEG ou un autre format qui correspond à vos besoins. Tous les navigateurs Web prennent en charge le format d’image JPEG ; il offre un bon compromis entre la taille de fichier réduite et la qualité de l’image. Toutefois, les images au format JPEG utilisent un type de compression avec perte, lequel est susceptible d’introduire des artefacts d’image indésirables si le paramètre de compression est trop faible. C'est pourquoi Dynamic Media Classic recommande de définir la qualité de compression (sur le curseur) à 75. Ce paramètre offre un bon compromis entre qualité d’image et taille de fichier réduite.

   **Accentuation** Ne sélectionnez pas Accentuation (ce filtre d'accentuation offre moins de contrôle que les paramètres de masquage flou).

   **Mode de ré-échantillonnage** Sélectionnez Bicubique.

   **Options de masquage flou (USM)** Saisissez les paramètres illustrés ici :

   | Type de paramètre prédéfini | Taille | Quantité | Rayon | Seuil |
   |--- |--- |--- |--- |--- |
   | Très petite miniature | 75 x 75 | 1,5 | 0,8 | 5 |
   | Miniature | 150 x 150 | 1,1 | 1 | 5 |
   | Image principale | 350 x 350 | 1 | 1 | 6 |
   | Agrandissement | 500 x 500 | 1,2 | 1,2 | 5 |

1. Cliquez sur **Enregistrer**.

Les options « Meilleures pratiques » de Media Classic Classic pour la création de paramètres d'image prédéfinis répertoriés ici sont des recommandations générales ; l'accentuation est hautement subjective. Ces paramètres sont basés sur une image originale de 2 000 x 2 000 ; il se peut que les paramètres relatifs à des images originales plus grandes ou plus petites soient différents. Si vous souhaitez ajuster les paramètres Masquage flou, Dynamic Media Classic recommande les plages suivantes :

**Montant** compris entre 0,8 et 1,5.

**Rayon** entre 0,6 et 2.

**Seuil** de 1 à 6.

Pour supprimer un paramètre d’image prédéfini, sélectionnez-le dans l’écran Paramètres d’image prédéfinis, puis cliquez sur le bouton Supprimer.

>[!MORELIKETHIS]
>
>* [Création et modification des paramètres d’image prédéfinis](application-setup.md#creating_and_editing_image_presets)
>* [Options des paramètres d’image prédéfinis](application-setup.md#image_preset_options)
>* [Prévisualisation d’un fichier d’image en fonction de son paramètre d’image prédéfini](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)
