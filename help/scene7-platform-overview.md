---
title: Présentation de la plate-forme Adobe Dynamic Media Classic
seo-title: Présentation de la plate-forme Adobe Dynamic Media Classic
description: 'null'
seo-description: Cette section présente la plate-forme et le processus de flux de travaux Dynamic Media Classic.
uuid: e 7 d 3 bfb 3-1 cfe -43 ea-b 862-aae 3 b 3928 c 71
contentOwner: admin
content-type: référence
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/getting_ started
discoiquuid: 2 b 134 cfa -7 f 46-4 f 5 f -959 e-b 30 aae 610 bb 9
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Présentation de la plate-forme Adobe Dynamic Media Classic{#adobe-scene-platform-overview}

Dynamic Media Classic est un environnement intégré de gestion des médias, de publication et de diffusion. Il est possible de diffuser le média enrichi sur tous les canaux de distribution et de vente, notamment le Web, les supports imprimés, les campagnes par e-mail, les portails Web, les bureaux et autres dispositifs.

## Flux de travaux {#workflow-process}

Les étapes clés de flux de travaux de Media Classic Classic sont les suivantes :

**Télécharger et gérer vos ressources** Téléchargez vos fichiers multimédia vers SPS. Vous pouvez organiser, explorer et rechercher des fichiers sur le système. Vous pouvez également appliquer des métadonnées aux fichiers. Si vous installez l’application de bureau Adobe Scene7 Publishing System, vous pouvez télécharger des fichiers et des dossiers en les faisant glisser de votre bureau vers un dossier de téléchargement.

**Création de médias enrichis** Créez différentes configurations de vos fichiers, tels que les catalogues électroniques, les visionneuses d'images, les visionneuses à 360 °, les séries d'échantillons, les visionneuses de supports variés, les modèles de base et les modèles FXG. Pour plus d’informations, voir A propos des médias enrichis.

**Publiez et gérez** les fichiers Publier sur le réseau Dynamic Media Classic Saas, et contrôlez l'état des fichiers lorsqu'ils sont publiés, administrez les droits utilisateur et gérez la sécurité.

**Diffuser Diffuser** des médias du réseau Dynamic Media Classic saas vers des pages Web, des applications et des périphériques mobiles ; Les médias sont optimisés aux performances et sont fournis avec la mise en cache CDN. Dynamic Media Classic fournit une URL pour chaque fichier. Une fois le fichier publié, l’URL s’active.

![Processus de flux de travaux Dynamic Media Classic](/help/assets/gs_workflow.png)

## Images originales uniques et appels d’URL uniques {#single-master-images-and-single-url-calls}

Dynamic Media Classic est fondamentalement différent des autres systèmes car vous pouvez utiliser Dynamic Media Classic pour diffuser dynamiquement le média à partir de fichiers originaux uniques et d'appels d'URL.

Les chaînes URL que vous générez avec Dynamic Media Classic incluent des instructions indiquant au serveur comment afficher le fichier lors de sa diffusion. Par exemple, il est possible de mettre à disposition une même image originale selon des tailles, formats, poids, couleurs et vues de zoom différents. Dans le cadre de la création et de la publication de fichiers multimédia avec Dynamic Media Classic, vous pouvez visuellement configurer les effets. Ainsi, vous créez les appels d’URL qui indiquent correctement au serveur les modalités de présentation du fichier original dans les applications.

![Dynamic Media Classic peut diffuser la même image originale à différents supports selon différents formats et tailles.](/help/assets/gs_dynamic_publishing.png)

## Mise en cache du contenu {#content-caching}

Les images générées dynamiquement par Dynamic Media Classic sont compatibles avec le cache ; dans la plupart des cas, il s'agit d'images JPEG avec des appels d'URL uniques qui les identifient. Les images sont acheminées sur le réseau de diffusion de contenu (CDN), un système de serveurs en réseau sur Internet permettant de diffuser plus rapidement le contenu. Les images sont distribuées aux ordinateurs à partir de serveurs répartis dans le monde. Lors de la mise en œuvre d'un mécanisme de mise en cache utilisant un fournisseur CDN, vous devez simplement modifier le nom du serveur pour qu'il pointe vers le serveur Dynamic Media Image Server compatible CDN. Toutes les éditions Dynamic Media Classic comprennent une mise en cache CDN intégrée.
