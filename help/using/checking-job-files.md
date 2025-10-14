---
title: Vérifier les fichiers de traitement
description: Découvrez comment vérifier les fichiers de traitement dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: b6b11e1c-5eda-4bdb-8ffb-ecd3678f2352
topic: Administration, Content Management
level: Intermediate
source-git-commit: bb229047c0c9b3855453ea15dcd1f9754bc65cef
workflow-type: tm+mt
source-wordcount: '1633'
ht-degree: 23%

---

# Vérifier les fichiers de traitement{#checking-job-files}

Pour surveiller les chargements de fichiers vers Adobe Dynamic Media Classic et les fichiers que vous publiez sur les serveurs Adobe Dynamic Media Classic, Adobe Dynamic Media Classic propose la page Tâches . Vous pouvez vérifier, charger et publier des tâches sur la page Tâches, vérifier le statut des tâches et annuler les tâches de publication à partir de cette page. Vous pouvez également planifier des tâches de téléchargement et de publication.

Lorsque vous téléchargez des fichiers, une icône rotative apparaît en regard du menu Tâches, indiquant qu’une tâche est en cours, ainsi que le nombre de fichiers en cours. Vous pouvez sélectionner l’icône pour afficher plus d’informations sur la tâche active.

>[!NOTE]
>
>la liste des tâches récemment publiées est également disponible sur la page Activités récentes. Sélectionnez **[!UICONTROL Récent]** dans la barre de navigation générale.

## A propos de la page Tâches {#about-the-jobs-page}

Sélectionnez **[!UICONTROL Tâches]** dans la barre de navigation générale pour ouvrir la page Tâches . Par défaut, les tâches sont répertoriées de la plus récente à la moins récente.

Sur l’onglet Historique de la page Tâches, les tâches sont répertoriées selon les catégories suivantes :

* **[!UICONTROL Type de tâche]** : une icône indique le type de tâche : Charger et Publier sont les types de tâche les plus courants.

* **[!UICONTROL Nom de la tâche]** : nom de la tâche. Le nom comprend la partie du nom saisie par l’utilisateur, ainsi que la date et l’heure.

* **[!UICONTROL Démarré]** : date à laquelle le traitement a démarré.

* **[!UICONTROL Total]** : nombre de fichiers transférés.

* **[!UICONTROL W (avertissements)]** : nombre d’avertissements dans la tâche (le cas échéant). Les avertissements indiquent des problèmes associés à la tâche qui sont sans effet sur son exécution globale. Ces avertissements peuvent généralement être ignorés parce qu’ils sont signalés dans des fichiers masqués. Par exemple, les fichiers `.DS_store` (Mac) et les fichiers Thumbs.db (Windows®) contiennent des informations sur l’affichage des fichiers image aux utilisateurs. Les entrées d’avertissement concernant ces fichiers peuvent toutefois être ignorées, car elles ne se rapportent pas à la manière dont ces fichiers sont utilisés dans Adobe Dynamic Media Classic. Vous pouvez cliquer deux fois sur un nom de tâche pour obtenir des informations détaillées sur les avertissements la concernant.

* **[!UICONTROL E (erreurs)]** : répertorie le nombre d’erreurs dans la tâche (le cas échéant). Vous pouvez cliquer deux fois sur un nom de tâche pour obtenir des informations détaillées sur les erreurs la concernant.

* **[!UICONTROL Durée]** : temps nécessaire pour terminer le traitement.

* **[!UICONTROL Statut]** : affiche le statut du traitement.

* **[!UICONTROL Destination]** : pour les tâches de chargement, la destination est le nom de la société et le dossier dans lesquels les fichiers ont été chargés. Cette catégorie ne s’applique pas aux tâches de publication.

* **[!UICONTROL Envoyé par]** : répertorie les personnes qui ont chargé les ressources.

>[!NOTE]
>
>Vous pouvez annuler les tâches de publication et de chargement en cours en sélectionnant le bouton **[!UICONTROL Annuler]** en regard de la barre de progression.

## Modifier les vues dans la page Tâches {#changing-views-on-the-jobs-page}

Pour trier des tâches ou modifier votre affichage sur l’onglet Historique de la page Tâches, appliquez les techniques suivantes :

* **[!UICONTROL Tri]** : sélectionnez le nom d’une colonne pour trier la liste en fonction d’une colonne particulière. Vous pouvez sélectionner le bouton bascule près du nom de la colonne pour trier les entrées par ordre croissant ou décroissant.

* **[!UICONTROL Période]** : sélectionnez le menu **[!UICONTROL Période]** et choisissez une option pour limiter la liste des tâches à la date du jour, à la semaine précédente ou au mois précédent. Sélectionnez **[!UICONTROL Période personnalisée]** puis saisissez une période spécifique.

* **[!UICONTROL Type de tâche]** : sélectionnez le menu **[!UICONTROL Type de tâche]** et choisissez **[!UICONTROL Publier]** ou **[!UICONTROL Télécharger]** pour limiter la liste aux tâches de publication ou de chargement. Sélectionnez **[!UICONTROL Tous]** pour afficher les deux types de tâches.

