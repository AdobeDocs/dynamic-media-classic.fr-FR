---
title: "Quick Start : Integrate Adobe Dynamic Media Classic and Adobe Analytics"
description: Présentation et démarrage rapide sur la manière d’intégrer Adobe Dynamic Media Classic et Adobe Analytics.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: a8fa2414-af01-4a58-bb33-dfd12c1056cc
topic: Integrations
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '689'
ht-degree: 21%

---

# Démarrage rapide : Intégration d’Adobe Dynamic Media Classic et d’Adobe Analytics {#quick-start-integrating-dmc-analytics}

Produit incontournable du secteur, Adobe Analytics dote les marketeurs d’une plateforme centralisée où mesurer, analyser et optimiser les données intégrées de toutes les initiatives en ligne à travers plusieurs canaux marketing.

Après l’intégration d’Adobe Analytics à Adobe Dynamic Media Classic, vous pouvez obtenir sur votre site web des rapports sur le comportement des visiteurs de sites web utilisant des visionneuses Adobe Dynamic Media Classic. Par exemple, lorsqu’un visiteur d’un site web sélectionne une cible de zoom dans une visionneuse de zoom Adobe Dynamic Media Classic, Adobe Analytics enregistre cette action. Les rapports Adobe Analytics peuvent recueillir des informations cumulatives sur l’activité des utilisateurs dans les visionneuses Adobe Dynamic Media Classic.

En utilisant les rapports Adobe Analytics, vous obtenez des données précises sur l’activité des internautes sur votre site Web. Vous pouvez déterminer les présentations de produits qui génèrent des conversions et celles qui n’attirent pas l’intérêt des clients.

Voir aussi [Mesure vidéo dans Adobe Analytics](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-overview).

>[!NOTE]
>
>Un compte Adobe Analytics valide est nécessaire pour intégrer Analytics à Adobe Dynamic Media Classic et générer des rapports Analytics.

Ce didacticiel de mise en route est conçu pour vous aider à démarrer rapidement avec le kit d’instrumentation Adobe Analytics.

## 1. Connectez-vous à Adobe Analytics par le biais d’Adobe Dynamic Media Classic et téléchargez les variables de rapports Adobe Analytics.

>[!NOTE]
>
>Vérifiez que vous êtes ajouté en tant que membre du groupe Accès aux services web dans Adobe Analytics. Effectuez cette vérification avant de configurer les rapports Adobe Analytics. Avant de faire correspondre des variables de rapports Adobe Analytics à des événements Adobe Dynamic Media Classic. Les membres de ce groupe peuvent accéder à tous les rapports des suites de rapports spécifiées. Vous pouvez le faire à l’aide de l’API des services Web de l’Experience Cloud, quelles que soient les autorisations définies dans l’interface. Pour ajouter un membre au groupe, dans Adobe Analytics, accédez à **[!UICONTROL Outils d’administration]** > **[!UICONTROL Gestion des utilisateurs]** > **[!UICONTROL Modification de groupes]**.

Une fois que vous avez vérifié que vous êtes membre du groupe Accès aux services web , dans Adobe Dynamic Media Classic, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Adobe Analytics]**. Sur la page Configuration d’Adobe Analytics, sélectionnez **[!UICONTROL Connexion Adobe Analytics]**.

Voir [Connexion à Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Dans la boîte de dialogue Connexion à Adobe Analytics, saisissez votre ID d’organisation Experience Cloud (facultatif), vos informations d’identification complètes, puis sélectionnez **[!UICONTROL Connexion]**. Dans le menu déroulant Suite de rapports, sélectionnez le nom de la suite de rapports à utiliser.

## 2. Attribuer des variables de rapport Adobe Analytics aux événements de visionneuse Adobe Dynamic Media Classic et aux variables Adobe Dynamic Media Classic

Sur la page Configuration d’Adobe Analytics, spécifiez les informations souhaitées dans les rapports d’Adobe Analytics. Pour chaque événement de visionneuse Adobe Dynamic Media Classic dont vous souhaitez obtenir des informations, choisissez une variable Adobe Analytics (dans votre suite de rapports) et une variable Adobe Dynamic Media Classic.

* Les événements de visionneuse décrivent l’activité utilisateur que vous souhaitez mesurer à travers les rapports.
* Les variables Adobe Dynamic Media Classic décrivent les données sur les événements utilisateur que vous souhaitez que les rapports diffusent.

La configuration d’Adobe Analytics propose également des outils pour activer, modifier et supprimer des événements de visionneuse.

Après avoir sélectionné **[!UICONTROL Enregistrer]** sur la page Configuration d’Adobe Analytics , un code de suivi personnalisé pour mesurer l’activité des utilisateurs est inséré dans les visionneuses Adobe Dynamic Media Classic. Cette fonctionnalité vous permet d’assurer le suivi de l’activité des utilisateurs dans les rapports Adobe Analytics.

Voir [Configuration des rapports Adobe Analytics](configuring-analytics-reports.md#configuring_adobe_analytics_reports).

## 3. Publiez vos visionneuses Adobe Dynamic Media Classic

Publiez vos visionneuses Adobe Dynamic Media Classic afin que les visionneuses (avec le code permettant de suivre l’activité des utilisateurs dans les rapports Adobe Analytics) soient chargées sur les serveurs Adobe Dynamic Media Classic. Après la publication, ces informations sont incluses dans les visionneuses. Utilisez-le pour une analyse par Adobe Analytics.

Voir [Publication des informations de configuration](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## 4. Placez les visionneuses Adobe Dynamic Media Classic sur votre site web

Placez les visionneuses Adobe Dynamic Media Classic avec le code de suivi Adobe Analytics sur votre site web.

## 5. Testez l’intégration Adobe Analytics en affichant un rapport Adobe Analytics

Pour consulter les rapports Adobe Analytics, accédez au site Web Adobe Analytics. La page de création de rapports vous permet de consulter les données, mais aussi de générer des graphiques et des tableaux afin de mesurer l’activité des utilisateurs pour différentes visionneuses.

Voir [Tester l’intégration Adobe Analytics en affichant un rapport Adobe Analytics](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report).
