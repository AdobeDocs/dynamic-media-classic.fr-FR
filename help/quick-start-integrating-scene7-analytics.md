---
title: '« Démarrage rapide : Intégration de Dynamic Media Classic et Adobe Analytics »'
seo-title: '« Démarrage rapide : Intégration de Dynamic Media Classic et Adobe Analytics »'
description: 'null'
seo-description: Introduction et démarrage rapide à l'intégration de Dynamic Media Classic et d'Adobe Analytics pour vous aider à maîtriser rapidement les opérations.
uuid: 3 f 9 e 2 c 91-15 d 4-4 b 53-8220-9 b 1 ca 57 c 0 b 1 d
contentOwner: admin
content-type: référence
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/adobe_ analytics_ instrumentation_ kit
discoiquuid: abec 9 a 85-013 c -4030-b 129-bf 27 a 89 cb 464
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Démarrage rapide : Intégration de Dynamic Media Classic et d'Adobe Analytics {#quick-start-integrating-scene-and-adobe-analytics}

Produit incontournable du secteur, Adobe Analytics dote les marketeurs d’une plateforme centralisée où mesurer, analyser et optimiser les données intégrées de toutes les initiatives en ligne à travers plusieurs canaux marketing.

Après avoir intégré Adobe Analytics à Scene 7 Publishing System, vous pouvez obtenir des rapports sur le comportement des visiteurs du site Web à l'aide de visionneuses dynamiques Media Classic sur votre site Web. Par exemple, lorsqu'un visiteur de site Web clique sur une cible de zoom dans une visionneuse de zoom classique de Media Classic, Adobe Analytics enregistre cette action. Les rapports Adobe Analytics peuvent collecter des informations cumulatives sur l'activité des utilisateurs dans les visionneuses de médias dynamiques dynamiques.

En utilisant les rapports Adobe Analytics, vous obtenez des données précises sur l’activité des internautes sur votre site Web. Vous pouvez déterminer quelles présentations de produits se transforment en achats et quelles présentations ne suscitent pas l’intérêt du client.

Voir aussi [Mesure des vidéos dans Adobe Analytics](https://marketing.adobe.com/resources/help/en_US/sc/appmeasurement/hbvideo/).

>[!NOTE]
>
>un compte Adobe Analytics valide est requis pour intégrer Analytics à Scene7 Publishing System et générer des rapports Analytics.

**Démarrage rapide**

Cette section de démarrage rapide est conçue pour vous familiariser rapidement avec le kit d’instrumentation d’Adobe Analytics. 

**Cookie. Log in to Adobe Analytics by way of Dynamic Media Classic and download Adobe Analytics report variables**

>[!NOTE]
>
>Avant de pouvoir configurer les rapports Adobe Analytics et de faire correspondre les variables de rapports Adobe Analytics aux événements Dynamic Media Classic, vérifiez que vous êtes ajouté en tant que membre du groupe Accès aux services Web dans Adobe Analytics. Les membres de ce groupe ont accès à tous les rapports des suites de rapports spécifiées au moyen des API des services Web de Marketing Cloud, quelles que soient les autorisations définies dans l’interface. Pour ajouter un membre au groupe, dans Adobe Analytics, cliquez sur **Outils d’administration** &gt; **Gestion des utilisateurs** &gt; **Modifier les groupes**.

After you have verified that you are a member of the Web Service Access group, in Dynamic Media Classic, click **Setup** &gt; **Application Setup** &gt; **Adobe Analytics**. Sur la page Configuration d’Adobe Analytics, cliquez sur **Connexion à Adobe Analytics**.

Voir [Connexion à Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Dans la boîte de dialogue Connexion à Adobe Analytics, saisissez votre identifiant d'entreprise Marketing Cloud (facultatif) et vos informations d'identification complètes, puis cliquez **sur Connexion**. Dans le menu déroulant Suite de rapports, sélectionnez le nom de la suite de rapports à utiliser.

**2. Affecter des variables de rapports Adobe Analytics aux événements de visionneuse Dynamic Media Classic et aux variables Dynamic Media Classic**

Sur la page Configuration d’Adobe Analytics, spécifiez les informations souhaitées dans les rapports d’Adobe Analytics. Pour chaque événement de visionneuse Dynamic Media Classic dont vous souhaitez recueillir les informations, choisissez une variable Adobe Analytics (dans votre suite de rapports) et une variable Dynamic Media Classic.

* Les événements de visionneuse décrivent l’activité utilisateur que vous souhaitez mesurer à travers les rapports.
* Les variables Dynamic Media Classic décrivent les données sur les événements d'utilisateurs que vous souhaitez fournir aux rapports.

La configuration d’Adobe Analytics propose également des outils pour activer, modifier et supprimer des événements de visionneuse.

Une fois que vous avez cliqué sur Enregistrer dans l'écran de configuration d'Adobe Analytics, le code de suivi personnalisé permettant de mesurer l'activité utilisateur est inséré dans les visionneuses Dynamic Media Classic. Cette fonctionnalité vous permet d’assurer le suivi de l’activité des utilisateurs dans les rapports Adobe Analytics.

Voir [Configuration des rapports Adobe Analytics](configuring-analytics-reports.md#configuring_adobe_analytics_reports).

**Cookie. Publication de vos visionneuses Dynamic Media Classic**

Publiez vos visionneuses Dynamic Media Classic afin que les visionneuses (avec le code permettant de suivre l'activité des utilisateurs dans les rapports Adobe Analytics) soient chargées sur les serveurs Dynamic Media Classic. Après la publication, ces informations sont incluses aux visionneuses et peuvent être utilisées dans le cadre des analyses d’Adobe Analytics.

Voir [Publication des informations de configuration](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

**4. Importation de visionneuses dynamiques Media Classic sur votre site Web**

Placez les visionneuses Dynamic Media Classic à l'aide du code de suivi Adobe Analytics sur votre site Web.

**5. Test de l’intégration d’Adobe Analytics en affichant un rapport Adobe Analytics**

Pour consulter les rapports Adobe Analytics, accédez au site Web Adobe Analytics. La page de création de rapports vous permet de consulter les données, mais aussi de générer des graphiques et des tableaux afin de mesurer l’activité des utilisateurs pour différentes visionneuses.

Voir [Test de l’intégration d’Adobe Analytics en affichant un rapport Adobe Analytics](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report).
