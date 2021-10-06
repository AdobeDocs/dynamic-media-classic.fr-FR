---
title: Présentation du programme Adobe Dynamic Media Classic
description: Une vue d’ensemble du programme Adobe Dynamic Media Classic et de l’ensemble de son processus de workflow.
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
feature: Dynamic Media Classic
role: Admin,User
exl-id: ac50cb9c-fd87-4608-80cb-8d40a0b8f131
source-git-commit: 2616c067215196e8145043ba57fba1e3a5667cdc
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 25%

---

# Présentation du programme Adobe Dynamic Media Classic{#adobe-scene-platform-overview}

Adobe Dynamic Media Classic est un environnement intégré de gestion, de publication et de service des médias riches. Il est possible de diffuser le média enrichi sur tous les canaux de distribution et de vente, notamment le Web, les supports imprimés, les campagnes par e-mail, les portails Web, les bureaux et autres dispositifs.

Voir aussi [Vidéo de formation sur la présentation de la plateforme](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/572_Platform%20Overview_converted%20renamed_Getting%20Started-AVS).

## Flux de travaux {#workflow-process}

Les étapes clés du workflow Adobe Dynamic Media Classic sont les suivantes :

* **Charger et gérer vos ressources**  : téléchargez vos ressources multimédias vers Adobe Dynamic Media Classic. Vous pouvez organiser, explorer et rechercher des fichiers sur le système. Vous pouvez également appliquer des métadonnées aux fichiers.

* **Créer un média enrichi**  : créez différentes configurations de vos ressources telles que des catalogues électroniques, des visionneuses d’images, des visionneuses à 360°, des séries d’échantillons, des visionneuses de médias mixtes, des modèles de base et des modèles FXG.

* **Publier et administrer**  : publiez des ressources sur le réseau Adobe Dynamic Media Classic SaaS. Surveillez l’état des ressources lorsqu’elles sont publiées. Gérez les droits des utilisateurs et maintenez la sécurité.

* **Diffuser**  : diffuser du contenu multimédia du réseau Adobe Dynamic Media Classic SaaS vers des pages web, des applications et des appareils mobiles ; les médias sont optimisés en termes de performances et sont fournis avec la mise en cache CDN. Adobe Dynamic Media Classic fournit une URL pour chaque ressource. Une fois le fichier publié, l’URL s’active.

![Processus du processus Adobe Dynamic Media Classic](/help/assets/gs_workflow.png)

## Images originales uniques et appels d’URL uniques {#single-master-images-and-single-url-calls}

Adobe Dynamic Media Classic est fondamentalement différent des autres systèmes, car vous pouvez utiliser Adobe Dynamic Media Classic pour diffuser dynamiquement des médias à partir de ressources maître uniques et d’appels URL.

Les chaînes d’URL que vous générez avec Adobe Dynamic Media Classic incluent des instructions qui indiquent au serveur comment afficher la ressource lorsqu’elle est diffusée. Par exemple, il est possible de mettre à disposition une même image originale selon des tailles, formats, poids, couleurs et vues de zoom différents. Dans le cadre de la création et de la publication de ressources multimédias avec Adobe Dynamic Media Classic, vous configurez visuellement les effets. Ainsi, vous créez les appels d’URL qui indiquent correctement au serveur les modalités de présentation du fichier original dans les applications.

![Adobe Dynamic Media Classic peut diffuser la même image originale sur différents supports, dans des formats et des tailles différents.](/help/assets/gs_dynamic_publishing.png)
*Adobe Dynamic Media Classic s’assure que des expériences de qualité cohérentes sont diffusées sur n’importe quel écran, quelle que soit la taille ou la bande passante.*

## Mise en cache du contenu {#content-caching}

Les images générées dynamiquement par Adobe Dynamic Media Classic sont compatibles avec le cache. il s’agit généralement d’images JPEG avec des appels d’URL uniques qui les identifient. Les images sont acheminées sur le réseau de diffusion de contenu (CDN), un système de serveurs en réseau sur Internet permettant de diffuser plus rapidement le contenu. Les images sont distribuées aux ordinateurs à partir de serveurs répartis dans le monde. Lors de l’implémentation d’un mécanisme de mise en cache à l’aide de n’importe quel fournisseur de réseau de diffusion de contenu, vous modifiez simplement le nom du serveur pour qu’il pointe vers le serveur Dynamic Media Image compatible avec le réseau de diffusion de contenu. Toutes les éditions Adobe Dynamic Media Classic incluent la mise en cache CDN groupée.
