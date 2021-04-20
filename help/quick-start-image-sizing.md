---
title: '"Démarrage rapide : Dimensionnement des images"'
description: Cette section contient une introduction et un Début rapide au dimensionnement des images pour vous aider à maîtriser rapidement les techniques de dimensionnement des images.
uuid: 6c4ad4b7-549d-4daa-b6b9-5997a8427af8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: dcaa9b21-b925-4dbb-865e-7918cdbda50c
feature: Dynamic Media Classic,Asset Management
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '853'
ht-degree: 55%

---


# Démarrage rapide : Dimensionnement des images{#quick-start-image-sizing}

Le dimensionnement des images fait référence à la capacité de Dynamic Media Classic à créer plusieurs images dérivées basées sur une seule image haute résolution. Plutôt que de créer manuellement plusieurs images (par exemple, une image miniature et une image à vue agrandie) pour votre site Web ou votre application, vous fournissez une image originale unique. Dynamic Media Classic génère toutes les images modifiées à la demande. La capacité de fournir des images de façon dynamique à partir d’une image originale unique présente de nombreux avantages :

* Vous n’êtes pas tenu de créer manuellement plusieurs copies de l’image selon différentes tailles. Vous fournissez une image originale à Dynamic Media Classic, et Dynamic Media Classic génère des dérivés de différentes tailles à partir de l’image originale.
* Vous pouvez rapidement modifier la taille d’un type d’image sur votre site Web ou dans votre application. Par exemple, pour modifier toutes les images miniatures, vous pouvez modifier le paramètre d’image prédéfini « miniature ». Un paramètre d’image prédéfini s’apparente à une macro ; il représente un ensemble d’attributs de taille et de formatage. Vous pouvez modifier le paramètre d’image prédéfini « miniature » en vue de changer la taille de toutes les images miniatures de votre site Web ou de votre application.
* Vous n’êtes pas tenu de gérer les images originales et l’ensemble des images dérivées dans vos systèmes de gestion de contenu, en interne ou en externe.

![Vous pouvez créer plusieurs images dérivées de tailles différentes à partir du même fichier original haute résolution.](/help/assets/is_derivative_sizes_popup.png)

**Début rapide**

Ce Début rapide de dimensionnement d’image est conçu pour vous aider à maîtriser rapidement les techniques de dimensionnement d’image dans Dynamic Media Classic. Suivez les étapes 1 à 5. A la fin de chaque étape, un renvoi vous permet d’obtenir davantage d’informations, si nécessaire.

**1. Téléchargement des images originales**

Début en téléchargeant vos images originales dans Dynamic Media Classic. En ce qui concerne la taille, Dynamic Media Classic recommande d’utiliser des images de la taille la plus grande que vous prévoyez d’utiliser sur votre site Web ou dans votre application. Par exemple, si vous souhaitez que les visionneuses effectuent un zoom, téléchargez des images dont la dimension la plus grande correspond au moins à 2 000 pixels. Dynamic Media Classic prend en charge de nombreux formats de fichier d’images, mais les images TIFF et PNG sans perte sont recommandées.

Sélectionnez le bouton Télécharger de la barre de navigation globale pour télécharger des fichiers de votre ordinateur vers un dossier de Dynamic Media Classic. (voir [Téléchargement des images originales](uploading-master-images.md#uploading_master_images)).

**2. Configuration des paramètres d’image prédéfinis**

Semblable à une macro, un paramètre d’image prédéfini est un ensemble de commandes prédéfinies de taille et de formatage enregistrées sous un nom. Un paramètre d’image prédéfini régit la taille et le formatage des images diffusées à partir des serveurs Dynamic Media Image Server. Vous pouvez définir vous-même des paramètres d’image prédéfinis si vous avez le statut d’administrateur. Dynamic Media Classic est également fourni avec des paramètres d’image prédéfinis par défaut et vous pouvez les utiliser pour diffuser des images de manière dynamique.

Pour créer un paramètre prédéfini d’image (si vous êtes administrateur), choisissez Configuration > Configuration de l’application. Dans l’écran qui apparaît, affichez les options Configuration de l’application, puis choisissez l’option Paramètres d’image prédéfinis. Cliquez ensuite sur **Ajouter** ou **Modifier** pour créer un paramètre d’image prédéfini.

Le paramètre créé est ajouté au menu Paramètres d’image prédéfinis dans l’écran de prévisualisation. Vous pouvez utiliser le nouveau paramètre d’image prédéfini pour afficher des images dynamiquement sur vos sites Web et dans vos applications (voir [Configuration des paramètres d’image prédéfinis](setting-image-presets.md#setting_up_image_presets)).

**Cookie. Prévisualisation des paramètres d’image prédéfinis**

L’étape suivante consiste à prévisualiser les paramètres d’image prédéfinis que votre administrateur a configurés selon différentes tailles.

Pour explorer les paramètres d’image prédéfinis, cliquez sur **Configuration** > **Paramètres d’image prédéfinis**, puis recherchez un paramètre d’image prédéfini.

Testez les différents paramètres d’image prédéfinis. Découvrez l’apparence de votre image lorsqu’elle est diffusée dynamiquement vers votre site Web ou votre application, selon différentes tailles.

Voir [Prévisualisation d’un fichier d’image en fonction de son paramètre d’image prédéfini](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset).

**4. Publication de vos images originales**

La publication des fichiers d’images originaux présente deux objectifs essentiels :

* Publication des images originales sur les serveurs Dynamic Media Image Server afin que les images puissent être diffusées de manière dynamique sur votre site Web et dans votre application.
* La publication active les chaînes URL pour l’appel d’images depuis les serveurs Dynamic Media Image Server vers votre site Web ou votre application. Après la publication, vous pouvez copier et placer les URL générées par Dynamic Media Classic lorsque cela s’avère nécessaire sur votre site Web ou dans votre application.

Cliquez sur le bouton Publier de la barre de navigation globale pour lancer une publication. Dans l’écran de publication qui s’affiche, cliquez sur le bouton Lancer publication (voir [Publication des images originales](publishing-master-images.md#publishing_master_images)).

**5. Liaison des URL à une application Web**

Dynamic Media Classic crée des chaînes d’appel URL pour les images. Lorsque vous publiez des images sur les serveurs Dynamic Media Image Server, les URL deviennent principales. Vous pouvez copier ces chaînes URL à partir du panneau de navigation (Affichage des détails) ou de l’écran de prévisualisation. Une fois que vous avez copié les chaînes URL, vous pouvez les utiliser dans votre site Web et vos applications. L’URL de dimensionnement d’image remplace la référence à un nom d’image statique dans votre code de page Web. L’URL référence un nom d’image originale, qui est remplacé par votre base de données pour chaque nouvelle image à afficher.

Les chaînes URL générées avec des paramètres d’image prédéfinis contiennent le nom d’un paramètre d’image prédéfini. Ce nom est placé entre des signes dollar (`$`). Par exemple, `$thumbnail$` peut être le paramètre d’image prédéfini conçu pour afficher les images originales sous forme de miniature. (voir [Liaison des URL à une application Web](linking-urls-web-application.md#linking_urls_to_your_web_application)).
