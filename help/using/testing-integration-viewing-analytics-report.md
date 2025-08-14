---
title: Tester l’intégration en affichant un rapport Adobe Analytics
description: Découvrez comment tester l’intégration dans Adobe Dynamic Media Classic en affichant un rapport Adobe Analytics.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 6186fcf0-99b4-447d-ae94-b4124dcb405b
topic: Integrations, Development
level: Experienced
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 5%

---

# Tester l’intégration en affichant un rapport Adobe Analytics{#testing-the-integration-by-viewing-an-adobe-analytics-report}

Après avoir créé les variables nécessaires dans Adobe Analytics, les avoir liées à des événements Adobe Dynamic Media Classic et avoir effectué les étapes d’implémentation nécessaires, vous pouvez tester la configuration. Vous pouvez tester et vérifier que les données sont capturées dans Adobe Analytics. Si la configuration fonctionne ici, aucune autre étape n’est nécessaire. En supposant que vous ayez suivi les étapes ci-dessus et lié vos données d’événement Adobe Dynamic Media Classic à une ou plusieurs variables de trafic personnalisé, suivez ce workflow pour tester vos données dans Adobe Analytics.

**Pour tester l’intégration en affichant un rapport Adobe Analytics, procédez comme suit**

1. Démarrez une visionneuse Adobe Dynamic Media Classic à partir de votre compte, en particulier une visionneuse qui diffuse la mesure que vous souhaitez obtenir, et interagissez avec elle pour créer des données d’événement.

   Par exemple, si vous souhaitez mesurer des vues alternatives populaires dans une visionneuse d’images, prévisualisez une visionneuse d’images et cliquez sur les différentes miniatures.

1. Dans Adobe Analytics, accédez à **[!UICONTROL Trafic personnalisé]** > **[!UICONTROL Trafic personnalisé 1-10]** > [Nom de la prop], en sélectionnant votre nom de prop de trafic parmi les choix de menu.

   Par exemple, pour accéder à la prop **[!UICONTROL LoadAsset]** dans le compte d’exemple, le choix de menu approprié est **[!UICONTROL Trafic personnalisé]** > **[!UICONTROL Trafic personnalisé 1-10]** > **[!UICONTROL LoadAsset]**. Si vous disposez de plus de dix props personnalisées, d’autres choix de menu s’affichent également.

1. Affichez le diagramme généré par Adobe Analytics. Ce graphique ne représente généralement que les données d’une seule mesure. Si vous souhaitez également savoir à quelle ressource ces données sont associées, obtenez les données de ressource de cet événement. Par exemple, il est souvent utile de savoir quelle vidéo est visionnée à 50 % seulement ou quelle image d’une visionneuse est la plus populaire.

>[!NOTE]
>
>Toutes les données de la visionneuse Adobe Dynamic Media Classic sont affichées et consignées dans les rapports de trafic personnalisé ou les rapports de conversion personnalisés d’Adobe Analytics.

Pour plus d’informations, voir [Tutoriels Analytics](https://experienceleague.adobe.com/en/docs/analytics-learn/tutorials/overview).