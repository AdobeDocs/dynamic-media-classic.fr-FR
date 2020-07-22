---
title: Activation des rapports vidéo d’Adobe Analytics
seo-title: Activation des rapports vidéo d’Adobe Analytics
description: 'null'
seo-description: Découvrez comment activer les rapports vidéo Adobe Analytics.
uuid: 078594b2-7d53-4714-8128-ff3b5c3a5e36
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 18644a53-92da-40ab-b961-318d8332c54d
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 26%

---


# Activation des rapports vidéo d’Adobe Analytics{#enabling-adobe-analytics-video-reports}

Grâce au rapports vidéo basé sur la pulsation Adobe, vous n’avez plus besoin d’activer les quatre événements de visionneuse de vidéos (Lecture, Pause, Arrêt, Jalon) lorsque vous configurez Adobe dans Dynamic Media Classic. La pulsation vidéo fonctionne avec les visionneuses de vidéos HTML5 et de supports variés Dynamic Media Classic prêtes à l’emploi. Le lecteur vidéo génère des données de suivi à afficher dans les rapports vidéo d’Adobe Analytics.

* L’intégration des rapports vidéo Adobe Analytics avec Dynamic Media Classic prend en charge les variables de solution, mais pas les variables personnalisées.

   See [Configure Analytics Video Reporting](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/video_analytics_config.html) for more information about solution variables and custom variables.

* Des segments prêts à l’emploi par incréments d’une minute sont pris en charge. Toutefois, les rapports de segments personnalisés, comme les jalons définis par l’utilisateur d’après des incréments temporels, les jalons de pourcentage ou les jalons de décalage, ne sont pas pris en charge.

For more information about Video Heartbeat requirements and setup, see [Measuring Video in Adobe Analytics using Video Heartbeat](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/).

>[!NOTE]
>
>Si votre solution sous licence d’Adobe Analytics n’inclut pas Video Heartbeat, vous devez continuer à utiliser les étapes décrites dans ce chapitre pour attribuer des variables Adobe Analytics à des événements et des variables de visionneuse Dynamic Media Classic.

