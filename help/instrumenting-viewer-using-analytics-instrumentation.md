---
title: Instrumentation d’une visionneuse avec le kit d’instrumentation Adobe Analytics
description: Découvrez comment instrumenter une visionneuse à l’aide du kit d’instrumentation Adobe Analytics.
uuid: cf9a4002-966d-4641-9cd0-2ee8b5454f60
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: a2824244-1755-42de-a167-42af117cf038
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
exl-id: 9ea1546d-e6d1-4ba4-8fa1-26b4e69375ba
source-git-commit: 27d9a9b9f158846b54e4318119aec9e4dc9c4c0d
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 28%

---

# Instrumentation d’une visionneuse avec le kit d’instrumentation Adobe Analytics{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Vous pouvez utiliser le kit d’instrumentation Adobe Analytics pour intégrer une visionneuse HTML5 à Adobe Analytics.

Si vous utilisez l’un des paramètres prédéfinis de la visionneuse HTML5 Dynamic Media Classic prédéfinis, ils contiennent déjà tout le code d’implémentation pour envoyer des données à Adobe Analytics ; aucune autre instrumentation n’est requise de votre part.

## Configuration du suivi Adobe Analytics à partir de Dynamic Media Classic {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

Pour toutes les visionneuses HTML5, ajoutez le code JavaScript™ suivant au conteneur HTML, généralement dans l’élément &lt;head> :

```as3
<!-- ***** Adobe Analytics Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

Où `Dynamic Media Classic Company ID` est défini sur le nom de la société Dynamic Media Classic. `&preset` est facultatif, sauf si le nom du paramètre prédéfini de l’entreprise n’est pas `companypreset`. Dans ce cas, il peut s’agir de `companypreset-1, companypreset-2`, etc. Le plus grand nombre correspond à une nouvelle instance du paramètre prédéfini. Pour déterminer le nom de la valeur prédéfinie de l’entreprise appropriée, cliquez sur **[!UICONTROL Copier l’URL]** , puis examinez le paramètre `preset=`pour trouver le nom du paramètre prédéfini de l’entreprise.

Continuez en ajoutant une fonction qui transmet l’événement de visionneuse au code de suivi Adobe Analytics.

Ajoutez la fonction `s7ComponentEvent()` au conteneur HTML (ou JSP, ASPX ou autre) :

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

Le nom de la fonction est sensible à la casse. Le seul paramètre transmis à `s7componentEvent`obligatoire est le dernier : `eventData`. Où `s7track()` est défini dans s_code.jsp inclus ci-dessus. Et `s7track` gère le suivi pour chaque événement. (Si vous devez personnaliser davantage les données transmises à Adobe Analytics, vous devez le faire ici.)

## Activation des événements HREF et ITEM {#enabling-href-and-item-events}

Vous pouvez activer les événements HREF (survoler) et ITEM (cliquer avec la souris/toucher) dans les visionneuses via la commande d’édition de la zone cliquable. Définissez les identificateurs pour HREF et ITEM dans la zone cliquable associée au contenu de la visionneuse Ajoutez un paramètre `&rolloverKey=` à la valeur HREF dans la zone cliquable.
