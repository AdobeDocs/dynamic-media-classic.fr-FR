---
title: Activer les rapports vidéo Adobe Analytics
description: Découvrez comment activer les rapports vidéo Adobe Analytics dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: 9d017742-1ed2-411d-a8a6-438102bf1557
topic: Development, Integrations
level: Experienced
autotag-review: '2026-05-13T19:47:00.853Z'
TQID: 'https://experienceleague.adobe.com/bXlrGU0zMEyfa-E-x-29-biChC17GJTEViBP8GoouTU'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 270
ht-degree: 0%

---

# Activer les rapports vidéo Adobe Analytics{#enabling-adobe-analytics-video-reports}

Grâce aux rapports vidéo basés sur les pulsations Adobe Analytics, vous n’avez plus besoin d’activer les quatre événements de visionneuse de vidéos (Lecture, Pause, Arrêt, Jalon) lorsque vous configurez Adobe Analytics dans Adobe Dynamic Media Classic. La pulsation vidéo fonctionne avec les visionneuses de vidéos et de médias mixtes Adobe Dynamic Media Classic prêtes à l’emploi. Le lecteur vidéo génère des données de suivi à des fins d’affichage dans les rapports vidéo Adobe Analytics.

* Pour une présentation des médias en flux continu et de la « mesure de pulsation », voir [&#x200B; À propos d’Adobe Analytics for Streaming Media &#x200B;](https://experienceleague.adobe.com/fr/docs/media-analytics/using/media-overview).

* L’intégration des rapports vidéo Adobe Analytics à Adobe Dynamic Media Classic prend en charge les variables de solution, mais pas les variables personnalisées.

  Voir [Paramètres audio et vidéo](https://experienceleague.adobe.com/en/docs/media-analytics/using/implementation/variables/audio-video-parameters) pour plus d’informations sur les variables de solution et les variables personnalisées.

* Les segments prêts à l’emploi d’incréments d’une minute sont pris en charge. Cependant, les rapports sur les segments personnalisés, tels que les jalons définis par le client en fonction d’incréments temporels, de % jalons ou de décalages jalons, ne sont pas pris en charge.

  Pour plus d’informations sur les exigences et la configuration relatives aux médias en flux continu, voir [Mesure des médias en flux continu dans Adobe Analytics](https://experienceleague.adobe.com/fr/docs/media-analytics/using/media-overview).

* Pour plus d’informations sur les variables personnalisées et de solution, voir [Activation des rapports multimédia](https://experienceleague.adobe.com/fr/docs/media-analytics/using/media-reports/media-reports-enable#media-reports).

>[!NOTE]
>
>Si votre solution sous licence d’Adobe Analytics n’inclut pas Video Heartbeat, continuez à suivre les étapes décrites dans ce chapitre pour affecter des variables Adobe Analytics aux événements et variables de la visionneuse Adobe Dynamic Media Classic.
