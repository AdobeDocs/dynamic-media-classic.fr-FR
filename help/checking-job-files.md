---
title: Vérification des fichiers de tâche
description: Découvrez comment vérifier les fichiers de tâche dans Adobe Dynamic Media Classic.
uuid: 8241a894-3014-4a5c-96ef-71f3aaa3716a
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: d53ae5dd-8daf-4d87-b9a6-3039bad30538
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: b6b11e1c-5eda-4bdb-8ffb-ecd3678f2352
source-git-commit: cb55e09a997b9d36002c4ac429603576d52fb8bd
workflow-type: tm+mt
source-wordcount: '1596'
ht-degree: 34%

---

# Vérification des fichiers de tâche{#checking-job-files}

Pour surveiller les chargements de fichiers vers Adobe Dynamic Media Classic et les fichiers que vous publiez sur les serveurs Adobe Dynamic Media Classic, Adobe Dynamic Media Classic propose la page Tâches . Vous pouvez consulter des tâches de téléchargement et de publication sur la page Tâches, y vérifier l’état des tâches et annuler des publications. Vous pouvez également planifier des tâches de téléchargement et de publication.

Lorsque vous téléchargez des fichiers, une icône rotative apparaît en regard du menu Tâches, indiquant qu’une tâche est en cours, ainsi que le nombre de fichiers en cours. Vous pouvez sélectionner l’icône pour afficher plus d’informations sur la tâche principale.

>[!NOTE]
>
>la liste des tâches récemment publiées est également disponible sur la page Activités récentes. Sélectionner **[!UICONTROL Récent]** dans la barre de navigation globale.

## A propos de la page Tâches {#about-the-jobs-page}

Sélectionner **[!UICONTROL Tâches]** dans la barre de navigation globale afin que la page Tâches s’ouvre. Par défaut, les tâches sont répertoriées de la plus récente à la moins récente.

Sur l’onglet Historique de la page Tâches, les tâches sont répertoriées selon les catégories suivantes :

* **[!UICONTROL Type de tâche]** - Une icône indique le type de tâche : Télécharger et publier sont les types de tâche les plus courants.

* **[!UICONTROL Nom de la tâche]** - Nom de la tâche. Le nom comprend la partie du nom saisie par l’utilisateur, ainsi que la date et l’heure.

* **[!UICONTROL Démarré]** - Lorsque la tâche a commencé.

* **[!UICONTROL Total]** - Nombre de fichiers transférés.

* **[!UICONTROL W (warnings)]** - Nombre d’avertissements dans la tâche (le cas échéant). Les avertissements indiquent des problèmes associés à la tâche qui sont sans effet sur son exécution globale. Ces avertissements peuvent généralement être ignorés parce qu’ils sont signalés dans des fichiers masqués. Par exemple : `.DS_store` Les fichiers (Macintosh) et les fichiers Thumbs.db (Windows®) contiennent des informations sur l’affichage des fichiers image aux utilisateurs. Toutefois, les entrées d’avertissement concernant ces fichiers peuvent être ignorées, car elles ne concernent pas l’utilisation de ces fichiers dans Adobe Dynamic Media Classic. Vous pouvez cliquer deux fois sur un nom de tâche pour obtenir des informations détaillées sur les avertissements la concernant.

* **[!UICONTROL E (Erreurs)]** - Répertorie le nombre d’erreurs dans la tâche (le cas échéant). Vous pouvez cliquer deux fois sur un nom de tâche pour obtenir des informations détaillées sur les erreurs la concernant.

* **[!UICONTROL Durée]** - Le temps nécessaire pour terminer le travail.

* **[!UICONTROL État]** - Affiche l’état de la tâche.

* **[!UICONTROL Destination]** - Pour les tâches de chargement, le nom de l’entreprise et le dossier dans lequel les fichiers ont été chargés. Cette catégorie ne s’applique pas aux tâches publiées.

* **[!UICONTROL Envoyé par]** - Répertorie les personnes qui ont chargé les ressources.

>[!NOTE]
>
>Vous pouvez annuler des tâches de publication et de chargement en cours en sélectionnant **[!UICONTROL Annuler]** en regard de la barre de progression.

## Modification des vues sur la page Tâches {#changing-views-on-the-jobs-page}

Pour trier des tâches ou modifier votre affichage sur l’onglet Historique de la page Tâches, appliquez les techniques suivantes :

* **[!UICONTROL Tri]** - Sélectionnez un nom de colonne pour trier la liste selon une colonne particulière. Vous pouvez sélectionner le bouton bascule près du nom de la colonne pour trier les entrées par ordre croissant ou décroissant.

* **[!UICONTROL Période]** - Sélectionnez la variable **[!UICONTROL Période]** et choisissez une option pour limiter la liste des tâches à la date actuelle, à la semaine précédente ou au mois précédent. Sélectionner **[!UICONTROL Période personnalisée]**, puis saisissez une période spécifique.

