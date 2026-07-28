---
title: Présentation du programme Adobe Dynamic Media Classic
description: Présentation du programme Adobe Dynamic Media Classic et de l’ensemble de son processus de workflow.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
feature: Dynamic Media Classic
role: Admin,User
exl-id: ac50cb9c-fd87-4608-80cb-8d40a0b8f131
topic: Administration
level: Beginner
autotag-review: '2026-05-13T19:46:13.313Z'
TQID: 'https://experienceleague.adobe.com/qaWxQCcT9VjPt4MmahAR3-voOpUBjYztzNFXSZG6R6k'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: ef0a24ad6af986b394d8838318fd870be66732a6
workflow-type: tm+mt
source-wordcount: 495
ht-degree: 6%

---

# Présentation du programme Adobe Dynamic Media Classic{#adobe-scene-platform-overview}

Adobe Dynamic Media Classic est un environnement intégré de gestion, de publication et de diffusion des médias riches. Les médias riches peuvent être diffusés sur tous les canaux marketing et de vente. Ces canaux comprennent le web, les documents imprimés, les campagnes par e-mail, les portails web, les ordinateurs de bureau et les appareils.

Consultez également la vidéo de formation [Présentation de Platform](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/572_Platform%20Overview_converted%20renamed_Getting%20Started-AVS).

## Flux de travaux {#workflow-process}

Les étapes clés du workflow Adobe Dynamic Media Classic sont les suivantes :

* **Charger et gérer vos ressources** : chargez vos ressources multimédias vers Adobe Dynamic Media Classic. Vous pouvez organiser, explorer et rechercher des fichiers sur le système. Vous pouvez également appliquer des métadonnées aux fichiers.

* **Créer des médias riches** : créez des configurations de ressources telles que des catalogues électroniques, des visionneuses d’images, à 360°, des visionneuses d’échantillons, des visionneuses de médias mixtes et des modèles.

* **Publier et administrer** : publiez des ressources sur le réseau SaaS Adobe Dynamic Media Classic. Surveillez le statut des ressources lorsqu’elles sont publiées. Gérez les droits des utilisateurs et maintenez la sécurité.

* **Serve** : diffusez des médias à partir du réseau SaaS Adobe Dynamic Media Classic vers des pages web, des applications et des appareils mobiles. Le média est optimisé pour les performances et est fourni avec la mise en cache CDN. Adobe Dynamic Media Classic fournit une URL pour chaque ressource. Une fois le fichier publié, l’URL s’active.

![Processus de workflow Adobe Dynamic Media Classic](/help/using/assets/gs_workflow.png)

## Images principales uniques et appels d’URL uniques {#single-master-images-and-single-url-calls}

Adobe Dynamic Media Classic se distingue des autres systèmes dans la mesure où vous pouvez utiliser Adobe Dynamic Media Classic pour diffuser dynamiquement des médias à partir de ressources principales individuelles et de requêtes d’URL.

Les chaînes d’URL que vous générez avec Adobe Dynamic Media Classic incluent des instructions indiquant au serveur comment afficher la ressource lors de sa diffusion. Par exemple, une même image principale peut être diffusée dans différentes tailles, formats, poids, couleurs ou vues. Dans le cadre de la création et de la publication de ressources multimédias avec Adobe Dynamic Media Classic, vous pouvez configurer visuellement les effets. Ce faisant, vous créez les appels d’URL qui indiquent correctement au serveur comment présenter votre ressource principale aux applications.

![Adobe Dynamic Media Classic peut diffuser la même image principale sur différents supports, dans des formats et des tailles différents.](/help/using/assets/gs_dynamic_publishing.png)
*Adobe Dynamic Media Classic garantit la cohérence et la qualité des expériences diffusées sur n’importe quel écran, quelle que soit leur taille ou leur bande passante.*

## Mise en cache du contenu {#content-caching}

Les images générées dynamiquement par Adobe Dynamic Media Classic sont adaptées à la mise en cache ; il s’agit généralement d’images JPEG avec des appels d’URL uniques qui les identifient. Les images sont diffusées sur le réseau de diffusion de contenu (CDN), un système de serveurs connectés à Internet pour diffuser plus rapidement du contenu. Les images sont distribuées à partir de serveurs situés dans le monde entier, puis vers des ordinateurs. Pour mettre en œuvre un mécanisme de mise en cache à l’aide d’un fournisseur de réseau CDN, modifiez le nom du serveur afin qu’il pointe vers le serveur d’images Dynamic Media compatible CDN. Toutes les éditions d’Adobe Dynamic Media Classic incluent la mise en cache groupée du réseau CDN.
