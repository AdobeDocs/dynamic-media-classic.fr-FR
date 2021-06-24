---
title: Vérification de fichiers de tâche
description: Découvrez comment vérifier les fichiers de tâche.
uuid: 8241a894-3014-4a5c-96ef-71f3aaa3716a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: d53ae5dd-8daf-4d87-b9a6-3039bad30538
feature: Dynamic Media Classic,Gestion des ressources
role: Business Practitioner
exl-id: b6b11e1c-5eda-4bdb-8ffb-ecd3678f2352
source-git-commit: bd0659c015f259e25d6d07b620f5b1e948cabcbf
workflow-type: tm+mt
source-wordcount: '1583'
ht-degree: 61%

---

# Vérification de fichiers de tâche{#checking-job-files}

Pour surveiller les téléchargements de fichiers vers Dynamic Media Classic et les fichiers que vous publiez sur les serveurs Dynamic Media Classic, Dynamic Media Classic propose la page Tâches . Vous pouvez consulter des tâches de téléchargement et de publication sur la page Tâches, y vérifier l’état des tâches et annuler des publications. Vous pouvez également planifier des tâches de téléchargement et de publication.

Lorsque vous téléchargez des fichiers, une icône rotative apparaît en regard du menu Tâches, indiquant qu’une tâche est en cours, ainsi que le nombre de fichiers en cours. Vous pouvez cliquer sur cette icône pour consulter davantage d’informations sur la tâche active.

>[!NOTE]
>
>la liste des tâches récemment publiées est également disponible sur la page Activités récentes. Cliquez sur **[!UICONTROL Récent]** dans la barre de navigation globale pour ouvrir cette page.

## A propos de la page Tâches {#about-the-jobs-page}

Sélectionnez **[!UICONTROL Tâches]** dans la barre de navigation globale pour ouvrir la page Tâches. Par défaut, les tâches sont répertoriées de la plus récente à la moins récente.

Sur l’onglet Historique de la page Tâches, les tâches sont répertoriées selon les catégories suivantes :

**Type** de tâcheUne icône indique le type de tâche : Télécharger et publier sont les types de tâche les plus courants.

**Nom de la tâche** : nom de la tâche. Le nom inclut la partie du nom saisie par l’utilisateur et la date et l’heure.

**** DémarréLorsque la tâche a commencé.

**** TotalNombre de fichiers transférés.

**W (avertissements)** Nombre d’avertissements dans la tâche (le cas échéant). Les avertissements indiquent des problèmes associés à la tâche qui sont sans effet sur son exécution globale. Ces avertissements peuvent généralement être ignorés parce qu’ils sont signalés dans des fichiers masqués. Par exemple, les fichiers `.DS_store` (Macintosh) et Thumbs.db (Windows®) contiennent des informations sur l’affichage des fichiers image aux utilisateurs. Les entrées d’avertissement concernant ces fichiers peuvent toutefois être ignorées, car elles ne se rapportent pas à la manière dont ces fichiers sont utilisés dans Dynamic Media Classic. Vous pouvez cliquer deux fois sur un nom de tâche pour obtenir des informations détaillées sur les avertissements la concernant.

**E (Erreurs)** Répertorie le nombre d’erreurs dans la tâche (le cas échéant). Vous pouvez cliquer deux fois sur un nom de tâche pour obtenir des informations détaillées sur les erreurs la concernant.

**** Durée : temps nécessaire pour terminer la tâche.

**** StatusAffiche l’état de la tâche.

**** DestinationPour les tâches de transfert, le nom de l’entreprise et le dossier dans lequel les fichiers ont été chargés. Cette catégorie ne s’applique pas aux tâches publiées.

**Envoyé** par les listes qui ont chargé les ressources.

>[!NOTE]
>
>vous pouvez annuler des tâches de publication et de téléchargement en cours en cliquant sur le bouton Annuler en regard de la barre de progression.

## Modification des vues de la page Tâches {#changing-views-on-the-jobs-page}

Pour trier des tâches ou modifier votre affichage sur l’onglet Historique de la page Tâches, appliquez les techniques suivantes :

**** Tri : sélectionnez un nom de colonne pour trier la liste selon une colonne particulière. Vous pouvez sélectionner le bouton bascule près du nom de la colonne pour trier les entrées par ordre croissant ou décroissant.

**** Période : sélectionnez le menu Période et choisissez une option pour réduire la liste des tâches à la date actuelle, à la semaine précédente ou au mois précédent. Choisissez Période personnalisée, puis saisissez une période spécifique.

**Type de tâche** : sélectionnez le menu Type de tâche et choisissez Publier ou Télécharger pour restreindre la liste aux tâches de publication ou de téléchargement. Choisissez l’option Tout pour voir les deux types de tâche.