* **[!UICONTROL Type de tâche]** - Sélectionnez la variable **[!UICONTROL Type de tâche]** et choisissez **[!UICONTROL Publier]** ou **[!UICONTROL Télécharger]** pour restreindre la liste afin de publier des tâches ou de charger des tâches. Sélectionner **[!UICONTROL Tous]** pour afficher les deux types de tâches.

* **[!UICONTROL Afficher]** - Accédez à **[!UICONTROL Afficher]** > **[!UICONTROL Mes tâches]** ou **[!UICONTROL Afficher]** > **[!UICONTROL Toutes les tâches]** pour restreindre la liste aux tâches commandées ou aux tâches commandées par des personnes de votre entreprise.

## Affichage, copie ou impression d’un rapport Détails de la tâche {#viewing-copying-or-printing-a-job-details-report}

Double-cliquez sur le nom d’un rapport sur la page Tâches pour ouvrir la page Détails de la tâche. Cette page présente un récapitulatif sur les fichiers de la tâche. Sélectionner **[!UICONTROL Afficher les détails]** afin que vous puissiez voir l’Adobe Dynamic Media Classic ID, le chemin de destination et les informations d’état d’une entrée. Si vous avez téléchargé un fichier PDF ou PostScript qui nécessite des polices qui ne sont pas disponibles dans Adobe Dynamic Media Classic, le rapport répertorie les polices manquantes.

Vous pouvez copier ces informations dans le Presse-papiers.

1. Double-cliquez sur le nom d’un rapport sur la page Tâches.
1. Sur la page Détails de la tâche, sélectionnez **[!UICONTROL Afficher les détails]** pour obtenir un rapport détaillé sur une entrée.
1. Sélectionner **[!UICONTROL Copier dans le Presse-papiers]**.

## Gestion des tâches de chargement et de publication récurrentes {#handling-recurring-upload-and-publish-jobs}

Les tâches de téléchargement et de publication périodiques que vous créez dans les pages Télécharger et Publier sont répertoriées dans l’onglet Planifiée de la page Tâches. Vous pouvez éditer et supprimer des tâches périodiques dans l’onglet Planifiée.

Sélectionnez le bouton Tâches dans la barre de navigation globale, puis, sur la page Tâches, sélectionnez l’option **[!UICONTROL Planifié]** pour pouvoir modifier et supprimer des tâches récurrentes.

>[!NOTE]
>
>Vous pouvez filtrer la liste des tâches sur la page **[!UICONTROL Planifié]** avec l’onglet **[!UICONTROL Type de tâche]** et **[!UICONTROL Afficher]** menus. Sélectionnez un type de tâche afin de limiter la liste aux tâches d’un type spécifique. Sélectionnez une **[!UICONTROL Afficher]** si vous souhaitez afficher les tâches que vous avez créées ou créées par toutes les personnes de votre entreprise.

### Modification, suppression, pause et reprise de tâches récurrentes {#editing-deleting-pausing-and-resuming-recurring-jobs}

Sélectionnez une tâche récurrente sur la page Tâches et suivez ces instructions si vous souhaitez la modifier ou la supprimer :

* **Modification d’une tâche récurrente** - Sélectionnez la variable **[!UICONTROL Modifier]** et saisissez les informations de planification dans la boîte de dialogue Modifier la tâche planifiée . Si vous souhaitez que la tâche se répète à l’intervalle de votre choix, accédez à **[!UICONTROL Répéter]** > **[!UICONTROL Personnalisé]**.

