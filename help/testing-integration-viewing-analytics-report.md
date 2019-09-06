---
title: Test de l’intégration en affichant un rapport Adobe Analytics
seo-title: Test de l’intégration en affichant un rapport Adobe Analytics
description: 'null'
seo-description: Découvrez comment tester l'intégration en affichant un rapport Adobe Analytics.
uuid: 937375 e 0-6 dea -4 baa-a 2 b 0-4 f 3 e 461 c 9 ee 2
contentOwner: admin
content-type: référence
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/adobe_ analytics_ instrumentation_ kit
discoiquuid: 1 ddc 89 ff-d 2 e 9-42 eb-a 442-aa 6 b 9871 c 991
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Test de l’intégration en affichant un rapport Adobe Analytics{#testing-the-integration-by-viewing-an-adobe-analytics-report}

Après avoir créé les variables nécessaires dans Adobe Analytics, les avoir associées aux événements Dynamic Media Classic et effectuer les étapes de mise en œuvre nécessaires, testez la configuration. Vous pouvez tester et vérifier que les données sont capturées, dans Adobe Analytics même. Si la configuration fonctionne ici, aucune autre étape n’est nécessaire. En supposant que vous avez suivi les étapes ci-dessus et lié vos données d'événement Dynamic Media Classic à une ou plusieurs variables de trafic personnalisées, suivez ce processus pour tester vos données dans Adobe Analytics.

**Test de l’intégration en affichant un rapport Adobe Analytics**

1. Lancez une visionneuse Dynamic Media Classic à partir de votre compte, notamment celle qui diffuse la mesure que vous souhaitez capturer, puis interagissez avec elle pour créer des données d'événement.

   Si, par exemple, vous souhaitez mesurer les vues alternatives les plus populaires dans une visionneuse d’images, prévisualisez une visionneuse d’images et cliquez sur les différentes images de miniatures.

1. Inside Adobe Analytics, go to Custom Traffic &gt; Custom Traffic 1-10 &gt; [Name of prop], selecting your traffic prop name from the menu choices.

   Par exemple, pour accéder à la variable prop LoadAsset dans notre exemple de compte, sélectionnez Trafic personnalisé &gt; Trafic personnalisé 1-10 &gt; LoadAsset. Si vous avez plus de dix variables prop personnalisées, d’autres options de menu sont disponibles.

1. Affichez le diagramme généré par Adobe Analytics. Notez qu’il s’agit en général uniquement des données pour une seule mesure. Si vous souhaitez également savoir avec quelle ressource ces données sont associées (par exemple, quelle vidéo est regardée à 50 % uniquement ou quelle image d'une visionneuse est la plus utilisée), veillez à capturer également les données de ressources de cet événement.

>[!NOTE]
>
>Toutes les données de visionneuse Classic Media Classic sont affichées et rapportées dans les rapports Trafic personnalisé ou Conversion personnalisée d'Adobe Analytics.

Pour plus d'informations, voir [www.adobe.com/go/learn_sc7_sitecatalystguide_en](https://www.adobe.com/go/learn_sc7_sitecatalystguide_en).
