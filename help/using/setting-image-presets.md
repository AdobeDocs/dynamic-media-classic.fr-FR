---
title: Configuration des paramètres d’image prédéfinis
description: Découvrez comment configurer des paramètres d’image prédéfinis dans Adobe Dynamic Media Classic.
uuid: 90530948-dee9-41bd-b39e-684140446abc
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 1ec39fe5-7b2a-4034-9570-6b5595f97052
feature: Dynamic Media Classic,Image Presets
role: User
exl-id: 336802cc-b032-49b2-b2e6-d699bc997ee5
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 50%

---

# Configuration des paramètres d’image prédéfinis{#setting-up-image-presets}

Semblable à une macro, un paramètre d’image prédéfini est un ensemble prédéfini de commandes de dimensionnement et de formatage enregistrées sous un nom. Pour comprendre le fonctionnement des paramètres d’image prédéfinis, supposons que votre site web exige que chaque image de produit apparaisse à deux tailles différentes : 500 x 500 pixels et 150 x 150 pixels. Vous créez deux paramètres d’image prédéfinis, l’un nommé « Agrandissement » pour afficher des images de 500 x 500 pixels et l’autre nommé « Miniature » pour afficher des images de 150 x 150 pixels. Pour diffuser des images aux dimensions &quot;Agrandir&quot; et &quot;Miniature&quot;, un serveur d’images Dynamic Media recherche la définition du paramètre prédéfini d’image agrandie et du paramètre prédéfini d’image miniature. Ensuite, le serveur génère en mode dynamique une image dont la taille et le format correspondent à chaque type de paramètre prédéfini.

Adobe Dynamic Media Classic est fourni avec plusieurs paramètres d’image prédéfinis de &quot;bonne pratique&quot; qui sont déjà configurés pour que vous puissiez les utiliser. Les administrateurs peuvent également créer des paramètres d’image prédéfinis. Vous pouvez créer un paramètre d’image prédéfini entièrement nouveau ou exploiter un paramètre existant et enregistrer votre création sous un nouveau nom.

Les images de taille réduite, lorsqu’elles sont diffusées dynamiquement à partir d’un serveur, peuvent perdre en netteté et en détail. C’est la raison pour laquelle chaque paramètre d’image prédéfini contient des commandes de formatage permettant d’optimiser l’image lorsqu’elle est diffusée avec une taille particulière. Ces commandes garantissent une image nette et claire au moment de la diffusion vers le site Web ou l’application.

## Création d’un paramètre d’image prédéfini {#creating-an-image-preset}

Si vous avez le statut d’administrateur, vous pouvez créer vos propres paramètres d’image prédéfinis. Vous pouvez créer des paramètres d’image prédéfinis ou commencer avec un paramètre d’image prédéfini par défaut fourni par Adobe Dynamic Media Classic, le modifier et l’enregistrer sous un nouveau nom.

**Pour créer un paramètre d’image prédéfini:**

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Paramètres d’image prédéfinis]**.

   Dans cet écran, vous pouvez sélectionner le nom d’un paramètre d’image prédéfini pour le prévisualiser. Lorsque vous sélectionnez un nom de paramètre d’image prédéfini, l’échantillon d’image de la fenêtre de prévisualisation change de taille et d’apparence.

1. Effectuez l’une des opérations suivantes :

   * **Création d’un paramètre d’image prédéfini** - Sélectionner **[!UICONTROL Ajouter]**.
   * **Modification d’un paramètre d’image prédéfini** - Accédez au paramètre d’image prédéfini qui ressemble le plus à celui que vous souhaitez créer, puis sélectionnez **[!UICONTROL Modifier]**.

1. Entrez le nom du paramètre.
1. Complétez les champs Largeur et Hauteur en pixels. Ces mesures déterminent la taille à laquelle les images sont diffusées.
1. Renseignez l’écran Ajouter un paramètre prédéfini ou Modifier le paramètre prédéfini. Pour plus de détails, voir [Options des paramètres d’image prédéfinis](application-setup.md#image_preset_options).

   Adobe Dynamic Media Classic recommande les options &quot;bonnes pratiques&quot; suivantes pour commencer :

   * **[!UICONTROL Format]** - Sélectionnez JPEG ou un autre format qui répond à vos besoins. Tous les navigateurs Web prennent en charge le format d’image JPEG ; il offre un bon compromis entre la taille de fichier réduite et la qualité de l’image. Toutefois, les images au format JPEG utilisent un type de compression avec perte, lequel est susceptible d’introduire des artefacts d’image indésirables si le paramètre de compression est trop faible. Pour cette raison, Adobe Dynamic Media Classic recommande de définir la qualité de compression (sur le curseur) sur 75. Ce paramètre offre un bon compromis entre qualité d’image et taille de fichier réduite.

   * **[!UICONTROL Accentuation]** - Ne sélectionnez pas l’accentuation (ce filtre d’accentuation offre moins de contrôle que **[!UICONTROL Accentuation]** ).

   * **[!UICONTROL Mode de rééchantillonnage]** - Choose **[!UICONTROL Bicubique]**.

   * **[!UICONTROL Accentuation]** (USM) - Saisissez les paramètres suivants :

   | Type de paramètre prédéfini | Taille | Quantité | Rayon | Seuil |
   | --- | --- | --- | --- | --- |
   | Très petite miniature | 75 x 75 | 1,5 | 0,8 | 5 |
   | Miniature | 150 x 150 | 1,1 | 1 | 5 |
   | Image principale | 350 x 350 | 1 | 1 | 6 |
   | Agrandissement | 500 x 500 | 1,2 | 1,2 | 5 |

1. Sélectionner **[!UICONTROL Enregistrer]**.

Les options &quot;bonnes pratiques&quot; d’Adobe Dynamic Media Classic pour la création de paramètres d’image prédéfinis répertoriés ici sont des recommandations générales ; l’accentuation est hautement subjective. Ces paramètres de &quot;bonne pratique&quot; étaient basés sur une image Principale de 2 000 x 2 000 ; les paramètres des fichiers Principaux plus volumineux ou plus petits peuvent être différents. Si vous souhaitez ajuster les paramètres Masquage flou, Adobe Dynamic Media Classic recommande les plages suivantes :

* **[!UICONTROL Quantité]** - Entre 0,8 et 1,5.

* **[!UICONTROL Rayon]** - Entre 0,6 et 2.

* **[!UICONTROL Seuil]** - De 1 à 6.

Pour supprimer un paramètre d’image prédéfini, sélectionnez-le dans l’écran Paramètres d’image prédéfinis, puis sélectionnez **[!UICONTROL Supprimer]**.

>[!MORELIKETHIS]
>
>* [Création et modification des paramètres d’image prédéfinis](application-setup.md#creating_and_editing_image_presets)
>* [Options des paramètres d’image prédéfinis](application-setup.md#image_preset_options)
>* [Prévisualiser une ressource d’image en fonction de son paramètre d’image prédéfini](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)
