---
title: Optimisation du référencement de la vidéo
description: Découvrez comment configurer les paramètres d’optimisation du référencement des vidéos.
uuid: bac2c6a9-8466-4b8f-b835-6cb0b4168513
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 34ecd868-775f-452b-b26e-d139f0e280ae
feature: Dynamic Media Classic
role: Administrator
exl-id: f76b0e09-f148-46aa-b710-ec35bfebcb37
translation-type: tm+mt
source-git-commit: 06bd65c92c88595786b14213944a7cebd0d2590b
workflow-type: tm+mt
source-wordcount: '1021'
ht-degree: 40%

---

# Optimisation du référencement de la vidéo{#video-seo-search-engine-optimization}

L’optimisation du référencement de la vidéo consiste à améliorer le volume de trafic vers un site Web à partir des moteurs de recherche. Les moteurs de recherche sont des outils parfaits pour collecter des informations à partir d’un contenu texte. Par contre, ils sont moins performants pour obtenir des informations sur des vidéos, sauf si ces informations leur sont fournies.

L’optimisation du référencement des vidéos Dynamic Media Classic vous permet d’appliquer des métadonnées vidéo afin de fournir aux moteurs de recherche des descriptions de vos vidéos. Dynamic Media Classic vous permet de créer des plans de site vidéo et des flux mRSS. Ces fichiers XML standard sont utilisés pour envoyer des informations sur les vidéos aux moteurs de recherche :

* **Plan de site**  vidéo : informe Google exactement où et quel est le contenu vidéo sur un site. Ainsi, les vidéos peuvent faire l&#39;objet de recherches sur Google. Par exemple, un plan de site vidéo peut préciser le temps d’exécution et la catégorie. Pour plus d’informations sur les plans de site vidéo, voir [Plans de site vidéo et alternatives aux plans de site vidéo](https://developers.google.com/search/docs/advanced/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

* **Flux**  mRSS (Media Really Simple Syndication) - Utilisé par les éditeurs de contenu pour alimenter des fichiers multimédia dans Yahoo! Video Search. Pour plus d’informations sur les flux mRSS, voir [Cartes de site vidéo et solutions de plan de site vidéo](https://developers.google.com/search/docs/advanced/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

>[!NOTE]
>
>Google prend en charge à la fois le plan de site vidéo et le protocole de flux mRSS pour envoyer des informations aux moteurs de recherche.

Dynamic Media Classic peut générer des plans de site vidéo et des flux mRSS à partir de métadonnées stockées avec chaque vidéo. Lorsque vous créez des plans de site vidéo et des flux mRSS, vous choisissez les champs de métadonnées à partir des fichiers vidéo à inclure. Ainsi, vous décrivez vos vidéos aux moteurs de recherche pour qu’ils puissent plus facilement rediriger le trafic vers les vidéos de votre site Web.

>[!NOTE]
>
>avant de créer un plan de site vidéo ou un flux mRSS, cherchez quels champs sont nécessaires au moteur de recherche dans le fichier XML et comment les structurer. Pour qu’un plan de site vidéo ou un flux mRSS soit réussi, il doit répondre aux exigences du moteur de recherche.

Dynamic Media Classic crée des rapports sur les plans de site vidéo et les flux mRSS après leur génération. Ces rapports sont disponibles sur la page Rapport d’optimisation du référencement des vidéos.

>[!NOTE]
>
>Pour les plans de site vidéo et les flux mRSS, Dynamic Media Classic capture uniquement les métadonnées des vidéos marquées pour publication. Les vidéos marquées pour la publication incluent leurs métadonnées dans les plans de site vidéo et les flux mRSS.

## Choix des paramètres d’optimisation du référencement de la vidéo {#choosing-video-seo-settings}

Cliquez sur Paramètres d’optimisation du référencement de la vidéo pour les plans de site vidéo et les flux mRSS sur la page **[!UICONTROL Paramètres d’optimisation du moteur de recherche vidéo]**. Pour ouvrir cette page, dans la barre de navigation globale, cliquez sur **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Optimisation du référencement de la vidéo]** > **[!UICONTROL Paramètres]**.

Dans la zone **[!UICONTROL Paramètres généraux]**, choisissez de générer des plans de site vidéo, des flux mRSS ou les deux. Dans la zone **[!UICONTROL Paramètres de génération]**, mappez les champs de métadonnées aux champs d’entrée.

Après avoir choisi les paramètres, cliquez sur **[!UICONTROL Enregistrer]** (ou **[!UICONTROL Enregistrer et générer]**) pour créer le plan de site vidéo, les flux mRSS ou les deux.

### Choix des paramètres généraux {#choosing-general-settings}

Dans la liste déroulante **[!UICONTROL Mode de génération]**, choisissez un mode de rapport :

