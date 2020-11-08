---
title: Test de l’intégration en affichant un rapport Adobe Analytics
seo-title: Test de l’intégration en affichant un rapport Adobe Analytics
description: 'null'
seo-description: Découvrez comment tester l’intégration en affichant un rapport Adobe Analytics.
uuid: 937375e0-6dea-4baa-a2b0-4f3e461c9ee2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 1ddc89ff-d2e9-42eb-a442-aa6b9871c991
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 42%

---


# Test de l’intégration en affichant un rapport Adobe Analytics{#testing-the-integration-by-viewing-an-adobe-analytics-report}

Après avoir créé les variables nécessaires en Adobe Analytics, les avoir liées aux événements Dynamic Media Classic et avoir suivi les étapes de mise en oeuvre nécessaires, testez la configuration. Vous pouvez tester et vérifier que les données sont capturées, dans Adobe Analytics même. Si la configuration fonctionne ici, aucune autre étape n’est nécessaire. En supposant que vous ayez suivi les étapes ci-dessus et lié vos données de événement Contenu multimédia dynamique à une ou plusieurs variables de trafic personnalisées, suivez ce processus pour tester vos données dans Adobe Analytics.

**Test de l’intégration en affichant un rapport Adobe Analytics**

1. Lancez une visionneuse de contenu multimédia dynamique classique à partir de votre compte, en particulier une visionneuse qui diffuse la mesure à capturer, et interagissez avec elle pour créer des données de événement.

   Si, par exemple, vous souhaitez mesurer les vues alternatives les plus populaires dans une visionneuse d’images, prévisualisez une visionneuse d’images et cliquez sur les différentes images de miniatures.

1. Inside Adobe Analytics, go to Custom Traffic > Custom Traffic 1-10 > [Name of prop], selecting your traffic prop name from the menu choices.

   Par exemple, pour accéder à la variable prop LoadAsset dans notre exemple de compte, sélectionnez Trafic personnalisé > Trafic personnalisé 1-10 > LoadAsset. Si vous avez plus de dix variables prop personnalisées, d’autres options de menu sont disponibles.

1. Affichez le diagramme généré par Adobe Analytics. Notez qu’il s’agit en général uniquement des données pour une seule mesure. Si vous souhaitez également savoir avec quelle ressource ces données sont associées (par exemple, quelle vidéo est visionnée à 50 % ou quelle image d’une visionneuse est la plus populaire), veillez également à capturer les données de ressources de ce événement.

>[!NOTE]
>
>Toutes les données du lecteur de contenu Contenu multimédia dynamique classique sont affichées et rapportées dans les rapports Trafic personnalisé ou Conversion personnalisée d’Adobe Analytics.

Pour plus d’informations, voir [www.adobe.com/go/learn_sc7_sitecatalystguide_en](https://www.adobe.com/go/learn_sc7_sitecatalystguide_en).
