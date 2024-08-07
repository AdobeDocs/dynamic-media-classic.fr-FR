---
title: Connexion à Adobe Analytics
description: Découvrez comment vous connecter à Adobe Analytics à partir d’Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 261b8f7c-c61c-4ce3-b9dc-8549347aca2e
topic: Integrations, Development
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 0%

---

# Connexion à Adobe Analytics{#log-in-to-adobe-analytics}

Vérifiez que vous êtes membre du groupe Accès aux services web dans Adobe Analytics. Avant de vous connecter, configurez les rapports Adobe Analytics et faites correspondre les variables de rapports Adobe Analytics aux événements Adobe Dynamic Media Classic. Les membres de ce groupe peuvent accéder à tous les rapports des suites de rapports spécifiées. Utilisez l’API des services Web de l’Experience Cloud, quelles que soient les autorisations définies dans l’interface. Pour ajouter un membre au groupe, dans Adobe Analytics, accédez à **[!UICONTROL Outils d’administration]** > **[!UICONTROL Gestion des utilisateurs]** > **[!UICONTROL Modifier les groupes]**.

Lorsque vous vous connectez, vous avez la possibilité de saisir votre ID d’organisation Experience Cloud afin d’utiliser la dernière mise en oeuvre d’analyse vidéo. Si vous choisissez de ne pas saisir votre identifiant, les rapports vidéo fonctionnent toujours. Cependant, cela peut empêcher l’intégration correcte des données avec d’autres données pour ce client en dehors d’Adobe Dynamic Media Classic.

>[!NOTE]
>
>Si votre compte Adobe Analytics a été migré vers l’authentification Adobe IMS (système Identity Management) pour la connexion, la saisie des informations d’identification directes ne fonctionne pas.

## Connexion à Adobe Analytics à partir d’Adobe Dynamic Media Classic {#log-in-to-analytics-from-dmc}

Commencez par intégrer Dynamic Media Classic à Adobe Analytics OAuth. L’intégration d’Adobe Analytics OAuth à Dynamic Media Classic n’est généralement effectuée qu’une seule fois par utilisateur.