* **[!UICONTROL Afficher]** : accédez à **[!UICONTROL Afficher]** > **[!UICONTROL Mes tâches]** ou **[!UICONTROL Afficher]** > **[!UICONTROL Toutes les tâches]** pour limiter la liste aux tâches que vous avez commandées ou aux tâches que des personnes de votre entreprise ont commandées.

## Afficher, copier ou imprimer un rapport Détails de la tâche {#viewing-copying-or-printing-a-job-details-report}

Double-cliquez sur le nom d’un rapport sur la page Tâches pour ouvrir la page Détails de la tâche. Cette page présente un récapitulatif sur les fichiers de la tâche. Sélectionnez **[!UICONTROL Afficher les détails]** afin de voir l’identifiant Adobe Dynamic Media Classic d’une entrée, le chemin de destination et les informations sur le statut. Si vous avez chargé un fichier PDF ou PostScript qui nécessite des polices qui ne sont pas disponibles dans Adobe Dynamic Media Classic, le rapport répertorie les polices manquantes.

Vous pouvez copier ces informations dans le Presse-papiers.

1. Double-cliquez sur le nom d’un rapport sur la page Tâches .
1. Sur la page Détails de la tâche, sélectionnez **[!UICONTROL Afficher les détails]** pour obtenir un rapport détaillé sur une entrée.
1. Sélectionnez **[!UICONTROL Copier dans le presse-papiers]**.

## Gestion des tâches récurrentes de chargement et de publication {#handling-recurring-upload-and-publish-jobs}

Les tâches de chargement et de publication récurrentes que vous créez sur les pages Charger et Publier sont répertoriées dans l’onglet Planifié de la page Tâches. Vous pouvez éditer et supprimer des tâches périodiques dans l’onglet Planifiée.

Sélectionnez le bouton Tâches dans la barre de navigation générale, puis, sur la page Tâches, sélectionnez l’onglet **[!UICONTROL Planifié]** afin de pouvoir modifier et supprimer des tâches récurrentes.

>[!NOTE]
>
>Vous pouvez filtrer la liste des tâches dans l’onglet **[!UICONTROL Planifié]** avec les menus **[!UICONTROL Type de tâche]** et **[!UICONTROL Afficher]**. Sélectionnez un type de tâche afin de pouvoir affiner la liste pour publier des tâches d’un type spécifique. Sélectionnez une option **[!UICONTROL Afficher]** pour afficher les tâches que vous avez créées ou celles créées par tous les membres de votre entreprise.

### Modifier, supprimer, mettre en pause et reprendre les tâches récurrentes {#editing-deleting-pausing-and-resuming-recurring-jobs}

Sélectionnez une tâche récurrente sur la page Tâches et suivez ces instructions si vous souhaitez la modifier ou la supprimer :

* **Modifier une tâche récurrente** : sélectionnez le bouton **[!UICONTROL Modifier]** et saisissez les informations de planification dans la boîte de dialogue Modifier la tâche planifiée. Si vous souhaitez que la tâche se répète à un intervalle de votre choix, sélectionnez **[!UICONTROL Répéter]** > **[!UICONTROL Personnalisé]**.

