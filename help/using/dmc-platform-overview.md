---
title: Présentation du programme Adobe Dynamic Media Classic
description: Une vue d’ensemble du programme Adobe Dynamic Media Classic et de l’ensemble de son processus de workflow.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
feature: Dynamic Media Classic
role: Admin,User
exl-id: ac50cb9c-fd87-4608-80cb-8d40a0b8f131
topic: Administration
level: Beginner
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 12%

---

# Présentation du programme Adobe Dynamic Media Classic{#adobe-scene-platform-overview}

Adobe Dynamic Media Classic est un environnement intégré de gestion, de publication et de service des médias riches. Les médias riches peuvent être diffusés sur tous les canaux marketing et de vente. Ces canaux comprennent le web, le matériel d’impression, les campagnes par e-mail, les portails web, les ordinateurs de bureau et les appareils.

Voir aussi [Présentation de Platform](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/572_Platform%20Overview_converted%20renamed_Getting%20Started-AVS) vidéo de formation.

## Flux de travaux {#workflow-process}

Les étapes clés du workflow Adobe Dynamic Media Classic sont les suivantes :

* **Chargement et gestion de vos ressources**: téléchargez vos ressources multimédias vers Adobe Dynamic Media Classic. Vous pouvez organiser, explorer et rechercher des fichiers sur le système. Vous pouvez également appliquer des métadonnées aux ressources.

* **Créer un contenu multimédia**: créez différentes configurations de vos ressources, telles que des catalogues électroniques, des visionneuses d’images, des visionneuses à 360°, des séries d’échantillons, des visionneuses de médias mixtes, des modèles de base et des modèles FXG.

* **Publier et administrer**: publiez des ressources sur le réseau Adobe Dynamic Media Classic SaaS. Surveillez l’état des ressources lorsqu’elles sont publiées. Gérez les droits des utilisateurs et maintenez la sécurité.

* **Serve**: diffuser du contenu multimédia du réseau SaaS Adobe Dynamic Media Classic vers des pages web, des applications et des appareils mobiles ; les médias sont optimisés en termes de performances et sont fournis avec la mise en cache du réseau de diffusion de contenu. Adobe Dynamic Media Classic fournit une URL pour chaque ressource. Une fois le fichier publié, l’URL s’active.

![Processus du processus Adobe Dynamic Media Classic](/help/using/assets/gs_workflow.png)

## Images primaires uniques et appels d’URL uniques {#single-master-images-and-single-url-calls}

Adobe Dynamic Media Classic est fondamentalement différent des autres systèmes, car vous pouvez utiliser Adobe Dynamic Media Classic pour diffuser dynamiquement des médias à partir de ressources primaires uniques et d’appels d’URL.

Les chaînes d’URL que vous avez générées avec Adobe Dynamic Media Classic incluent des instructions qui indiquent au serveur comment afficher la ressource lorsqu’elle est diffusée. Par exemple, une même image principale peut être diffusée dans des tailles, des formats, des poids, des couleurs et des vues de zoom différents. Dans le cadre de la création et de la publication de ressources multimédias avec Adobe Dynamic Media Classic, vous pouvez visuellement configurer les effets. Ce faisant, vous créez les appels d’URL qui indiquent correctement au serveur comment présenter votre ressource principale aux applications.

![Adobe Dynamic Media Classic peut fournir la même image principale à différents supports, dans des formats et des tailles différents.](/help/using/assets/gs_dynamic_publishing.png)
*Adobe Dynamic Media Classic s’assure que des expériences de qualité cohérentes sont diffusées sur n’importe quel écran, quelle que soit la taille ou la bande passante.*

## Mise en cache du contenu {#content-caching}

Les images générées dynamiquement par Adobe Dynamic Media Classic sont favorables au cache ; il s’agit généralement d’images JPEG avec des appels d’URL uniques qui les identifient. Les images sont acheminées sur le réseau de diffusion de contenu (CDN), un système de serveurs en réseau sur Internet permettant de diffuser plus rapidement le contenu. Les images sont distribuées aux ordinateurs à partir de serveurs répartis dans le monde. Lors de l’implémentation d’un mécanisme de mise en cache à l’aide de n’importe quel fournisseur de réseau de diffusion de contenu, vous modifiez simplement le nom du serveur pour qu’il pointe vers le serveur Dynamic Media Image compatible avec le réseau de diffusion de contenu. Toutes les éditions Adobe Dynamic Media Classic incluent la mise en cache CDN groupée.