1. Accédez à [Adobe Developer Console](https://developer.adobe.com/console). Assurez-vous que votre compte dispose des autorisations d’administrateur pour l’organisation pour laquelle l’intégration est requise.
1. Près du coin supérieur droit de la page d’accueil, dans la liste déroulante, sélectionnez la société appropriée. (La capture d’écran ci-dessous est fournie à titre d’information uniquement ; le nom réel de la société que vous sélectionnez peut varier.)

   ![Créer un projet](assets/analytics-oauth1.png)

1. Effectuez l’une des opérations suivantes :

   * En haut de la page, dans l’onglet **[!UICONTROL Accueil]**, sélectionnez **[!UICONTROL Créer un projet]**.
   * En haut de la page, dans l’onglet **[!UICONTROL Projets]** . Près du coin droit de la page, sélectionnez **[!UICONTROL Créer un projet]**.

1. Sur la page du projet, sélectionnez **[!UICONTROL Ajouter une API]**.
1. Sur la page **[!UICONTROL Ajouter une API]**, sélectionnez **[!UICONTROL Adobe Analytics]**.
1. Près du coin inférieur droit de la page, sélectionnez **[!UICONTROL Suivant]**.

   ![Ajouter une API](assets/analytics-oauth2.png)

1. Sur la page **[!UICONTROL `Configure API`]**, sélectionnez **[!UICONTROL USER AUTHENTICATION OAuth]**.
1. Près du coin inférieur droit de la page, sélectionnez **[!UICONTROL Suivant]**.
1. Sur la page **[!UICONTROL `Configure API`]**, sélectionnez **[!UICONTROL OAUTH 2.0 Web]**.
1. Dans le champ de texte **[!UICONTROL URI de redirection par défaut]**, saisissez le chemin suivant exactement comme indiqué :

   `https://exploreadobe.com/dynamic-media-upgrade/`

1. Dans le champ de texte **[!UICONTROL Redirect URI pattern]** , saisissez le chemin suivant exactement comme indiqué :

   `https://exploreadobe\.com/dynamic-media-upgrade/`

1. Dans le coin inférieur droit de la page, sélectionnez **[!UICONTROL Enregistrer l’API configurée]**.
1. Dans le panneau de navigation, sur le côté gauche de la page Adobe Analytics, sous **[!UICONTROL Credentials]**, sélectionnez **[!UICONTROL OAuth Web]**.
1. Sous **[!UICONTROL Credential details]**, procédez comme suit :
   * Sous **[!UICONTROL ID client]**, sélectionnez **[!UICONTROL Copier]** pour copier la valeur. Vous avez besoin de cette valeur pour la configuration Analytics suivante dans l’application de bureau Dynamic Media Classic à suivre.
   * Sous **[!UICONTROL Client Secret]**, sélectionnez **[!UICONTROL Récupérer le secret client]** pour afficher la valeur associée. Sélectionnez **[!UICONTROL Copy]** pour copier la valeur. Vous avez besoin de cette valeur pour la configuration Adobe Analytics suivante dans l’application de bureau Dynamic Media Classic à suivre.

## Configuration d’Adobe Analytics dans Adobe Dynamic Media Classic {#configure-analytics-in-dmc}

>[!NOTE]
>
>Après la configuration initiale d’Adobe Analytics dans Dynamic Media Classic, la seule fois où vous devez rétablir la configuration est dans les cas suivants :
>
>* Un nouveau rapport est ajouté dans Analytics et l’utilisateur souhaite commencer à envoyer des données à ce nouveau rapport.
>* Le serveur de suivi est mis à jour dans Adobe Analytics.
>* Une nouvelle variable de suivi est introduite dans un rapport et vous souhaitez lier une variable de visionneuse spécifique dans l’interface utilisateur de Dynamic Media Classic à cette nouvelle variable Analytics.
>

1. Près du coin supérieur droit de l’application de bureau Adobe Dynamic Media Classic, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]**.
1. Dans le panneau de gauche, sous **[!UICONTROL Configuration de l’application]**, sélectionnez **[!UICONTROL Adobe Analytics]**.
1. Sur la page **[!UICONTROL Configuration Adobe Analytics]**, sélectionnez **[!UICONTROL Adobe Analytics Login]**.
1. Dans la boîte de dialogue **[!UICONTROL Connexion Adobe Analytics]**, dans le champ **[!UICONTROL ID CLIENT]** et le champ **[!UICONTROL SECRET CLIENT]**, collez les valeurs respectives que vous avez copiées précédemment.
1. Dans le coin inférieur droit de la boîte de dialogue, sélectionnez **[!UICONTROL Login]** et connectez-vous à Adobe IMS (Identity Management Services).

   Une fois que vous êtes connecté, la boîte de dialogue Connexion Adobe Analytics s’affiche à nouveau avec la liste déroulante **[!UICONTROL SOCIÉTÉS]**, lancée par les entreprises à votre disposition.

1. Dans la liste déroulante **[!UICONTROL SOCIÉTÉS]** , sélectionnez une société.

   Une fois que vous avez sélectionné une société, la liste déroulante **[!UICONTROL SUITES]**, lancée par les suites de rapports disponibles pour la société sélectionnée, devient visible.

1. Dans la liste déroulante **[!UICONTROL SUITES]** , choisissez une suite de rapports.

   >[!NOTE]
   >
   >Par défaut, l’utilisateur doit savoir que les listes déroulantes **[!UICONTROL COMPANIES]** et **[!UICONTROL SUITES]** sont vides. Ainsi, l’utilisateur doit sélectionner une valeur dans chaque liste.

1. Sélectionnez **[!UICONTROL OK]** pour enregistrer la configuration.

   >[!NOTE]
   >
   >Le champ **[!UICONTROL Serveur Adobe Analytics]** est renseigné avec un serveur de suivi tiers suggéré qui correspond à votre espace de noms Analytics lorsque vous sélectionnez **[!UICONTROL OK]**. Si vous utilisez un autre serveur de suivi, mettez-le à jour dans ce champ pour éviter toute perte de données.

1. Dans le coin inférieur gauche de la page Configuration Adobe Analytics, sélectionnez **[!UICONTROL Enregistrer]** pour vous assurer que la configuration de votre compte Adobe Analytics est mise à jour.

>[!MORELIKETHIS]
>
>* [Configuration des rapports Adobe Analytics](configuring-analytics-reports.md#configuring_adobe_analytics_reports)
