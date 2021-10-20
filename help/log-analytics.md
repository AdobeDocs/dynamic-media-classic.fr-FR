---
title: Connexion à Adobe Analytics
description: Découvrez comment vous connecter à Adobe Analytics depuis Adobe Dynamic Media Classic.
uuid: 5614babe-1097-4228-a3dc-27e5a25366d5
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: e5b510a8-8b7f-4c60-869e-d664a8157e63
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 261b8f7c-c61c-4ce3-b9dc-8549347aca2e
source-git-commit: 8111895ac527b92b152382ea80b7b383659f00a9
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 1%

---

# Connexion à Adobe Analytics{#log-in-to-adobe-analytics}

Avant de vous connecter pour configurer les rapports Adobe Analytics et faire correspondre les variables de rapport Adobe Analytics aux événements Adobe Dynamic Media Classic, vérifiez que vous êtes membre du groupe Accès aux services Web dans Adobe Analytics. Les membres de ce groupe peuvent accéder à tous les rapports des suites de rapports spécifiées par le biais de l’API des services Web de l’Experience Cloud, indépendamment des autorisations définies dans l’interface. Pour ajouter un membre au groupe, dans Adobe Analytics, accédez à la section **[!UICONTROL Outils d’administration]** > **[!UICONTROL Gestion des utilisateurs]** > **[!UICONTROL Modifier les groupes]**.

Lorsque vous vous connectez, vous avez la possibilité de saisir votre ID d’organisation d’Experience Cloud pour utiliser la dernière mise en oeuvre de l’analyse vidéo. Si vous choisissez de ne pas saisir votre ID, la création de rapports vidéo fonctionne toujours. Toutefois, cela peut entraîner une mauvaise intégration des données avec d&#39;autres données pour ce client en provenance d&#39;Adobe Dynamic Media Classic externe.

>[!NOTE]
>
>Si votre compte Adobe Analytics a été migré vers l’authentification Adobe IMS (système Identity Management) pour la connexion, la saisie d’informations d’identification directes ne fonctionne pas.

## Connectez-vous à Adobe Analytics à partir de Adobe Dynamic Media Classic. {#log-in-to-analytics-from-dmc}

Commencez par intégrer Dynamic Media Classic à Adobe Analytics OAuth. L’intégration Adobe Analytics OAuth avec Dynamic Media Classic n’est généralement effectuée qu’une seule fois par utilisateur.

