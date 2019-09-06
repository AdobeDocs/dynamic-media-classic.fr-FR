---
title: '"Meilleure pratique : Utilisation de la visionneuse de vidéos HTML5"'
seo-title: '"Meilleure pratique : Utilisation de la visionneuse de vidéos HTML5"'
description: 'null'
seo-description: Découvrez les meilleures pratiques relatives à l'utilisation de la visionneuse de vidéos HTML 5.
uuid: 3 c 8924 dc -7 bea -4 c 25-b 77 b -005 f 57 b 71 b 64
contentOwner: admin
content-type: référence
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/video
discoiquuid: 4 b 11 cab 7-88 cf -42 dd -8554-2 eea 530753 bb
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Meilleure pratique : Utilisation de la visionneuse de vidéos HTML5{#best-practice-using-the-html-video-viewer}

Les paramètres prédéfinis de visionneuse vidéo HTML 5 Dynamic Media Classic sont des lecteurs vidéo fiables. En ce qui concerne la conception du lecteur, vous pouvez créer toutes les fonctionnalités du lecteur vidéo à l'aide d'outils de développement Web standard. Vous pouvez, par exemple, concevoir les boutons, les commandes et les affiches personnalisées en arrière-plan au moyen du code HTML5 et CSS afin de mieux cibler les utilisateurs avec un aspect personnalisé.

En ce qui concerne la lecture, la visionneuse, détecte automatiquement les fonctionnalités vidéo du navigateur. Il diffuse ensuite la vidéo à l'aide de HLS (diffusion de vidéo adaptative). Ou, si cette méthode de livraison n'est pas présente, le progressif HTML 5 est utilisé à la place.

En combinant dans un lecteur unique la capacité de concevoir les composants de lecture à l’aide de code HTML5 et CSS, d’avoir accès à la lecture incorporée et d’utiliser les flux continus adaptatifs et progressifs selon la capacité du navigateur, vous pouvez étendre la portée de votre contenu multimédia aux utilisateurs d’appareils mobiles et d’ordinateurs de bureau et garantir ainsi une expérience vidéo rationalisée.

Voir aussi [A propos des visionneuses HTML 5](https://marketing.adobe.com/resources/help/en_US/s7/viewers_ref/c_html5_viewers_about.html) dans le guide de référence des visionneuses Adobe.

## Lecture de vidéos sur les ordinateurs de bureau et les périphériques mobiles à l'aide de la visionneuse vidéo Classic Media Classic {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

Pour la diffusion en flux continu de vidéo adaptative pour ordinateur de bureau et mobile, les vidéos utilisées pour le changement de débit sont basées sur toutes les vidéos MP 4 dans la visionneuse de vidéos adaptative.

La lecture vidéo se produit à l'aide de HLS ou vidéo progressive. HLS (HTTP Live Streaming) est une norme Apple de diffusion en flux continu de vidéo adaptative qui ajuste automatiquement la lecture en fonction de la capacité de la bande passante du réseau. Il permet également au client de rechercher un point dans la vidéo sans avoir à attendre le téléchargement du reste de la vidéo (voir également Diffusion [en flux](#UnresolvedLink-https://developer.apple.com/streaming/)continu HTTP). La vidéo progressive est diffusée en téléchargeant et en stockant la vidéo localement sur l'écran de bureau ou le périphérique mobile d'un utilisateur.

Le tableau suivant décrit l'appareil, le navigateur et la méthode de lecture des vidéos sur les ordinateurs de bureau et les périphériques mobiles à l'aide de la visionneuse de vidéos Classic Media Classic.

| Dispositif | Navigateur | Mode lecture vidéo |
|--- |--- |--- |
| Deskop | Internet Explorer 9 et 10 | Téléchargement progressif. |
| Bureau | Internet Explorer 11 + | Diffusion vidéo HLS. |
| Bureau | Firefox 23-44 | Téléchargement progressif. |
| Bureau | Firefox 45 ou une version ultérieure | Diffusion vidéo HLS. |
| Bureau | Chrome | Diffusion vidéo HLS. |
| Bureau | Safari (Mac) | Diffusion vidéo HLS. |
| Dispositif portable | Chrome (Android 6 ou version antérieure) | Téléchargement progressif. |
| Dispositif portable | Chrome (Android 7 ou version ultérieure) | Diffusion vidéo HLS. |
| Dispositif portable | Android (navigateur par défaut) | Téléchargement progressif. |
| Dispositif portable | Safari (ios) | Diffusion vidéo HLS. |
| Dispositif portable | Chrome (ios) | Diffusion vidéo HLS. |
| Dispositif portable | Blackberry | Diffusion vidéo HLS. |
