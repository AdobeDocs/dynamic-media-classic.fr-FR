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
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '1022'
ht-degree: 27%

---

# Optimisation du référencement de la vidéo{#video-seo-search-engine-optimization}

L’optimisation du référencement de la vidéo consiste à améliorer le volume de trafic vers un site Web à partir des moteurs de recherche. Bien que les moteurs de recherche excellent dans la collecte d&#39;informations sur le contenu textuel, ils ne peuvent pas acquérir correctement des informations sur la vidéo. Ces renseignements doivent leur être fournis.

Grâce à l’optimisation du référencement vidéo d’Adobe Dynamic Media Classic, vous pouvez appliquer des métadonnées vidéo pour fournir aux moteurs de recherche des descriptions de vos vidéos. Adobe Dynamic Media Classic vous permet de créer des plans de site vidéo et des flux mRSS. Ces fichiers XML standard sont utilisés pour envoyer des informations vidéo aux moteurs de recherche :

* **Plan de site vidéo** : indique à Google où et quel est le contenu vidéo sur un site. Ainsi, les vidéos sont entièrement consultables sur Google. Par exemple, un plan de site vidéo peut préciser le temps d’exécution et la catégorie. Pour plus d’informations sur les plans de site vidéo, voir [&#x200B; Plans de site vidéo et alternatives aux plans de site vidéo &#x200B;](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&rd=1).

* Flux **mRSS (Media Really Simple Syndication)** : utilisé par les éditeurs de contenu pour alimenter Yahoo en fichiers multimédias ! Video Search. Pour plus d’informations sur les flux RSS, voir [Plans de site vidéo et alternatives aux plans de site vidéo](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&rd=1).

>[!NOTE]
>
>Google prend en charge à la fois le plan de site vidéo et le protocole de flux mRSS pour envoyer des informations aux moteurs de recherche.

Adobe Dynamic Media Classic peut générer des plans de site vidéo et des flux mRSS à partir des métadonnées stockées avec chaque vidéo. Lorsque vous créez des plans de site vidéo et des flux mRSS, vous choisissez les champs de métadonnées à partir des fichiers vidéo à inclure. Ainsi, vous décrivez vos vidéos aux moteurs de recherche afin que ces derniers puissent diriger plus précisément le trafic vers les vidéos de votre site Web.

>[!NOTE]
>
>avant de créer un plan de site vidéo ou un flux mRSS, cherchez quels champs sont nécessaires au moteur de recherche dans le fichier XML et comment les structurer. Pour qu’un plan de site vidéo ou un flux mRSS soit réussi, il doit répondre aux exigences du moteur de recherche.

Adobe Dynamic Media Classic crée des rapports sur les plans de site vidéo et les flux mRSS après les avoir générés. Ces rapports sont disponibles sur la page Rapport d’optimisation pour les moteurs de recherche vidéo .

>[!NOTE]
>
>Pour les plans de site vidéo et les flux mRSS, Adobe Dynamic Media Classic capture les métadonnées uniquement des vidéos marquées pour publication. Marquez les vidéos à publier afin d’inclure leurs métadonnées dans les plans de site vidéo et les flux mRSS.

## Choisir les paramètres d’optimisation du moteur de recherche (SEO) vidéo

Sélectionnez les paramètres d’optimisation du moteur de recherche vidéo pour les plans de site vidéo et les flux mRSS sur la page **[!UICONTROL Paramètres d’optimisation du moteur de recherche vidéo]**. Pour ouvrir cette page, sur la barre de navigation générale, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Optimisation du moteur de recherche vidéo]** > **[!UICONTROL Paramètres]**.

Dans la zone **[!UICONTROL Paramètre général]**, choisissez de générer des plans de site vidéo, des flux mRSS ou les deux. Dans la zone **[!UICONTROL Paramètres de génération]** mappez les champs de métadonnées aux champs de saisie.

Après avoir choisi les paramètres, sélectionnez **[!UICONTROL Enregistrer]** (ou **[!UICONTROL Enregistrer et générer]**) pour créer le plan de site vidéo, les flux RSS ou les deux.

### Configurer les paramètres généraux {#choosing-general-settings}

Dans la liste déroulante **[!UICONTROL Mode de génération]**, choisissez un mode de rapport :

* **Plan de site vidéo** : créez un plan de site vidéo.

* **flux mRSS** : créez un flux RSS pour les médias (mRSS).

* **Les deux** : créez les deux types de fichiers XML.

* **Désactivé** : pour arrêter la génération de plans de site vidéo et de flux RSS multimédia (mRSS), sélectionnez cette option.

