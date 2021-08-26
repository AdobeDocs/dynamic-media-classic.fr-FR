---
title: Connexion à Adobe Analytics
description: Découvrez comment vous connecter à Adobe Analytics à partir d’Adobe Dynamic Media Classic.
uuid: 5614babe-1097-4228-a3dc-27e5a25366d5
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: e5b510a8-8b7f-4c60-869e-d664a8157e63
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 261b8f7c-c61c-4ce3-b9dc-8549347aca2e
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 20%

---

# Connexion à Adobe Analytics{#log-in-to-adobe-analytics}

Avant de vous connecter pour configurer des rapports Adobe Analytics et faire correspondre des variables de rapports Adobe Analytics à des événements Dynamic Media Classic Adobe, vérifiez que vous êtes membre du groupe Accès aux services web dans Adobe Analytics. Les membres de ce groupe peuvent accéder à tous les rapports des suites de rapports spécifiées à l’aide de l’API des services Web de l’Experience Cloud, quelles que soient les autorisations définies dans l’interface. Pour ajouter un membre au groupe, dans Adobe Analytics, accédez à **[!UICONTROL Outils d’administration]** > **[!UICONTROL Gestion des utilisateurs]** > **[!UICONTROL Modifier les groupes]**.

Lorsque vous vous connectez, vous avez la possibilité de saisir votre ID d’organisation Experience Cloud afin d’utiliser la dernière mise en oeuvre d’analyse vidéo. Si vous choisissez de ne pas saisir votre identifiant, les rapports vidéo fonctionnent toujours. Cependant, cela peut entraîner une mauvaise intégration des données avec d’autres données pour ce client en dehors d’Adobe Dynamic Media Classic.

>[!NOTE]
>
>Si votre compte Adobe Analytics a été migré vers l’authentification Adobe IMS (système Identity Management) pour la connexion, la saisie des informations d’identification directes ne fonctionne pas.

**Connexion à Adobe Analytics:**

1. Près du coin supérieur droit de la page Adobe Dynamic Media Classic, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]**.
1. Dans le volet de gauche, sous **[!UICONTROL Configuration de l’application]**, appuyez sur **[!UICONTROL Adobe Analytics]**.
1. Dans la page Configuration Adobe Analytics, appuyez sur **[!UICONTROL Connexion Adobe Analytics]**.
1. Dans la boîte de dialogue **[!UICONTROL Connexion Adobe Analytics]**, saisissez le nom de votre société, l’identifiant de l’organisation Experience Cloud (facultatif), le nom d’utilisateur et la clé *secret partagé* dans le champ de texte **[!UICONTROL Mot de passe]**.

   Vous pouvez récupérer la clé *secret partagé* à partir du Admin Console Analytics. Voir [Comment obtenir des informations d’identification d’API pour les comptes d’utilisateurs](https://github.com/AdobeDocs/analytics-2.0-apis/blob/master/create-oauth-client.md).

1. Sélectionnez **[!UICONTROL Connexion]**.
1. Dans le menu déroulant **[!UICONTROL Suite de rapports]**, choisissez une suite de rapports, puis sélectionnez **[!UICONTROL OK]**.

   >[!NOTE]
   >
   >lorsque vous vous connectez à Adobe Analytics pour la première fois, la liste déroulante Suite de rapports est vide. Lors de votre première connexion, vous ne choisissez pas de suite de rapports. Après vous être connecté pour la première fois, déconnectez-vous, puis revenez à l’écran Adobe Analytics. Connectez-vous de nouveau pour pouvoir choisir une suite de rapports.

>[!MORELIKETHIS]
>
>* [Configuration des rapports Adobe Analytics](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

