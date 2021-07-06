---
title: Connexion à Adobe Analytics
description: Découvrez comment vous connecter à Adobe Analytics.
uuid: 5614babe-1097-4228-a3dc-27e5a25366d5
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: e5b510a8-8b7f-4c60-869e-d664a8157e63
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 261b8f7c-c61c-4ce3-b9dc-8549347aca2e
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 35%

---

# Connexion à Adobe Analytics{#log-in-to-adobe-analytics}

Avant de vous connecter pour configurer les rapports Adobe Analytics et faire correspondre les variables de rapports Adobe Analytics aux événements Dynamic Media Classic, vérifiez que vous êtes membre du groupe Accès aux services Web dans Adobe Analytics. Les membres de ce groupe ont accès à tous les rapports des suites de rapports spécifiées au moyen des API des services Web de Marketing Cloud, quelles que soient les autorisations définies dans l’interface. Pour ajouter un membre au groupe, dans Adobe Analytics, cliquez sur **[!UICONTROL Outils d’administration]** > **[!UICONTROL Gestion des utilisateurs]** > **[!UICONTROL Modifier les groupes]**.

Lorsque vous vous connectez, vous avez la possibilité de saisir votre ID d’organisation de Marketing Cloud pour utiliser la dernière mise en oeuvre d’analyse vidéo. Si vous choisissez de ne pas saisir votre identifiant, les rapports vidéo fonctionnent toujours. Cependant, cela peut entraîner une mauvaise intégration des données avec d’autres données pour ce client en dehors de Dynamic Media Classic.

>[!NOTE]
>
>Si votre compte Adobe Analytics a été migré vers l’authentification IMS par Adobe (système Identity Management) pour se connecter, la saisie des informations d’identification directes ne fonctionne pas.

**Connexion à Adobe Analytics:**

1. Dans le coin supérieur droit de la page Dynamic Media Classic, appuyez sur **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]**.
1. Dans le volet de gauche, sous **[!UICONTROL Configuration de l’application]**, appuyez sur **[!UICONTROL Adobe Analytics]**.
1. Dans la page Configuration Adobe Analytics, appuyez sur **[!UICONTROL Connexion Adobe Analytics]**.
1. Dans la boîte de dialogue **[!UICONTROL Connexion Adobe Analytics]**, saisissez le nom de votre société, l’identifiant de l’organisation du Marketing Cloud (facultatif), le nom d’utilisateur et la clé *secret partagé* dans le champ de texte **[!UICONTROL Mot de passe]**.

   Vous pouvez récupérer la clé *secret partagé* à partir du Admin Console Analytics. Voir [Comment obtenir des informations d’identification d’API pour les comptes d’utilisateurs](https://github.com/AdobeDocs/analytics-2.0-apis/blob/master/create-oauth-client.md).

1. Cliquez sur **[!UICONTROL Connexion]**.
1. Dans le menu déroulant **[!UICONTROL Suite de rapports]**, choisissez une suite de rapports, puis cliquez sur **[!UICONTROL OK]**.

   >[!NOTE]
   >
   >lorsque vous vous connectez à Adobe Analytics pour la première fois, la liste déroulante Suite de rapports est vide. Lors de votre première connexion, vous ne choisissez pas de suite de rapports. Après vous être connecté pour la première fois, déconnectez-vous, puis revenez à l’écran Adobe Analytics. Connectez-vous de nouveau pour pouvoir choisir une suite de rapports.

>[!MORELIKETHIS]
>
>* [Configuration des rapports Adobe Analytics](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

