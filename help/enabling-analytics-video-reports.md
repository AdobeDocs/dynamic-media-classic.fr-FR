---
title: Activation des rapports vidéo d’Adobe Analytics
description: Découvrez comment activer les rapports vidéo Adobe Analytics.
uuid: 078594b2-7d53-4714-8128-ff3b5c3a5e36
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 18644a53-92da-40ab-b961-318d8332c54d
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 23%

---


# Activation des rapports vidéo d’Adobe Analytics{#enabling-adobe-analytics-video-reports}

Grâce au rapports vidéo Adobe Analytics basé sur la pulsation, vous n’avez plus besoin d’activer les quatre événements de visionneuse de vidéos (Lecture, Pause, Arrêt, Jalon) lorsque vous configurez Adobe Analytics dans Dynamic Media Classic. La pulsation vidéo fonctionne avec les visionneuses de vidéos HTML5 et de supports variés Dynamic Media Classic prêtes à l’emploi. Le lecteur vidéo génère des données de suivi à afficher dans les rapports vidéo d’Adobe Analytics.

* L’intégration des rapports vidéo Adobe Analytics avec Dynamic Media Classic prend en charge les variables de solution, mais pas les variables personnalisées.

   Voir [Configuration du Rapports vidéo Analytics](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/video_analytics_config.html) pour plus d’informations sur les variables de solution et les variables personnalisées.

* Des segments prêts à l’emploi par incréments d’une minute sont pris en charge. Toutefois, les rapports de segments personnalisés, comme les jalons définis par l’utilisateur d’après des incréments temporels, les jalons de pourcentage ou les jalons de décalage, ne sont pas pris en charge.

Pour plus d’informations sur les exigences et la configuration de Video Heartbeat, voir [Mesure vidéo en Adobe Analytics à l’aide de Video Heartbeat](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/).

>[!NOTE]
>
>Si votre solution sous licence d’Adobe Analytics n’inclut pas Video Heartbeat, vous devez continuer à utiliser les étapes décrites dans ce chapitre pour affecter des variables Adobe Analytics aux événements et variables de la visionneuse Dynamic Media Classic.

