---
title: Vérification des fichiers de tâche
description: Découvrez comment vérifier les fichiers de tâche dans Adobe Dynamic Media Classic.
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
source-wordcount: '1622'
ht-degree: 23%

---

# Vérification des fichiers de tâche{#checking-job-files}

Pour surveiller les chargements de fichiers vers Adobe Dynamic Media Classic et les fichiers que vous publiez sur les serveurs Adobe Dynamic Media Classic, Adobe Dynamic Media Classic propose la page Tâches. Vous pouvez consulter, charger et publier des tâches sur la page Tâches, vérifier l’état des tâches et annuler des tâches de publication à partir de cette page. Vous pouvez également planifier des tâches de téléchargement et de publication.

Lorsque vous téléchargez des fichiers, une icône rotative apparaît en regard du menu Tâches, indiquant qu’une tâche est en cours, ainsi que le nombre de fichiers en cours. Vous pouvez sélectionner l’icône pour afficher plus d’informations sur la tâche active.

>[!NOTE]
>
>la liste des tâches récemment publiées est également disponible sur la page Activités récentes. Sélectionnez **[!UICONTROL Récent]** dans la barre de navigation globale.

## A propos de la page Tâches {#about-the-jobs-page}

Sélectionnez **[!UICONTROL Tâches]** dans la barre de navigation globale afin que la page Tâches s’ouvre. Par défaut, les tâches sont répertoriées de la plus récente à la moins récente.

Sur l’onglet Historique de la page Tâches, les tâches sont répertoriées selon les catégories suivantes :

* **[!UICONTROL Type de tâche]** : une icône indique le type de tâche : Télécharger et Publish sont les types de tâche les plus courants.

* **[!UICONTROL Nom de la tâche]** : nom de la tâche. Le nom comprend la partie du nom saisie par l’utilisateur, ainsi que la date et l’heure.

* **[!UICONTROL Démarré]** : date de démarrage de la tâche.

* **[!UICONTROL Total]** : nombre de fichiers transférés.

* **[!UICONTROL W (warnings)]** : nombre d’avertissements dans la tâche (le cas échéant). Les avertissements indiquent des problèmes associés à la tâche qui sont sans effet sur son exécution globale. Ces avertissements peuvent généralement être ignorés parce qu’ils sont signalés dans des fichiers masqués. Par exemple, les fichiers `.DS_store` (Mac) et les fichiers Thumbs.db (Windows®) contiennent des informations sur l’affichage des fichiers image aux utilisateurs. Les entrées d’avertissement concernant ces fichiers peuvent toutefois être ignorées, car elles ne concernent pas la manière dont ces fichiers sont utilisés dans Adobe Dynamic Media Classic. Vous pouvez cliquer deux fois sur un nom de tâche pour obtenir des informations détaillées sur les avertissements la concernant.

* **[!UICONTROL E (errors)]** : répertorie le nombre d’erreurs dans la tâche (le cas échéant). Vous pouvez cliquer deux fois sur un nom de tâche pour obtenir des informations détaillées sur les erreurs la concernant.

* **[!UICONTROL Durée]** : temps nécessaire pour terminer la tâche.

* **[!UICONTROL Status]** : affiche l’état de la tâche.

* **[!UICONTROL Destination]** : pour les tâches de chargement, la destination est le nom de l’entreprise et le dossier vers lequel les fichiers ont été chargés. Cette catégorie ne s’applique pas aux traitements de publication.

* **[!UICONTROL Envoyé par]** : Répertorie les personnes qui ont chargé les ressources.

>[!NOTE]
>
>Vous pouvez annuler les tâches de publication et de chargement en cours en sélectionnant le bouton **[!UICONTROL Annuler]** en regard de la barre de progression.

## Modification des vues sur la page Tâches {#changing-views-on-the-jobs-page}

Pour trier des tâches ou modifier votre affichage sur l’onglet Historique de la page Tâches, appliquez les techniques suivantes :

* **[!UICONTROL Tri]** : sélectionnez un nom de colonne pour trier la liste selon une colonne particulière. Vous pouvez sélectionner le bouton bascule près du nom de la colonne pour trier les entrées par ordre croissant ou décroissant.

* **[!UICONTROL Plage de dates]** : sélectionnez le menu **[!UICONTROL Plage de dates]** et choisissez une option pour restreindre la liste des tâches à la date actuelle, à la semaine précédente ou au mois précédent. Sélectionnez **[!UICONTROL Plage de dates personnalisée]**, puis saisissez une plage de dates spécifique.

* **[!UICONTROL Type de tâche]** : sélectionnez le menu **[!UICONTROL Type de tâche]** et choisissez **[!UICONTROL Publish]** ou **[!UICONTROL Télécharger]** pour limiter la liste aux tâches de publication ou de téléchargement. Sélectionnez **[!UICONTROL Tous]** pour afficher les deux types de tâches.

