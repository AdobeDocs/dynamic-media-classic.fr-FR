---
title: Activation des rapports vidéo Adobe Analytics
description: Découvrez comment activer les rapports vidéo Adobe Analytics dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9d017742-1ed2-411d-a8a6-438102bf1557
source-git-commit: 358284e6c9888e5188bec35eb7b5408563a71bad
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 12%

---

# Activation des rapports vidéo Adobe Analytics{#enabling-adobe-analytics-video-reports}

Grâce aux rapports vidéo basés sur la pulsation Adobe Analytics, vous ne devez plus activer les quatre événements de visionneuse de vidéos (Lecture, Pause, Arrêter, Jalon) lorsque vous configurez Adobe Analytics dans Adobe Dynamic Media Classic. La pulsation vidéo fonctionne avec les visionneuses vidéo et de médias mixtes Adobe Dynamic Media Classic HTML5 prêtes à l’emploi. Le lecteur vidéo génère des données de suivi à afficher dans les rapports vidéo d’Adobe Analytics.

* Pour une présentation de la diffusion en continu de médias et de la &quot;mesure de pulsation&quot;, voir [À propos d’Adobe Analytics pour les médias en streaming](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html#about-adobe-analytics-for-streaming-media).

* L’intégration des rapports vidéo Adobe Analytics avec Adobe Dynamic Media Classic prend en charge les variables de solution, mais pas les variables personnalisées.

   Voir [Paramètres audio et vidéo](https://experienceleague.adobe.com/docs/media-analytics/using/metrics-and-metadata/audio-video-parameters.html#metrics-and-metadata) pour plus d’informations sur les variables de solution et les variables personnalisées.

* Les segments prêts à l’emploi d’incréments d’une minute sont pris en charge. Toutefois, les rapports de segments personnalisés, comme les jalons définis par l’utilisateur d’après des incréments temporels, les jalons de pourcentage ou les jalons de décalage, ne sont pas pris en charge.

   Pour plus d’informations sur les exigences et la configuration de la diffusion en continu, voir [Mesurer les médias en flux continu dans Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

* Pour plus d’informations sur les variables personnalisées et de solution, voir [Activation des rapports multimédia](https://experienceleague.adobe.com/docs/media-analytics/using/media-reports/media-reports-enable.html?lang=en#media-reports).

>[!NOTE]
>
>Si votre solution sous licence d’Adobe Analytics n’inclut pas Video Heartbeat, vous devez continuer à utiliser les étapes décrites dans ce chapitre pour affecter des variables Adobe Analytics aux événements et variables de visionneuse Adobe Dynamic Media Classic.