1. Accès [Adobe Developer Console](https://developer.adobe.com/console). Assurez-vous que votre compte dispose d’autorisations d’administrateur pour l’organisation pour laquelle l’intégration est requise.
1. Dans la liste déroulante, dans le coin supérieur droit de la page d’accueil, sélectionnez la société appropriée. (La capture d’écran ci-dessous est fournie à titre d’information uniquement ; le nom de la société que vous sélectionnez peut varier.)

   ![Créez un projet](assets/analytics-oauth1.png)

1. Utilisez l’une des méthodes suivantes :

   * En haut de la page, à partir de **[!UICONTROL Accueil]** , sélectionnez **[!UICONTROL Créer un projet]**.
   * En haut de la page, à partir de **[!UICONTROL Projets]** . Dans le coin droit de la page, sélectionnez **[!UICONTROL Créer un projet]**.

1. Sur la page du projet, sélectionnez **[!UICONTROL Ajouter une API]**.
1. Sur la **[!UICONTROL Ajout d’une API]** , sélectionnez **[!UICONTROL Adobe Analytics]**.
1. Dans le coin inférieur droit de la page, sélectionnez **[!UICONTROL Suivant]**.

   ![Ajout d’une API](assets/analytics-oauth2.png)

1. Sur la **[!UICONTROL Configurer l’API]** , sélectionnez **[!UICONTROL AUTHENTIFICATION DE L’UTILISATEUR OAuth]**.
1. Dans le coin inférieur droit de la page, sélectionnez **[!UICONTROL Suivant]**.
1. Sur la **[!UICONTROL Configurer l’API]** , sélectionnez **[!UICONTROL Web OAUTH 2.0]**.
1. Dans la boîte de dialogue **[!UICONTROL URI de redirection par défaut]** , entrez le chemin suivant exactement comme indiqué :

   `https://exploreadobe.com/dynamic-media-upgrade/`

1. Dans la boîte de dialogue **[!UICONTROL Motif URI de redirection]** , entrez le chemin suivant exactement comme indiqué :

   `https://exploreadobe\.com/dynamic-media-upgrade/`

1. Dans le coin inférieur droit de la page, sélectionnez **[!UICONTROL Enregistrer l’API configurée]**.
1. Dans le panneau de navigation, sur le côté gauche de la page Adobe Analytics, sous **[!UICONTROL Informations]**, sélectionnez **[!UICONTROL OAuth Web]**.
1. Sous **[!UICONTROL Informations d’identification]**, procédez comme suit :
   * Sous **[!UICONTROL ID client]**, sélectionnez **[!UICONTROL Copier]** pour copier la valeur. Vous devez utiliser cette valeur pour la configuration suivante d’Analytics dans l’application de bureau Dynamic Media Classic à suivre.
   * Sous **[!UICONTROL Secret client]**, sélectionnez **[!UICONTROL Récupérer le secret client]** pour afficher la valeur associée. Sélectionner **[!UICONTROL Copier]** pour copier la valeur. Vous avez besoin de cette valeur pour la configuration Adobe Analytics ultérieure dans l’application de bureau Dynamic Media Classic à suivre.

## Configuration d’Adobe Analytics dans Adobe Dynamic Media Classic {#configure-analytics-in-dmc}

>[!NOTE]
>
>Après votre configuration initiale d’Adobe Analytics dans Dynamic Media Classic, les seules fois où vous devez rétablir la configuration sont les cas suivants :
>
>* Un nouveau rapport est ajouté dans Analytics et l’utilisateur souhaite commencer à envoyer des données à ce nouveau rapport.
>* Le serveur de suivi est mis à jour dans Adobe Analytics.
>* Une nouvelle variable de suivi est introduite dans un rapport et vous souhaitez lier une variable Visionneuse spécifique dans l’interface utilisateur Dynamic Media Classic à cette nouvelle variable Analytics.

>


1. Dans le coin supérieur droit de l’application pour postes de travail Adobe Dynamic Media Classic, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l&#39;application]**.
1. Dans le panneau de gauche, sous **[!UICONTROL Configuration de l&#39;application]**, sélectionnez **[!UICONTROL Adobe Analytics]**.
1. Sur la **[!UICONTROL Configuration d&#39;Adobe Analytics]** , sélectionnez **[!UICONTROL Connexion Adobe Analytics]**.
1. Dans la boîte de dialogue **[!UICONTROL Connexion Adobe Analytics]** , dans la boîte de dialogue **[!UICONTROL ID CLIENT]** et **[!UICONTROL SECRET CLIENT]** , collez les valeurs respectives que vous avez copiées précédemment.
1. Dans le coin inférieur droit de la boîte de dialogue, sélectionnez Se connecter et effectuez votre connexion Adobe IMS (Identity Management Services).

   Une fois que vous vous êtes connecté, la boîte de dialogue Connexion Adobe Analytics s’affiche de nouveau avec le **[!UICONTROL ENTREPRISES]** liste déroulante, lancée par les sociétés qui vous sont disponibles.

1. De **[!UICONTROL ENTREPRISES]** , sélectionnez une société.

   Une fois que vous avez sélectionné une société, la **[!UICONTROL SUITES]** La liste déroulante, lancée par les suites de rapports disponibles pour la société sélectionnée, devient visible.

1. De **[!UICONTROL SUITES]** , sélectionnez une suite de rapports.

   >[!NOTE]
   >
   >Par défaut, l’utilisateur doit être conscient du fait que les deux **[!UICONTROL ENTREPRISES]** et **[!UICONTROL SUITES]** les listes déroulantes sont vides. Ainsi, l’utilisateur doit sélectionner une valeur dans chaque liste.

1. Sélectionner **[!UICONTROL OK]** pour pouvoir enregistrer la configuration.

   >[!NOTE]
   >
   >Le **[!UICONTROL Serveur Adobe Analytics]** est renseigné avec un serveur de suivi tiers suggéré qui correspond à votre espace de noms analytique lorsque vous sélectionnez **[!UICONTROL OK]**. Si vous utilisez un autre serveur de suivi, mettez-le à jour dans ce champ pour éviter la perte de données.

1. Dans le coin inférieur gauche de la page Configuration Adobe Analytics, sélectionnez **[!UICONTROL Enregistrer]** pour vous assurer que la configuration de votre compte Adobe Analytics est mise à jour.

>[!MORELIKETHIS]
>
>* [Configuration des rapports Adobe Analytics](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

