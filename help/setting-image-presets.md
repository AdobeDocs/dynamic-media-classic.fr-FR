---
title: Configuration des paramètres d’image prédéfinis
description: Découvrez comment configurer des paramètres d’image prédéfinis.
uuid: 90530948-dee9-41bd-b39e-684140446abc
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 1ec39fe5-7b2a-4034-9570-6b5595f97052
feature: Dynamic Media Classic,Paramètres d’image prédéfinis
role: Business Practitioner
exl-id: 336802cc-b032-49b2-b2e6-d699bc997ee5
translation-type: tm+mt
source-git-commit: 7456226cf6469f40e66ff327475d4c605b6d6e13
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 64%

---

# Configuration des paramètres d’image prédéfinis{#setting-up-image-presets}

Semblable à une macro, un paramètre d’image prédéfini est un ensemble prédéfini de commandes de dimensionnement et de formatage enregistrées sous un nom. Pour comprendre le fonctionnement des paramètres d’image prédéfinis, imaginez que votre site Web nécessite l’affichage de chaque image d’un produit dans deux tailles différentes : 500 x 500 pixels et 150 x 150 pixels. Vous créez deux paramètres d’image prédéfinis, l’un nommé « Agrandissement » pour afficher des images de 500 x 500 pixels et l’autre nommé « Miniature » pour afficher des images de 150 x 150 pixels. Pour diffuser des images aux formats &quot;Agrandissement&quot; et &quot;Miniature&quot;, un serveur d’images Dynamic Media recherche la définition des paramètres prédéfinis Agrandissement et Miniature. Ensuite, le serveur génère en mode dynamique une image dont la taille et le format correspondent à chaque type de paramètre prédéfini.

Dynamic Media Classic est fourni avec plusieurs paramètres d’image prédéfinis &quot;recommandés&quot; qui sont déjà configurés pour que vous puissiez les utiliser. Les administrateurs peuvent également créer de nouveaux paramètres d’image prédéfinis. Vous pouvez créer un paramètre d’image prédéfini entièrement nouveau ou exploiter un paramètre existant et enregistrer votre création sous un nouveau nom.

Les images de taille réduite, lorsqu’elles sont diffusées dynamiquement à partir d’un serveur, peuvent perdre en netteté et en détail. C’est la raison pour laquelle chaque paramètre d’image prédéfini contient des commandes de formatage permettant d’optimiser l’image lorsqu’elle est diffusée avec une taille particulière. Ces commandes garantissent une image nette et claire au moment de la diffusion vers le site Web ou l’application.

## Création d’un paramètre d’image prédéfini  {#creating-an-image-preset}

Si vous avez le statut d’administrateur, vous pouvez créer vos propres paramètres d’image prédéfinis. Vous pouvez créer des paramètres d’image prédéfinis ou des débuts avec un paramètre d’image prédéfini par défaut fourni par Dynamic Media Classic, le modifier et l’enregistrer sous un nouveau nom.

**Pour créer un paramètre d’image prédéfini:**

1. Cliquez sur **Configuration** > **Paramètres d’image prédéfinis**.

   Dans cet écran, vous pouvez sélectionner le nom d’un paramètre d’image prédéfini pour le prévisualiser. Lorsque vous sélectionnez un nom de paramètre d’image prédéfini, l’échantillon d’image de la fenêtre de prévisualisation change de taille et d’apparence.

1. Effectuez l’une des opérations suivantes :

   * **Création d’un**
paramètre d’image prédéfiniAjoute de clic.

   * **Modification d’un**
paramètre d’image prédéfiniAccédez au paramètre d’image prédéfini qui ressemble le plus à celui que vous souhaitez créer, puis cliquez sur Modifier.

1. Entrez le nom du paramètre.
1. Complétez les champs Largeur et Hauteur en pixels. Ces mesures déterminent la taille à laquelle les images sont diffusées.
1. Renseignez l’écran Ajouter un paramètre prédéfini ou Modifier le paramètre prédéfini. Pour plus de détails, voir [Options des paramètres d’image prédéfinis](application-setup.md#image_preset_options).

   Dynamic Media Classic recommande ces options &quot;meilleures pratiques&quot; au début :

   * ****
FormatChoisissez JPEG ou un autre format qui répond à vos exigences. Tous les navigateurs web prennent en charge le format d’image JPEG ; celui-ci offre un bon équilibre entre taille de fichier réduite et qualité des images. Toutefois, les images au format JPEG utilisent un modèle de compression avec perte qui peut introduire des artefacts d’image indésirables si le paramètre de compression est trop faible. Pour cette raison, Dynamic Media Classic recommande de définir la qualité de compression (sur le curseur) sur 75. Ce paramètre offre un bon équilibre entre la qualité d’image et la taille de fichier réduite.

   * ****
AccentuationNe sélectionnez pas Accentuation (ce filtre d’accentuation est moins contrôlé que les paramètres de masquage flou).

   * **Rééchantillonner le**
modeChoisissez le mode bicubique.

   * ****
Options de masquage flouSaisissez les paramètres affichés ici :
   | Type de paramètre prédéfini | Taille | Quantité | Rayon | Seuil |
   |--- |--- |--- |--- |--- |
   | Très petite miniature | 75 x 75 | 1,5 | 0,8 | 5 |
   | Miniature | 150 x 150 | 1,1 | 1 | 5 |
   | Image principale | 350 x 350 | 1 | 1 | 6 |
   | Agrandissement | 500 x 500 | 1,2 | 1,2 | 5 |

1. Cliquez sur **Enregistrer**.

Les options de &quot;bonnes pratiques&quot; de Dynamic Media Classic pour la création de paramètres d’image prédéfinis répertoriées ici sont des recommandations générales ; l’accentuation est très subjective. Ces paramètres sont basés sur une image originale de 2 000 x 2 000 ; il se peut que les paramètres relatifs à des images originales plus grandes ou plus petites soient différents. Si vous souhaitez ajuster les paramètres de masquage flou, Dynamic Media Classic recommande les plages suivantes :

* ****
AmountBetween 08 to 1.5.

* ****
RadiusBetween .6 and 2.

* ****
SeuilDe 1 à 6.

Pour supprimer un paramètre d’image prédéfini, sélectionnez-le dans l’écran Paramètres d’image prédéfinis, puis cliquez sur le bouton Supprimer.

>[!MORELIKETHIS]
>
>* [Création et modification des paramètres d’image prédéfinis](application-setup.md#creating_and_editing_image_presets)
>* [Options des paramètres d’image prédéfinis](application-setup.md#image_preset_options)
>* [Prévisualisation d’un fichier d’image en fonction de son paramètre d’image prédéfini](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)

