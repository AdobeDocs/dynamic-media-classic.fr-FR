---
title: Présentation du programme Adobe Dynamic Media Classic
description: Une vue d’ensemble du programme Adobe Dynamic Media Classic et de l’ensemble de son processus de workflow.
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
feature: Dynamic Media Classic
role: Admin,User
exl-id: ac50cb9c-fd87-4608-80cb-8d40a0b8f131
topic: Administration
level: Beginner
source-git-commit: 1b90beb99b161b76da81403f5aed9755b3a92c8b
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 17%

---

# Présentation du programme Adobe Dynamic Media Classic{#adobe-scene-platform-overview}

Adobe Dynamic Media Classic est un environnement intégré de gestion, de publication et de service des médias riches. Il est possible de diffuser le média enrichi sur tous les canaux de distribution et de vente, notamment le Web, les supports imprimés, les campagnes par e-mail, les portails Web, les bureaux et autres dispositifs.

Voir aussi [Présentation de Platform](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/572_Platform%20Overview_converted%20renamed_Getting%20Started-AVS) vidéo de formation.

## Flux de travaux {#workflow-process}

Les étapes clés du workflow Adobe Dynamic Media Classic sont les suivantes :

* **Chargement et gestion de vos ressources** - Chargez vos ressources multimédia dans Adobe Dynamic Media Classic. Vous pouvez organiser, explorer et rechercher des fichiers sur le système. Vous pouvez également appliquer des métadonnées aux fichiers.

* **Créer un contenu multimédia** - Créez différentes configurations de vos ressources, telles que les catalogues électroniques, les visionneuses d’images, les visionneuses à 360°, les séries d’échantillons, les visionneuses de médias mixtes, les modèles de base et les modèles FXG.

* **Publier et administrer** - Publiez les ressources sur le réseau Adobe Dynamic Media Classic SaaS. Surveillez l’état des ressources lorsqu’elles sont publiées. Gérez les droits des utilisateurs et maintenez la sécurité.

* **Serve** - Diffusez du contenu multimédia depuis le réseau SaaS Adobe Dynamic Media Classic vers des pages web, des applications et des appareils mobiles ; les médias sont optimisés en termes de performances et sont fournis avec la mise en cache du réseau de diffusion de contenu. Adobe Dynamic Media Classic fournit une URL pour chaque ressource. Une fois le fichier publié, l’URL s’active.

![Processus du processus Adobe Dynamic Media Classic](/help/using/assets/gs_workflow.png)

## Images primaires uniques et appels d’URL uniques {#single-master-images-and-single-url-calls}

Adobe Dynamic Media Classic est fondamentalement différent des autres systèmes, car vous pouvez utiliser Adobe Dynamic Media Classic pour diffuser dynamiquement des médias à partir de ressources primaires uniques et d’appels d’URL.

Les chaînes d’URL que vous générez avec Adobe Dynamic Media Classic incluent des instructions qui indiquent au serveur comment afficher la ressource lorsqu’elle est diffusée. Par exemple, une même image principale peut être diffusée dans des tailles, des formats, des poids, des couleurs et des vues de zoom différents. Dans le cadre de la création et de la publication de ressources multimédias avec Adobe Dynamic Media Classic, vous configurez visuellement les effets. Ce faisant, vous créez les appels d’URL qui indiquent correctement au serveur comment présenter votre ressource principale aux applications.

![Adobe Dynamic Media Classic peut fournir la même image principale à différents supports, dans des formats et des tailles différents.](/help/using/assets/gs_dynamic_publishing.png)
*Adobe Dynamic Media Classic s’assure que des expériences de qualité cohérentes sont diffusées sur n’importe quel écran, quelle que soit la taille ou la bande passante.*

## Mise en cache du contenu {#content-caching}

Les images générées dynamiquement par Adobe Dynamic Media Classic sont favorables au cache ; il s’agit généralement d’images JPEG avec des appels d’URL uniques qui les identifient. Les images sont acheminées sur le réseau de diffusion de contenu (CDN), un système de serveurs en réseau sur Internet permettant de diffuser plus rapidement le contenu. Les images sont distribuées aux ordinateurs à partir de serveurs répartis dans le monde. Lors de l’implémentation d’un mécanisme de mise en cache à l’aide de n’importe quel fournisseur de réseau de diffusion de contenu, vous modifiez simplement le nom du serveur pour qu’il pointe vers le serveur Dynamic Media Image compatible avec le réseau de diffusion de contenu. Toutes les éditions Adobe Dynamic Media Classic incluent la mise en cache CDN groupée.
