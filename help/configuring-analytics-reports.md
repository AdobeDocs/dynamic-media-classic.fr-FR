---
title: Configuration des rapports Adobe Analytics
seo-title: Configuration des rapports Adobe Analytics
description: 'null'
seo-description: Découvrez comment configurer les rapports Adobe Analytics.
uuid: bf210f68-dcb0-4e86-be04-0a8b2117ef2a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: f4c8c2b3-cc95-416f-9a5d-da81c231dfc2
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '1204'
ht-degree: 51%

---


# Configuration des rapports Adobe Analytics{#configuring-adobe-analytics-reports}

Pour indiquer à Adobe Analytics quelles informations reporter dans les rapports Adobe Analytics, accédez à l’écran de configuration d’Adobe Analytics. Une fois les rapports configurés, cet écran liste, pour chaque événement de visionneuse dont vous souhaitez obtenir des informations, une variable Adobe Analytics correspondante et une variable Dynamic Media Classic. Ces combinaisons de variables de événements de visionneuse-Adobe Analytics-Dynamic Media Classic déterminent quelles informations sont rapportées.

En plus d’associer les événements de visionneuse aux variables, l’écran de configuration d’Adobe Analytics propose des outils permettant d’activer, de modifier et de supprimer des événements de visionneuse.

>[!NOTE]
>
>Chaque fois que vous modifiez les paramètres du rapport Adobe Analytics dans Adobe Analytics, veillez à vous reconnecter à Adobe Analytics à partir de Adobe Dynamic Media Classic, à réenregistrer vos paramètres de configuration Adobe Analytics, puis à republier.

