---
title: Bonne pratique pour utiliser la visionneuse de vidéos HTML5
description: Découvrez les bonnes pratiques relatives à l’utilisation de la visionneuse de vidéos HTML5.
uuid: 3c8924dc-7bea-4c25-b77b-005f57b71b64
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 4b11cab7-88cf-42dd-8554-2eea530753bb
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: ce49e4ce-8dc0-41e1-865a-249f23757553
source-git-commit: 352b1c383195fa03294ad3501207d63f3cfe3e42
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 11%

---

# Bonnes pratiques relatives à l’utilisation de la visionneuse de vidéos HTML5{#best-practice-using-the-html-video-viewer}

Les paramètres prédéfinis de la visionneuse de vidéos Adobe Dynamic Media Classic HTML5 sont des lecteurs vidéo fiables. Du côté de la conception du lecteur, vous pouvez créer l’ensemble des fonctionnalités du lecteur vidéo à l’aide d’outils de développement web standard. Vous pouvez, par exemple, concevoir les boutons, les commandes et les affiches personnalisées en arrière-plan au moyen du code HTML5 et CSS afin de mieux cibler les utilisateurs avec un aspect personnalisé.

En ce qui concerne la lecture, la visionneuse, détecte automatiquement les fonctionnalités vidéo du navigateur. Il diffuse ensuite la vidéo à l’aide de HLS (HTTP Live Streaming), également appelé diffusion en continu de vidéo adaptative. Ou, si cette méthode de diffusion n’est pas présente, HTML5 progressif est utilisé à la place.

En combinant en un seul lecteur les fonctionnalités suivantes :

* Composants de lecture conçus à l’aide de HTML5 et CSS
* Lecture incorporée
* Utilisation de la diffusion en continu adaptative et progressive en fonction des fonctionnalités du navigateur

Vous étendez la portée de votre contenu multimédia aux utilisateurs de bureau et mobiles. Vous garantissez également une expérience vidéo rationalisée.

Voir aussi [À propos des visionneuses HTML5](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers.html?lang=en#viewers-for-aem-assets-only) dans le Guide de référence des visionneuses Adobe.

Voir également la [vidéo de formation Paramètres prédéfinis de la visionneuse](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS).

## Lecture vidéo sur les ordinateurs de bureau et les appareils mobiles à l’aide de la visionneuse vidéo Adobe Dynamic Media Classic {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

Pour la diffusion en continu de la vidéo adaptative sur un poste de travail ou un appareil mobile, les vidéos utilisées pour le changement de débit reposent sur toutes les vidéos MP4 de la visionneuse de vidéos adaptative.

La lecture vidéo se produit à l’aide de la vidéo HLS ou progressive. HLS (HTTP Live Streaming) est une norme Apple pour la diffusion en continu de vidéo adaptative qui ajuste automatiquement la lecture en fonction de la capacité de bande passante du réseau. Il permet également au client de &quot;rechercher&quot; n’importe quel point de la vidéo sans avoir à attendre que le reste de la vidéo soit téléchargé. Voir aussi [HTTP Live Streaming](https://developer.apple.com/streaming/). La vidéo progressive est diffusée en téléchargeant et en stockant la vidéo localement sur l’écran de bureau ou l’appareil mobile d’un utilisateur.

Le tableau suivant décrit le périphérique, le navigateur et la méthode de lecture des vidéos sur les ordinateurs de bureau et les appareils mobiles à l’aide de la visionneuse vidéo Adobe Dynamic Media Classic.

| Dispositif | Navigateur | Mode de lecture vidéo |
|--- |--- |--- |
| Bureau | Internet Explorer 9 et 10 | Téléchargement progressif. |
| Bureau | Internet Explorer 11+ | Diffusion vidéo HLS en continu. |
| Bureau | Firefox 23-44 | Téléchargement progressif. |
| Bureau | Firefox 45 ou une version ultérieure | Diffusion vidéo HLS en continu. |
| Bureau | Chrome | Diffusion vidéo HLS en continu. |
| Bureau | Safari (Mac) | Diffusion vidéo HLS en continu. |
| Dispositif portable | Chrome (Android™ 6 ou version antérieure) | Téléchargement progressif. |
| Dispositif portable | Chrome (Android™ 7 ou version ultérieure) | Diffusion vidéo HLS en continu. |
| Dispositif portable | Android™ (navigateur par défaut) | Téléchargement progressif. |
| Dispositif portable | Safari (iOS) | Diffusion vidéo HLS en continu. |
| Dispositif portable | Chrome (iOS) | Diffusion vidéo HLS en continu. |
| Dispositif portable | BlackBerry® | Diffusion vidéo HLS en continu. |