* **Plan**  de site vidéo : créez un plan de site vidéo.

* **Flux**  mRSS - Créez un flux Media RSS (mRSS).

* **Les deux**  : créez les deux types de fichiers XML.

* **Désactivé**  : pour arrêter de générer des plans de site vidéo et des flux Media RSS (mRSS), sélectionnez cette option.

Dans la liste déroulante **[!UICONTROL Mode automatique/manuel]**, choisissez de générer automatiquement ou manuellement :

* **Mode**  automatique - Dynamic Media Classic génère automatiquement un plan de site vidéo, un flux Media RSS (mRSS), ou les deux, chaque jour. Sélectionnez l’option Marquer pour publication pour marquer automatiquement pour publication le fichier XML généré par Dynamic Media Classic.

   * **Marquer pour** PublishMarks pour publication du fichier XML généré.

* **Mode**  manuel - Dynamic Media Classic génère le plan de site vidéo, le flux Media RSS (mRSS) ou les deux, lorsque vous cliquez sur Générer ou sur Enregistrer et générer dans l’écran Paramètres d’optimisation de la recherche vidéo. Sélectionnez également ces options :

   * **Aucun autre paramètre**  : ne marque pas pour publication le fichier XML généré.

   * **Marquer pour publication**  - Marque pour publication le fichier XML généré.

   * **Autoriser la génération**  partielle : les moteurs de recherche peuvent rejeter un fichier XML s’il ne contient pas d’informations de métadonnées complètes pour toutes les vidéos. Cette option génère le fichier XML même si les métadonnées ne sont pas disponibles pour certaines vidéos. Un avertissement est enregistré dans l’écran de rapport. Sélectionnez cette option si vous essayez d’exporter le fichier XML et complétez les informations manquantes manuellement.

### Choix des paramètres de génération  {#choosing-generation-settings}

La zone Paramètres de génération liste les champs d’entrée pour le plan de site vidéo, ou le flux mRSS, ou les deux, et dans le panneau Métadonnées, les noms des champs de métadonnées. Utilisez la zone Paramètres généraux pour mapper les champs d’entrée aux champs de métadonnées. Ce faisant, vous indiquez à Dynamic Media Classic où obtenir les métadonnées pour le plan de site vidéo et/ou le flux mRSS.

1. Dans le menu Vues des métadonnées, choisissez un affichage de métadonnées. Après avoir choisi un affichage, les noms des champs de métadonnées apparaissent dans le panneau Métadonnées.
Voir [Vues des métadonnées](application-setup.md#metadata_views).
1. Faites glisser les noms de champ de métadonnées du panneau Métadonnées dans les champs de saisie Page de destination, Titre, Description, Balises et Catégorie. Les champs Page de destination, Titre et Description sont obligatoires.

   >[!NOTE]
   >
   >vous pouvez également saisir manuellement les données dans les champs d’entrée.

1. Effectuez l’une des opérations suivantes :

   * Pour enregistrer vos paramètres sans générer le fichier XML, cliquez sur **[!UICONTROL Enregistrer]**.
   * Pour enregistrer et générer le fichier, cliquez sur **[!UICONTROL Enregistrer et générer]**.

      Le fichier XML est généré et enregistré dans le journal de la tâche. Les fichiers de plan de site vidéo (plan de site-vidéo) et de flux Media RSS (mRSS) sont enregistrés dans le dossier racine de votre entreprise.

>[!NOTE]
>
>Publiez le plan de site vidéo ou le flux mRSS avant de l’envoyer aux moteurs de recherche. Les fichiers de plan de site vidéo et de flux Media RSS (mRSS) sont stockés dans le dossier racine de l’entreprise. Si nécessaire, marquez ces fichiers XML pour publication, puis cliquez sur **[!UICONTROL Publier]**.

## Envoi des fichiers de plan de site vidéo et de flux mRSS aux moteurs de recherche {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

Les fichiers de plan de site vidéo et de flux Media RSS (mRSS) sont stockés dans le dossier racine de l’entreprise :

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

Copiez l’une de ces URL dans les outils de l’administrateur Web du moteur de recherche pour envoyer votre fichier de plan de site vidéo ou de flux Media RSS (mRSS) aux moteurs de recherche.

## Affichage des rapports d’optimisation du référencement des vidéos  {#viewing-video-seo-reports}

Vue des rapports d’optimisation du référencement des vidéos sur la page de rapport d’optimisation du référencement des vidéos. Pour ouvrir cette page, dans la barre de navigation globale, cliquez sur **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Optimisation du référencement de la vidéo]** > **[!UICONTROL Rapports]**.

Si des erreurs se sont produites lors de la génération d’un rapport, elles sont répertoriées sur la page Rapport.