Voir [Connexion à Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Voir [Publication des informations de configuration](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## Affectation de variables Adobe Analytics à des événements et variables de visionneuse Dynamic Media Classic {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

Utilisez l’écran Configuration Adobe Analytics pour associer des événements de visionneuse à des variables Adobe et à des variables Dynamic Media Classic. Pour chaque événement de visionneuse, choisissez une variable Adobe Analytics et une variable Dynamic Media Classic. Pour obtenir des instructions sur l’ouverture de l’écran de configuration d’Adobe Analytics, voir [Connexion à Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

**Pour affecter des variables Adobe Analytics à des événements et variables de visionneuse Dynamic Media Classic**

1. After you log in to Adobe Analytics from within Dynamic Media Classic and select a report suite, on the Adobe Analytics Configuration page, in the far right column of the table, activate a viewer event by clicking **Enable**.
1. Sous la colonne Variables, affichez le sélecteur de paires de variables en cliquant sur la touche fléchée de l’événement de visionneuse de votre choix.

   Voir [Evénements de visionneuse](configuring-analytics-reports.md#viewer_events).

1. Ajoutez une variable Dynamic Media Classic.

   Voir Variables [](configuring-analytics-reports.md#scene7_variables)Dynamic Media Classic.

1. Ajoutez une variable Adobe Analytics.
1. (Facultatif) Pour ajouter une autre paire de variables, cliquez sur **Ajouter**.
1. Cliquez sur **Enregistrer**.

   Une fois que vous avez cliqué sur Enregistrer, le événement de la visionneuse, sa variable Adobe Analytics et sa variable Dynamic Media Classic sont répertoriés dans l’écran de configuration Adobe.

1. Dans le coin inférieur droit, cliquez sur **Fermer**.
1. Cliquez sur **Publier** > **Lancer public.** pour exécuter une publication sur hébergeur d’images.

   La publication est nécessaire pour que les informations contenues dans les visionneuses soient disponibles sur les serveurs Dynamic Media Classic.

### Evénements de visionneuse {#viewer-events}

Les événements de visionneuse décrivent les actions que les utilisateurs effectuent avec les visionneuses Dynamic Media Classic. Lorsqu’un utilisateur initie une certaine action (en cliquant sur une vignette ou en lançant ou arrêtant la lecture d’une vidéo, par exemple), la visionneuse « diffuse » un événement sur la page Web, avec les données associées à cet événement.

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
| LECTURE | **X** (vidéo) | Lorsqu’un utilisateur clique sur Lecture pour commencer à lire une vidéo dans une visionneuse de vidéos.<br><br>**Remarque :**Si vous utilisez le rapports vidéo basé sur la pulsation Adobe Analytics, vous n’avez pas besoin de mapper des variables à ce événement de visionneuse lorsque vous configurez Adobe dans Dynamic Media Classic. La pulsation vidéo fonctionne avec les visionneuses de vidéos HTML5 et de supports variés Dynamic Media Classic prêtes à l’emploi. Le lecteur vidéo génère des données de suivi à afficher dans les rapports vidéo d’Adobe Analytics. See[Enabling Adobe Analytics Video Reports](enabling-analytics-video-reports.md). |
| PAUSE | **X** (vidéo) | Lorsqu’un utilisateur clique sur Pause pour interrompre la lecture d’une vidéo dans une visionneuse de vidéos.<br><br>**Remarque :**Si vous utilisez le rapports vidéo basé sur la pulsation Adobe Analytics, vous n’avez pas besoin de mapper des variables à ce événement de visionneuse lorsque vous configurez Adobe dans Dynamic Media Classic. La pulsation vidéo fonctionne avec les visionneuses de vidéos HTML5 et de supports variés Dynamic Media Classic prêtes à l’emploi. Le lecteur vidéo génère des données de suivi à afficher dans les rapports vidéo d’Adobe Analytics. See[Enabling Adobe Analytics Video Reports](enabling-analytics-video-reports.md). |
| ARRET | **X** (vidéo) | Lorsqu’un utilisateur clique sur Arrêt pour arrêter la lecture d’une vidéo dans une visionneuse de vidéos.<br><br>**Remarque :**Si vous utilisez le rapports vidéo basé sur la pulsation Adobe Analytics, vous n’avez pas besoin de mapper des variables à ce événement de visionneuse lorsque vous configurez Adobe dans Dynamic Media Classic. La pulsation vidéo fonctionne avec les visionneuses de vidéos HTML5 et de supports variés Dynamic Media Classic prêtes à l’emploi. Le lecteur vidéo génère des données de suivi à afficher dans les rapports vidéo d’Adobe Analytics. See[Enabling Adobe Analytics Video Reports](enabling-analytics-video-reports.md). |
| JALON | **X**  (Vidéo) | Dans les visionneuses de vidéos, des événements de référence sont créés lorsque l’utilisateur regarde 0, 25, 50, 75 ou 100 % de la vidéo.<br><br>**Remarque :**Si vous utilisez le rapports vidéo basé sur la pulsation Adobe Analytics, vous n’avez pas besoin de mapper des variables à ce événement de visionneuse lorsque vous configurez Adobe dans Dynamic Media Classic. La pulsation vidéo fonctionne avec les visionneuses de vidéos HTML5 et de supports variés Dynamic Media Classic prêtes à l’emploi. Le lecteur vidéo génère des données de suivi à afficher dans les rapports vidéo d’Adobe Analytics. See[Enabling Adobe Analytics Video Reports](enabling-analytics-video-reports.md). |
| NUANCES | X (fenêtre déroulante, zoom) | Ce événement de visionneuse est mappé au événement de visionneuse PAGE dans Dynamic Media Classic. |
| ZOOM | **X** (catalogue électronique, visionneuse à 360°, zoom) | Non suivi par Adobe Analytics.<br> |
| PANORAMIQUE | **X** (catalogue électronique, visionneuse à 360°, zoom) | Non suivi par Adobe Analytics.<br> |
| ROTATION | **X** (visionneuse à 360°) | Non suivi par Adobe Analytics.<br> |


### Variables Dynamic Media Classic {#scene-variables}

For each viewer event on Adobe Analytics Configuration screen, choose a Adobe Analytics variable and a *Dynamic Media Classic variable*. Les variables Dynamic Media Classic représentent les données que vous pouvez obtenir pour un rapport. Par exemple, la variable `searchTerm` répertorie les mots-clés utilisés dans les recherches effectuées dans les catalogues électroniques.

Le tableau suivant décrit les variables Dynamic Media Classic.

| Variable Dynamic Media Classic | Description |
|--- |:--- |
| asset | ID de fichier ou fichier de chemin d’accès vidéo Dynamic Media Classic. |
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

* **Activation** Cliquez sur **[!UICONTROL Activer]** pour activer ou **[!UICONTROL désactiver]** la désactivation d’un événement de visionneuse sélectionné.

* **Modification** Sélectionnez un événement de visionneuse, puis cliquez sur le bouton gris **[!UICONTROL Vue/Modifier]** les variables. Dans les listes déroulantes Variable Dynamic Media Classic et Variable Analytics Adobe, choisissez une variable différente dans chaque liste respective. Pour plus d’informations, voir Affectation de variables Adobe Analytics à des événements et variables de visionneuse Dynamic Media Classic.

* **Suppression** Sélectionnez un événement de visionneuse, puis cliquez sur le bouton gris **[!UICONTROL Vue/Modifier]** les variables. Cliquez sur **[!UICONTROL Supprimer]**.
