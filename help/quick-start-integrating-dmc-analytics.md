---
title: '"Démarrage rapide : Intégration d’Adobe Dynamic Media Classic et d’Adobe Analytics"'
description: Une introduction et un démarrage rapide de l’intégration d’Adobe Dynamic Media Classic et d’Adobe Analytics pour vous aider à démarrer rapidement.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: a8fa2414-af01-4a58-bb33-dfd12c1056cc
source-git-commit: ad5270545be502d3aaabba574353787622ab0445
workflow-type: tm+mt
source-wordcount: '687'
ht-degree: 39%

---

# Démarrage rapide : Intégration d’Adobe Dynamic Media Classic et d’Adobe Analytics {#quick-start-integrating-dmc-analytics}

Produit incontournable du secteur, Adobe Analytics dote les marketeurs d’une plateforme centralisée où mesurer, analyser et optimiser les données intégrées de toutes les initiatives en ligne à travers plusieurs canaux marketing.

Après l’intégration d’Adobe Analytics à Adobe Dynamic Media Classic, vous pouvez obtenir des rapports sur le comportement des visiteurs de site web à l’aide des visionneuses Adobe Dynamic Media Classic sur votre site web. Par exemple, lorsqu’un visiteur d’un site web clique sur une cible de zoom dans une visionneuse de zoom Dynamic Media Classic Adobe, Adobe Analytics enregistre cette action. Les rapports Adobe Analytics peuvent recueillir des informations cumulatives sur l’activité des utilisateurs dans les visionneuses Dynamic Media Classic Adobe.

En utilisant les rapports Adobe Analytics, vous obtenez des données précises sur l’activité des internautes sur votre site Web. Vous pouvez déterminer les présentations de produits qui génèrent des conversions et celles qui n’attirent pas l’intérêt des clients.

Voir aussi [Mesure des vidéos dans Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

>[!NOTE]
>
>Un compte Adobe Analytics valide est nécessaire pour intégrer Analytics à Adobe Dynamic Media Classic et générer des rapports Analytics.

Cette section de démarrage rapide est conçue pour vous familiariser rapidement avec le kit d’instrumentation d’Adobe Analytics. 

## 1. Connectez-vous à Adobe Analytics par le biais d’Adobe Dynamic Media Classic et téléchargez les variables de rapports Adobe Analytics

>[!NOTE]
>
>Avant de pouvoir configurer des rapports Adobe Analytics et de faire correspondre des variables de rapports Adobe Analytics à des événements Dynamic Media Classic Adobe, vérifiez que vous êtes ajouté en tant que membre du groupe Accès aux services Web dans Adobe Analytics. Les membres de ce groupe ont accès à tous les rapports des suites de rapports spécifiées au moyen des API des services Web de Marketing Cloud, quelles que soient les autorisations définies dans l’interface. Pour ajouter un membre au groupe, dans Adobe Analytics, cliquez sur **[!UICONTROL Outils d’administration]** > **[!UICONTROL Gestion des utilisateurs]** > **[!UICONTROL Modifier les groupes]**.

Une fois que vous avez vérifié que vous êtes membre du groupe Accès aux services web, dans Adobe Dynamic Media Classic, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Adobe Analytics]**. Sur la page Configuration d’Adobe Analytics, cliquez sur **[!UICONTROL Connexion à Adobe Analytics]**.

Voir [Connexion à Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Dans la boîte de dialogue Connexion Adobe Analytics, saisissez votre ID d’organisation de Marketing Cloud (facultatif) et vos informations d’identification complètes, puis cliquez sur **[!UICONTROL Connexion]**. Dans le menu déroulant Suite de rapports, sélectionnez le nom de la suite de rapports à utiliser.

## 2. Affectez des variables de rapport Adobe Analytics à des événements de visionneuse Dynamic Media Classic et à des variables Dynamic Media Classic Adobe

Sur la page Configuration d’Adobe Analytics, spécifiez les informations souhaitées dans les rapports d’Adobe Analytics. Pour chaque événement de visionneuse Dynamic Media Classic Adobe dont vous souhaitez obtenir des informations, choisissez une variable Adobe Analytics (à partir de votre suite de rapports) et une variable Dynamic Media Classic Adobe.

* Les événements de visionneuse décrivent l’activité utilisateur que vous souhaitez mesurer à travers les rapports.
* Les variables Adobe Dynamic Media Classic décrivent les données sur les événements utilisateur que vous souhaitez que les rapports diffusent.

La configuration d’Adobe Analytics propose également des outils pour activer, modifier et supprimer des événements de visionneuse.

Après avoir cliqué sur **[!UICONTROL Enregistrer]** dans la page de configuration d’Adobe Analytics, le code de suivi personnalisé pour mesurer l’activité des utilisateurs est inséré dans les visionneuses Dynamic Media Classic Adobe. Cette fonctionnalité vous permet d’assurer le suivi de l’activité des utilisateurs dans les rapports Adobe Analytics.

Voir [Configuration des rapports Adobe Analytics](configuring-analytics-reports.md#configuring_adobe_analytics_reports).

## 3. Publiez vos visionneuses Dynamic Media Classic Adobe

Publiez vos visionneuses Dynamic Media Classic Adobe afin que les visionneuses (avec le code pour le suivi de l’activité des utilisateurs dans les rapports Adobe Analytics) soient chargées sur les serveurs Dynamic Media Classic Adobe. Après la publication, ces informations sont incluses aux visionneuses et peuvent être utilisées dans le cadre des analyses d’Adobe Analytics.

Voir [Publication des informations de configuration](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## 4. Placez les visionneuses Dynamic Media Classic Adobe dans votre site web

Placez les visionneuses Dynamic Media Classic Adobe avec le code de suivi Adobe Analytics sur votre site web.

## 5. Testez l’intégration Adobe Analytics en affichant un rapport Adobe Analytics

Pour consulter les rapports Adobe Analytics, accédez au site Web Adobe Analytics. La page de création de rapports vous permet de consulter les données, mais aussi de générer des graphiques et des tableaux afin de mesurer l’activité des utilisateurs pour différentes visionneuses.

Voir [Test de l’intégration d’Adobe Analytics en affichant un rapport Adobe Analytics](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report).
