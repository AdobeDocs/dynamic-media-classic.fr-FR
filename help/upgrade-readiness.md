---
title: Préparation à la mise à niveau
description: Une liste de contrôle de préparation à la mise à niveau lorsque vous souhaitez avancer depuis [!DNL Adobe Dynamic Media Classic] to [!DNL Dynamic Media] on [!DNL Adobe Experience Manager].
feature: Dynamic Media Classic
role: Admin,User
source-git-commit: 25e4f0d893c5963b648d75f65d099bca09e0f72f
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 2%

---


# Liste de contrôle de préparation à la mise à niveau

Utilisez la liste de contrôle suivante pour vous aider à comprendre et à vous préparer à une mise à niveau à partir de [!DNL Dynamic Media Classic] to [!DNL Dynamic Media].

|  | Tâche | Description |
| :--- | :--- | --- |
| **Phase 1 : Licences** | Exécuter le contrat | En fonction du trafic et du stockage, l’équipe du compte d’Adobe travaille avec vous pour effectuer la transition depuis la variable [!DNL Dynamic Media Classic] licence à renouveler sur le [!DNL Dynamic Media] licence. |
| **Phase 2 : Préparation** | Validation de l’utilisation des fonctionnalités | Confirmation des fonctionnalités utilisées dans [!DNL Dynamic Media Classic] sont disponibles dans [!DNL Dynamic Media]. Voir [Comparaison des fonctionnalités](/help/upgrade-feature-comparison.md) page. Fonctionnalités clés pas encore disponibles dans [!DNL Dynamic Media] incluez les éléments suivants :<br>・ Configurateur Visuel (auteur Image, rendu Image).<br>・ Modèles d’image (modèle 1:1).<br>• Catalogues électroniques.<br>Si les fonctionnalités ci-dessus sont utilisées, la mise à niveau peut toujours avoir lieu en supposant que ces fonctionnalités seraient accessibles au moyen de la fonction [!DNL Dynamic Media Classic]. |
|  | Identification des ressources | Recherchez et préparez des ressources et des paramètres prédéfinis à utiliser pour la mise à niveau. |
| **Phase 3 : Environnement** | Mettre à niveau [!DNL Adobe Experience Manager] | Toutes les instances de [!DNL Adobe Experience Manager] doit être mis à jour vers la dernière version. |
|  | Configuration [!DNL Dynamic Media] | Configurations des conseillers ou des partenaires Adobe [!DNL Dynamic Media] avec vos identifiants. |
| **Phase 4 : Mettre à niveau** | Réplication des ressources | Lors de la mise à niveau, désigné [!DNL Dynamic Media Classic] Les ressources sont répliquées vers Dynamic Media. |
| **Phase 5 : Configuration administrative** | Configuration des utilisateurs et des autorisations | Créez des utilisateurs et accordez les autorisations appropriées. |
|  | Configuration des profils de codage vidéo | Créez des profils de codage vidéo. |
|  | Configuration des paramètres prédéfinis de visionneuse | Créez des paramètres prédéfinis de visionneuse. |
|  | Définition des paramètres d’image prédéfinis | Configurez des paramètres d’image prédéfinis. |
| **Phase 6 : Validation** | Validation | Vérifiez les cas d’utilisation, les ressources, les liens et les API. |