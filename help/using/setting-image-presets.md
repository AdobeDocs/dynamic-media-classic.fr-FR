---
title: Configuration des paramètres d’image prédéfinis
description: Découvrez comment configurer les paramètres d’image prédéfinis dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic,Image Presets
role: User
exl-id: 336802cc-b032-49b2-b2e6-d699bc997ee5
topic: Content Management
level: Intermediate
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '667'
ht-degree: 32%

---

# Configuration des paramètres d’image prédéfinis{#setting-up-image-presets}

Semblable à une macro, un paramètre d’image prédéfini est un ensemble prédéfini de commandes de dimensionnement et de formatage enregistrées sous un nom. Pour comprendre le fonctionnement des paramètres d’image prédéfinis, supposons que votre site web exige que chaque image du produit s’affiche dans deux tailles différentes : 500 × 500 pixels et 150 × 150 pixels. Vous créez deux paramètres d’image prédéfinis, l’un appelé « Agrandir » pour afficher les images à 500 x 500 pixels et l’autre appelé « Miniature » pour afficher les images à 150 × 150 pixels. Pour diffuser des images aux tailles « Agrandir » et « Miniature », un serveur d’images Dynamic Media recherche la définition des paramètres prédéfinis « Agrandir l’image » et « Miniature ». Ensuite, le serveur génère en mode dynamique une image dont la taille et le format correspondent à chaque type de paramètre prédéfini.

Adobe Dynamic Media Classic s’accompagne de plusieurs paramètres d’image prédéfinis « conformes aux bonnes pratiques » déjà configurés pour être utilisés. L’administration peut également créer des paramètres d’image prédéfinis. Vous pouvez créer un paramètre d’image prédéfini entièrement nouveau ou exploiter un paramètre existant et enregistrer votre création sous un nouveau nom.

Les images de taille réduite, lorsqu’elles sont diffusées dynamiquement à partir d’un serveur, peuvent perdre en netteté et en détail. C’est la raison pour laquelle chaque paramètre d’image prédéfini contient des commandes de formatage permettant d’optimiser l’image lorsqu’elle est diffusée avec une taille particulière. Ces commandes permettent de s’assurer que vos images sont nettes et claires lorsqu’elles sont diffusées sur votre site web ou application.

## Création d’un paramètre d’image prédéfini {#creating-an-image-preset}

Si vous êtes administrateur d’entreprise, vous pouvez créer vos propres paramètres d’image prédéfinis. Vous pouvez créer des paramètres d’image prédéfinis ou commencer par un paramètre d’image prédéfini par défaut fourni par Adobe Dynamic Media Classic, le modifier et l’enregistrer sous un nouveau nom.

**Pour créer un paramètre d’image prédéfini :**

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Paramètres d’image prédéfinis]**.

   Dans cet écran, vous pouvez sélectionner le nom d’un paramètre d’image prédéfini pour le prévisualiser. Lorsque vous sélectionnez un nom de paramètre d’image prédéfini, l’échantillon d’image de la fenêtre de prévisualisation change de taille et d’apparence.

1. Effectuez l’une des opérations suivantes :

   * **Créer un paramètre d’image prédéfini** : sélectionnez **[!UICONTROL Ajouter]**.
   * **Modification d’un paramètre d’image prédéfini** : recherchez le paramètre d’image prédéfini qui ressemble le plus à celui que vous souhaitez créer, puis sélectionnez **[!UICONTROL Modifier]**.

1. Entrez le nom du paramètre.
1. Complétez les champs Largeur et Hauteur en pixels. Ces mesures déterminent la taille à laquelle les images sont diffusées.
1. Renseignez l’écran Ajouter un paramètre prédéfini ou Modifier le paramètre prédéfini. Pour plus de détails, voir [Options des paramètres d’image prédéfinis](application-setup.md#image_preset_options).

   Adobe Dynamic Media Classic recommande les options suivantes (correspondant aux « bonnes pratiques ») pour commencer :

   * **[!UICONTROL Format]** : sélectionnez JPEG ou un autre format répondant à vos besoins. Tous les navigateurs web prennent en charge le format d’image JPEG, qui offre un bon équilibre entre la petite taille des fichiers et la qualité de l’image. Toutefois, les images JPEG utilisent un schéma de compression avec perte qui peut introduire des artefacts d’image indésirables si le paramètre de compression est trop faible. Pour cette raison, Adobe Dynamic Media Classic recommande de définir la qualité de compression (sur le curseur) sur 75. Ce paramètre offre un bon compromis entre qualité d’image et taille de fichier réduite.

   * **[!UICONTROL Accentuation]** : ne sélectionnez pas l’option Accentuation (ce filtre d’accentuation offre moins de contrôle que les paramètres **[!UICONTROL Masquage flou]**).

   * **[!UICONTROL Mode Rééchantillonnage]** : Choisissez **[!UICONTROL Bicubique]**.

   * **[!UICONTROL Masquage flou]** (USM) : renseignez les paramètres suivants :

   | Type de paramètre prédéfini | Taille | Quantité | Rayon | Seuil |
   | --- | --- | --- | --- | --- |
   | Très petite miniature | 75 × 75 | 1,5 | 0,8 | 5 |
   | Miniature | 150 × 150 | 1,1 | 1 | 5 |
   | Image principale | 350 × 350 | 1 | 1 | 6 |
   | Agrandissement | 500 × 500 | 1,2 | 1,2 | 5 |

1. Sélectionnez **[!UICONTROL Enregistrer]**.

Les options des « bonnes pratiques » d’Adobe Dynamic Media Classic relatives à la création de paramètres d’image prédéfinis répertoriées ici sont des recommandations générales ; l’accentuation est très subjective. Ces paramètres de « bonnes pratiques » étaient basés sur une image principale de 2 000 × 2 000. Les paramètres des fichiers principaux plus petits ou plus grands peuvent être différents. Si vous souhaitez ajuster les paramètres de masquage flou, Adobe Dynamic Media Classic recommande les plages suivantes :

* **[!UICONTROL Montant]** : entre `.8` et `1.5`.

* **[!UICONTROL Rayon]** : entre `.6` et `2`.

* **[!UICONTROL Seuil]** : du `1` au `6`.

Pour supprimer un paramètre d’image prédéfini, sélectionnez-le dans l’écran Paramètres d’image prédéfinis, puis sélectionnez **[!UICONTROL Supprimer]**.

>[!MORELIKETHIS]
>
>* [Création et modification de paramètres d’image prédéfinis](application-setup.md#creating_and_editing_image_presets)
>* [Options des paramètres prédéfinis d’image](application-setup.md#image_preset_options)
>* [Prévisualisation d’une ressource image en fonction de son paramètre d’image prédéfini](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)
