---
title: 'Démarrage rapide : intégrer Adobe Dynamic Media Classic et Adobe Analytics'
description: Cette section présente et décrit rapidement comment intégrer Adobe Dynamic Media Classic et Adobe Analytics.
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

# Démarrage rapide : intégrer Adobe Dynamic Media Classic et Adobe Analytics {#quick-start-integrating-dmc-analytics}

Produit incontournable du secteur, Adobe Analytics dote les marketeurs d’une plateforme centralisée où mesurer, analyser et optimiser les données intégrées de toutes les initiatives en ligne à travers plusieurs canaux marketing.

Après l’intégration d’Adobe Analytics à Adobe Dynamic Media Classic, vous pouvez obtenir des rapports sur le comportement des visiteurs et visiteuses du site Web à l’aide des visionneuses Adobe Dynamic Media Classic sur votre site Web. Par exemple, lorsqu’un visiteur ou une visiteuse de site Web sélectionne une cible de zoom dans une visionneuse Zoom Adobe Dynamic Media Classic, Adobe Analytics enregistre cette action. Les rapports Adobe Analytics peuvent collecter des informations cumulatives sur l’activité des utilisateurs dans les visionneuses Adobe Dynamic Media Classic.

En utilisant les rapports Adobe Analytics, vous obtenez des données précises sur l’activité des internautes sur votre site Web. Vous pouvez déterminer les présentations de produits qui entraînent une conversion et celles qui n’attirent pas l’intérêt des clients.

Voir aussi [Mesure de la vidéo dans Adobe Analytics](https://experienceleague.adobe.com/fr/docs/media-analytics/using/media-overview).

>[!NOTE]
>
>Un compte Adobe Analytics valide est requis pour intégrer Analytics à Adobe Dynamic Media Classic et générer des rapports Analytics.

Ce démarrage rapide est conçu pour vous aider à maîtriser rapidement le kit d’instrumentation Adobe Analytics.

## &#x200B;1. Connectez-vous à Adobe Analytics via Adobe Dynamic Media Classic et téléchargez les variables de rapport Adobe Analytics

>[!NOTE]
>
>Vérifiez que vous êtes ajouté en tant que membre du groupe Accès aux services Web dans Adobe Analytics. Effectuez cette vérification avant de configurer les rapports Adobe Analytics. De plus, avant de faire correspondre des variables de rapport Adobe Analytics à des événements Adobe Dynamic Media Classic. Les membres de ce groupe peuvent accéder à tous les rapports des suites de rapports spécifiées. Vous pouvez le faire à l’aide de l’API Web Services d’Experience Cloud, quelles que soient les autorisations définies dans l’interface. Pour ajouter un membre au groupe, dans Adobe Analytics, accédez à **[!UICONTROL Outils d’administration]** > **[!UICONTROL Gestion des utilisateurs]** > **[!UICONTROL Modifier les groupes]**.

Après avoir vérifié que vous êtes membre du groupe Accès aux services web, dans Adobe Dynamic Media Classic, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Adobe Analytics]**. Sur la page de configuration d’Adobe Analytics, sélectionnez **[!UICONTROL Connexion Adobe Analytics]**.

Voir [Connexion à Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Dans la boîte de dialogue Connexion à Adobe Analytics, saisissez votre ID d’organisation Experience Cloud (facultatif) et vos informations d’identification complètes, puis sélectionnez **[!UICONTROL Connexion]**. Dans le menu déroulant Suite de rapports, sélectionnez le nom de la suite de rapports à utiliser.

## &#x200B;2. Attribuer des variables de rapport Adobe Analytics aux événements de visionneuse Adobe Dynamic Media Classic et aux variables Adobe Dynamic Media Classic

Sur la page Configuration d’Adobe Analytics, spécifiez les informations souhaitées dans les rapports d’Adobe Analytics. Pour chaque événement de visionneuse Adobe Dynamic Media Classic à propos duquel vous souhaitez obtenir des informations, choisissez une variable Adobe Analytics (dans votre suite de rapports) et une variable Adobe Dynamic Media Classic.

* Les événements de visionneuse décrivent l’activité utilisateur que vous souhaitez mesurer à travers les rapports.
* Les variables Adobe Dynamic Media Classic décrivent les données relatives aux événements utilisateur que les rapports doivent fournir.

La configuration d’Adobe Analytics propose également des outils pour activer, modifier et supprimer des événements de visionneuse.

Après avoir sélectionné **[!UICONTROL Enregistrer]** dans la page Configuration d’Adobe Analytics, un code de suivi personnalisé permettant de mesurer l’activité des utilisateurs est inséré dans les visionneuses Adobe Dynamic Media Classic. Cette fonctionnalité vous permet d’assurer le suivi de l’activité des utilisateurs dans les rapports Adobe Analytics.

Voir [Configuration des rapports Adobe Analytics](configuring-analytics-reports.md#configuring_adobe_analytics_reports).

## &#x200B;3. Publication de vos visionneuses Adobe Dynamic Media Classic

Publiez vos visionneuses Adobe Dynamic Media Classic afin que les visionneuses (avec le code de suivi de l’activité des utilisateurs dans les rapports Adobe Analytics) soient chargées sur les serveurs Adobe Dynamic Media Classic. Une fois la publication effectuée, ces informations sont incluses dans les visionneuses. Utilisez-le pour une analyse par Adobe Analytics.

Voir [Publication des informations de configuration](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## &#x200B;4. Placez les visionneuses Adobe Dynamic Media Classic sur votre site web

Placez les visionneuses Adobe Dynamic Media Classic avec le code de suivi Adobe Analytics sur votre site web.

## &#x200B;5. Tester l’intégration d’Adobe Analytics en affichant un rapport Adobe Analytics

Pour consulter les rapports Adobe Analytics, accédez au site Web Adobe Analytics. La page de création de rapports vous permet de consulter les données, mais aussi de générer des graphiques et des tableaux afin de mesurer l’activité des utilisateurs pour différentes visionneuses.

Voir [Tester l’intégration Adobe Analytics en affichant un rapport Adobe Analytics](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report).
