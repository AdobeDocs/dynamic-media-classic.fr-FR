---
title: Meilleure pratique pour l’utilisation de la visionneuse de vidéos HTML5
description: Découvrez les meilleures pratiques d’utilisation de la visionneuse de vidéos HTML5.
uuid: 3c8924dc-7bea-4c25-b77b-005f57b71b64
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 4b11cab7-88cf-42dd-8554-2eea530753bb
feature: Dynamic Media Classic, Visionneuses, Vidéo
role: Professionnel
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 25%

---


# Meilleures pratiques pour l’utilisation de la visionneuse de vidéos HTML5{#best-practice-using-the-html-video-viewer}

Les paramètres prédéfinis de la visionneuse de vidéos HTML5 Dynamic Media Classic sont des lecteurs vidéo fiables. Du côté de la conception du lecteur, vous pouvez créer toutes les fonctionnalités du lecteur vidéo à l’aide d’outils de développement Web standard. Vous pouvez, par exemple, concevoir les boutons, les commandes et les affiches personnalisées en arrière-plan au moyen du code HTML5 et CSS afin de mieux cibler les utilisateurs avec un aspect personnalisé.

En ce qui concerne la lecture, la visionneuse, détecte automatiquement les fonctionnalités vidéo du navigateur. Il diffuse ensuite la vidéo à l’aide de HLS (diffusion en flux continu de vidéo adaptative). Ou, si cette méthode de diffusion n’est pas présente, le format HTML5 progressif est utilisé à la place.

En combinant dans un lecteur unique la capacité de concevoir les composants de lecture à l’aide de code HTML5 et CSS, d’avoir accès à la lecture incorporée et d’utiliser les flux continus adaptatifs et progressifs selon la capacité du navigateur, vous pouvez étendre la portée de votre contenu multimédia aux utilisateurs d’appareils mobiles et d’ordinateurs de bureau et garantir ainsi une expérience vidéo rationalisée.

Voir aussi [A propos des visionneuses HTML5](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers.html?lang=en#viewers-for-aem-assets-only) dans le Guide de référence des visionneuses d’Adobes.

## Lecture de la vidéo sur les ordinateurs de bureau et les périphériques mobiles à l’aide de la visionneuse de vidéos Dynamic Media Classic {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

Pour la diffusion en flux continu de vidéo adaptative sur ordinateur et sur mobile, les vidéos utilisées pour le changement de débit reposent sur toutes les vidéos MP4 de la visionneuse de vidéos adaptative.

La lecture vidéo s’effectue à l’aide de HLS ou d’une vidéo progressive. HLS (HTTP Live Streaming) est une norme Apple pour la diffusion de vidéo adaptative en flux continu qui ajuste automatiquement la lecture en fonction de la capacité de la bande passante du réseau. Il permet également au client de &quot;rechercher&quot; à n’importe quel point de la vidéo sans avoir à attendre le téléchargement du reste de la vidéo. Voir aussi [HTTP Live Streaming](https://developer.apple.com/streaming/). La vidéo progressive est diffusée en téléchargeant et en stockant la vidéo localement sur l’écran de bureau ou le périphérique mobile d’un utilisateur.

Le tableau suivant décrit la méthode de lecture, de navigateur et de périphérique mobile des vidéos sur les ordinateurs de bureau et les périphériques mobiles à l’aide de la visionneuse de vidéos Dynamic Media Classic.

| Dispositif | Navigateur | Mode de lecture vidéo |
|--- |--- |--- |
| Bureau | Internet Explorer 9 et 10 | Téléchargement progressif. |
| Bureau | Internet Explorer 11+ | Diffusion vidéo en flux continu HLS. |
| Bureau | Firefox 23-44 | Téléchargement progressif. |
| Bureau | Firefox 45 ou une version ultérieure | Diffusion vidéo en flux continu HLS. |
| Bureau | Chrome | Diffusion vidéo en flux continu HLS. |
| Bureau | Safari (Mac) | Diffusion vidéo en flux continu HLS. |
| Dispositif portable | Chrome (Android 6 ou version antérieure) | Téléchargement progressif. |
| Dispositif portable | Chrome (Android 7 ou version ultérieure) | Diffusion vidéo en flux continu HLS. |
| Dispositif portable | Android (navigateur par défaut) | Téléchargement progressif. |
| Dispositif portable | Safari (iOS) | Diffusion vidéo en flux continu HLS. |
| Dispositif portable | Chrome (iOS) | Diffusion vidéo en flux continu HLS. |
| Dispositif portable | Blackberry | Diffusion vidéo en flux continu HLS. |