* **[!UICONTROL Afficher]** : accédez à **[!UICONTROL Afficher]** > **[!UICONTROL Mes tâches]** ou **[!UICONTROL Afficher]** > **[!UICONTROL Toutes les tâches]** pour restreindre la liste aux tâches que vous avez commandées ou aux tâches commandées par des personnes de votre entreprise.

## Afficher, copier ou imprimer un rapport Détails de la tâche {#viewing-copying-or-printing-a-job-details-report}

Double-cliquez sur le nom d’un rapport sur la page Tâches pour ouvrir la page Détails de la tâche. Cette page présente un récapitulatif sur les fichiers de la tâche. Sélectionnez **[!UICONTROL Afficher les détails]** afin de pouvoir afficher l’Adobe Dynamic Media Classic ID, le chemin de destination et les informations d’état d’une entrée. Si vous avez téléchargé un fichier PDF ou PostScript qui nécessite des polices qui ne sont pas disponibles dans Adobe Dynamic Media Classic, le rapport répertorie les polices manquantes.

Vous pouvez copier ces informations dans le Presse-papiers.

1. Double-cliquez sur le nom d’un rapport sur la page Tâches.
1. Sur la page Détails de la tâche, sélectionnez **[!UICONTROL Afficher les détails]** pour obtenir un rapport détaillé sur une entrée.
1. Sélectionnez **[!UICONTROL Copier dans le Presse-papiers]**.

## Gestion des tâches de chargement et de publication récurrentes {#handling-recurring-upload-and-publish-jobs}

Les tâches de chargement et de publication récurrentes, que vous créez sur les pages Télécharger et Publish, sont répertoriées dans l’onglet Planifié de la page Tâches. Vous pouvez éditer et supprimer des tâches périodiques dans l’onglet Planifiée.

Sélectionnez le bouton Tâches dans la barre de navigation globale, puis, sur la page Tâches, sélectionnez l’onglet **[!UICONTROL Planifié]** afin de pouvoir modifier et supprimer les tâches récurrentes.

>[!NOTE]
>
>Vous pouvez filtrer la liste des tâches sur l’onglet **[!UICONTROL Planifié]** avec les menus **[!UICONTROL Type de tâche]** et **[!UICONTROL Afficher]** . Sélectionnez un type de tâche afin de limiter la liste aux tâches d’un type spécifique. Sélectionnez une option **[!UICONTROL Afficher]** afin d’afficher les tâches que vous avez créées ou créées par toutes les personnes de votre entreprise.

### Modification, suppression, mise en pause et reprise de tâches récurrentes {#editing-deleting-pausing-and-resuming-recurring-jobs}

Sélectionnez une tâche récurrente sur la page Tâches et suivez ces instructions si vous souhaitez la modifier ou la supprimer :

* **Modifier une tâche récurrente** : sélectionnez le bouton **[!UICONTROL Modifier]** et saisissez des informations de planification dans la boîte de dialogue Modifier la tâche planifiée. Si vous souhaitez que la tâche se répète à l’intervalle de votre choix, accédez à **[!UICONTROL Répéter]** > **[!UICONTROL Personnalisé]**.

