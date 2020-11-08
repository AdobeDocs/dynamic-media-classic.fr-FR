---
title: Optimisation du référencement de la vidéo
seo-title: Optimisation du référencement de la vidéo
description: 'null'
seo-description: Découvrez comment configurer les paramètres d’optimisation du référencement des vidéos.
uuid: bac2c6a9-8466-4b8f-b835-6cb0b4168513
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 34ecd868-775f-452b-b26e-d139f0e280ae
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '984'
ht-degree: 66%

---


# Optimisation du référencement de la vidéo{#video-seo-search-engine-optimization}

L’optimisation du référencement de la vidéo consiste à améliorer le volume de trafic vers un site Web à partir des moteurs de recherche. Les moteurs de recherche sont des outils parfaits pour collecter des informations à partir d’un contenu texte. Par contre, ils sont moins performants pour obtenir des informations sur des vidéos, sauf si ces informations leur sont fournies.

L’optimisation du référencement des vidéos dans Dynamic Media Classic vous permet d’exploiter les métadonnées vidéo pour fournir aux moteurs de recherche des descriptions de vos vidéos. Dynamic Media Classic permet de créer des plans de site vidéo et des flux mRSS. Il s’agit de fichiers XML standard utilisés pour envoyer des informations sur la vidéo aux moteurs de recherche.

**Le plan de site** vidéo informe Google exactement où et quel contenu vidéo se trouve sur un site. Par conséquent, les vidéos peuvent faire l’objet d’une recherche sur Google. Par exemple, un plan de site vidéo peut préciser le temps d’exécution et la catégorie. Pour plus d’informations sur les plans de site vidéo, voir https://www.google.com/support/webmasters/bin/answer.py?answer=80471.

**Flux** mRSS (Media Really Simple Syndication) Utilisé par les éditeurs de contenu pour alimenter des fichiers multimédia dans Yahoo! Video Search. Pour plus d’informations sur les flux mRSS, voir https://www.rssboard.org/media-rss.

>[!NOTE]
>
>Google prend en charge à la fois le plan de site vidéo et le protocole de flux mRSS pour envoyer des informations aux moteurs de recherche.

Dynamic Media Classic peut générer des plans de site vidéo et des flux mRSS à partir de métadonnées stockées avec chaque vidéo. Lorsque vous créez des plans de site vidéo et des flux mRSS, vous choisissez les champs de métadonnées à partir des fichiers vidéo à inclure. Ainsi, vous décrivez vos vidéos aux moteurs de recherche pour qu’ils puissent plus facilement rediriger le trafic vers les vidéos de votre site Web.

>[!NOTE]
>
>avant de créer un plan de site vidéo ou un flux mRSS, cherchez quels champs sont nécessaires au moteur de recherche dans le fichier XML et comment les structurer. Pour qu’un plan de site vidéo ou un flux mRSS soit réussi, il doit répondre aux exigences du moteur de recherche.

Dynamic Media Classic crée des rapports sur les plans de site vidéo et les flux mRSS après leur génération. Ces rapports sont disponibles dans l’écran Rapport d’optimisation du référencement des vidéos.

>[!NOTE]
>
>Pour les plans de site vidéo et les flux mRSS, Dynamic Media Classic capture uniquement les métadonnées des vidéos marquées pour publication. Les vidéos marquées pour la publication incluent leurs métadonnées dans les plans de site vidéo et les flux mRSS.

## Choosing video SEO settings {#choosing-video-seo-settings}

Sélectionnez les paramètres d’optimisation du référencement de la vidéo pour les plans de site vidéo et les flux mRSS dans l’écran Paramètres d’optimisation du référencement des vidéos. Pour ouvrir cet écran, choisissez Configuration > Configuration de l’application > Optimisation du référencement de la vidéo > Paramètres.

Dans la zone Paramètres généraux, choisissez de générer des plans de site vidéo, des flux mRSS ou les deux. Dans la zone Paramètres de génération, mappez les champs de métadonnées aux champs d’entrée.

Lorsque vous avez choisi les paramètres, cliquez sur Générer (ou Enregistrer et générer) pour créer le plan de site vidéo, le flux mRSS ou les deux.

### Choix des paramètres généraux {#choosing-general-settings}

Dans la liste déroulante Mode de génération, choisissez un mode de rapport :

**Plan de site** vidéo Créez un plan de site vidéo.

