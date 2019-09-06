---
title: Instrumentation d’une visionneuse avec le kit d’instrumentation Adobe Analytics
seo-title: Instrumentation d’une visionneuse avec le kit d’instrumentation Adobe Analytics
description: 'null'
seo-description: Découvrez comment instrumenter une visionneuse à l'aide du kit d'instrumentation Adobe Analytics.
uuid: cf 9 a 4002-966 d -4641-9 cd 0-2 ee 8 b 5454 f 60
contentOwner: admin
content-type: référence
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/adobe_ analytics_ instrumentation_ kit
discoiquuid: a 2824244-1755-42 de-a 167-42 af 117 cf 038
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Instrumentation d’une visionneuse avec le kit d’instrumentation Adobe Analytics{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Vous pouvez utiliser le kit d'instrumentation Adobe Analytics pour intégrer une visionneuse HTML 5 à Adobe Analytics.

Si vous utilisez l'un des paramètres prédéfinis de visionneuse HTML 5 Dynamic Media Classic, gardez à l'esprit qu'ils contiennent déjà tout le code de mise en œuvre requis pour envoyer des données à Adobe Analytics ; aucune autre opération n'est nécessaire.

## Configuration du suivi Adobe Analytics à partir de Scene7 Publishing System {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

Pour toutes les visionneuses HTML 5, ajoutez le code JavaScript suivant au conteneur HTML, en général dans l'élément &lt; head &gt; :

```as3
<!-- ***** Site Catalyst Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<SPS Company ID>&preset=companypreset-1"></script>
```

`Company` représente le nom de l’entreprise SPS. `&preset` est facultative, sauf si le nom de paramètre prédéfini de l'entreprise ne `companypreset`l'est pas. In such cases, it could be `companypreset-1, companypreset-2`, and so on. Le plus grand nombre correspond à une nouvelle instance du paramètre prédéfini. To determine the correct company preset value name, click **Copy URL** , and then look at the `preset=`parameter to find the company preset name.

Vous allez maintenant ajouter une fonction qui transmet l’événement de visionneuse au code de suivi d’Adobe Analytics.

Add the `s7ComponentEvent()` function to the container HTML (or JSP, or ASPX or other):

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

Ce nom de fonction est sensible à la casse. The only parameter passed to `s7componentEvent`that is required is the last one: `eventData`. `s7track()` est définie dans s_ code. jsp inclus ci-dessus. `s7track` gère tous les suivis par événement. (Si vous devez personnaliser davantage les données transmises à Adobe Analytics, vous devez le faire ici.)

## Activation des événements HREF et ITEM {#enabling-href-and-item-events}

Vous pouvez activer les événements HREF (survoler) et ITEM (cliquer avec la souris/toucher) dans les visionneuses via la commande d’édition de la zone cliquable. Définissez les identificateurs pour HREF et ITEM dans la zone cliquable associée au contenu de la visionneuse Add a `&rolloverKey=` parameter to the HREF value within the Image Map.
