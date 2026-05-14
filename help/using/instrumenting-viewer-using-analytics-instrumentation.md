---
title: Instrumenter une visionneuse à l’aide du kit d’instrumentation Adobe Analytics
description: Découvrez comment instrumenter une visionneuse à l’aide du kit d’instrumentation Adobe Analytics dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: 9ea1546d-e6d1-4ba4-8fa1-26b4e69375ba
topic: Integrations, Development
level: Experienced
autotag-review: '2026-05-13T19:51:34.654Z'
TQID: 'https://experienceleague.adobe.com/veMzN35J6flKfCAFvdPfZPgxJ9oGy0LYYGhjr-hZLcY'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 307
ht-degree: 14%

---

# Instrumenter une visionneuse à l’aide du kit d’instrumentation Adobe Analytics{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Vous pouvez utiliser le kit d’instrumentation Adobe Analytics pour intégrer une visionneuse HTML5 à Adobe Analytics.

Si vous utilisez l’un des paramètres prédéfinis de la visionneuse Adobe Dynamic Media Classic HTML5, il contient déjà tout le code d’implémentation pour envoyer des données à Adobe Analytics. Vous n’avez pas besoin d’ajouter d’autres instruments.

## Configuration du suivi Adobe Analytics à partir d’Adobe Dynamic Media Classic {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

Pour toutes les visionneuses HTML5, ajoutez le JavaScript suivant au conteneur HTML, généralement dans l’élément &lt;head> :

```as3
<!-- ***** Adobe Analytics Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Adobe Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

Où `Adobe Dynamic Media Classic Company ID` correspond au nom de la société Adobe Dynamic Media Classic. Et `&preset` est facultatif. Si le nom du paramètre prédéfini de la société n’est pas `companypreset`, il n’est pas facultatif. Dans de tels cas, cela pourrait être `companypreset-1, companypreset-2`, et ainsi de suite. Le plus grand nombre correspond à une nouvelle instance du paramètre prédéfini. Pour déterminer le nom correct de la valeur de paramètre prédéfini de la société, sélectionnez **[!UICONTROL Copier l’URL]**, puis examinez le paramètre `preset=`pour trouver le nom du paramètre prédéfini de la société.

En continuant, ajoutez maintenant une fonction qui transmet l’événement de visionneuse au code de suivi Adobe Analytics.

Ajoutez la fonction `s7ComponentEvent()` au conteneur HTML (ou JSP, ASPX ou autre) :

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

Le nom de la fonction respecte la casse. Le seul paramètre transmis à `s7componentEvent`qui est requis est le dernier : `eventData`. Où `s7track()` est défini dans s_code.jsp inclus ci-dessus. Et `s7track` gère l’ensemble du suivi pour chaque événement. (Vous pouvez personnaliser davantage les données transmises à Adobe Analytics dans cette zone.)

## Activer les événements HREF et ITEM {#enabling-href-and-item-events}

Vous pouvez activer les événements HREF (survoler) et ITEM (cliquer avec la souris/toucher) dans les visionneuses via la commande d’édition de la zone cliquable. Définissez les identificateurs pour HREF et ITEM dans la zone cliquable associée au contenu de la visionneuse Ajoutez un paramètre `&rolloverKey=` à la valeur HREF dans la zone cliquable.
