---
title: Recours à une visionneuse à l’aide du kit d’instrumentation Adobe Analytics
description: Découvrez comment instrumenter une visionneuse à l’aide du kit d’instrumentation Adobe Analytics dans Adobe Dynamic Media Classic.
uuid: cf9a4002-966d-4641-9cd0-2ee8b5454f60
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: a2824244-1755-42de-a167-42af117cf038
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9ea1546d-e6d1-4ba4-8fa1-26b4e69375ba
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 20%

---

# Recours à une visionneuse à l’aide du kit d’instrumentation Adobe Analytics{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Vous pouvez utiliser le kit d’instrumentation Adobe Analytics pour intégrer une visionneuse HTML5 à Adobe Analytics.

Si vous utilisez l’un des paramètres prédéfinis de visionneuse HTML5 Adobe Classic prédéfinis, ils contiennent déjà tout le code d’implémentation pour envoyer des données à Adobe Analytics ; aucune autre instrumentation n’est requise de votre part.

## Configuration du suivi Adobe Analytics à partir d’Adobe Dynamic Media Classic {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

Pour toutes les visionneuses HTML5, ajoutez le code JavaScript suivant au conteneur HTML, généralement dans l’élément &lt;head> :

```as3
<!-- ***** Adobe Analytics Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Adobe Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

Où `Adobe Dynamic Media Classic Company ID` est défini sur le nom de la société Dynamic Media Classic Adobe. `&preset` est facultatif, sauf si le nom du paramètre prédéfini de l’entreprise n’est pas `companypreset`. Dans ce cas, il peut s’agir de `companypreset-1, companypreset-2`, etc. Le plus grand nombre correspond à une nouvelle instance du paramètre prédéfini. Pour déterminer le nom de valeur prédéfini de l’entreprise correct, sélectionnez **[!UICONTROL Copier l’URL]** , puis examinez le paramètre `preset=`pour trouver le nom du paramètre prédéfini de l’entreprise.

Continuez en ajoutant une fonction qui transmet l’événement de visionneuse au code de suivi Adobe Analytics.

Ajoutez la fonction `s7ComponentEvent()` au conteneur HTML (ou JSP, ASPX ou autre) :

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

Le nom de la fonction est sensible à la casse. Le seul paramètre transmis à `s7componentEvent`obligatoire est le dernier : `eventData`. Où `s7track()` est défini dans s_code.jsp inclus ci-dessus. Et `s7track` gère le suivi pour chaque événement. (Si vous devez personnaliser davantage les données transmises à Adobe Analytics, vous devez le faire ici.)

## Activation des événements HREF et article {#enabling-href-and-item-events}

Vous pouvez activer les événements HREF (survoler) et ITEM (cliquer avec la souris/toucher) dans les visionneuses via la commande d’édition de la zone cliquable. Définissez les identificateurs pour HREF et ITEM dans la zone cliquable associée au contenu de la visionneuse Ajoutez un paramètre `&rolloverKey=` à la valeur HREF dans la zone cliquable.
