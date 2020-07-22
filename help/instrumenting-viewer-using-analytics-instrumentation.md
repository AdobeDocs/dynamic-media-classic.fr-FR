---
title: Instrumentation d’une visionneuse avec le kit d’instrumentation Adobe Analytics
seo-title: Instrumentation d’une visionneuse avec le kit d’instrumentation Adobe Analytics
description: 'null'
seo-description: Découvrez comment instrumenter un lecteur à l’aide du kit d’instrumentation Adobe.
uuid: cf9a4002-966d-4641-9cd0-2ee8b5454f60
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: a2824244-1755-42de-a167-42af117cf038
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 38%

---


# Instrumentation d’une visionneuse avec le kit d’instrumentation Adobe Analytics{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Vous pouvez utiliser le kit d’instrumentation Adobe Analytics pour intégrer une visionneuse HTML5 à Adobe Analytics.

Si vous utilisez l’un des paramètres prédéfinis de la visionneuse HTML5 Dynamic Media Classic prédéfinis, sachez qu’ils contiennent déjà tout le code d’implémentation nécessaire pour envoyer les données à Adobe Analytics. Aucune autre instrumentation n’est requise de votre part.

## Configuration du suivi Adobe Analytics à partir de Dynamic Media Classic {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

Pour toutes les visionneuses HTML5, ajoutez le code JavaScript suivant au conteneur HTML, généralement dans l’élément &lt;head> :

```as3
<!-- ***** Site Catalyst Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

`Company` est définie sur le nom de la société Dynamic Media Classic. `&preset` est facultatif, sauf si le nom du paramètre prédéfini de société n’est pas `companypreset`indiqué. In such cases, it could be `companypreset-1, companypreset-2`, and so on. Le plus grand nombre correspond à une nouvelle instance du paramètre prédéfini. To determine the correct company preset value name, click **Copy URL** , and then look at the `preset=`parameter to find the company preset name.

Vous allez maintenant ajouter une fonction qui transmet l’événement de visionneuse au code de suivi d’Adobe Analytics.

Add the `s7ComponentEvent()` function to the container HTML (or JSP, or ASPX or other):

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

Ce nom de fonction est sensible à la casse. The only parameter passed to `s7componentEvent`that is required is the last one: `eventData`. `s7track()` est définie dans s_code.jsp inclus ci-dessus. `s7track` gère tous les suivis par événement. (Si vous devez personnaliser davantage les données transmises à Adobe Analytics, vous devez le faire ici.)

## Activation des événements HREF et ITEM {#enabling-href-and-item-events}

Vous pouvez activer les événements HREF (survoler) et ITEM (cliquer avec la souris/toucher) dans les visionneuses via la commande d’édition de la zone cliquable. Définissez les identificateurs pour HREF et ITEM dans la zone cliquable associée au contenu de la visionneuse Add a `&rolloverKey=` parameter to the HREF value within the Image Map.
