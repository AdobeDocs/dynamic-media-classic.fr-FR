---
title: Présentation de la plate-forme Adobe Dynamic Media Classic
description: Présentation de la plateforme et du processus Dynamic Media Classic.
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
feature: Dynamic Media Classic
role: Administrator,Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 32%

---


# Présentation de la plate-forme Adobe Dynamic Media Classic{#adobe-scene-platform-overview}

Dynamic Media Classic est un environnement intégré de gestion, de publication et de diffusion des médias enrichis. Il est possible de diffuser le média enrichi sur tous les canaux de distribution et de vente, notamment le Web, les supports imprimés, les campagnes par e-mail, les portails Web, les bureaux et autres dispositifs.

## Flux de travaux  {#workflow-process}

Les étapes clés du processus Dynamic Media Classic sont les suivantes :

* **Téléchargez et gérez vos**
fichiersTéléchargez vos fichiers multimédias vers Dynamic Media Classic. Vous pouvez organiser, explorer et rechercher des fichiers sur le système. Vous pouvez également appliquer des métadonnées aux fichiers.

* **Créer des**
médias enrichisCréez différentes configurations de vos fichiers, telles que des catalogues électroniques, des visionneuses d’images, des visionneuses à 360°, des séries d’échantillons, des visionneuses de supports variés, des modèles de base et des modèles FXG. Pour plus d’informations, voir A propos des médias enrichis.

* **Publiez et**
administrezPubliez des fichiers sur le réseau Dynamic Media Classic Saas, et contrôlez leur état lors de leur publication, administrez les droits d’utilisateur et maintenez la sécurité.

* ****
ServeFourniture de médias du réseau Dynamic Media Classic SaaS vers des pages Web, des applications et des périphériques mobiles ; les médias sont optimisés en termes de performances et sont fournis avec la mise en cache CDN. Dynamic Media Classic fournit une URL pour chaque fichier. Une fois le fichier publié, l’URL s’active.

![Processus Dynamic Media Classic](/help/assets/gs_workflow.png)

## Images originales uniques et appels d’URL uniques {#single-master-images-and-single-url-calls}

Dynamic Media Classic est fondamentalement différent des autres systèmes, car vous pouvez utiliser Dynamic Media Classic pour diffuser du contenu multimédia de manière dynamique à partir de fichiers originaux uniques et d’appels d’URL.

Les chaînes URL que vous générez avec Dynamic Media Classic incluent des instructions qui indiquent au serveur comment afficher le fichier lors de sa diffusion. Par exemple, il est possible de mettre à disposition une même image originale selon des tailles, formats, poids, couleurs et vues de zoom différents. Dans le cadre de la création et de la publication de fichiers multimédias avec Dynamic Media Classic, vous configurez visuellement les effets. Ainsi, vous créez les appels d’URL qui indiquent correctement au serveur les modalités de présentation du fichier original dans les applications.

![Dynamic Media Classic peut fournir la même image originale à différents supports, dans des tailles et des formats différents.](/help/assets/gs_dynamic_publishing.png)

## Mise en cache du contenu {#content-caching}

Les images générées dynamiquement par Dynamic Media Classic sont compatibles avec le cache ; dans la plupart des cas, il s’agit d’images JPEG avec des appels d’URL uniques qui les identifient. Les images sont acheminées sur le réseau de diffusion de contenu (CDN), un système de serveurs en réseau sur Internet permettant de diffuser plus rapidement le contenu. Les images sont distribuées aux ordinateurs à partir de serveurs répartis dans le monde. Lors de l’implémentation d’un mécanisme de mise en cache à l’aide de n’importe quel fournisseur CDN, il vous suffit de modifier le nom du serveur pour pointer vers le serveur Dynamic Media Image Server compatible CDN. Toutes les éditions Dynamic Media Classic incluent une mise en cache CDN intégrée.