**** AfficherSélectionnez Afficher > Mes tâches ou Afficher > Toutes les tâches pour restreindre la liste aux tâches que vous avez commandées ou aux tâches commandées par des personnes de votre entreprise.

## Affichage, copie ou impression d’un rapport Détails de la tâche {#viewing-copying-or-printing-a-job-details-report}

Cliquez deux fois sur le nom d’un rapport sur la page Tâches pour ouvrir la page Détails sur la tâche. Cette page présente un récapitulatif sur les fichiers de la tâche. Cliquez sur Afficher les détails pour afficher l’identifiant Dynamic Media Classic d’une entrée, le chemin de destination et les informations d’état. Si vous avez téléchargé un fichier PDF ou PostScript qui nécessite des polices qui ne sont pas disponibles dans Dynamic Media Classic, le rapport répertorie les polices manquantes.

Vous pouvez copier ces informations dans le Presse-papiers.

1. Cliquez deux fois sur le nom d’un rapport sur la page Tâches pour ouvrir la page Détails sur la tâche. 
1. Cliquez sur Afficher les détails pour obtenir un rapport détaillé sur une entrée.
1. Cliquez sur Copier dans le Presse-papiers.

## Gestion de tâches de téléchargement et de publication périodiques {#handling-recurring-upload-and-publish-jobs}

Les tâches de téléchargement et de publication périodiques que vous créez dans les pages Télécharger et Publier sont répertoriées dans l’onglet Planifiée de la page Tâches. Vous pouvez éditer et supprimer des tâches périodiques dans l’onglet Planifiée.

Cliquez sur le bouton Tâches dans la barre de navigation globale et, sur la page Tâches qui apparaît, sélectionnez l’onglet Planifiée pour éditer et supprimer des tâches périodiques.

>[!NOTE]
>
>vous pouvez filtrer la liste des tâches dans l’onglet Planifiée avec les menus Type de tâche et Afficher. Choisissez un type de tâche pour restreindre la liste à des tâches de publication spécifiques. Choisissez une option Afficher pour afficher les tâches créées par vos soins ou par quelqu’un de l’entreprise.

### Edition, suppression, interruption et reprise de tâches {#editing-deleting-pausing-and-resuming-recurring-jobs}

Sélectionnez une tâche périodique sur la page Tâches, puis procédez comme suit pour l’éditer ou la supprimer :

**Modification d’une** tâche récurrente : sélectionnez le bouton Modifier et saisissez les informations de planification dans la boîte de dialogue Modifier la tâche planifiée . Si vous souhaitez planifier la tâche selon l’intervalle de votre choix, choisissez l’option Répéter > Personnalisé 

(voir [Création d’un intervalle de téléchargement ou de publication personnalisé](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval)).

**Suppression d’une** tâche récurrenteSélectionnez le bouton Supprimer .

**Suspension (et reprise) d’une** tâche récurrenteDans la colonne Principale, décochez une case pour suspendre une tâche. cochez une case pour reprendre une tâche en pause.

### Création d’un intervalle de téléchargement ou de publication personnalisé {#creating-a-custom-upload-or-publish-job-time-interval}

Pour créer un intervalle personnalisé pour une tâche de téléchargement (via FTP) ou de publication, choisissez l’option Répéter > Personnalisé sur la page Télécharger ou Publier. Puis, entrez des numéros et des caractères génériques dans la zone Règle pour définir l’intervalle de périodicité de la tâche en question.

La syntaxe de définition des intervalles personnalisés de périodicité de téléchargement ou de publication dans la zone Règle se présente comme suit :

`[seconds]` `[minutes]` `[hour of day]` `[day of month]` `[month]` `[day of week]`

Par exemple, `0 15 10 * * ?` programme une tâche à 10:15.00 tous les jours.

Les tableaux et la liste ci-après expliquent comment définir un intervalle dans la zone Règle.

Ce tableau indique les incréments temporels, leurs valeurs autorisées et les caractères génériques qu’ils prennent en charge :

| Incréments temporels | Valeurs autorisées | Commentaires | Caractères génériques pris en charge |
|--- |--- |--- |--- |
| Secondes | 0 à 59 |  | `, - * /` |
| Minutes | 0 à 59 |  | `, - * /` |
| Heures | 0 à 23 | Notez l’utilisation d’une horloge à cycle de 24 heures. | `, - * /` |
| Jour du mois | 1-31 | Il est impossible de spécifier une valeur numérique à la fois pour « Jour du mois » et « Jour de la semaine ». L’un de ces champs doit utiliser un caractère générique `?`. | `, - * / ? L C` |
| Mois | 1er-12 ou 1er janvier, février, mars, avril, mai, juin, juillet, août, septembre, septembre, octobre, novembre, décembre | Les valeurs sont sensibles à la casse. | `, - * /` |
| Jour de la semaine | Lun, Mar, Mer, Jeu, Ven, Sam, Dim | Les valeurs sont sensibles à la casse. Il est impossible de spécifier une valeur numérique à la fois pour « Jour du mois » et « Jour de la semaine ». L’un de ces champs doit utiliser un caractère générique `?`. | `, - * / ? L C #` |
| Année (facultatif) | Vide ou 1970-2099 |  | `, - * /` |


