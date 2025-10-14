---
title: 'Démarrage rapide : Dimensionnement des images'
description: Cette section présente et didacticiel de mise en route du dimensionnement des images pour vous aider à maîtriser rapidement les techniques de dimensionnement des images dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic,Asset Management
role: User
topic: Content Management
level: Beginner
exl-id: f1d46f03-57a1-43d8-a0ee-74b92b590736
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 7%

---

# Démarrage rapide : Dimensionnement des images{#quick-start-image-sizing}

Le dimensionnement des images fait référence à la capacité d’Adobe Dynamic Media Classic à créer plusieurs images dérivées en fonction d’une seule image haute résolution. Plutôt que de créer manuellement plusieurs images pour votre site web ou votre application (une miniature et une image à vue agrandie, par exemple), vous ne fournissez qu’une seule image principale. Adobe Dynamic Media Classic génère toutes les images modifiées comme vous le demandez. La possibilité de diffuser des images de manière dynamique à partir d’une seule image principale présente de nombreux avantages :

* La création manuelle de plusieurs copies de l’image à des tailles différentes n’est pas nécessaire. Vous fournissez une image principale à Adobe Dynamic Media Classic, et Adobe Dynamic Media Classic génère des dérivés de différentes tailles à partir de l’image principale.
* Vous pouvez rapidement modifier la taille d’un type d’image sur l’ensemble de votre site web ou de votre application. Par exemple, pour modifier toutes les images miniatures, vous pouvez modifier le paramètre prédéfini d’image « miniature ». Un paramètre d’image prédéfini, qui est similaire à une macro, est un ensemble d’attributs de taille et de formatage. Vous pouvez modifier le paramètre prédéfini d’image « miniature » pour modifier la taille de toutes les miniatures sur votre site web ou application.
* Vous n’avez pas à gérer les fichiers principaux et tous les différents dérivés dans l’un de vos systèmes de gestion de contenu ou de ressources en interne ou en externe.

![Vous pouvez créer plusieurs images dérivées de tailles différentes à partir du même fichier principal haute résolution.](/help/using/assets/is_derivative_sizes_popup.png)

Voir la vidéo de formation [&#x200B; Dimensionnement d’image &#x200B;](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/557_Image%20Sizing_converted%20renamed_Dynamic%20Imaging-AVS) Dynamic Imaging .

Le didacticiel de mise en route du dimensionnement d’image suivant est conçu pour vous aider à maîtriser rapidement les techniques de dimensionnement d’image dans Adobe Dynamic Media Classic. Suivez les étapes 1 à 5. Après chaque étape, il existe une référence croisée où vous pouvez trouver plus d’informations si vous en avez besoin.

## &#x200B;1. Chargement des images principales

Commencez par charger vos images principales dans Adobe Dynamic Media Classic. En ce qui concerne la taille, Adobe Dynamic Media Classic recommande d’utiliser des images ayant la plus grande taille que vous prévoyez d’utiliser sur votre site web ou application. Par exemple, si vous souhaitez que les observateurs zooment les images, chargez les images dont la plus grande taille est d’au moins 2 000 pixels. Adobe Dynamic Media Classic prend en charge de nombreux formats de fichiers image, mais les images TIFF et PNG sans perte sont recommandées.

Sur la barre de navigation générale, sélectionnez **[!UICONTROL Télécharger]** pour télécharger des fichiers depuis votre ordinateur vers un dossier d’Adobe Dynamic Media Classic. Voir [Chargement des images principales](uploading-master-images.md#uploading_master_images).

## &#x200B;2. Configuration des paramètres d’image prédéfinis

Semblable à une macro, un paramètre d’image prédéfini est un ensemble de commandes prédéfinies de taille et de formatage enregistrées sous un nom. Un paramètre d’image prédéfini régit la taille et la mise en forme avec lesquelles les images sont diffusées à partir des serveurs d’images Dynamic Media. Vous pouvez configurer vous-même les paramètres d’image prédéfinis si vous disposez du statut d’administrateur d’entreprise. Vous pouvez diffuser des images de manière dynamique à l’aide des paramètres d’image prédéfinis par défaut déjà fournis avec Adobe Dynamic Media Classic.

Pour créer un paramètre d’image prédéfini (si vous êtes administrateur), sur la barre de navigation globale, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Paramètres d’image prédéfinis]**. Sélectionnez ensuite **[!UICONTROL Ajouter]** pour créer un paramètre d’image prédéfini, ou sélectionnez **[!UICONTROL Modifier]** pour modifier un paramètre d’image prédéfini existant.

Le paramètre d’image prédéfini que vous créez est ajouté au menu Paramètre d’image prédéfini de la page Aperçu . Vous pouvez utiliser votre nouveau paramètre d’image prédéfini pour afficher les images de manière dynamique sur vos sites web et applications. Voir [Configuration des paramètres d’image prédéfinis](setting-image-presets.md#setting_up_image_presets).

## &#x200B;3. Prévisualisation des paramètres d’image prédéfinis

L’étape suivante consiste à prévisualiser les paramètres d’image prédéfinis que votre administrateur a configurés selon différentes tailles.

Pour explorer les paramètres d’image prédéfinis, sur la barre de navigation globale, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Paramètres d’image prédéfinis]**, puis accédez à un paramètre d’image prédéfini.

Testez les différents paramètres d’image prédéfinis. Découvrez comment votre image s’affiche lorsqu’elle est diffusée dynamiquement à votre site web ou à votre application à différentes tailles.

Voir [Prévisualisation d’une ressource d’image en fonction de son paramètre d’image prédéfini](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset).

## &#x200B;4. Publiez vos images principales

La publication de vos fichiers image principaux remplit deux fonctions essentielles :

* Publier vos images principales sur les serveurs d’images Dynamic Media afin que les images puissent être diffusées dynamiquement sur votre site web et votre application.
* La publication active les chaînes URL permettant d’appeler des images depuis les serveurs d’images Dynamic Media vers votre site web ou application. Après la publication, vous pouvez copier et placer les URL générées par Adobe Dynamic Media Classic si nécessaire sur votre site web ou application.

Sur la barre de navigation générale, sélectionnez **[!UICONTROL Publier]** pour lancer une tâche de publication. Dans la boîte de dialogue Publication, sélectionnez **[!UICONTROL Envoyer la publication]**. Voir [Publication des images principales](publishing-master-images.md#publishing_master_images).

## &#x200B;5. Liaison d’URL à une application web

Adobe Dynamic Media Classic crée des chaînes de légende URL pour les images. Lorsque vous publiez des images sur les serveurs d’images Dynamic Media, les URL deviennent actives. Vous pouvez copier ces chaînes d’URL à partir du panneau Parcourir (dans l’affichage des détails) ou de l’écran Aperçu. Après avoir copié les chaînes d’URL, vous pouvez les utiliser dans votre site web et vos applications. L’URL pour le dimensionnement de l’image remplace la référence à un nom d’image statique dans le code de votre page web. L’URL fait référence à un nom d’image principale que la base de données remplace pour chaque nouvelle image à afficher.

Les chaînes URL générées avec des paramètres d’image prédéfinis contiennent le nom d’un paramètre d’image prédéfini. Ce nom est encadré de signes dollar (`$`). Par exemple, `$thumbnail$` peut être le paramètre d’image prédéfini conçu pour afficher les images principales au format d’une miniature. Voir [Liaison d’URL à une application web](linking-urls-web-application.md#linking_urls_to_your_web_application).
