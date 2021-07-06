---
title: Présentation du programme Adobe Dynamic Media Classic
description: Présentation du programme Dynamic Media Classic et du processus de workflow.
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
feature: Dynamic Media Classic
role: Admin,User
exl-id: ac50cb9c-fd87-4608-80cb-8d40a0b8f131
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 30%

---

# Présentation du programme Adobe Dynamic Media Classic{#adobe-scene-platform-overview}

Dynamic Media Classic est un environnement intégré de gestion, de publication et de service des médias riches. Il est possible de diffuser le média enrichi sur tous les canaux de distribution et de vente, notamment le Web, les supports imprimés, les campagnes par e-mail, les portails Web, les bureaux et autres dispositifs.

## Flux de travaux {#workflow-process}

Les principales étapes du processus Dynamic Media Classic sont les suivantes :

* **Charger et gérer vos ressources**  : téléchargez vos ressources multimédia vers Dynamic Media Classic. Vous pouvez organiser, explorer et rechercher des fichiers sur le système. Vous pouvez également appliquer des métadonnées aux fichiers.

* **Créer un média enrichi**  : créez différentes configurations de vos ressources telles que des catalogues électroniques, des visionneuses d’images, des visionneuses à 360°, des séries d’échantillons, des visionneuses de médias mixtes, des modèles de base et des modèles FXG.

* **Publier et administrer**  - Publiez des ressources sur le réseau SaaS de Dynamic Media Classic, ainsi que surveillez l’état des ressources lorsqu’elles sont publiées, administrez les droits d’utilisateur et maintenez la sécurité.

* **Service**  : diffuser du contenu multimédia du réseau SaaS de Dynamic Media Classic vers des pages web, des applications et des appareils mobiles ; les médias sont optimisés en termes de performances et sont fournis avec la mise en cache CDN. Dynamic Media Classic fournit une URL pour chaque ressource. Une fois le fichier publié, l’URL s’active.

![Processus de workflow Dynamic Media Classic](/help/assets/gs_workflow.png)

## Images originales uniques et appels d’URL uniques {#single-master-images-and-single-url-calls}

Dynamic Media Classic est fondamentalement différent des autres systèmes, car vous pouvez utiliser Dynamic Media Classic pour diffuser dynamiquement des médias à partir de ressources maître uniques et d’appels URL.

Les chaînes d’URL que vous générez avec Dynamic Media Classic incluent des instructions qui indiquent au serveur comment afficher la ressource lorsqu’elle est diffusée. Par exemple, il est possible de mettre à disposition une même image originale selon des tailles, formats, poids, couleurs et vues de zoom différents. Dans le cadre de la création et de la publication de ressources multimédias avec Dynamic Media Classic, vous configurez visuellement les effets. Ainsi, vous créez les appels d’URL qui indiquent correctement au serveur les modalités de présentation du fichier original dans les applications.

![Dynamic Media Classic peut fournir la même image originale à différents supports, dans des formats et des tailles différents.](/help/assets/gs_dynamic_publishing.png)
*Dynamic Media Classic garantit que des expériences de qualité cohérentes sont diffusées sur n’importe quel écran, quelle que soit la taille ou la bande passante.*

## Mise en cache du contenu {#content-caching}

Les images générées dynamiquement par Dynamic Media Classic sont compatibles avec le cache. il s’agit généralement d’images JPEG avec des appels d’URL uniques qui les identifient. Les images sont acheminées sur le réseau de diffusion de contenu (CDN), un système de serveurs en réseau sur Internet permettant de diffuser plus rapidement le contenu. Les images sont distribuées aux ordinateurs à partir de serveurs répartis dans le monde. Lors de l’implémentation d’un mécanisme de mise en cache à l’aide de n’importe quel fournisseur de réseau de diffusion de contenu, vous modifiez simplement le nom du serveur pour qu’il pointe vers le serveur Dynamic Media Image compatible avec le réseau de diffusion de contenu. Toutes les éditions Dynamic Media Classic incluent la mise en cache CDN groupée.
