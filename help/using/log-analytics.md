---
title: Connexion à Adobe Analytics
description: Découvrez comment vous connecter à Adobe Analytics à partir d’Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: e5b510a8-8b7f-4c60-869e-d664a8157e63
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 261b8f7c-c61c-4ce3-b9dc-8549347aca2e
topic: Integrations, Development
level: Experienced
source-git-commit: ae7d0c6d3047d68ed3da4187ef516dc51c95de30
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 0%

---

# Connexion à Adobe Analytics{#log-in-to-adobe-analytics}

Avant de vous connecter pour configurer les rapports Adobe Analytics et faire correspondre les variables de rapports Adobe Analytics aux événements Adobe Dynamic Media Classic, vérifiez que vous êtes membre du groupe Accès aux services Web dans Adobe Analytics. Les membres de ce groupe peuvent accéder à tous les rapports des suites de rapports spécifiées par le biais de l’API des services Web de l’Experience Cloud, quels que soient les autorisations définies dans l’interface. Pour ajouter un membre au groupe, dans Adobe Analytics, accédez à **[!UICONTROL Outils d’administration]** > **[!UICONTROL Gestion des utilisateurs]** > **[!UICONTROL Modification de groupes]**.

Lorsque vous vous connectez, vous avez la possibilité de saisir votre ID d’organisation Experience Cloud afin d’utiliser la dernière mise en oeuvre d’analyse vidéo. Si vous choisissez de ne pas saisir votre identifiant, les rapports vidéo fonctionnent toujours. Cependant, cela peut entraîner une mauvaise intégration des données avec d’autres données pour ce client en dehors d’Adobe Dynamic Media Classic.

>[!NOTE]
>
>Si votre compte Adobe Analytics a été migré vers l’authentification Adobe IMS (système Identity Management) pour la connexion, la saisie des informations d’identification directes ne fonctionne pas.

## Connexion à Adobe Analytics à partir d’Adobe Dynamic Media Classic {#log-in-to-analytics-from-dmc}

Commencez par intégrer Dynamic Media Classic à Adobe Analytics OAuth. L’intégration d’Adobe Analytics OAuth à Dynamic Media Classic n’est généralement effectuée qu’une seule fois par utilisateur.

