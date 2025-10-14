---
title: 'Démarrage rapide : Visionneuses d’images'
description: Cette section présente et décrit le démarrage rapide des visionneuses d’images pour vous aider à maîtriser rapidement les techniques des visionneuses d’images dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: 280e7201-84d6-46b1-94bb-0499beca2992
topic: Content Management
level: Beginner
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 11%

---

# Démarrage rapide : Visionneuses d’images{#quick-start-image-sets}

Les visionneuses d’images Adobe Dynamic Media Classic offrent aux utilisateurs une expérience de visionnage intégrée. Dans la visionneuse d’images dynamique, les utilisateurs peuvent voir différentes vues d’un élément en sélectionnant une image miniature. Les visionneuses d’images vous permettent de présenter d’autres vues haute résolution d’un élément.

Les outils de zoom de la visionneuse d’images sont pratiques pour examiner les images de plus près. Si vous le souhaitez, vous pouvez ajouter les cibles de zoom guidées et les zones cliquables à votre visionneuse d’images. Les visionneuses d’images garantissent une visualisation concertée et privée.

Consultez la vidéo de formation [Images et visionneuses à 360° : Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/556_Image%20&%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS).

Lorsque vous créez une visionneuse d’images, Adobe recommande les bonnes pratiques suivantes et applique les limites suivantes :

| Type de limite | Pratique recommandée | Limite imposée |
| --- | --- | --- |
| Nombre de ressources en double par visionneuse | Aucun doublon | 20 ‡ |
| Nombre maximal d’images par visionneuse | 5 à 10 images par ensemble | 1 000 |

‡ Il est recommandé de ne pas avoir de ressources en double dans un ensemble. La limite est de 20 doublons pour une seule ressource. Si vous ajoutez un autre doublon pour cette ressource (dans ce jeu), la requête soit génère une erreur, soit ignore le doublon.

Voir aussi [Limites de Dynamic Media](/help/using/limitations.md).

Le démarrage rapide des visionneuses d’images suivant est conçu pour vous aider à maîtriser rapidement les techniques des visionneuses d’images dans Adobe Dynamic Media Classic.

## &#x200B;1. Chargez vos images principales pour plusieurs vues et échantillons

Commencez par télécharger les images pour les visionneuses d’images. Comme les utilisateurs peuvent zoomer sur les images dans la visionneuse d’images, veillez à tenir compte de cette fonctionnalité lors du choix des images. Assurez-vous que les images font au moins 2 000 pixels dans leur plus grande taille. Adobe Dynamic Media Classic prend en charge de nombreux formats de fichiers image, mais les formats sans perte TIFF, PNG et EPS sont recommandés.

Sur la barre de navigation générale, sélectionnez **[!UICONTROL Télécharger]** pour télécharger des fichiers depuis votre ordinateur vers un dossier d’Adobe Dynamic Media Classic.

Voir [&#x200B; Préparation du chargement de ressources de visionneuse d’images](preparing-image-set-assets-upload.md#preparing-image-set-assets-for-upload) et [&#x200B; Chargement des fichiers](uploading-files.md#uploading-your-files).

## &#x200B;2. Création d’une visionneuse d’images

Dans les visionneuses d’images, les utilisateurs sélectionnent les images miniatures dans la visionneuse d’images pour afficher une image d’un autre côté ou sous un autre angle.

Pour créer une visionneuse d’images, sur la barre de navigation générale, sélectionnez **[!UICONTROL Créer]** puis choisissez **[!UICONTROL Visionneuses d’images]**. Dans la fenêtre Visionneuse d’images, faites glisser vos images sur la page pour composer votre visionneuse d’images. Organisez, ajoutez et supprimez des images, en fonction de vos besoins.

Voir [Création d’une visionneuse d’images](creating-image-set.md#creating-an-image-set).

Voir aussi [Inclure des cibles de zoom et des zones cliquables dans les visionneuses d’images](/help/using/including-zoom-targets-image-maps-image-sets.md)

## &#x200B;3. Préparation des paramètres prédéfinis de visionneuse d’images, si nécessaire

Les administrateurs peuvent créer ou modifier les paramètres prédéfinis de la visionneuse d’images. Adobe Dynamic Media Classic est fourni avec des paramètres prédéfinis de visionneuse par défaut pour chaque type de média enrichi. Utilisez la visionneuse Zoom : **[!UICONTROL Personnalisé]** > **[!UICONTROL Images]** ou **[!UICONTROL Visionneuses d’images]**/**[!UICONTROL Vues multiples]** paramètres prédéfinis pour afficher vos visionneuses d’images.

Vous pouvez ajouter ou modifier des paramètres prédéfinis de visionneuse à partir de l’écran Configuration de l’application .

Voir [Création et modification des paramètres prédéfinis de visionneuse](application-setup.md#adding-and-editing-viewer-presets).

## &#x200B;4. Prévisualisation d’une visionneuse d’images

Sélectionnez la visionneuse d’images dans le panneau Parcourir, puis sélectionnez **[!UICONTROL Aperçu]**. Dans la page Aperçu , sélectionnez les icônes de miniature pour examiner votre visionneuse d’images dans la visionneuse sélectionnée. Différentes visionneuses sont disponibles dans le menu Paramètres prédéfinis.

Voir [Aperçu d’une ressource](previewing-asset.md#previewing-an-asset).

## &#x200B;5. Publication d’une visionneuse d’images

La publication d’une visionneuse d’images la place sur les serveurs Adobe Dynamic Media Classic et active la chaîne URL.

>[!NOTE]
>
>Cette étape n’est pas nécessaire si vous avez sélectionné **[!UICONTROL Publier après un enregistrement]** (par défaut) au moment de la création et de l’enregistrement de la visionneuse d’images.

Sélectionnez l’icône **[!UICONTROL Marquer pour publication]** à gauche de son nom dans le panneau de navigation. Sélectionnez ensuite **[!UICONTROL Publier]**. Sur la page Publication, sélectionnez **[!UICONTROL Envoyer la publication]**.

Voir [Publication de fichiers](publishing-files.md#publishing-files).

## &#x200B;6. Liaison d’une visionneuse d’images à votre site web

Adobe Dynamic Media Classic crée des appels URL pour les visionneuses d’images et les active après leur publication. Vous pouvez copier ces chaînes URL depuis l’écran de prévisualisation.

Sélectionnez la visionneuse d’images, puis sélectionnez **[!UICONTROL Aperçu]**. Sélectionnez maintenant un paramètre prédéfini de visionneuse d’images, puis cliquez sur le bouton **[!UICONTROL Copier l’URL]**.

Voir [Liaison de la visionneuse d’images à une page web](linking-image-set-web-page.md#linking-an-image-set-to-a-web-page).
