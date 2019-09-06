---
title: '"Démarrage rapide : Zoom"'
seo-title: '"Démarrage rapide : Zoom"'
description: 'null'
seo-description: Une introduction et un démarrage rapide pour effectuer un zoom pour vous aider à maîtriser rapidement les opérations.
uuid: 31 eda 632-3469-4 f 90-885 b-e 90 c 6 a 2 e 5 e 75
contentOwner: admin
content-type: référence
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/zoom
discoiquuid: 559 c 986 d -313 d -46 df-a 5 ff -0 b 49316 ad 3 a 7
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Démarrage rapide : Zoom{#quick-start-zoom}

Zoom permet d'afficher de manière interactive les détails haute résolution dans les images. Vous pouvez, par exemple, voir les couleurs, les options, les angles et les détails d’une image dans une visionneuse intégrée, entièrement configurable et dynamique. Cette visionneuse peut être incorporée à une page Web ou s’afficher dans une fenêtre contextuelle. Vous pouvez examiner des images de près et effectuer un panoramique à des résolutions élevées pour les inspecter en détail. La fonction de zoom permet à vos clients de bénéficier d’une expérience de visualisation plus interactive, instructive et dynamique. 

Dynamic Media Classic offre également un zoom guidé, moyen de mettre en évidence les fonctionnalités importantes d'une image. Vous pouvez par exemple créer une cible de zoom pour un logo afin d’attirer l’attention des utilisateurs sur ce dernier. Lorsque les utilisateurs cliquent sur cette cible de zoom, ils effectuent un zoom sur le logo.

Toutes les images de zoom sont créées et servies à partir d’images originales uniques, de graphiques et d’attributs gérés par des bases de données. La fonction de zoom dynamique Media Classic permet de réduire considérablement le temps et le coût de production et de diffusion d'images. Vous pouvez utiliser des visionneuses de zoom pour effectuer un zoom avant ou arrière sur les images. La visionneuse de zoom comporte des boutons sur lesquels il suffit de cliquer pour effectuer un zoom et un panoramique ; à cela s’ajoute la possibilité d’effectuer un panoramique par glissement sur l’écran. Des paramètres prédéfinis de visionneuse de zoom permettent de configurer la visionneuse utilisée pour effectuer un zoom sur les images.

**Démarrage rapide**

Cette section de démarrage rapide de Zoom est conçue pour maîtriser rapidement les techniques de zoom dans Dynamic Media Classic. Suivez les étapes 1 à 6. Chaque étape se termine par un renvoi à une rubrique contenant de plus amples informations.

**Cookie. Téléchargement des images de zoom**

Commencez par télécharger vos images de zoom vers Scene7 Publishing System. Pour un zoom optimal, Dynamic Media Classic recommande que les images soient au moins 2 000 pixels dans la dimension la plus longue.

Sélectionnez le bouton Télécharger sur la barre de navigation globale pour télécharger des images depuis votre ordinateur ou votre réseau dans un dossier de Scene7 Publishing System (voir [Téléchargement des images de zoom](uploading-zoom-images.md#uploading_zoom_images)).

**2. Création de cibles de zoom pour un zoom guidé**

Les cibles de zoom vous permettent de mettre en valeur des sections particulières d’une image. Vous pouvez, par exemple, attirer l’attention des utilisateurs sur les sections d’une image qui la caractérisent ou la distinguent. Les cibles de zoom s’affichent sous la forme de miniatures, à côté de l’image, dans la fenêtre de la visionneuse de zoom. La sélection d’une de ces miniatures de cible de zoom permet d’effectuer un zoom automatique sur la section de l’image que vous définissez.

Pour créer une cible de zoom, cliquez sur le bouton de survol Modifier et choisissez Cibles de zoom ou ouvrez une image dans le panneau de navigation en mode Affichage des détails, puis cliquez sur Cibles de zoom. Utilisez ensuite les outils de zoom disponibles sur l’écran de l’éditeur de cible de zoom pour définir une partie de l’image comme cible (voir [Création de cibles de zoom pour un zoom guidé](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom)).

**Cookie. Configuration des paramètres prédéfinis de la visionneuse de zoom**

Les paramètres prédéfinis de visionneuse de zoom déterminent le style et le comportement des visionneuses de zoom. Vous pouvez configurer les paramètres prédéfinis de la visionneuse de zoom si vous êtes un administrateur ; Dynamic Media Classic est fourni avec des paramètres prédéfinis par défaut « meilleures pratiques ».

Pour créer un paramètre prédéfini de visionneuse de zoom, cliquez sur le bouton Configuration dans la barre de navigation globale et choisissez Paramètres prédéfinis de la visionneuse. Ensuite, sur l’écran Paramètres prédéfinis de la visionneuse, cliquez sur le bouton Ajouter, choisissez une plate-forme, choisissez une visionneuse de zoom, puis cliquez sur Ajouter. Ensuite, sélectionnez des options sur l’écran Configurer la visionneuse 

Dynamic Media Classic propose des options de paramètre prédéfini de visionneuse de zoom qui permettent de sélectionner le style de bouton et l'aspect global du lecteur. Vous avez également la possibilité de personnaliser les paramètres de zoom pour votre site Web (voir [Configuration des paramètres prédéfinis de la visionneuse de zoom](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets)).

**4. Prévisualisation des images avec la visionneuse de zoom**

Vous pouvez prévisualiser des images dans une visionneuse de zoom afin de vérifier le résultat obtenu lorsque vous effectuez un zoom sur les images.

Pour faire des essais avec divers paramètres prédéfinis de visionneuse de zoom, choisissez une image dans le panneau de navigation, puis cliquez sur le bouton Prévisualiser. L’écran Prévisualiser s’ouvre. Choisissez la commande Paramètres prédéfinis &gt; Zoom, puis sélectionnez un paramètre prédéfini avec les menus Zoom.

Les boutons de zoom apparaissent. Vous pouvez alors vérifier l’aspect des images de zoom sur votre site Web. Sélectionnez les boutons de zoom (et les cibles de zoom) pour tester le paramètre prédéfini de visionneuse de zoom choisi (voir [Prévisualisation d’images avec différentes visionneuses de zoom](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers)).

**5. Publication des images de zoom**

Lorsque vous publiez vos images de zoom, elles sont placées sur les serveurs Dynamic Media Image Server afin de pouvoir être diffusées sur votre site Web et dans votre application. Scene7 Publishing System active des chaînes URL dans le cadre du processus de publication. Ces chaînes URL permettent d'invoquer les images de zoom dynamique des serveurs d'images de médias dynamiques vers votre site Web ou votre application.

Cliquez sur le bouton Publier de la barre de navigation globale pour lancer une publication. Dans l’écran de publication qui s’affiche, cliquez sur le bouton Lancer publication (voir [Publication des images de zoom](publishing-zoom-images.md#publishing_zoom_images)).

**6. Liaison des visionneuses de zoom à une page Web**

Dynamic Media Classic crée les chaînes d'appel URL nécessaires pour effectuer un zoom sur les images et les active lorsque vous publiez des images sur les serveurs d'images dynamiques de médias. Vous pouvez copier ces chaînes URL depuis l’écran Prévisualiser. Une fois copiées, les chaînes URL peuvent être utilisées dans vos applications et sur vos sites Web (voir [Liaison des visionneuses de zoom à une page Web](linking-zoom-viewers-web-pages.md#linking_zoom_viewers_to_your_web_pages)).