**Flux** mRSS Créez un flux Media RSS (mRSS).

**Les deux** créent les deux types de fichiers XML.

**Désactivé** Sélectionnez cette option pour arrêter de générer des plans de site vidéo et un flux Media RSS (mRSS).

Dans la liste déroulante Mode automatique/Mode manuel, choisissez de générer automatiquement ou manuellement :

**Le mode** automatique Contenu multimédia dynamique classique génère automatiquement un plan de site vidéo, un flux Media RSS (mRSS), ou les deux, chaque jour. Sélectionnez l’option Marquer pour publication pour marquer automatiquement pour publication le fichier XML généré par Dynamic Media Classic.

**Le mode** manuel Contenu multimédia dynamique classique génère le plan de site vidéo, le flux Media RSS (mRSS) ou les deux, lorsque vous cliquez sur Générer ou Enregistrer et générer dans l’écran Paramètres d’optimisation de la recherche vidéo. Sélectionnez également ces options :

**Aucun autre paramètre** Ne marque pas pour publication le fichier XML généré.

**Marquer pour publication** Marques pour publication du fichier XML généré.

**Autoriser la génération** partielle Les moteurs de recherche peuvent rejeter un fichier XML s’il ne contient pas d’informations de métadonnées complètes pour toutes les vidéos. Cette option génère le fichier XML même si les métadonnées ne sont pas disponibles pour certaines vidéos. Un avertissement est enregistré dans l’écran de rapport. Sélectionnez cette option si vous essayez d’exporter le fichier XML et complétez les informations manquantes manuellement.

### Choix des paramètres de génération {#choosing-generation-settings}

La zone Paramètres de génération répertorie les champs d’entrée du plan de site vidéo et/ou du flux mRSS, et, dans le panneau Métadonnées, les noms des champs de métadonnées. Utilisez la zone Paramètres généraux pour mapper les champs d’entrée aux champs de métadonnées. Ce faisant, vous indiquez à Dynamic Media Classic où obtenir les métadonnées pour le plan de site vidéo et/ou le flux mRSS.

1. Dans le menu Vues des métadonnées, choisissez un affichage de métadonnées. Après avoir choisi un affichage, les noms des champs de métadonnées apparaissent dans le panneau Métadonnées. (Pour plus d’informations sur les vues de métadonnées, voir [Vues des métadonnées](application-setup.md#metadata_views).)
1. Faites glisser les noms de champ de métadonnées du panneau Métadonnées dans les champs de saisie Page de destination, Titre, Description, Balises et Catégorie. Les champs Page de destination, Titre et Description sont obligatoires.

   >[!NOTE]
   >
   >vous pouvez également saisir manuellement les données dans les champs d’entrée.

1. Cliquez sur Enregistrer (pour enregistrer les paramètres sans générer le fichier XML), Générer (pour générer le fichier XML) ou Enregistrer et générer (pour enregistrer et générer le fichier).

   Le fichier XML est généré et enregistré dans le journal de la tâche. Les fichiers de plan de site vidéo (plan de site-vidéo) et de flux Media RSS (mRSS) sont enregistrés dans le dossier racine de votre entreprise.

>[!NOTE]
>
>vous devez publier le plan de site vidéo ou le flux mRSS avant de pouvoir l’envoyer aux moteurs de recherche. Les fichiers de plan de site vidéo et de flux Media RSS (mRSS) sont stockés dans le dossier racine de l’entreprise. Si nécessaire, marquez ces fichiers XML pour publication et cliquez sur Publier.

## Envoi des fichiers de plan de site vidéo et de flux mRSS aux moteurs de recherche {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

Les fichiers de plan de site vidéo et de flux Media RSS (mRSS) sont stockés dans le dossier racine de l’entreprise :

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

Copiez l’une de ces URL dans les outils de l’administrateur Web du moteur de recherche pour envoyer votre fichier de plan de site vidéo ou de flux Media RSS (mRSS) aux moteurs de recherche.

## Affichage des rapports d’optimisation du référencement des vidéos {#viewing-video-seo-reports}

Affichez les rapports d’optimisation du référencement des vidéos dans l’écran Rapport d’optimisation du référencement des vidéos. Pour ouvrir cet écran, cliquez sur Configuration > Configuration de l’application > Optimisation du référencement de la vidéo > Rapports.

Si une erreur se produit lors de la génération d’un rapport, elle est répertoriée dans l’écran Rapport.
