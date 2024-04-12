---
title: Désactivation du suivi Adobe Analytics
description: Découvrez comment désactiver le suivi Adobe Analytics dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: fa5b3971-1c7d-4371-8d69-c399cec0390d
topic: Development, Integrations
level: Experienced
source-git-commit: 914fde11270dc731a261da3305b29dd573584d93
workflow-type: tm+mt
source-wordcount: '85'
ht-degree: 3%

---

# Désactivation du suivi Adobe Analytics{#disabling-adobe-analytics-tracking}

**Pour désactiver le suivi Adobe Analytics :**

1. Désactivez tous les événements sur la page de configuration d’Adobe Analytics dans Adobe Dynamic Media Classic.
1. Enregistrez et publiez.

Ces étapes désactivent la prise en charge par Adobe Dynamic Media Classic et par le biais des URL obtenues à partir de la variable **[!UICONTROL CopyURL]** fonction . Si vous implémentez le suivi personnalisé, désactivez le suivi Adobe Analytics comme configuré dans la page Configuration afin d’éviter tout conflit avec l’implémentation personnalisée.