---
title: Bonne pratique pour l’utilisation de la visionneuse de vidéos HTML5
description: Découvrez les bonnes pratiques relatives à l’utilisation de la visionneuse de vidéos HTML5.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: ce49e4ce-8dc0-41e1-865a-249f23757553
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T17:39:23.475Z'
TQID: 'https://experienceleague.adobe.com/wGnoHGEOQLVV-rnoKBOE8wzphK3VaM-vr9YB1Y-gT8c'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 499
ht-degree: 8%

---

# Recommandations relatives à l’utilisation de la visionneuse de vidéos HTML5{#best-practice-using-the-html-video-viewer}

Les paramètres prédéfinis de la visionneuse de vidéos Adobe Dynamic Media Classic HTML5 sont des lecteurs vidéo fiables. En ce qui concerne la conception du lecteur, vous pouvez créer l’ensemble des fonctionnalités du lecteur vidéo à l’aide d’outils de développement web standard. Vous pouvez, par exemple, concevoir les boutons, les commandes et les affiches personnalisées en arrière-plan au moyen du code HTML5 et CSS afin de mieux cibler les utilisateurs avec un aspect personnalisé.

En ce qui concerne la lecture, la visionneuse détecte automatiquement les fonctionnalités vidéo du navigateur. Il diffuse ensuite la vidéo en utilisant HLS (HTTP Live Streaming), également appelé diffusion en continu de vidéo adaptative. Si cette méthode de diffusion n’est pas présente, HTML5 progressive est utilisé à la place.

En combinant dans un seul lecteur les capacités suivantes :

* Composants de lecture conçus à l’aide d’HTML5 et de CSS
* Lecture incorporée
* Utilisation de la diffusion en continu adaptative et progressive basée sur les fonctionnalités du navigateur

Vous pouvez étendre la portée de votre contenu multimédia aux utilisateurs d’ordinateurs de bureau et d’appareils mobiles. Vous garantissez également une expérience vidéo rationalisée.

Voir aussi [À propos des visionneuses HTML5](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers#viewers-for-aem-assets-only) dans le Guide de référence des visionneuses Adobe.

Voir aussi [Paramètres prédéfinis de la visionneuse](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) vidéo de formation.

## Lecture vidéo sur les ordinateurs de bureau et les appareils mobiles à l’aide de la visionneuse de vidéos Adobe Dynamic Media Classic {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

Pour la diffusion en continu de la vidéo adaptative sur un poste de travail et un appareil mobile, les vidéos utilisées pour le changement de débit reposent sur toutes les vidéos MP4 dans la visionneuse de vidéos adaptative.

La lecture vidéo se produit à l’aide d’HLS ou d’une vidéo progressive. HLS (HTTP Live Streaming) est une norme Apple pour la diffusion en continu de vidéo adaptative qui ajuste automatiquement la lecture en fonction de la capacité de bande passante du réseau. Il permet également au client ou à la cliente de « rechercher » n’importe quel point de la vidéo sans avoir à attendre que le reste de la vidéo soit téléchargé. Voir aussi [Diffusion en direct HTTP](https://developer.apple.com/streaming/). La vidéo progressive est diffusée en téléchargeant et en stockant la vidéo localement sur l’écran du bureau ou l’appareil mobile d’un utilisateur ou d’une utilisatrice.

Le tableau suivant décrit l’appareil, le navigateur et la méthode de lecture des vidéos sur les ordinateurs de bureau et les appareils mobiles à l’aide de la visionneuse de vidéos Adobe Dynamic Media Classic.

| Dispositif | Navigateur | Mode de lecture vidéo |
|--- |--- |--- |
| Bureau | Internet Explorer 9 et 10 | Téléchargement progressif. |
| Bureau | Internet Explorer 11+ | Diffusion vidéo en continu HLS. |
| Bureau | Firefox 23-44 | Téléchargement progressif. |
| Bureau | Firefox 45 ou version ultérieure | Diffusion vidéo en continu HLS. |
| Bureau | Chrome | Diffusion vidéo en continu HLS. |
| Bureau | Safari (Mac) | Diffusion vidéo en continu HLS. |
| Dispositif portable | Chrome (Android™ 6 ou version antérieure) | Téléchargement progressif. |
| Dispositif portable | Chrome (Android™ 7 ou version ultérieure) | Diffusion vidéo en continu HLS. |
| Dispositif portable | ™ (navigateur par défaut) | Téléchargement progressif. |
| Dispositif portable | Safari (iOS) | Diffusion vidéo en continu HLS. |
| Dispositif portable | Chrome (iOS) | Diffusion vidéo en continu HLS. |
| Dispositif portable | BlackBerry® | Diffusion vidéo en continu HLS. |
