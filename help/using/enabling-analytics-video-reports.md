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
topic: Development, Integrations
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# Activation des rapports vidéo Adobe Analytics{#enabling-adobe-analytics-video-reports}

Grâce aux rapports vidéo basés sur la pulsation Adobe Analytics, vous ne devez plus activer les quatre événements de visionneuse de vidéos (Lecture, Pause, Arrêter, Jalon) lorsque vous configurez Adobe Analytics dans Adobe Dynamic Media Classic. La pulsation vidéo fonctionne avec les visionneuses vidéo et de médias mixtes Adobe Dynamic Media Classic HTML5 prêtes à l’emploi. Le lecteur vidéo génère des données de suivi à afficher dans les rapports vidéo Adobe Analytics.

* Pour une présentation sur la diffusion en continu de médias et la &quot;mesure des pulsations&quot;, voir [À propos d’Adobe Analytics pour les médias en streaming](https://experienceleague.adobe.com/fr/docs/media-analytics/using/media-overview).

* L’intégration des rapports vidéo Adobe Analytics avec Adobe Dynamic Media Classic prend en charge les variables de solution, mais pas les variables personnalisées.

  Voir [Paramètres audio et vidéo](https://experienceleague.adobe.com/fr/docs/media-analytics/using/implementation/variables/audio-video-parameters) pour plus d’informations sur les variables de solution et les variables personnalisées.

* Les segments prêts à l’emploi d’incréments d’une minute sont pris en charge. Toutefois, les rapports de segments personnalisés, tels que les jalons définis par le client en fonction des incréments de temps, des jalons de pourcentage ou des jalons de décalage, ne sont pas pris en charge.

  Pour plus d’informations sur les exigences et la configuration des médias en continu, voir [Mesurer les médias en flux continu dans Adobe Analytics](https://experienceleague.adobe.com/fr/docs/media-analytics/using/media-overview).

* Pour plus d’informations sur les variables personnalisées et de solution, voir [ Activation des rapports multimédia](https://experienceleague.adobe.com/fr/docs/media-analytics/using/media-reports/media-reports-enable#media-reports).

>[!NOTE]
>
>Si votre solution sous licence d’Adobe Analytics n’inclut pas Video Heartbeat, continuez à utiliser les étapes décrites dans ce chapitre pour affecter des variables Adobe Analytics aux événements et variables de visionneuse Adobe Dynamic Media Classic.