Voir [Création d’un intervalle de temps de tâche de téléchargement ou de publication personnalisé](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

* **Suppression d’une tâche récurrente** - Sélectionnez la variable **[!UICONTROL Supprimer]** bouton .

* **Suspension (et reprise) d’une tâche récurrente** - Dans la colonne Principale, désélectionnez une case à cocher pour suspendre une tâche. cochez une case pour reprendre une tâche en pause.

### Création d’un intervalle de temps de tâche de téléchargement ou de publication personnalisé {#creating-a-custom-upload-or-publish-job-time-interval}

Pour créer un intervalle de temps personnalisé pour une tâche de téléchargement (via FTP) ou de publication, sur la page Télécharger ou Publier , accédez à **[!UICONTROL Répéter]** > **[!UICONTROL Personnalisé]**. Saisissez ensuite des nombres et des caractères génériques dans la zone Règle pour décrire un intervalle de temps entre les tâches de téléchargement ou de publication à répéter.

La syntaxe de définition des intervalles personnalisés de périodicité de téléchargement ou de publication dans la zone Règle se présente comme suit :

`[seconds]` `[minutes]` `[hour of day]` `[day of month]` `[month]` `[day of week]`

Par exemple : `0 15 10 * * ?` planifie une tâche à 10h15 tous les jours.

Les tableaux et la liste ci-après expliquent comment définir un intervalle dans la zone Règle.

Ce tableau indique les incréments temporels, leurs valeurs autorisées et les caractères génériques qu’ils prennent en charge :

| Incréments temporels | Valeurs autorisées | Commentaires | Caractères génériques pris en charge |
|--- |--- |--- |--- |
| Secondes | 0 à 59 |  | `, - * /` |
| Minutes | 0 à 59 |  | `, - * /` |
| Heures | 0 à 23 | Notez l’utilisation d’une horloge à cycle de 24 heures. | `, - * /` |
| Jour du mois | 1-31 | Il est impossible de spécifier une valeur numérique à la fois pour « Jour du mois » et « Jour de la semaine ». L’un de ces champs doit utiliser une `?` caractère générique. | `, - * / ? L C` |
| Mois | 1er-12 ou 1er janvier, février, mars, avril, mai, juin, juillet, août, septembre, septembre, octobre, novembre, décembre | Les valeurs sont sensibles à la casse. | `, - * /` |
| Jour de la semaine | Lun, Mar, Mer, Jeu, Ven, Sam, Dim | Les valeurs sont sensibles à la casse. Il est impossible de spécifier une valeur numérique à la fois pour « Jour du mois » et « Jour de la semaine ». L’un de ces champs doit utiliser une `?` caractère générique. | `, - * / ? L C #` |
| Année (facultatif) | Vide ou 1970-2099 |  | `, - * /` |


Ce tableau indique les caractères génériques qui sont autorisés dans la zone Règle et explique comment les utiliser :

| Caractère générique | Nom | Description |
|--- |--- |--- |
| `*` | Astérisque | Toutes les valeurs (par exemple, « toutes les minutes »). |
| `?` | Point d’interrogation | Aucune valeur spécifique (par exemple, n’importe quelle minute comprise dans l’heure spécifiée). |
| `,` | Virgule | Autres valeurs (par exemple, &quot;Lundi et mercredi&quot;). |
| `-` | Trait d’union | Plage de valeurs (par exemple, du lundi au vendredi). |
| `/` | Barre oblique | Incréments (par exemple, toutes les 15 minutes). |
| `L` | Lettre L majuscule | Dernier « jour du mois » ou « jour de la semaine » (disponible pour ces champs uniquement). Par exemple, pour le mois de janvier, la valeur L du champ « jour du mois » planifie la tâche pour le 31 janvier. Pour le champ « jour de la semaine », vous pouvez entrer ce caractère seul pour planifier la tâche le samedi. Vous pouvez l’utiliser avec un nombre (par exemple, `6L`) pour indiquer le dernier vendredi du mois. Ne spécifiez pas `L` avec la virgule ou les caractères génériques de trait d’union. |
| `#` | Carré | « N-ième » jour du mois (disponible pour le champ « jour de la semaine » uniquement). Par exemple : `6#3` dans le champ &quot;jour de la semaine&quot;, indiquez le troisième vendredi du mois. Le `6` indique &quot;vendredi&quot; (le sixième jour de la semaine) et la variable `3` indique la troisième occurrence du mois. |
| `C` | # lettre C majuscule | Premier « jour du mois » ou « jour de la semaine » du calendrier (disponible pour ces champs uniquement). Par exemple, la spécification d’une valeur de `1C` pour &quot;jour du mois&quot;, planifie le premier jour du calendrier qui survient le ou après le cinquième jour. Pour le champ &quot;jour de la semaine&quot;, la spécification `1C` planifie le premier jour du calendrier qui survient le dimanche ou après le dimanche |

Cette liste donne des exemples de définition d’intervalle dans la zone Règle :

* `0 0 12 * * ?` : Midi tous les jours
* `0 15 10 ? * *` : 10h15 tous les jours
* `0 0/5 14 * * ?`: Toutes les 5 minutes entre 14 h et 14 h 55 tous les jours
* `0 0/5 14,18 * * ?` : Toutes les 5 minutes entre 14h00 et 14h55 tous les jours et toutes les 5 minutes entre 18h00 et 18h55 tous les jours
* `0 10,44 14 ? 3` : Mer à 14h10 et 14h44 tous les mercredis de mars
* `0 15 10 ? *` : Lun-vendredi à 10h15 tous les jours de la semaine
* `0 15 10 20 * ?` : À 10h15 le 20e jour de chaque mois
* `0 15 10 L * ?` : À 10h15 le dernier jour de chaque mois
* `0 15 10 ? * 6L` : À 10h15 le dernier vendredi de chaque mois
* `0 15 10 * * 6#3` : À 10h15 le troisième vendredi de chaque mois

## Utilisation d’une tâche de téléchargement ou de publication comme déclencheur {#using-an-upload-or-publish-job-as-a-trigger}

Lorsque vous transférez des ressources par FTP ou exécutez une tâche de publication, vous pouvez planifier une tâche ultérieure qui commencera une fois le transfert terminé. (Si d’autres tâches doivent alors commencer, la tâche que vous programmez ici est mise en file d’attente derrière elles.) La nouvelle tâche envoie une notification à l’adresse que vous spécifiez afin que le code à cet emplacement puisse être déclenché. Le même nom que la tâche de téléchargement actuelle est attribué à la tâche de téléchargement à suivre, si ce n’est qu’il est accompagné du préfixe _Pub.

Pour qu’une tâche de téléchargement ou de publication déclenche une autre tâche, sélectionnez **[!UICONTROL Avancé]** sur la page Télécharger ou Publier . Entrez ensuite l’URL dans le champ Notification HTTP.
