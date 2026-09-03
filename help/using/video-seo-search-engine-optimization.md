---
title: Optimisation du référencement de la vidéo
description: Découvrez comment configurer les paramètres d’optimisation du moteur de recherche (SEO) vidéo dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
feature: Dynamic Media Classic
role: Admin
exl-id: f76b0e09-f148-46aa-b710-ec35bfebcb37
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T20:17:45.884Z'
TQID: 'https://experienceleague.adobe.com/I9wTnanImSLtXv4Nff2uW92cNkMhoGf5hc8cXsPFNYc'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: c2296997-5d79-4905-b32e-99b5aa892429id: cdd65e7e-8839-44a2-bc21-0e03623b5dd1
source-git-commit: 66b6e10c324d5b154cd39146b5a129f36aa55622
workflow-type: tm+mt
source-wordcount: 1042
ht-degree: 22%

---

# Optimisation du référencement de la vidéo{#video-seo-search-engine-optimization}

L’optimisation du moteur de recherche est le processus d’amélioration du volume de trafic vers un site web à partir des moteurs de recherche. Bien que les moteurs de recherche soient efficaces pour collecter des informations sur le contenu textuel, ils ne peuvent pas traiter correctement les informations vidéo. Ces renseignements doivent leur être fournis.

Pour fournir aux moteurs de recherche des descriptions de vos vidéos, utilisez l’optimisation du moteur de recherche des vidéos Adobe Dynamic Media Classic pour appliquer des métadonnées vidéo. Adobe Dynamic Media Classic vous permet de créer des plans de site vidéo et des flux mRSS. Ces fichiers XML standard sont utilisés pour envoyer des informations vidéo aux moteurs de recherche :

* **Plan de site vidéo** : indique à Google où et quel est le contenu vidéo sur un site. Les vidéos sont entièrement consultables sur Google. Par exemple, un plan de site vidéo peut préciser le temps d’exécution et la catégorie. Pour plus d’informations sur les plans de site vidéo, voir [ Plans de site vidéo et alternatives aux plans de site vidéo ](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&rd=1).

* Flux **mRSS (Media Really Simple Syndication)** : utilisé par les éditeurs de contenu pour alimenter Yahoo en fichiers multimédias ! Video Search. Pour plus d’informations sur les flux RSS, voir [Plans de site vidéo et alternatives aux plans de site vidéo](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&rd=1).

>[!NOTE]
>
>Google prend en charge à la fois le plan de site vidéo et le protocole de flux mRSS pour envoyer des informations aux moteurs de recherche.

Adobe Dynamic Media Classic peut générer des plans de site vidéo et des flux mRSS à partir des métadonnées stockées avec chaque vidéo. Lorsque vous créez des plans de site vidéo et des flux mRSS, vous choisissez les champs de métadonnées à partir des fichiers vidéo à inclure. Vous décrivez vos vidéos aux moteurs de recherche afin que ceux-ci puissent diriger plus précisément le trafic vers les vidéos de votre site web.

>[!NOTE]
>
>Avant de créer un plan de site vidéo ou un flux mRSS, déterminez les champs dont le moteur de recherche a besoin dans le fichier XML et comment structurer ces champs. Pour qu’un plan de site vidéo ou un flux mRSS soit réussi, il doit répondre aux exigences du moteur de recherche.

Adobe Dynamic Media Classic crée des rapports sur les plans de site vidéo et les flux mRSS après les avoir générés. Ces rapports sont disponibles sur la page Rapport d’optimisation pour les moteurs de recherche vidéo .

>[!NOTE]
>
>Pour les plans de site vidéo et les flux mRSS, Adobe Dynamic Media Classic capture les métadonnées uniquement des vidéos marquées pour publication. Marquez les vidéos à publier afin d’inclure leurs métadonnées dans les plans de site vidéo et les flux mRSS.

## Choisir les paramètres d’optimisation du moteur de recherche (SEO) vidéo

Sélectionnez les paramètres d’optimisation du moteur de recherche vidéo pour les plans de site vidéo et les flux mRSS sur la page **[!UICONTROL Paramètres d’optimisation du moteur de recherche vidéo]**. Pour ouvrir cette page, sur la barre de navigation générale, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Optimisation du moteur de recherche vidéo]** > **[!UICONTROL Paramètres]**.

Dans la zone **[!UICONTROL Paramètre général]**, choisissez de générer des plans de site vidéo, des flux mRSS ou les deux. Pour mapper les champs de métadonnées aux champs d’entrée, utilisez la zone **[!UICONTROL Paramètres de génération]**.

Après avoir choisi les paramètres, sélectionnez **[!UICONTROL Enregistrer]** (ou **[!UICONTROL Enregistrer et générer]**) pour créer le plan de site vidéo, les flux RSS ou les deux.

### Configurer les paramètres généraux {#choosing-general-settings}

