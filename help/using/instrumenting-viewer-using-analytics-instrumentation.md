---
title: Recours à une visionneuse à l’aide du kit d’instrumentation Adobe Analytics
description: Découvrez comment instrumenter une visionneuse à l’aide du kit d’instrumentation Adobe Analytics dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9ea1546d-e6d1-4ba4-8fa1-26b4e69375ba
topic: Integrations, Development
level: Experienced
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 15%

---

# Recours à une visionneuse à l’aide du kit d’instrumentation Adobe Analytics{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Vous pouvez utiliser le kit d’instrumentation Adobe Analytics pour intégrer une visionneuse HTML5 à Adobe Analytics.

Si vous utilisez l’un des paramètres prédéfinis de visionneuse Adobe Dynamic Media Classic HTML5 prédéfinis, ils contiennent déjà tout le code de mise en oeuvre pour envoyer des données à Adobe Analytics. Vous n’avez pas besoin d’ajouter d’autres instruments.

## Configuration du suivi Adobe Analytics à partir d’Adobe Dynamic Media Classic {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

Pour toutes les visionneuses HTML5, ajoutez le code JavaScript suivant au conteneur de HTMLS, généralement dans la variable &lt;head> element:

```as3
<!-- ***** Adobe Analytics Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Adobe Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

Où `Adobe Dynamic Media Classic Company ID` est définie sur le nom de la société Adobe Dynamic Media Classic. Et `&preset` est facultatif. Si le nom du paramètre prédéfini de l’entreprise n’est pas `companypreset`, il n’est pas facultatif. Dans de tels cas, cela pourrait être le cas : `companypreset-1, companypreset-2`, etc. Le plus grand nombre correspond à une nouvelle instance du paramètre prédéfini. Pour déterminer le nom de valeur prédéfini de l’entreprise approprié, sélectionnez **[!UICONTROL Copier l’URL]**, puis observez le `preset=`pour rechercher le nom du paramètre prédéfini de l’entreprise.

Continuez en ajoutant une fonction qui transmet l’événement de visionneuse au code de suivi Adobe Analytics.

Ajoutez la variable `s7ComponentEvent()` au HTML conteneur (ou JSP, ASPX ou autre) :

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

Le nom de la fonction est sensible à la casse. Le seul paramètre transmis à `s7componentEvent`qui est requis est le dernier : `eventData`. Où `s7track()` est défini dans s_code.jsp inclus ci-dessus. Et `s7track` gère l’ensemble du suivi par événement. (Vous pouvez personnaliser davantage les données transmises à Adobe Analytics dans cette zone.)

## Activation des événements HREF et article {#enabling-href-and-item-events}

Vous pouvez activer les événements HREF (survoler) et ITEM (cliquer avec la souris/toucher) dans les visionneuses via la commande d’édition de la zone cliquable. Définissez les identificateurs pour HREF et ITEM dans la zone cliquable associée au contenu de la visionneuse Ajouter un `&rolloverKey=` à la valeur HREF dans la zone cliquable.
