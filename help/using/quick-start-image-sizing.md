---
title: "Démarrage rapide : dimensionnement des images"
description: Cette section vous présente et vous aide à maîtriser rapidement les techniques de dimensionnement des images dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: dcaa9b21-b925-4dbb-865e-7918cdbda50c
feature: Dynamic Media Classic,Asset Management
role: User
topic: Content Management
level: Beginner
exl-id: f1d46f03-57a1-43d8-a0ee-74b92b590736
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '877'
ht-degree: 17%

---

# Démarrage rapide : Dimensionnement des images{#quick-start-image-sizing}

Le dimensionnement des images fait référence à la capacité d’Adobe Dynamic Media Classic à créer plusieurs images dérivées basées sur une seule image haute résolution. Au lieu de créer manuellement plusieurs images (une miniature et une image agrandie, par exemple) pour votre site web ou votre application, vous fournissez une seule image principale. Adobe Dynamic Media Classic génère toutes les images modifiées comme vous le souhaitez. Être en mesure de diffuser des images dynamiquement à partir d’une seule image principale présente de nombreux avantages :

* Vous n’êtes pas tenu de créer manuellement plusieurs copies de l’image selon différentes tailles. Vous fournissez une image principale à Adobe Dynamic Media Classic et Adobe Dynamic Media Classic génère des dérivés de différentes dimensions à partir de l’image principale.
* Vous pouvez rapidement modifier la taille d’un type d’image sur votre site Web ou dans votre application. Par exemple, pour modifier toutes les images miniatures, vous pouvez modifier le paramètre d’image prédéfini &quot;miniature&quot;. Un paramètre d’image prédéfini (similaire à une macro) est un ensemble d’attributs de taille et de mise en forme. Vous pouvez modifier le paramètre d’image prédéfini &quot;miniature&quot; afin de modifier la taille de toutes les images miniatures sur votre site web ou dans votre application.
* Vous n’avez pas à gérer les fichiers principaux et tous les dérivés dans aucun de vos systèmes de gestion de contenu ou de ressources en interne ou en externe.

![Vous pouvez créer plusieurs images dérivées à une taille différente à partir du même fichier principal haute résolution.](/help/using/assets/is_derivative_sizes_popup.png)

Voir [Taille d’image : Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/557_Image%20Sizing_converted%20renamed_Dynamic%20Imaging-AVS) vidéo de formation.

Le démarrage rapide suivant relatif au dimensionnement des images est conçu pour vous aider à maîtriser rapidement les techniques de dimensionnement des images dans Adobe Dynamic Media Classic. Suivez les étapes 1 à 5. Après chaque étape, il existe une référence croisée où vous trouverez plus d’informations si vous en avez besoin.

## 1. Chargement des images principales

Commencez par charger vos images principales dans Adobe Dynamic Media Classic. En ce qui concerne la taille, Adobe Dynamic Media Classic recommande d’utiliser des images de la taille la plus grande que vous prévoyez d’utiliser sur votre site web ou votre application. Si vous souhaitez, par exemple, que les visionneuses effectuent un zoom sur des images, chargez des images d’au moins 2 000 pixels de la taille la plus grande. Adobe Dynamic Media Classic prend en charge de nombreux formats de fichier image, mais les formats TIFF sans perte et PNG sont recommandés.

Dans la barre de navigation globale, sélectionnez **[!UICONTROL Télécharger]** pour charger des fichiers depuis votre ordinateur vers un dossier sur Adobe Dynamic Media Classic. Voir [Chargement des images principales](uploading-master-images.md#uploading_master_images).

## 2. Configuration de paramètres d’image prédéfinis

Semblable à une macro, un paramètre d’image prédéfini est un ensemble de commandes prédéfinies de taille et de formatage enregistrées sous un nom. Un paramètre d’image prédéfini détermine la taille et le formatage avec lesquels les images sont diffusées à partir des serveurs d’images Dynamic Media. Vous pouvez définir vous-même des paramètres d’image prédéfinis si vous avez le statut d’administrateur. Adobe Dynamic Media Classic est également fourni avec des paramètres d’image prédéfinis par défaut, que vous pouvez utiliser pour diffuser des images de manière dynamique.

Pour créer un paramètre d’image prédéfini (si vous êtes administrateur), dans la barre de navigation globale, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Paramètres d’image prédéfinis]**. Sélectionnez **[!UICONTROL Ajouter]** pour créer un paramètre d’image prédéfini, ou sélectionnez **[!UICONTROL Modifier]** pour modifier un paramètre d’image prédéfini existant.

Le paramètre d’image prédéfini que vous créez est ajouté au menu Paramètre d’image prédéfini de la page Aperçu. Vous pouvez utiliser le nouveau paramètre d’image prédéfini pour afficher des images dynamiquement sur vos sites Web et dans vos applications Voir [Configuration des paramètres d’image prédéfinis](setting-image-presets.md#setting_up_image_presets).

## 3. Aperçu des paramètres d’image prédéfinis

L’étape suivante consiste à prévisualiser les paramètres d’image prédéfinis que votre administrateur a configurés selon différentes tailles.

Pour explorer les paramètres d’image prédéfinis, dans la barre de navigation globale, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Paramètres d’image prédéfinis]**, puis accédez à un paramètre d’image prédéfini.

Testez les différents paramètres d’image prédéfinis. Découvrez comment votre image apparaît lorsqu’elle est diffusée dynamiquement vers votre site web ou votre application, selon différentes tailles.

Voir [Prévisualiser une ressource d’image en fonction de son paramètre d’image prédéfini](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset).

## 4. Publiez vos images principales

La publication de vos fichiers image principaux a deux objectifs essentiels :

* Publier vos images principales sur les serveurs d’images Dynamic Media afin que les images puissent être diffusées dynamiquement vers votre site web et votre application.
* La publication active les chaînes URL pour appeler des images à partir des serveurs Dynamic Media Image Server vers votre site web ou votre application. Après la publication, vous pouvez copier et placer les URL générées par Adobe Dynamic Media Classic si nécessaire dans votre site web ou votre application.

Dans la barre de navigation globale, sélectionnez **[!UICONTROL Publier]** pour démarrer une tâche de publication. Dans la boîte de dialogue Publication, sélectionnez **[!UICONTROL Envoyer la publication]**. Voir [Publication des images principales](publishing-master-images.md#publishing_master_images).

## 5. Liaison d’URL à une application web

Adobe Dynamic Media Classic crée des chaînes d’légende URL pour les images. Lorsque vous publiez des images sur les serveurs Dynamic Media Image, les URL deviennent actives. Vous pouvez copier ces chaînes d’URL à partir du panneau de navigation (dans la vue Détails) ou de l’écran de prévisualisation. Une fois que vous avez copié les chaînes URL, vous pouvez les utiliser dans votre site Web et vos applications. L’URL de dimensionnement d’image remplace la référence à un nom d’image statique dans votre code de page Web. L’URL fait référence à un nom d’image principal, qui est remplacé par votre base de données pour chaque nouvelle image à afficher.

Les chaînes URL générées avec des paramètres d’image prédéfinis contiennent le nom d’un paramètre d’image prédéfini. Ce nom est encadré de signes dollar (`$`). Par exemple : `$thumbnail$` peut être le paramètre d’image prédéfini conçu pour afficher les images principales à la taille de la miniature. Voir [Liaison d’URL à une application web](linking-urls-web-application.md#linking_urls_to_your_web_application).