Dans la liste déroulante **[!UICONTROL Mode automatique/manuel]**, choisissez de générer automatiquement ou manuellement :

* **Mode automatique** : Adobe Dynamic Media Classic génère automatiquement un plan de site vidéo, un flux RSS pour les médias (mRSS) ou les deux, chaque jour. Sélectionnez l’option **[!UICONTROL Marquer pour publication]** afin de marquer automatiquement pour publication le fichier XML généré par Adobe Dynamic Media Classic.

   * **Marquer pour publication** marque pour publication le fichier XML généré.

* **Mode manuel** : Adobe Dynamic Media Classic génère le plan de site vidéo, le flux RSS du média (mRSS) ou les deux, lorsque vous sélectionnez **[!UICONTROL Générer]** ou **[!UICONTROL Enregistrer et générer]** dans l’écran Paramètres d’optimisation de la recherche de vidéos. Sélectionnez également ces options :

   * **Aucun autre paramètre** : ne marque pas pour publication le fichier XML généré.

   * **Marquer pour publication** : marque pour publication le fichier XML généré.

   * **Autoriser la génération partielle** : les moteurs de recherche peuvent rejeter un fichier XML s’il ne contient pas d’informations de métadonnées complètes pour toutes les vidéos. Cette option génère le fichier XML même si les métadonnées ne sont pas disponibles pour certaines vidéos. Un avertissement est enregistré dans l’écran de rapport. Sélectionnez cette option si vous essayez d’exporter le fichier XML et complétez les informations manquantes manuellement.

### Choix des paramètres de génération {#choosing-generation-settings}

La zone Paramètres de génération répertorie les champs de saisie du plan de site vidéo, du flux RSS ou des deux. Dans le panneau Métadonnées, les noms des champs de métadonnées sont répertoriés. Utilisez la zone Paramètres généraux pour mapper les champs d’entrée aux champs de métadonnées. Ce faisant, vous indiquez à Adobe Dynamic Media Classic où obtenir les métadonnées du plan de site vidéo et/ou du flux mRSS.

1. Dans le menu Vues des métadonnées, choisissez un affichage de métadonnées. Une fois que vous avez choisi une vue, les noms des champs de métadonnées s’affichent dans le panneau Métadonnées.
Voir [Vues des métadonnées](application-setup.md#metadata_views).
1. Faites glisser les noms de champ de métadonnées du panneau Métadonnées dans les champs de saisie Page de destination, Titre, Description, Balises et Catégorie. Les champs Page de destination, Titre et Description sont obligatoires.

   >[!NOTE]
   >
   >vous pouvez également saisir manuellement les données dans les champs d’entrée.

1. Effectuez l’une des opérations suivantes :

   * Pour enregistrer vos paramètres sans générer le fichier XML, sélectionnez **[!UICONTROL Enregistrer]**.
   * Pour enregistrer et générer le fichier, sélectionnez **[!UICONTROL Enregistrer et générer]**.

     Le fichier XML est généré et enregistré dans le journal de la tâche. Les fichiers de plan de site vidéo (plan de site-vidéo) et de flux Media RSS (mRSS) sont enregistrés dans le dossier racine de votre entreprise.

>[!NOTE]
>
>Publiez le plan de site vidéo ou le flux RSS avant de l’envoyer aux moteurs de recherche. Les fichiers de plan de site vidéo et de flux Media RSS (mRSS) sont stockés dans le dossier racine de l’entreprise. Marquez ces fichiers XML pour publication, si nécessaire, puis sélectionnez **[!UICONTROL Publier]**.

## Envoi de fichiers de plan de site vidéo et de flux RSS à un moteur de recherche {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

Les fichiers de plan de site vidéo et de flux Media RSS (mRSS) sont stockés dans le dossier racine de l’entreprise :

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

Copiez l&#39;une de ces URL dans les outils de webmaster du moteur de recherche pour envoyer votre fichier de flux RSS (mRSS) de vidéos ou de médias aux moteurs de recherche.

## Affichage des rapports d’optimisation du moteur de recherche (SEO) vidéo {#viewing-video-seo-reports}

Consultez les rapports d’optimisation du moteur de recherche vidéo sur la page Rapport d’optimisation du moteur de recherche vidéo . Pour ouvrir cette page, sur la barre de navigation générale, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Optimisation du moteur de recherche vidéo]** > **[!UICONTROL Rapports]**.

Si des erreurs se sont produites lors de la génération d’un rapport, elles sont répertoriées dans la page Rapport .
