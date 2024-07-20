---
title: Préparation à la mise à niveau
description: Une liste de contrôle de préparation à la mise à niveau lorsque vous souhaitez passer de [!DNL Adobe Dynamic Media Classic] à [!DNL Dynamic Media] on [!DNL Adobe Experience Manager].
feature: Dynamic Media Classic
role: Admin,User
exl-id: 86537998-b7e9-449c-83eb-6fd04533a00f
topic: Administration, Migration
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 1%

---

# Liste de contrôle de préparation à la mise à niveau

Utilisez la liste de contrôle suivante pour vous aider à comprendre et à vous préparer à une mise à niveau de [!DNL Dynamic Media Classic] vers [!DNL Dynamic Media].

|  | Tâche | Description |
| :--- | :--- | --- |
| **Phase 1 : octroi de licences** | Exécuter le contrat | En fonction du trafic et du stockage, l’équipe du compte d’Adobe travaille avec vous pour effectuer la transition de la licence [!DNL Dynamic Media Classic] à renouveler avec la licence [!DNL Dynamic Media]. |
| **Phase 2 : préparation** | Validation de l’utilisation des fonctionnalités | Vérifiez que les fonctionnalités utilisées dans [!DNL Dynamic Media Classic] sont disponibles dans [!DNL Dynamic Media]. Consultez la page [Comparaison des fonctionnalités](/help/using/upgrade-feature-comparison.md) . Les fonctionnalités clés non encore disponibles dans [!DNL Dynamic Media] sont les suivantes :<br> ・ visualisateur (auteur d’images, rendu d’images).<br> ・ Modèles d’image (modèle 1:1).<br> ・ catalogues électroniques.<br>Si les fonctionnalités ci-dessus sont utilisées, la mise à niveau peut toujours avoir lieu en supposant que ces fonctionnalités seraient accessibles par le biais de [!DNL Dynamic Media Classic]. |
|   | Identification des ressources | Recherchez et préparez des ressources et des paramètres prédéfinis à utiliser pour la mise à niveau. |
| **Phase 3 : environnement** | Mise à niveau [!DNL Adobe Experience Manager] | Toutes les instances de [!DNL Adobe Experience Manager] doivent être mises à jour vers la dernière version. |
|   | Configuration [!DNL Dynamic Media] | Adobe Consulting ou Partner configure [!DNL Dynamic Media] avec vos identifiants. |
| **Phase 4 : mise à niveau** | Réplication des ressources | Au cours du processus de mise à niveau, les ressources [!DNL Dynamic Media Classic] désignées sont répliquées vers Dynamic Media. |
| **Phase 5 : configuration administrative** | Configuration des utilisateurs et des autorisations | Créez des utilisateurs et accordez les autorisations appropriées. |
|   | Configuration des profils de codage vidéo | Créez des profils de codage vidéo. |
|   | Configuration de paramètres prédéfinis de visionneuse | Création de paramètres de visionneuse prédéfinis. |
|   | Définition des paramètres d’image prédéfinis | Configuration de paramètres d’image prédéfinis. |
| **Phase 6 : validation** | Validation | Vérifiez les cas d’utilisation, les ressources, les liens et les API. |