1. Accès [Console Adobe Developer](https://developer.adobe.com/console). Assurez-vous que votre compte dispose des autorisations d’administrateur pour l’organisation pour laquelle l’intégration est requise.
1. Près du coin supérieur droit de la page d’accueil, dans la liste déroulante, sélectionnez la société appropriée. (La capture d’écran ci-dessous est fournie à titre d’information uniquement ; le nom réel de la société que vous sélectionnez peut varier.)

   ![Création d’un projet](assets/analytics-oauth1.png)

1. Effectuez l’une des opérations suivantes :

   * Dans la partie supérieure de la page, dans la **[!UICONTROL Accueil]** onglet, sélectionnez **[!UICONTROL Créer un projet]**.
   * Dans la partie supérieure de la page, dans la **[!UICONTROL Projets]** . Dans le coin droit de la page, sélectionnez **[!UICONTROL Créer un projet]**.

1. Sur la page du projet, sélectionnez **[!UICONTROL Ajouter une API]**.
1. Sur le **[!UICONTROL Ajout d’une API]** page, sélectionnez **[!UICONTROL Adobe Analytics]**.
1. Dans le coin inférieur droit de la page, sélectionnez **[!UICONTROL Suivant]**.

   ![Ajout d’une API](assets/analytics-oauth2.png)

1. Sur le **[!UICONTROL Configuration de l’API]** page, sélectionnez **[!UICONTROL AUTHENTIFICATION DES UTILISATEURS OAuth]**.
1. Dans le coin inférieur droit de la page, sélectionnez **[!UICONTROL Suivant]**.
1. Sur le **[!UICONTROL Configuration de l’API]** page, sélectionnez **[!UICONTROL OAUTH 2.0 Web]**.
1. Dans le **[!UICONTROL URI de redirection par défaut]** , saisissez le chemin d’accès suivant tel qu’affiché :

   `https://exploreadobe.com/dynamic-media-upgrade/`

1. Dans le **[!UICONTROL Redirection du modèle URI]** , saisissez le chemin d’accès suivant tel qu’affiché :

   `https://exploreadobe\.com/dynamic-media-upgrade/`

1. Dans le coin inférieur droit de la page, sélectionnez **[!UICONTROL Enregistrer l’API configurée]**.
1. Dans le panneau de navigation, sur le côté gauche de la page Adobe Analytics, sous **[!UICONTROL Informations d’identification]**, sélectionnez **[!UICONTROL OAuth Web]**.
1. Sous **[!UICONTROL Informations d’identification]**, procédez comme suit :
   * Sous **[!UICONTROL ID client]**, sélectionnez **[!UICONTROL Copier]** pour copier la valeur. Vous avez besoin de cette valeur pour la configuration Analytics suivante dans l’application de bureau Dynamic Media Classic à suivre.
   * Sous **[!UICONTROL Secret du client]**, sélectionnez **[!UICONTROL Récupération du secret client]** pour afficher la valeur associée. Sélectionner **[!UICONTROL Copier]** pour copier la valeur. Vous avez besoin de cette valeur pour la configuration Adobe Analytics suivante dans l’application de bureau Dynamic Media Classic à suivre.

## Configuration d’Adobe Analytics dans Adobe Dynamic Media Classic {#configure-analytics-in-dmc}

>[!NOTE]
>
>Après la configuration initiale d’Adobe Analytics dans Dynamic Media Classic, vous devez rétablir la configuration uniquement dans les cas suivants :
>
>* Un nouveau rapport est ajouté dans Analytics et l’utilisateur souhaite commencer à envoyer des données à ce nouveau rapport.
>* Le serveur de suivi est mis à jour dans Adobe Analytics.
>* Une nouvelle variable de suivi est introduite dans un rapport et vous souhaitez lier une variable de visionneuse spécifique dans l’interface utilisateur de Dynamic Media Classic à cette nouvelle variable Analytics.
>

1. Dans le coin supérieur droit de l’application de bureau Adobe Dynamic Media Classic, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]**.
1. Dans le panneau de gauche, sous **[!UICONTROL Configuration de l’application]**, sélectionnez **[!UICONTROL Adobe Analytics]**.
1. Sur le **[!UICONTROL Configuration Adobe Analytics]** page, sélectionnez **[!UICONTROL Connexion Adobe Analytics]**.
1. Dans le **[!UICONTROL Connexion Adobe Analytics]** dans la boîte de dialogue **[!UICONTROL ID CLIENT]** et le champ **[!UICONTROL SECRET CLIENT]** collez les valeurs respectives que vous avez copiées précédemment.
1. Dans le coin inférieur droit de la boîte de dialogue, sélectionnez **[!UICONTROL Connexion]** et connectez-vous à Adobe IMS (Identity Management Services).

   Une fois la connexion établie, la boîte de dialogue de connexion à Adobe Analytics s’affiche à nouveau, avec le **[!UICONTROL SOCIÉTÉS]** liste déroulante, lancée par les entreprises à votre disposition.

1. Dans la **[!UICONTROL SOCIÉTÉS]** , choisissez une société.

   Une fois que vous avez sélectionné une société, la variable **[!UICONTROL SUITES]** La liste déroulante, lancée par les suites de rapports disponibles pour la société sélectionnée, devient visible.

1. Dans la **[!UICONTROL SUITES]** , choisissez une suite de rapports.

   >[!NOTE]
   >
   >Par défaut, l’utilisateur doit savoir que les deux **[!UICONTROL SOCIÉTÉS]** et **[!UICONTROL SUITES]** Les listes déroulantes sont vides. Ainsi, l’utilisateur doit sélectionner une valeur dans chaque liste.

1. Sélectionner **[!UICONTROL OK]** vous pouvez enregistrer la configuration.

   >[!NOTE]
   >
   >La variable **[!UICONTROL Serveur Adobe Analytics]** est renseigné avec un serveur de suivi tiers suggéré qui correspond à votre espace de noms analytics lorsque vous sélectionnez **[!UICONTROL OK]**. Si vous utilisez un autre serveur de suivi, mettez-le à jour dans ce champ pour éviter toute perte de données.

1. Dans le coin inférieur gauche de la page Configuration d’Adobe Analytics, sélectionnez **[!UICONTROL Enregistrer]** pour vous assurer que la configuration de votre compte Adobe Analytics est mise à jour.

>[!MORELIKETHIS]
>
>* [Configuration des rapports Adobe Analytics](configuring-analytics-reports.md#configuring_adobe_analytics_reports)