Voir [Création d’un intervalle de temps de tâche de téléchargement ou de publication personnalisé](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

* **Suppression d&#39;une tâche récurrente** : sélectionnez le bouton **[!UICONTROL Supprimer]** .

* **Suspension (et reprise) d’une tâche récurrente** : dans la colonne Actif, décochez une case pour suspendre une tâche ; cochez une case pour reprendre une tâche en pause.

### Création d’un intervalle de temps de tâche de téléchargement ou de publication personnalisé {#creating-a-custom-upload-or-publish-job-time-interval}

Pour créer un intervalle de temps personnalisé pour une tâche de téléchargement (par FTP) ou de publication, sur la page Télécharger ou Publish, accédez à **[!UICONTROL Répéter]** > **[!UICONTROL Personnalisé]**. Saisissez ensuite des nombres et des caractères génériques dans la zone Règle pour décrire un intervalle de temps entre les tâches de téléchargement ou de publication à répéter.

La syntaxe de définition des intervalles personnalisés de périodicité de téléchargement ou de publication dans la zone Règle se présente comme suit :

`[seconds]` `[minutes]` `[hour of day]` `[day of month]` `[month]` `[day of week]`

Par exemple, `0 15 10 * * ?` planifie une tâche à 10:15.00 tous les jours.

Les tableaux et la liste ci-après expliquent comment définir un intervalle dans la zone Règle.

Ce tableau indique les incréments temporels, leurs valeurs autorisées et les caractères génériques qu’ils prennent en charge :

| Incréments temporels | Valeurs autorisées | Commentaires | Caractères génériques pris en charge |
|--- |--- |--- |--- |
| Secondes | 0-59 |  | `,: * /` |
| Minutes | 0-59 |  | `,: * /` |
| Heures | 0-23 | Notez l’utilisation d’une horloge à cycle de 24 heures. | `,: * /` |
| Jour du mois | 1-31 | Vous ne pouvez pas spécifier de valeur numérique pour &quot;jour du mois&quot; et &quot;jour de la semaine&quot;. L’un de ces champs doit utiliser un caractère générique `?`. | `,: * / ? L C` |
| Mois | 1-12 ou jan, fév, mar, avr, mai, jun, jul, aoû, sep, oct, nov, déc | Les valeurs sont sensibles à la casse. | `,: * /` |
| Jour de la semaine | Lun, Mar, Mer, Jeu, Ven, Sam, Dim | Les valeurs sont sensibles à la casse. Vous ne pouvez pas spécifier de valeur numérique pour &quot;jour du mois&quot; et &quot;jour de la semaine&quot;. L’un de ces champs doit utiliser un caractère générique `?`. | `,: * / ? L C #` |
| Année (facultatif) | Vide ou 1970-2099 |  | `,: * /` |


Ce tableau indique les caractères génériques qui sont autorisés dans la zone Règle et explique comment les utiliser :

| Caractère générique | Nom | Description |
| --- | --- | --- |
| `*` | Astérisque | Toutes les valeurs (par exemple, &quot;toutes les minutes&quot;). |
| `?` | Point d’interrogation | Aucune valeur spécifique (par exemple, &quot;toute minute au cours de l’heure spécifiée&quot;). |
| `,` | Virgule | Autres valeurs (par exemple, &quot;Lundi et mercredi&quot;). |
| `-` | Trait d’union | Plage de valeurs (par exemple, &quot;du lundi au vendredi&quot;). |
| `/` | Barre oblique | Incréments (par exemple, toutes les 15 minutes). |
| `L` | Lettre L majuscule | Dernier &quot;jour du mois&quot; ou &quot;jour de la semaine&quot; (disponible uniquement pour ces champs). Par exemple, si le mois est janvier, une valeur L pour le champ &quot;jour du mois&quot; programme la tâche pour le 31 janvier. Pour le champ &quot;jour de la semaine&quot;, vous pouvez saisir ce caractère seul pour planifier la tâche le samedi. Vous pouvez l’utiliser avec un nombre (par exemple, `6L`) pour spécifier le dernier vendredi du mois. Ne spécifiez pas `L` avec la virgule ou les caractères génériques de trait d’union. |
| `#` | Carré | &quot;Nième&quot; jour du mois en semaine (disponible uniquement pour le champ &quot;jour de la semaine&quot;). Par exemple, `6#3` dans le champ &quot;jour de la semaine&quot; indique le troisième vendredi du mois. Le `6` indique &quot;vendredi&quot; (le sixième jour de la semaine) et le `3` indique la troisième occurrence du mois. |
| `C` | # lettre C majuscule | Premier calendrier &quot;jour du mois&quot; ou &quot;jour de la semaine&quot; (disponible uniquement pour ces champs). Par exemple, la spécification d’une valeur de `1C` pour &quot;jour du mois&quot; planifie le premier jour du calendrier qui survient le ou après le cinquième. Pour le champ &quot;jour de la semaine&quot;, la spécification de `1C` planifie le premier jour du calendrier qui survient le ou après le dimanche. |

Cette liste donne des exemples de définition d’intervalle dans la zone Règle :

* `0 0 12 * * ?` : midi tous les jours
* `0 15 10 ? * *` : 10:15 tous les jours
* `0 0/5 14 * * ?` : Toutes les 5 minutes entre 14 h 00 et 14 h 55 tous les jours
* `0 0/5 14,18 * * ?` : toutes les 5 minutes entre 14 h 00 et 14 h 55 tous les jours et toutes les 5 minutes entre 18 h 00 et 18 h 55 tous les jours
* `0 10,44 14 ? 3` : Mer à 14h10 et 14h44 tous les mercredis de mars
* `0 15 10 ? *` : du lundi au vendredi à 10h15 tous les jours de la semaine
* `0 15 10 20 * ?` : à 10h15 le 20e jour de chaque mois
* `0 15 10 L * ?` : à 10h15 le dernier jour de chaque mois
* `0 15 10 ? * 6L` : à 10h15 le dernier vendredi de chaque mois
* `0 15 10 * * 6#3` : à 10h15 le troisième vendredi de chaque mois

## Utilisation d’une tâche de téléchargement ou de publication comme déclencheur {#using-an-upload-or-publish-job-as-a-trigger}

Lorsque vous transférez des ressources par FTP ou exécutez une tâche de publication, vous pouvez planifier une tâche ultérieure qui commencera une fois le transfert terminé. (Si d’autres tâches doivent alors commencer, la tâche que vous programmez ici est mise en file d’attente derrière elles.) La nouvelle tâche envoie une notification à l’adresse que vous spécifiez afin que le code à cet emplacement puisse être déclenché. Le même nom que la tâche de téléchargement actuelle est attribué à la tâche de téléchargement à suivre, si ce n’est qu’il est accompagné du préfixe _Pub.

Pour qu’une tâche de téléchargement ou de publication déclenche une autre tâche, sélectionnez **[!UICONTROL Avancé]** sur la page Télécharger ou Publish. Entrez ensuite l’URL dans le champ Notification HTTP.
