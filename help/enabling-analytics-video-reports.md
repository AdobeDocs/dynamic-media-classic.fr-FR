---
title: Activation des rapports vidéo d’Adobe Analytics
description: Découvrez comment activer les rapports vidéo Adobe Analytics.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
exl-id: 9d017742-1ed2-411d-a8a6-438102bf1557
source-git-commit: 27d9a9b9f158846b54e4318119aec9e4dc9c4c0d
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 17%

---

# Activation des rapports vidéo d’Adobe Analytics{#enabling-adobe-analytics-video-reports}

Grâce aux rapports vidéo basés sur la pulsation Adobe Analytics, vous ne devez plus activer les quatre événements de visionneuse de vidéos (Lecture, Pause, Arrêt, Jalon) lorsque vous configurez Adobe Analytics dans Dynamic Media Classic. La pulsation vidéo fonctionne avec les visionneuses vidéo HTML5 et de médias mixtes Dynamic Media Classic prêtes à l’emploi. Le lecteur vidéo génère des données de suivi à afficher dans les rapports vidéo d’Adobe Analytics.

* Pour une introduction aux médias en flux continu et à la &quot;mesure des pulsations&quot;, voir [À propos d’Adobe Analytics for Streaming Media](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html#about-adobe-analytics-for-streaming-media).

* L’intégration des rapports vidéo Adobe Analytics avec Dynamic Media Classic prend en charge les variables de solution, mais pas les variables personnalisées.

   Voir [Paramètres audio et vidéo](https://experienceleague.adobe.com/docs/media-analytics/using/metrics-and-metadata/audio-video-parameters.html#metrics-and-metadata) pour plus d’informations sur les variables de solution et les variables personnalisées.

* Les segments prêts à l’emploi d’incréments d’une minute sont pris en charge. Toutefois, les rapports de segments personnalisés, comme les jalons définis par l’utilisateur d’après des incréments temporels, les jalons de pourcentage ou les jalons de décalage, ne sont pas pris en charge.

   Pour plus d’informations sur les exigences et la configuration des médias en flux continu, voir [Mesure des médias en flux continu dans Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

* Pour plus d’informations sur les variables personnalisées et de solution, voir [Activation des rapports multimédia](https://experienceleague.adobe.com/docs/media-analytics/using/media-reports/media-reports-enable.html?lang=en#media-reports).

>[!NOTE]
>
>Si votre solution sous licence d’Adobe Analytics n’inclut pas Video Heartbeat, vous devez continuer à utiliser les étapes décrites dans ce chapitre pour affecter des variables Adobe Analytics aux événements et variables de visionneuse Dynamic Media Classic.
