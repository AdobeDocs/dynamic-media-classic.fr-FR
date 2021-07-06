---
title: Configuration des rapports Adobe Analytics
description: Découvrez comment configurer des rapports Adobe Analytics.
uuid: bf210f68-dcb0-4e86-be04-0a8b2117ef2a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: f4c8c2b3-cc95-416f-9a5d-da81c231dfc2
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: d9fda3b8-7da8-4a30-a5f8-9bb34ec1b43d
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '1196'
ht-degree: 46%

---

# Configuration des rapports Adobe Analytics{#configuring-adobe-analytics-reports}

Pour indiquer à Adobe Analytics quelles informations reporter dans les rapports Adobe Analytics, accédez à l’écran de configuration d’Adobe Analytics. Une fois les rapports configurés, cet écran répertorie, pour chaque événement de visionneuse dont vous souhaitez obtenir des informations, une variable Adobe Analytics et une variable Dynamic Media Classic correspondantes. Ces combinaisons d’événements de visionneuse-variable Adobe Analytics-variable Dynamic Media Classic déterminent les informations signalées.

Outre l’association d’événements de visionneuse à des variables, l’écran de configuration d’Adobe Analytics propose des outils pour activer, modifier et supprimer des événements de visionneuse.

>[!NOTE]
>
>Chaque fois que vous modifiez les paramètres du rapport Adobe Analytics dans Adobe Analytics, assurez-vous de vous reconnecter à Adobe Analytics depuis Adobe Dynamic Media Classic, de réenregistrer vos paramètres de configuration Adobe Analytics, puis de republier.