Ce tableau indique les caractères génériques qui sont autorisés dans la zone Règle et explique comment les utiliser :

| Caractère générique | Nom | Description |
|--- |--- |--- |
| `*` | Astérisque | Toutes les valeurs (par exemple, « toutes les minutes »). |
| `?` | Point d’interrogation | Aucune valeur spécifique (par exemple, n’importe quelle minute comprise dans l’heure spécifiée). |
| `,` | Virgule | Autres valeurs (par exemple, &quot;Lundi et mercredi&quot;). |
| `-` | Trait d’union | Plage de valeurs (par exemple, du lundi au vendredi). |
| `/` | Barre oblique | Incréments (par exemple, toutes les 15 minutes). |
| `L` | Lettre L majuscule | Dernier « jour du mois » ou « jour de la semaine » (disponible pour ces champs uniquement). Par exemple, pour le mois de janvier, la valeur L du champ « jour du mois » planifie la tâche pour le 31 janvier. Pour le champ « jour de la semaine », vous pouvez entrer ce caractère seul pour planifier la tâche le samedi. Vous pouvez l’utiliser avec un nombre (par exemple, `6L`) pour spécifier le dernier vendredi du mois. N’indiquez pas `L` avec la virgule ou le caractère générique (tiret). |
| `#` | Carré | « N-ième » jour du mois (disponible pour le champ « jour de la semaine » uniquement). Par exemple, `6#3` dans le champ &quot;jour de la semaine&quot; indique le troisième vendredi du mois. `6` indique &quot;vendredi&quot; (le sixième jour de la semaine) et `3` indique la troisième occurrence du mois. |
| `C` | # lettre C majuscule | Premier « jour du mois » ou « jour de la semaine » du calendrier (disponible pour ces champs uniquement). Par exemple, la spécification d’une valeur de `1C` pour &quot;jour du mois&quot; planifie le premier jour du calendrier qui survient le ou après le cinquième. Pour le champ &quot;jour de la semaine&quot;, la spécification de `1C` planifie le premier jour du calendrier qui survient le ou après le dimanche. |

Cette liste donne des exemples de définition d’intervalle dans la zone Règle :

* 0 0 12 * * ? : à midi tous les jours
* 0 15 10 ? * * : à 10h15 tous les jours
* 0 0/5 14 * * ? : toutes les 5 minutes entre 14h00 et 14h55 tous les jours
* 0 0/5 14,18 * * ? : toutes les 5 minutes entre 14h00 et 14h55 tous les jours et toutes les 5 minutes entre 18h00 et 18h55 tous les jours
* 0 10,44 14 ? 3 : le mercredi à 14h10 et à 14h44 tous les mercredis du mois de mars
* 0 15 10 ? *: Lun-vendredi à 10h15 tous les jours de la semaine
* 0 15 10 20 * ? : à 10h15 le 20e jour de chaque mois
* 0 15 10 L * ? : à 10h15 le dernier jour de chaque mois
* 0 15 10 ? * 6L : à 10h15 le dernier vendredi de chaque mois
* 0 15 10 * * 6#3 : à 10h15 le troisième vendredi de chaque mois

## Utilisation d’une tâche de téléchargement ou de publication comme déclencheur {#using-an-upload-or-publish-job-as-a-trigger}

Lorsque vous transférez des ressources par FTP ou exécutez une tâche de publication, vous pouvez planifier une tâche ultérieure qui commencera une fois le transfert terminé. (Si d’autres tâches doivent alors commencer, la tâche que vous programmez ici est mise en file d’attente derrière elles.) La nouvelle tâche envoie une notification à l’adresse spécifiée par vos soins de manière à déclencher ce code à cet emplacement. Le même nom que la tâche de téléchargement actuelle est attribué à la tâche de téléchargement à suivre, si ce n’est qu’il est accompagné du préfixe _Pub.

Pour faire en sorte qu’une tâche de téléchargement ou de publication serve de déclencheur à une autre tâche, sélectionnez l’option Avancé sur la page Télécharger ou Publier. Entrez ensuite l’URL dans le champ Notification HTTP.
