---
title: Optimisation du référencement de la vidéo
description: Découvrez comment configurer les paramètres d’optimisation du référencement des vidéos dans Adobe Dynamic Media Classic.
uuid: bac2c6a9-8466-4b8f-b835-6cb0b4168513
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 34ecd868-775f-452b-b26e-d139f0e280ae
feature: Dynamic Media Classic
role: Admin
exl-id: f76b0e09-f148-46aa-b710-ec35bfebcb37
source-git-commit: cb55e09a997b9d36002c4ac429603576d52fb8bd
workflow-type: tm+mt
source-wordcount: '1037'
ht-degree: 37%

---

# Optimisation du référencement de la vidéo{#video-seo-search-engine-optimization}

L’optimisation du référencement de la vidéo consiste à améliorer le volume de trafic vers un site Web à partir des moteurs de recherche. Les moteurs de recherche sont des outils parfaits pour collecter des informations à partir d’un contenu texte. Par contre, ils sont moins performants pour obtenir des informations sur des vidéos, sauf si ces informations leur sont fournies.

L’optimisation pour les moteurs de recherche vidéo Adobe Dynamic Media Classic vous permet d’appliquer des métadonnées vidéo afin de fournir aux moteurs de recherche des descriptions de vos vidéos. Adobe Dynamic Media Classic vous permet de créer des plans de site vidéo et des flux mRSS. Ces fichiers XML standard sont utilisés pour envoyer des informations vidéo aux moteurs de recherche :