Voir [Connexion à Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Voir [Publication des informations de configuration](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## Affectation de variables Adobe Analytics à des événements et variables de visionneuse Dynamic Media Classic {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

Utilisez l’écran Configuration d’Adobe Analytics pour associer des événements de visionneuse à des variables Adobe Analytics et à des variables Dynamic Media Classic. Pour chaque événement de visionneuse, choisissez une variable Adobe Analytics et une variable Dynamic Media Classic. Pour obtenir des instructions sur l’ouverture de l’écran de configuration d’Adobe Analytics, voir [Connexion à Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

**Pour affecter des variables Adobe Analytics aux événements et variables de visionneuse Dynamic Media Classic**

1. Après vous être connecté à Adobe Analytics à partir de Dynamic Media Classic et avoir sélectionné une suite de rapports, sur la page de configuration d’Adobe Analytics, dans la colonne de droite du tableau, activez un événement de visionneuse en cliquant sur **[!UICONTROL Activer]**.
1. Sous la colonne Variables, affichez le sélecteur de paires de variables en cliquant sur la touche fléchée de l’événement de visionneuse de votre choix.

   Voir [Evénements de visionneuse](configuring-analytics-reports.md#viewer_events).

1. Ajoutez une variable Dynamic Media Classic.

   Voir [Variables Dynamic Media Classic](configuring-analytics-reports.md#scene7_variables).

1. Ajoutez une variable Adobe Analytics.
1. (Facultatif) Pour ajouter une autre paire de variables, cliquez sur **Ajouter**.
1. Cliquez sur **Enregistrer**.

   Une fois que vous avez cliqué sur Enregistrer, l’événement de visionneuse, sa variable Adobe Analytics et sa variable Dynamic Media Classic sont répertoriés dans l’écran de configuration d’Adobe Analytics.

1. Dans le coin inférieur droit, cliquez sur **Fermer**.
1. Cliquez sur **Publier** > **Lancer public.** pour exécuter une publication sur hébergeur d’images.

   La publication est nécessaire pour que les informations contenues dans les visionneuses soient disponibles sur les serveurs Dynamic Media Classic.

### Evénements de visionneuse {#viewer-events}

Les événements de visionneuse décrivent les actions que les utilisateurs effectuent avec les visionneuses Dynamic Media Classic. Lorsqu’un utilisateur lance une action spécifique, comme un clic sur une miniature ou le démarrage ou l’arrêt d’une vidéo, la visionneuse &quot;diffuse&quot; un événement sur la page web, ainsi que les données associées à cet événement.

Le tableau ci-après décrit les événements de visionneuse que vous pouvez ajouter à l’écran de configuration d’Adobe Analytics.

| Evénement de visionneuse | Prise en charge et visionneuses de la plate-forme de la visionneuse HTML5 | Description |
|--- |--- |--- |
| CHARGEMENT | **X** (catalogue électronique, fenêtre déroulante, visionneuse à 360°, vidéo, zoom) | Lorsqu’un utilisateur démarre la visionneuse. |
| PAGE | **X** (catalogue électronique) | Lorsqu’un utilisateur tourne une page d’un catalogue électronique ; lorsqu’un utilisateur clique sur une autre cible ou une autre nuance dans des visionneuses de zoom ciblées. |
| PERMUTATION | **X** (catalogue électronique, fenêtre déroulante, visionneuse à 360°, vidéo, zoom) | Lorsqu’un utilisateur clique sur une autre miniature pour voir une autre image. |
| OBJET | **X** (catalogue électronique) | Lorsqu’un utilisateur place le pointeur sur une zone cliquable afin d’afficher le texte de survol associé, et ce, dans une visionneuse prenant en charge les zones cliquables comportant du texte de survol. |
| HREF | **X** (catalogue électronique) | Lorsqu’un utilisateur clique sur une URL dans une zone cliquable dans des visionneuses prenant en charge les zones cliquables. |
| CIBLE |  | Lorsqu’un utilisateur clique sur une cible de zoom pour zoomer sur une partie d’une image dans des visionneuses de zoom ciblées. |
| RECHERCHE |  | Lorsqu’un utilisateur effectue une recherche textuelle dans des catalogues électroniques. |
| LECTURE | **X** (vidéo) | Lorsqu’un utilisateur clique sur Lecture pour commencer à lire une vidéo dans une visionneuse de vidéos.<br><br>**Remarque :** Si vous utilisez les rapports vidéo basés sur la pulsation Adobe Analytics, vous n’avez pas besoin de mapper de variables à cet événement de visionneuse lorsque vous configurez Adobe Analytics dans Dynamic Media Classic. Video Heartbeat fonctionne avec les visionneuses vidéo HTML5 et de supports variés Dynamic Media Classic prêtes à l’emploi. Le lecteur vidéo génère des données de suivi à afficher dans les rapports vidéo d’Adobe Analytics. Voir [Activation des rapports vidéo Adobe Analytics](enabling-analytics-video-reports.md). |
| PAUSE | **X** (vidéo) | Lorsqu’un utilisateur clique sur Pause pour interrompre la lecture d’une vidéo dans une visionneuse de vidéos.<br><br>**Remarque :** Si vous utilisez les rapports vidéo basés sur la pulsation Adobe Analytics, vous n’avez pas besoin de mapper de variables à cet événement de visionneuse lorsque vous configurez Adobe Analytics dans Dynamic Media Classic. Video Heartbeat fonctionne avec les visionneuses vidéo HTML5 et de supports variés Dynamic Media Classic prêtes à l’emploi. Le lecteur vidéo génère des données de suivi à afficher dans les rapports vidéo d’Adobe Analytics. Voir [Activation des rapports vidéo Adobe Analytics](enabling-analytics-video-reports.md). |
| ARRET | **X** (vidéo) | Lorsqu’un utilisateur clique sur Arrêt pour arrêter la lecture d’une vidéo dans une visionneuse de vidéos.<br><br>**Remarque :** Si vous utilisez les rapports vidéo basés sur la pulsation Adobe Analytics, vous n’avez pas besoin de mapper de variables à cet événement de visionneuse lorsque vous configurez Adobe Analytics dans Dynamic Media Classic. Video Heartbeat fonctionne avec les visionneuses vidéo HTML5 et de supports variés Dynamic Media Classic prêtes à l’emploi. Le lecteur vidéo génère des données de suivi à afficher dans les rapports vidéo d’Adobe Analytics. Voir [Activation des rapports vidéo Adobe Analytics](enabling-analytics-video-reports.md). |
| JALON | **X**  (Vidéo) | Dans les visionneuses de vidéos, des événements de référence sont créés lorsque l’utilisateur regarde 0, 25, 50, 75 ou 100 % de la vidéo.<br><br>**Remarque :** Si vous utilisez les rapports vidéo basés sur la pulsation Adobe Analytics, vous n’avez pas besoin de mapper de variables à cet événement de visionneuse lorsque vous configurez Adobe Analytics dans Dynamic Media Classic. Video Heartbeat fonctionne avec les visionneuses vidéo HTML5 et de supports variés Dynamic Media Classic prêtes à l’emploi. Le lecteur vidéo génère des données de suivi à afficher dans les rapports vidéo d’Adobe Analytics. Voir [Activation des rapports vidéo Adobe Analytics](enabling-analytics-video-reports.md). |
| NUANCES | X (fenêtre déroulante, zoom) | Cet événement de visionneuse est mappé sur l’événement de visionneuse PAGE dans Dynamic Media Classic. |
| ZOOM | **X** (catalogue électronique, visionneuse à 360°, zoom) | Non suivi par Adobe Analytics.<br> |
| PANORAMIQUE | **X** (catalogue électronique, visionneuse à 360°, zoom) | Non suivi par Adobe Analytics.<br> |
| ROTATION | **X** (visionneuse à 360°) | Non suivi par Adobe Analytics.<br> |


### Variables Dynamic Media Classic {#scene-variables}

Pour chaque événement de visionneuse de l’écran de configuration d’Adobe Analytics, choisissez une variable Adobe Analytics et une *variable Dynamic Media Classic*. Les variables Dynamic Media Classic représentent les données que vous pouvez obtenir pour un rapport. Par exemple, la variable `searchTerm` répertorie les mots-clés utilisés dans les recherches effectuées dans les catalogues électroniques.

Le tableau suivant décrit les variables Dynamic Media Classic.

| Variable Dynamic Media Classic | Description |
|--- |:--- |
| asset | Identifiant de ressource ou fichier de chemin d’accès vidéo Dynamic Media Classic. |
| viewerId | Numéro arbitraire attribué à chaque type de visionneuse |
| pageLabel | Dans un catalogue électronique, page affichée par une visionneuse |
| label | Valeur de l’étiquette (chaîne). |
| frame | Page ou référence de page dans une visionneuse d’images. |
| rollover_keyRaw | Valeur HREF complète, et non pas seulement la partie traitée. |
| rollover_keyProc | ID d’un objet référencé dans une zone cliquable (valide pour les événements href et objet) |
| searchTerm | Terme utilisé dans le cadre d’une recherche de catalogue électronique |
| timeStamp | Lecture, Arrêt et Pause choisis dans les visionneuses de vidéos. |
| progress | Pourcentage d’achèvement d’un événement de référence |
| targetId | Valeur de l’ID (nombre). |

## Activation, modification et suppression d’événements de visionneuse {#activating-editing-and-deleting-viewer-events}

Sur l’écran de configuration d’Adobe Analytics, vous pouvez activer, modifier et supprimer des événements de visionneuse :

* ****
ActivationCliquez sur  **** Activer pour activer ou  **** désactiver l’événement de visionneuse sélectionné.

* ****
Modification : sélectionnez un événement de visionneuse, puis cliquez sur le bouton gris  **[!UICONTROL Afficher/]** Modifier les variables. Dans les listes déroulantes Variable Dynamic Media Classic et Variable Adobe Analytics , sélectionnez une variable différente dans chaque liste respective. Pour plus d’informations, voir Attribution de variables Adobe Analytics aux événements et variables de visionneuse Dynamic Media Classic .

* ****
Suppression : sélectionnez un événement de visionneuse, puis cliquez sur le bouton gris  **[!UICONTROL Afficher/]** Modifier les variables. Cliquez sur **[!UICONTROL Supprimer]**.
