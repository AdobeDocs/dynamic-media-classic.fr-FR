---
title: Préparation à la mise à niveau
description: Une liste de contrôle de préparation à la mise à niveau lorsque vous souhaitez avancer depuis [!DNL Adobe Dynamic Media Classic] to [!DNL Dynamic Media] on [!DNL Adobe Experience Manager].
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

Utilisez la liste de contrôle suivante pour vous aider à comprendre et préparer une mise à niveau à partir de [!DNL Dynamic Media Classic] to [!DNL Dynamic Media].

|  | Tâche | Description |
| :--- | :--- | --- |
| **Phase 1 : octroi de licences** | Exécuter le contrat | En fonction du trafic et du stockage, l’équipe du compte d’Adobe travaille avec vous pour effectuer la transition depuis la variable [!DNL Dynamic Media Classic] licence à renouveler sur le [!DNL Dynamic Media] licence. |
| **Phase 2 : préparation** | Validation de l’utilisation des fonctionnalités | Vérifiez que les fonctionnalités utilisées dans [!DNL Dynamic Media Classic] sont disponibles dans [!DNL Dynamic Media]. Voir [Comparaison des fonctionnalités](/help/using/upgrade-feature-comparison.md) page. Fonctionnalités clés pas encore disponibles dans [!DNL Dynamic Media] incluez les éléments suivants :<br>・ Configurateur Visuel (auteur Image, rendu Image).<br>・ Modèles d’image (modèle 1:1).<br>・ Catalogues électroniques.<br>Si les fonctionnalités ci-dessus sont utilisées, la mise à niveau peut toujours avoir lieu en supposant que ces fonctionnalités seraient accessibles au moyen de la fonction [!DNL Dynamic Media Classic]. |
|   | Identification des ressources | Recherchez et préparez des ressources et des paramètres prédéfinis à utiliser pour la mise à niveau. |
| **Phase 3 : environnement** | Mettre à niveau [!DNL Adobe Experience Manager] | Toutes les instances de [!DNL Adobe Experience Manager] doit être mis à jour vers la dernière version. |
|   | Configuration [!DNL Dynamic Media] | Configurations des conseillers ou des partenaires Adobe [!DNL Dynamic Media] avec vos identifiants. |
| **Phase 4 : mise à niveau** | Réplication des ressources | Lors de la mise à niveau, désigné [!DNL Dynamic Media Classic] Les ressources sont répliquées vers Dynamic Media. |
| **Phase 5 : configuration administrative** | Configuration des utilisateurs et des autorisations | Créez des utilisateurs et accordez les autorisations appropriées. |
|   | Configuration des profils de codage vidéo | Créez des profils de codage vidéo. |
|   | Configuration de paramètres prédéfinis de visionneuse | Création de paramètres de visionneuse prédéfinis. |
|   | Définition des paramètres d’image prédéfinis | Configuration de paramètres d’image prédéfinis. |
| **Phase 6 : validation** | Validation | Vérifiez les cas d’utilisation, les ressources, les liens et les API. |