Dans la liste déroulante **[!UICONTROL Mode de génération]**, choisissez un mode de rapport :

* **Plan de site vidéo** : créez un plan de site vidéo.

* **flux mRSS** : créez un flux RSS pour les médias (mRSS).

* **Les deux** : créez les deux types de fichiers XML.

* **Désactivé** : pour arrêter la génération de plans de site vidéo et de flux RSS multimédia (mRSS), sélectionnez cette option.

Dans la liste déroulante **[!UICONTROL Mode automatique/manuel]**, choisissez de générer automatiquement ou manuellement :

* **Mode automatique** : Adobe Dynamic Media Classic génère automatiquement un plan de site vidéo, un flux RSS pour les médias (mRSS) ou les deux, tous les jours. Sélectionnez l’option **[!UICONTROL Marquer pour publication]** pour marquer les fichiers XML générés par Adobe Dynamic Media Classic pour la publication.

  * **Marquer pour publication** marque pour publication le fichier XML généré.

* **Mode manuel** : Adobe Dynamic Media Classic génère le plan de site vidéo, le flux RSS du média (mRSS) ou les deux, lorsque vous sélectionnez **[!UICONTROL Générer]** ou **[!UICONTROL Enregistrer et générer]** dans l’écran Paramètres d’optimisation du moteur de recherche vidéo. Configurez également ces options :

  * **Aucun autre paramètre** : ne marque pas pour publication le fichier XML généré.

  * **Marquer pour publication** : marque pour publication le fichier XML généré.

  * **Autoriser la génération partielle** : les moteurs de recherche peuvent rejeter un fichier XML s’il ne contient pas d’informations de métadonnées complètes pour toutes les vidéos. Cette option génère le fichier XML même si les métadonnées ne sont pas disponibles pour certaines vidéos. Un avertissement est enregistré dans l’écran de rapport. Sélectionnez cette option si vous essayez d’exporter le fichier XML et complétez les informations manquantes manuellement.

### Choix des paramètres de génération {#choosing-generation-settings}

La zone Paramètres de génération répertorie les champs de saisie du plan de site vidéo, du flux RSS ou des deux. Dans le panneau Métadonnées, les noms des champs de métadonnées sont répertoriés. Utilisez la zone Paramètres généraux pour mapper les champs d’entrée aux champs de métadonnées. Vous configurez Adobe Dynamic Media Classic pour obtenir des métadonnées pour le plan de site vidéo et/ou le flux mRSS.

1. Dans le menu Vues des métadonnées, choisissez un affichage de métadonnées. Après avoir choisi un affichage, les noms des champs de métadonnées apparaissent dans le panneau Métadonnées.
Voir [Vues des métadonnées](application-setup.md#metadata_views).
1. Faites glisser les noms de champ de métadonnées du panneau Métadonnées dans les champs de saisie Page de destination, Titre, Description, Balises et Catégorie. Les champs Page de destination, Titre et Description sont obligatoires.

   >[!NOTE]
   >
   >vous pouvez également saisir manuellement les données dans les champs d’entrée.

1. Effectuez l’une des opérations suivantes :

   * Pour enregistrer vos paramètres sans générer le fichier XML, sélectionnez **[!UICONTROL Enregistrer]**.
   * Pour enregistrer et générer le fichier, sélectionnez **[!UICONTROL Enregistrer et générer]**.

     Le fichier XML est généré et enregistré dans le journal de la tâche. Le plan de site vidéo (video-sitemap) et un flux RSS pour les médias (mRSS) (mrss-feed) sont stockés dans le dossier racine de votre entreprise.

>[!NOTE]
>
>Publiez le plan de site vidéo ou le flux RSS avant de l’envoyer aux moteurs de recherche. Les fichiers de plan de site vidéo et de flux Media RSS (mRSS) sont stockés dans le dossier racine de l’entreprise. Marquez ces fichiers XML pour publication, si nécessaire, puis sélectionnez **[!UICONTROL Publier]**.

## Envoi de fichiers de plan de site vidéo et de flux RSS à un moteur de recherche {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

Les fichiers de plan de site vidéo et de flux Media RSS (mRSS) sont stockés dans le dossier racine de l’entreprise :

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

Pour envoyer votre fichier de flux RSS de vidéos ou de médias (mRSS) aux moteurs de recherche, copiez l&#39;une de ces URL dans les outils de webmaster du moteur de recherche.

## Affichage des rapports d’optimisation du moteur de recherche (SEO) vidéo {#viewing-video-seo-reports}

Consultez les rapports d’optimisation du moteur de recherche vidéo sur la page Rapport d’optimisation du moteur de recherche vidéo . Pour ouvrir cette page, sur la barre de navigation générale, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Optimisation du moteur de recherche vidéo]** > **[!UICONTROL Rapports]**.

Si des erreurs se sont produites lors de la génération d’un rapport, elles sont répertoriées dans la page Rapport .
