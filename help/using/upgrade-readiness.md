---
title: Préparation à la mise à niveau
description: Une liste de contrôle de préparation à la mise à niveau lorsque vous souhaitez avancer de  [!DNL Adobe Dynamic Media Classic]  à  [!DNL Dynamic Media] ’ [!DNL Adobe Experience Manager].
feature: Dynamic Media Classic
role: Admin,User
exl-id: 86537998-b7e9-449c-83eb-6fd04533a00f
topic: Administration, Migration
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 1%

---

# Liste de contrôle de préparation à la mise à niveau

Utilisez la liste de contrôle suivante pour comprendre et préparer une mise à niveau de [!DNL Dynamic Media Classic] vers [!DNL Dynamic Media].

|  | Tâche | Description |
| :--- | :--- | --- |
| **Phase 1 : Licences** | Exécuter le contrat | En fonction du trafic et du stockage, l’équipe du compte Adobe travaille avec vous pour passer de la licence [!DNL Dynamic Media Classic] au renouvellement de la licence [!DNL Dynamic Media]. |
| **Phase 2 : Préparation** | Valider l’utilisation des fonctionnalités | Vérifiez que les fonctionnalités utilisées dans [!DNL Dynamic Media Classic] sont disponibles dans [!DNL Dynamic Media]. Voir la page [Comparaison des fonctionnalités](/help/using/upgrade-feature-comparison.md). Les fonctionnalités clés qui ne sont pas encore disponibles dans [!DNL Dynamic Media] sont les suivantes :<br>· Configurateur visuel (auteur d’images, rendu d’image).<br>· Modèles d’image (1:1 Modèles).<br>· Catalogues électroniques.<br>Si les fonctionnalités ci-dessus sont utilisées, la mise à niveau peut toujours se produire en supposant que ces fonctionnalités soient accessibles par le biais de [!DNL Dynamic Media Classic]. |
|   | Identification des ressources | Recherchez et préparez les ressources et les paramètres prédéfinis à utiliser pour la mise à niveau. |
| **Phase 3 : Environnement** | Mettre à niveau le [!DNL Adobe Experience Manager] | Toutes les instances de [!DNL Adobe Experience Manager] doivent être mises à jour vers la dernière version. |
|   | [!DNL Dynamic Media] de configuration | Adobe Consulting ou un partenaire configure [!DNL Dynamic Media] avec vos informations d’identification. |
| **Phase 4 : mise à niveau** | Réplication des ressources | Pendant le processus de mise à niveau, les ressources [!DNL Dynamic Media Classic] désignées sont répliquées vers Dynamic Media. |
| **Phase 5 : configuration administrative** | Configuration des utilisateurs et des autorisations | Créez des utilisateurs et accordez les autorisations appropriées. |
|   | Configurer des profils de codage vidéo | Création de profils de codage vidéo. |
|   | Configuration des paramètres prédéfinis de visionneuse | Création de paramètres prédéfinis de visionneuse. |
|   | Définition de paramètres d’image prédéfinis | Configurez les paramètres d’image prédéfinis. |
| **Phase 6 : validation** | Validation | vérifier les cas d’utilisation, les ressources, les liens et les API ; |
