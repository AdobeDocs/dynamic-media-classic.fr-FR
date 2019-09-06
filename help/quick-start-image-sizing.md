---
title: '"Démarrage rapide : Dimensionnement des images"'
seo-title: '"Démarrage rapide : Dimensionnement des images"'
description: 'null'
seo-description: Introduction et démarrage rapide au dimensionnement des images pour vous aider à maîtriser rapidement les opérations liées aux techniques de dimensionnement des images.
uuid: 6 c 4 ad 4 b 7-549 d -4 daa-b 6 b 9-5997 a 8427 af 8
contentOwner: admin
content-type: référence
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/image_ sizing
discoiquuid: dcaa 9 b 21-b 925-4 dbb -865 e -7918 cdbda 50 c
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Démarrage rapide : Dimensionnement des images{#quick-start-image-sizing}

Le dimensionnement d'image fait référence à la capacité de Dynamic Media Classic à créer plusieurs images dérivées basées sur une image haute résolution unique. Plutôt que de créer manuellement plusieurs images (par exemple, une image miniature et une image agrandie) pour votre site Web ou votre application, vous fournissez une image originale unique. Dynamic Media Classic génère toutes les images modifiées à mesure que vous les demandez. La capacité de fournir des images de façon dynamique à partir d’une image originale unique présente de nombreux avantages :

* Vous n’êtes pas tenu de créer manuellement plusieurs copies de l’image selon différentes tailles. Vous fournissez une image originale à Dynamic Media Classic, et Dynamic Media Classic génère des dérivés différents à partir de l'image originale.
* Vous pouvez rapidement modifier la taille d’un type d’image sur votre site Web ou dans votre application. Par exemple, pour modifier toutes les images miniatures, vous pouvez modifier le paramètre d’image prédéfini « miniature ». Un paramètre d’image prédéfini s’apparente à une macro ; il représente un ensemble d’attributs de taille et de formatage. Vous pouvez modifier le paramètre d’image prédéfini « miniature » en vue de changer la taille de toutes les images miniatures de votre site Web ou de votre application.
* Vous n’êtes pas tenu de gérer les images originales et l’ensemble des images dérivées dans vos systèmes de gestion de contenu, en interne ou en externe.

![Vous pouvez créer plusieurs images dérivées à une taille différente du même fichier original haute résolution.](/help/assets/is_derivative_sizes_popup.png)

**Démarrage rapide**

Cette section a pour but de vous aider à vous familiariser rapidement avec les techniques de dimensionnement d’image de Scene7 Publishing System. Suivez les étapes 1 à 5. A la fin de chaque étape, un renvoi vous permet d’obtenir davantage d’informations, si nécessaire.

**Cookie. Téléchargement des images originales**

Dans un premier temps, téléchargez vos images originales vers Scene7 Publishing System. En ce qui concerne la taille, Dynamic Media Classic recommande d'utiliser des images qui sont la plus grande que vous prévoyez d'utiliser sur votre site Web ou dans votre application. Par exemple, si vous souhaitez que les visionneuses effectuent un zoom, téléchargez des images dont la dimension la plus grande correspond au moins à 2 000 pixels. Dynamic Media Classic prend en charge de nombreux formats de fichiers image, mais les images TIFF et PNG sans perte sont recommandées.

Cliquez sur le bouton Télécharger de la barre de navigation globale pour télécharger des fichiers depuis votre ordinateur vers un dossier de Scene7 Publishing System (voir [Téléchargement des images originales](uploading-master-images.md#uploading_master_images)).

**2. Configuration des paramètres d’image prédéfinis**

Semblable à une macro, un paramètre d’image prédéfini est un ensemble de commandes prédéfinies de taille et de formatage enregistrées sous un nom. Un paramètre d'image prédéfini gère la taille et le formatage des images diffusées à partir de serveurs d'images de médias dynamiques. Vous pouvez définir vous-même des paramètres d’image prédéfinis si vous avez le statut d’administrateur. Dynamic Media Classic est également fourni avec des paramètres d'image prédéfinis par défaut et vous pouvez les utiliser pour diffuser dynamiquement des images.

Pour créer un paramètre prédéfini d’image (si vous êtes administrateur), choisissez Configuration &gt; Configuration de l’application. Dans l’écran qui apparaît, affichez les options Configuration de l’application, puis choisissez l’option Paramètres d’image prédéfinis. Cliquez ensuite **sur Ajouter** ou **Modifier** pour créer un paramètre d'image prédéfini.

Le paramètre créé est ajouté au menu Paramètres d’image prédéfinis dans l’écran de prévisualisation. Vous pouvez utiliser le nouveau paramètre d’image prédéfini pour afficher des images dynamiquement sur vos sites Web et dans vos applications (voir [Configuration des paramètres d’image prédéfinis](setting-image-presets.md#setting_up_image_presets)).

**Cookie. Prévisualisation des paramètres d’image prédéfinis**

L’étape suivante consiste à prévisualiser les paramètres d’image prédéfinis que votre administrateur a configurés selon différentes tailles.

To explore Image Presets, click **Setup** &gt; **Image Presets**, and then browse to an Image Preset.

Testez les différents paramètres d’image prédéfinis. Découvrez l’apparence de votre image lorsqu’elle est diffusée dynamiquement vers votre site Web ou votre application, selon différentes tailles.

Voir [Prévisualisation d’un fichier d’image en fonction de son paramètre d’image prédéfini](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset).

**4. Publication de vos images originales**

La publication des fichiers d’images originaux présente deux objectifs essentiels :

* La publication des images originales sur les serveurs d'images de médias dynamiques permet de diffuser les images de manière dynamique sur votre site Web et dans votre application.
* La publication active les chaînes URL pour l'appel des images à partir des serveurs d'images de médias dynamiques vers votre site Web ou votre application. Après la publication, vous pouvez copier et placer les URL générées par Dynamic Media Classic lorsque cela s'avère nécessaire sur votre site Web ou dans votre application.

Cliquez sur le bouton Publier de la barre de navigation globale pour lancer une publication. Dans l’écran de publication qui s’affiche, cliquez sur le bouton Lancer publication (voir [Publication des images originales](publishing-master-images.md#publishing_master_images)).

**5. Liaison des URL à une application Web**

Dynamic Media Classic crée des chaînes d'appel URL pour les images. Lorsque vous publiez des images sur des serveurs d'images dynamiques, les URL deviennent actives. Vous pouvez copier ces chaînes URL à partir du panneau de navigation (Affichage des détails) ou de l’écran de prévisualisation. Une fois que vous avez copié les chaînes URL, vous pouvez les utiliser dans votre site Web et vos applications. L’URL de dimensionnement d’image remplace la référence à un nom d’image statique dans votre code de page Web. L’URL référence un nom d’image originale, qui est remplacé par votre base de données pour chaque nouvelle image à afficher.

Les chaînes URL générées avec des paramètres d’image prédéfinis contiennent le nom d’un paramètre d’image prédéfini. This name is enclosed in dollar signs (`$`). For example, `$thumbnail$` can be the Image Preset designed to show master images at thumbnail size. (voir [Liaison des URL à une application Web](linking-urls-web-application.md#linking_urls_to_your_web_application)).
