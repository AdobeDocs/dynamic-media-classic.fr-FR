---
title: "Démarrage rapide\_: Visionneuses d’images"
description: Présentation et démarrage rapide des visionneuses d’images pour vous aider à maîtriser rapidement les techniques de visionneuse d’images dans Adobe Dynamic Media Classic.
uuid: daf17d13-9c06-41f0-8fc5-2e56d460d341
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: 612a425f-2840-46c4-8e5a-c0bc5f738f4e
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: 280e7201-84d6-46b1-94bb-0499beca2992
topic: Content Management
level: Beginner
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 21%

---

# Démarrage rapide : Visionneuses d’images{#quick-start-image-sets}

Les visionneuses d’images Adobe Dynamic Media Classic offrent aux utilisateurs une expérience de visionnage intégrée. La visionneuse d’images dynamique vous permet d’afficher différentes vues d’un objet d’un simple clic sur une image miniature. Les visionneuses d’images vous permettent de présenter d’autres vues haute résolution d’un élément.

Les outils de zoom de la visionneuse d’images sont pratiques pour examiner les images de plus près. Si vous le souhaitez, vous pouvez intégrer des cibles de zoom guidé et des zones cliquables dans votre visionneuse d’images. Les visionneuses d’images garantissent une visualisation concertée et privée.

Voir [Visionneuses d’images et à 360° : Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/556_Image%20&amp;%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS) vidéo de formation.

Lorsque vous créez une visionneuse d’images, Adobe recommande les bonnes pratiques suivantes et applique les limites suivantes :

| Type de limite | Pratique recommandée | Limite imposée |
| --- | --- | --- |
| Nombre de ressources en double par ensemble | Aucun doublon | 20 |
| Nombre maximal d’images par visionneuse | 5 à 10 images par visionneuse | 1 000 |

Voir aussi [Limites de Dynamic Media](/help/using/limitations.md).

Le démarrage rapide des visionneuses d’images suivant est conçu pour vous aider à maîtriser rapidement les techniques de visionneuse d’images dans Adobe Dynamic Media Classic.

## 1. Chargez les images Principales pour plusieurs vues et échantillons

Commencez par télécharger les images pour les visionneuses d’images. Comme les utilisateurs peuvent zoomer sur les images dans la visionneuse d’images, veillez à en tenir compte lors du choix des images. Assurez-vous que la taille des images est d’au moins 2 000 pixels. Adobe Dynamic Media Classic prend en charge de nombreux formats de fichier image, mais les formats TIFF, PNG et EPS sans perte sont recommandés.

Dans la barre de navigation globale, sélectionnez **[!UICONTROL Télécharger]** pour charger des fichiers depuis votre ordinateur vers un dossier sur Adobe Dynamic Media Classic.

Voir [Préparation du chargement de ressources de visionneuse d’images](preparing-image-set-assets-upload.md#preparing-image-set-assets-for-upload) et [Chargement des fichiers](uploading-files.md#uploading-your-files).

## 2. Création d’une visionneuse d’images

Dans les visionneuses d’images, les utilisateurs sélectionnent des miniatures dans la visionneuse d’images pour afficher une image d’un autre côté ou d’un autre angle.

Pour créer une visionneuse d’images, dans la barre de navigation globale, sélectionnez **[!UICONTROL Build]**, puis choisissez **[!UICONTROL Visionneuses d’images]**. Dans la fenêtre Visionneuse d’images, faites glisser les images sur la page pour composer la visionneuse. Organisez, ajoutez et supprimez des images, en fonction de vos besoins.

Voir [Création d’une visionneuse d’images](creating-image-set.md#creating-an-image-set).

Voir aussi [Inclusion de cibles de zoom et de zones cliquables dans les visionneuses d’images](/help/using/including-zoom-targets-image-maps-image-sets.md)

## 3. Préparez les paramètres prédéfinis de la visionneuse d’images, si nécessaire

Les administrateurs peuvent créer ou modifier les paramètres prédéfinis de la visionneuse d’images. Adobe Dynamic Media Classic est fourni avec des paramètres prédéfinis de visionneuse par défaut pour chaque type de média enrichi. Utilisez la visionneuse de zoom : **[!UICONTROL Personnalisé]** > **[!UICONTROL Images]** ou **[!UICONTROL Visionneuses d’images]**/**[!UICONTROL Vues multiples]** paramètres prédéfinis pour afficher vos visionneuses d’images.

L’ajout et la modification des paramètres prédéfinis de visionneuse s’effectuent à partir de l’écran Configuration de l’application.

Voir [Création et modification de paramètres prédéfinis de visionneuse](application-setup.md#adding-and-editing-viewer-presets).

## 4. Prévisualisation d’une visionneuse d’images

Sélectionnez la visionneuse d’images dans le panneau de navigation, puis sélectionnez **[!UICONTROL Aperçu]**. Dans la page Aperçu , sélectionnez les icônes de miniature pour examiner votre visionneuse d’images dans la visionneuse sélectionnée. Différentes visionneuses sont disponibles dans le menu Paramètres prédéfinis.

Voir [Aperçu d’une ressource](previewing-asset.md#previewing-an-asset).

## 5. Publication d’une visionneuse d’images

La publication d’une visionneuse d’images la place sur les serveurs Adobe Dynamic Media Classic et active la chaîne URL.

>[!NOTE]
>
>Cette étape n’est pas nécessaire si vous avez sélectionné **[!UICONTROL Publish after save]**(« Publier après l’enregistrement ») (valeur par défaut) au moment de la création et de l’enregistrement de la visionneuse d’images.

Sélectionner **[!UICONTROL Marquer pour publication]** à gauche de son nom dans le panneau de navigation. Sélectionnez ensuite **[!UICONTROL Publier]**. Sur la page Publier, sélectionnez **[!UICONTROL Envoyer la publication]**.

Voir [Publication de fichiers](publishing-files.md#publishing-files).

## 6. Liez une visionneuse d’images à votre site Web.

Adobe Dynamic Media Classic crée des appels URL pour les visionneuses d’images et les active après leur publication. Vous pouvez copier ces chaînes URL depuis l’écran de prévisualisation.

Sélectionnez la visionneuse d’images, puis cliquez sur **[!UICONTROL Aperçu]**. Sélectionnez maintenant un paramètre prédéfini de visionneuse d’images, puis cliquez sur **[!UICONTROL Copier l’URL]**.

Voir [Liaison d’une visionneuse d’images à une page web](linking-image-set-web-page.md#linking-an-image-set-to-a-web-page).
