---
title: Activation des rapports vidéo d’Adobe Analytics
description: Découvrez comment activer les rapports vidéo Adobe Analytics.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
translation-type: tm+mt
source-git-commit: 2f7366a77c0fa5f3953721cdd5328123d9c2a052
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 20%

---


# Activation des rapports vidéo d’Adobe Analytics{#enabling-adobe-analytics-video-reports}

Grâce au rapports vidéo Adobe Analytics basé sur la pulsation, vous n’avez plus besoin d’activer les quatre événements de visionneuse de vidéos (Lecture, Pause, Arrêt, Jalon) lorsque vous configurez Adobe Analytics dans Dynamic Media Classic. La pulsation vidéo fonctionne avec les visionneuses de vidéos HTML5 et de supports variés Dynamic Media Classic prêtes à l’emploi. Le lecteur vidéo génère des données de suivi à afficher dans les rapports vidéo d’Adobe Analytics.

* Pour une introduction à la diffusion en flux continu et à la mesure de pulsation, voir [À propos de Adobe Analytics pour la diffusion en flux continu de médias](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html#about-adobe-analytics-for-streaming-media).

* L’intégration des rapports vidéo Adobe Analytics avec Dynamic Media Classic prend en charge les variables de solution, mais pas les variables personnalisées.

   Voir [Paramètres audio et vidéo](https://experienceleague.adobe.com/docs/media-analytics/using/metrics-and-metadata/audio-video-parameters.html#metrics-and-metadata) pour plus d’informations sur les variables de solution et les variables personnalisées.

* Des segments prêts à l’emploi par incréments d’une minute sont pris en charge. Toutefois, les rapports de segments personnalisés, comme les jalons définis par l’utilisateur d’après des incréments temporels, les jalons de pourcentage ou les jalons de décalage, ne sont pas pris en charge.

   Pour plus d’informations sur les exigences et la configuration des médias en flux continu, voir [Mesure des médias en flux continu en Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

* Pour plus d’informations sur les variables personnalisées et de solution, voir [Activation des rapports média](https://experienceleague.adobe.com/docs/media-analytics/using/media-reports/media-reports-enable.html?lang=en#media-reports).

>[!NOTE]
>
>Si votre solution sous licence d’Adobe Analytics n’inclut pas Video Heartbeat, vous devez continuer à utiliser les étapes décrites dans ce chapitre pour affecter des variables Adobe Analytics aux événements et variables de la visionneuse Dynamic Media Classic.

