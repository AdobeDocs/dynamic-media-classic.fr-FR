---
title: Présentation de la plate-forme Adobe Dynamic Media Classic
seo-title: Présentation de la plate-forme Adobe Dynamic Media Classic
description: 'null'
seo-description: Présentation de la plate-forme et du processus de flux de travaux Dynamic Media Classic.
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: admin
content-type: référence
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Présentation de la plate-forme Adobe Dynamic Media Classic{#adobe-scene-platform-overview}

Dynamic Media Classic est un environnement intégré de gestion, de publication et de diffusion de contenu multimédia enrichi. Il est possible de diffuser le média enrichi sur tous les canaux de distribution et de vente, notamment le Web, les supports imprimés, les campagnes par e-mail, les portails Web, les bureaux et autres dispositifs.

## Flux de travaux {#workflow-process}

Les étapes clés du flux de travaux de Dynamic Media Classic sont les suivantes :

* **Téléchargez et gérez vos fichiers** Téléchargez vos fichiers multimédia vers SPS. Vous pouvez organiser, explorer et rechercher des fichiers sur le système. Vous pouvez également appliquer des métadonnées aux fichiers. Si vous installez l’application de bureau Adobe Scene7 Publishing System, vous pouvez télécharger des fichiers et des dossiers en les faisant glisser de votre bureau vers un dossier de téléchargement.

* **Créer un média** enrichi Créez différentes configurations de vos ressources, telles que des catalogues électroniques, des visionneuses d’images, des visionneuses à 360°, des séries d’échantillons, des visionneuses de supports variés, des modèles de base et des modèles FXG. Pour plus d’informations, voir A propos des médias enrichis.

* **Publiez et administrez** Publiez des fichiers sur le réseau Dynamic Media Classic Saas, contrôlez l’état des fichiers lorsqu’ils sont publiés, administrez les droits d’utilisateur et maintenez la sécurité.

* **diffuser** diffuser du contenu multimédia du réseau SaaS Dynamic Media Classic vers des pages Web, des applications et des périphériques mobiles ; les médias sont optimisés pour les performances et sont fournis avec la mise en cache CDN. Dynamic Media Classic fournit une URL pour chaque fichier. Une fois le fichier publié, l’URL s’active.

![Processus de flux de travaux de Dynamic Media Classic](/help/assets/gs_workflow.png)

## Images originales uniques et appels d’URL uniques {#single-master-images-and-single-url-calls}

Dynamic Media Classic est fondamentalement différent des autres systèmes, car vous pouvez utiliser Dynamic Media Classic pour diffuser du contenu multimédia dynamique à partir de fichiers originaux uniques et d’appels d’URL.

Les chaînes URL que vous générez avec Dynamic Media Classic incluent des instructions qui indiquent au serveur comment afficher le fichier lorsqu’il est diffusé. Par exemple, il est possible de mettre à disposition une même image originale selon des tailles, formats, poids, couleurs et vues de zoom différents. Dans le cadre de la création et de la publication de fichiers multimédia avec Dynamic Media Classic, vous configurez visuellement les effets. Ainsi, vous créez les appels d’URL qui indiquent correctement au serveur les modalités de présentation du fichier original dans les applications.

![Dynamic Media Classic permet de diffuser la même image originale sur différents supports dans différents formats et tailles.](/help/assets/gs_dynamic_publishing.png)

## Mise en cache du contenu {#content-caching}

Les images générées dynamiquement par Dynamic Media Classic sont compatibles avec le cache ; dans la plupart des cas, il s’agit d’images JPEG avec des appels d’URL uniques qui les identifient. Les images sont acheminées sur le réseau de diffusion de contenu (CDN), un système de serveurs en réseau sur Internet permettant de diffuser plus rapidement le contenu. Les images sont distribuées aux ordinateurs à partir de serveurs répartis dans le monde. Lors de l’implémentation d’un mécanisme de mise en cache à l’aide d’un fournisseur CDN, il vous suffit de modifier le nom du serveur pour qu’il pointe vers le serveur d’images Dynamic Media compatible CDN. Toutes les éditions de Dynamic Media Classic incluent la mise en cache CDN intégrée.