Voir [&#x200B; Création d’un intervalle personnalisé de chargement ou de publication](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

* **Suppression d’une tâche récurrente** : sélectionnez le bouton **[!UICONTROL Supprimer]**.

* **Suspension (et reprise) d’un traitement récurrent** : dans la colonne Actif, désélectionnez une case pour suspendre un traitement ; cochez une case pour reprendre un traitement qui était en pause.

### Création d’un intervalle personnalisé entre les tâches de chargement ou de publication {#creating-a-custom-upload-or-publish-job-time-interval}

Pour créer un intervalle personnalisé pour un chargement (par FTP) ou une tâche de publication, sur la page Charger ou Publier , accédez à **[!UICONTROL Répéter]** > **[!UICONTROL Personnalisé]**. Saisissez ensuite des chiffres et des caractères génériques dans la zone Règle décrivant un intervalle de temps pour la périodicité des tâches de chargement ou de publication.

La syntaxe de définition des intervalles personnalisés de périodicité de téléchargement ou de publication dans la zone Règle se présente comme suit :

`[seconds]` `[minutes]` `[hour of day]` `[day of month]` `[month]` `[day of week]`

Par exemple, `0 15 10 * * ?` planifie un traitement à 10 :15 tous les jours.

Les tableaux et la liste ci-après expliquent comment définir un intervalle dans la zone Règle.

Ce tableau indique les incréments temporels, leurs valeurs autorisées et les caractères génériques qu’ils prennent en charge :

| Incréments temporels | Valeurs autorisées | Commentaires | Caractères génériques pris en charge |
|--- |--- |--- |--- |
| Secondes | 0-59 |  | `,: * /` |
| Minutes | 0-59 |  | `,: * /` |
| Heures | 0-23 | Notez l’utilisation d’une horloge à cycle de 24 heures. | `,: * /` |
| Jour du mois | 1-31 | Vous ne pouvez pas spécifier de valeur numérique pour « jour du mois » et « jour de la semaine ». L’un de ces champs doit utiliser un caractère générique `?`. | `,: * / ? L C` |
| Mois | 1-12 ou jan, fév, mar, avr, mai, jun, jul, aoû, sep, oct, nov, déc | Les valeurs respectent la casse. | `,: * /` |
| Jour de la semaine | Lun, Mar, Mer, Jeu, Ven, Sam, Dim | Les valeurs respectent la casse. Vous ne pouvez pas spécifier de valeur numérique pour « jour du mois » et « jour de la semaine ». L’un de ces champs doit utiliser un caractère générique `?`. | `,: * / ? L C #` |
| Année (facultatif) | Vide ou 1970-2099 |  | `,: * /` |


Ce tableau indique les caractères génériques qui sont autorisés dans la zone Règle et explique comment les utiliser :

| Caractère générique | Nom | Description |
| --- | --- | --- |
| `*` | Astérisque | Toutes les valeurs (par exemple, « toutes les minutes »). |
| `?` | Point d’interrogation | Aucune valeur spécifique (par exemple, « toute minute dans l’heure spécifiée »). |
| `,` | Virgule | Autres valeurs (par exemple, « Lundi et mercredi »). |
| `-` | Trait d’union | Plage de valeurs (par exemple, « Du lundi au vendredi »). |
| `/` | Barre oblique | Incréments (par exemple, « toutes les 15 minutes »). |
| `L` | Lettre L majuscule | Dernier « jour du mois » ou « jour de la semaine » (disponible uniquement pour ces champs). Par exemple, si le mois de janvier est défini, une valeur L pour le champ « jour du mois » planifie le traitement pour le 31 janvier. Pour le champ « Jour de la semaine », vous pouvez saisir ce caractère seul pour programmer le travail le samedi. Vous pouvez l’utiliser avec un nombre (par exemple, `6L`) pour spécifier le dernier vendredi du mois. Ne spécifiez pas de `L` à l’aide de la virgule ou du trait d’union. |
| `#` | Carré | « Nème » jour de la semaine du mois (disponible pour le champ « jour de la semaine » uniquement). Par exemple, la mention `6#3` dans le champ « jour de la semaine » indique le troisième vendredi du mois. Le `6` indique « vendredi » (le sixième jour de la semaine) et le `3` indique la troisième occurrence du mois. |
| `C` | # lettre C majuscule | Premier calendrier : « jour du mois » ou « jour de la semaine » (disponible uniquement pour ces champs). Par exemple, la spécification d’une valeur `1C` pour « Jour du mois » planifie le premier jour du calendrier qui se produit le cinquième ou après le cinquième. Pour le champ « Jour de la semaine », la spécification de `1C` planifie le premier jour du calendrier qui se produit le dimanche ou après le dimanche. |

Cette liste donne des exemples de définition d’intervalle dans la zone Règle :

* `0 0 12 * * ?` : midi tous les jours
* `0 15 10 ? * *` : 10 :15 tous les jours
* `0 0/5 14 * * ?` : Toutes les 5 minutes entre 14:00 et 14:55 tous les jours
* `0 0/5 14,18 * * ?` : toutes les 5 minutes entre 14:00 et 14:55 tous les jours et toutes les 5 minutes entre 18:00 et 18:55 tous les jours
* `0 10,44 14 ? 3` : Mercredi à 14:10h et 14:44h tous les mercredis de mars
* `0 15 10 ? *` : lundi-vendredi à 10:15 tous les jours de la semaine
* `0 15 10 20 * ?` : à 10 :15 le 20 de chaque mois
* `0 15 10 L * ?` : à 10 :15 le dernier jour de chaque mois
* `0 15 10 ? * 6L` : à 10 :15 le dernier vendredi de chaque mois
* `0 15 10 * * 6#3` : à 10 :15 le troisième vendredi de chaque mois

## Utiliser une tâche de chargement ou de publication comme déclencheur {#using-an-upload-or-publish-job-as-a-trigger}

Lorsque vous chargez des ressources par FTP ou que vous exécutez une tâche de publication, vous pouvez planifier une tâche ultérieure pour qu’elle commence une fois le chargement terminé. (Si d’autres tâches sont planifiées pour commencer alors, la tâche que vous planifiez ici est mise en file d’attente derrière elles.) Le nouveau traitement envoie une notification à l’adresse que vous spécifiez afin que le code de cet emplacement puisse être déclenché. Le même nom que la tâche de téléchargement actuelle est attribué à la tâche de téléchargement à suivre, si ce n’est qu’il est accompagné du préfixe _Pub.

Pour qu’une tâche de chargement ou de publication déclenche une autre tâche, sélectionnez **[!UICONTROL Avancé]** sur la page Charger ou Publier. Entrez ensuite l’URL dans le champ Notification HTTP.