* **Plan du site vidéo** - Informe Google exactement où et quel contenu vidéo se trouve sur un site. Les vidéos peuvent donc faire l’objet de recherches complètes sur Google. Par exemple, un plan de site vidéo peut préciser le temps d’exécution et la catégorie. Pour plus d’informations sur les plans de site vidéo, voir [Cartes de site vidéo et alternatives de plans de site vidéo](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

* **Flux mRSS (Media Really Simple Syndication)** - Utilisé par les éditeurs de contenu pour alimenter des fichiers multimédia dans Yahoo! Video Search. Pour plus d’informations sur les flux mRSS, voir [Cartes de site vidéo et alternatives de plans de site vidéo](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

>[!NOTE]
>
>Google prend en charge à la fois le plan de site vidéo et le protocole de flux mRSS pour envoyer des informations aux moteurs de recherche.

Adobe Dynamic Media Classic peut générer des plans de site vidéo et des flux mRSS à partir de métadonnées stockées avec chaque vidéo. Lorsque vous créez des plans de site vidéo et des flux mRSS, vous choisissez les champs de métadonnées à partir des fichiers vidéo à inclure. Ainsi, vous décrivez vos vidéos aux moteurs de recherche pour qu’ils puissent plus facilement rediriger le trafic vers les vidéos de votre site Web.

>[!NOTE]
>
>avant de créer un plan de site vidéo ou un flux mRSS, cherchez quels champs sont nécessaires au moteur de recherche dans le fichier XML et comment les structurer. Pour qu’un plan de site vidéo ou un flux mRSS soit réussi, il doit répondre aux exigences du moteur de recherche.

Adobe Dynamic Media Classic crée des rapports sur les plans de site vidéo et les flux mRSS une fois que vous les avez générés. Ces rapports sont disponibles sur la page Rapport d’optimisation pour les moteurs de recherche vidéo .

>[!NOTE]
>
>Pour les plans de site vidéo et les flux mRSS, Adobe Dynamic Media Classic capture uniquement les métadonnées des vidéos marquées pour publication. Les vidéos marquées pour la publication incluent leurs métadonnées dans les plans de site vidéo et les flux mRSS.

## Sélection des paramètres d’optimisation du référencement vidéo {#choosing-video-seo-settings}

Sélectionnez les paramètres d’optimisation du référencement vidéo pour les plans de site vidéo et les flux mRSS dans le **[!UICONTROL Paramètres d’optimisation du moteur de recherche vidéo]** page. Pour ouvrir cette page, dans la barre de navigation globale, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL SEO vidéo]** > **[!UICONTROL Paramètres]**.

Dans le **[!UICONTROL Paramètre général]** , choisissez de générer des plans de site vidéo, des flux mRSS ou les deux. Dans le **[!UICONTROL Paramètres de génération]** zone, mappez les champs de métadonnées aux champs de saisie.

Après avoir choisi les paramètres, sélectionnez **[!UICONTROL Enregistrer]** (ou **[!UICONTROL Enregistrer et générer]**) pour créer le plan de site vidéo, les flux mRSS ou les deux.

### Configuration des paramètres généraux {#choosing-general-settings}

Sur le **[!UICONTROL Mode de génération]** , choisissez un mode de rapport :

* **Plan du site vidéo** - Création d’un plan de site vidéo.

* **Flux mRSS** - Créez un flux Media RSS (mRSS).

* **Les** - Créez les deux types de fichiers XML.

* **Off** - Pour arrêter de générer des plans de site vidéo et des flux Media RSS (mRSS), sélectionnez cette option.

Sur le **[!UICONTROL Mode automatique/manuel]** , choisissez de générer automatiquement ou manuellement la liste déroulante :

* **Mode automatique** - Adobe Dynamic Media Classic génère automatiquement un plan de site vidéo, un flux Media RSS (mRSS), ou les deux, chaque jour. Sélectionnez la **[!UICONTROL Marquer pour publication]** pour marquer automatiquement pour publication le fichier XML généré par Adobe Dynamic Media Classic.

   * **Marquer pour publication** Marque pour publication le fichier XML généré.

* **Mode manuel** - Adobe Dynamic Media Classic génère le plan de site vidéo, le flux Media RSS (mRSS), ou les deux, lorsque vous sélectionnez **[!UICONTROL Générer]** ou **[!UICONTROL Enregistrer et générer]** dans l’écran Paramètres d’optimisation de la recherche vidéo. Sélectionnez également ces options :

   * **Aucun autre paramètre** - Ne marque pas pour publication le fichier XML généré.

   * **Marquer pour publication** - Marque pour publication le fichier XML généré.

   * **Autoriser la génération partielle** - Les moteurs de recherche peuvent rejeter un fichier XML s’il ne contient pas d’informations de métadonnées complètes pour toutes les vidéos. Cette option génère le fichier XML même si les métadonnées ne sont pas disponibles pour certaines vidéos. Un avertissement est enregistré dans l’écran de rapport. Sélectionnez cette option si vous essayez d’exporter le fichier XML et complétez les informations manquantes manuellement.

### Choix des paramètres de génération {#choosing-generation-settings}

La zone Paramètres de génération répertorie les champs de saisie du plan de site vidéo, du flux mRSS ou des deux, ainsi que les noms des champs de métadonnées dans le panneau Métadonnées. Utilisez la zone Paramètres généraux pour mapper les champs d’entrée aux champs de métadonnées. Ce faisant, vous indiquez à Adobe Dynamic Media Classic où obtenir des métadonnées pour le plan de site vidéo et/ou le flux mRSS.

1. Dans le menu Vues des métadonnées, choisissez un affichage de métadonnées. Après avoir choisi un affichage, les noms des champs de métadonnées apparaissent dans le panneau Métadonnées.
Voir [Vues des métadonnées](application-setup.md#metadata_views).
1. Faites glisser les noms de champ de métadonnées du panneau Métadonnées dans les champs de saisie Page de destination, Titre, Description, Balises et Catégorie. Les champs Page de destination, Titre et Description sont obligatoires.

   >[!NOTE]
   >
   >vous pouvez également saisir manuellement les données dans les champs d’entrée.

1. Effectuez l’une des opérations suivantes :

   * Pour enregistrer vos paramètres sans générer de fichier XML, sélectionnez **[!UICONTROL Enregistrer]**.
   * Pour enregistrer et générer le fichier, sélectionnez **[!UICONTROL Enregistrer et générer]**.

      Le fichier XML est généré et enregistré dans le journal de la tâche. Les fichiers de plan de site vidéo (plan de site-vidéo) et de flux Media RSS (mRSS) sont enregistrés dans le dossier racine de votre entreprise.

>[!NOTE]
>
>Publiez le plan de site vidéo ou le flux mRSS avant de l’envoyer aux moteurs de recherche. Les fichiers de plan de site vidéo et de flux Media RSS (mRSS) sont stockés dans le dossier racine de l’entreprise. Si nécessaire, marquez ces fichiers XML pour publication, puis sélectionnez **[!UICONTROL Publier]**.

## Envoyer des fichiers plan de site vidéo et flux mRSS à un moteur de recherche {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

Les fichiers de plan de site vidéo et de flux Media RSS (mRSS) sont stockés dans le dossier racine de l’entreprise :

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

Copiez l’une de ces URL dans les outils de l’administrateur Web du moteur de recherche pour envoyer votre fichier de plan de site vidéo ou de flux Media RSS (mRSS) aux moteurs de recherche.

## Affichage des rapports d’optimisation du référencement vidéo {#viewing-video-seo-reports}

Affichez les rapports d’optimisation du référencement vidéo sur la page Rapport d’optimisation du moteur de recherche vidéo. Pour ouvrir cette page, dans la barre de navigation globale, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL SEO vidéo]** > **[!UICONTROL Rapports]**.

Si des erreurs se sont produites lors de la génération d’un rapport, elles sont répertoriées sur la page Rapport .
