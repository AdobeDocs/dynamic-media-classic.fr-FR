---
title: Fichiers Publish
description: Découvrez comment publier vos ressources sur les serveurs d’images Dynamic Media.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 91b73a09-c5b5-4001-b36f-6bebe65717ff
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '1674'
ht-degree: 21%

---

# Fichiers Publish{#publishing-files}

Vous publiez vos ressources sur les serveurs d’images Dynamic Media. Vous pouvez publier des ressources ponctuellement ou organiser Adobe Dynamic Media Classic pour les publier selon une planification récurrente. Une fois vos fichiers publiés, vous en disposez pour les diffuser. Vous pouvez copier les appels d’URL d’Adobe Dynamic Media Classic et les ajouter à votre site web ou à votre application.

Adobe Dynamic Media Classic prend désormais en charge la diffusion de toutes les images et vidéos sur HTTP/2. En d’autres termes, une URL publiée ou un code intégré pour l’image ou la vidéo peut être intégré à toute application qui accepte une ressource hébergée. Cette ressource publiée utilise le protocole HTTP/2 pour la diffuser. Cette méthode de remise améliore la communication entre les navigateurs et les serveurs, ce qui permet de bénéficier de meilleurs temps de réponse et de chargement de toutes vos ressources Adobe Dynamic Media Classic. Voir [FAQ sur la diffusion de contenu HTTP2](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/dynamic/http2).

## Publication après le téléchargement {#publish-after-uploading}

Fichiers dans un état publié ou non publié. Par défaut, toutes les ressources que vous chargez dans Adobe Dynamic Media Classic sont automatiquement marquées pour publication.

Pour plus d’informations, voir le [PDF Instant Publish Notice](/help/using/assets/rendering-instant-publish-notification.pdf).

Utilisez ces techniques pour marquer les ressources à des fins de publication :

* **[!UICONTROL Publish After Uploading]** : sur la page Upload, près du bas, sélectionnez **[!UICONTROL Publish After Uploading]**. La valeur par défaut est un état sélectionné.

* **[!UICONTROL Publish After Uploading]** : dans la boîte de dialogue Job Options, sélectionnez **[!UICONTROL Publish After Uploading]**. La valeur par défaut est un état sélectionné.

Certains fichiers « enfants » sont systématiquement marqués pour publication lorsque leurs parents le sont. Ce tableau répertorie les ressources enfants qui sont automatiquement marquées pour publication.

| Elément (groupe) parent | Eléments (membre) enfants |
| --- | --- |
| Visionneuses d’images | Images dans la visionneuse. |
| Série d’échantillons | Echantillons dans la visionneuse. |
| Visionneuses à 360° | Images dans la visionneuse. |
| Modèles | Fichiers de modèle, pages et images. |

Les images dérivées sont également automatiquement marquées pour publication lorsque leurs images parentes sont en cours de publication. Les images dérivées incluent les images que vous avez modifiées avec des options d’édition d’image. Vous pouvez voir ces images dérivées dans la vue Détails sous Créé et dérivés.

## Création d’une tâche de publication {#creating-a-publish-job}

Créez une tâche de publication pour publier les ressources que vous avez chargées sur les serveurs Adobe Dynamic Media Classic, mais que vous ne souhaitez pas qu’elles soient publiées automatiquement pour l’instant. Vous pouvez effectuer une tâche de publication ponctuelle ou planifier la récurrence régulière des tâches. Adobe Dynamic Media Classic propose des options de publication avancées pour la publication sur des serveurs spécifiques et des options pour la republication de ressources qui ont déjà été publiées.

**Pour créer une tâche de publication :**

1. Dans la barre de navigation globale, sélectionnez **[!UICONTROL Publish]**.
1. Dans la boîte de dialogue Publication, choisissez si vous souhaitez une tâche de publication ponctuelle ou récurrente.

   Voir [Création d’une tâche de publication unique](publishing-files.md#creating_a_one_time_publish_job) et [Création d’une tâche de publication récurrente](publishing-files.md#creating_a_recurring_publish_job).

1. Entrez un nom de tâche.
1. (Facultatif) Affichez les options avancées, puis choisissez parmi elles 

   (voir [Options de publication avancées](publishing-files.md#advanced_publish_options)).

1. Sélectionnez **[!UICONTROL Submit Publish]**.

Adobe Dynamic Media Classic effectue le suivi des tâches de publication sur la page Tâches. Vous pouvez consulter les tâches de publication sur cette page.

>[!NOTE]
>
>Assets que vous avez republié (vous les avez déjà publiés) n’apparaît pas immédiatement sur votre site web en raison du mécanisme de mise en cache web sur le réseau de diffusion de contenu (CDN). (voir [Fichiers republiés et délais CDN](publishing-files.md#republished_assets_and_cdn_delays)).

### Création d’une tâche de publication unique {#creating-a-one-time-publish-job}

Créez une tâche de publication unique en sélectionnant l’option **[!UICONTROL Unique]** sur la page Publication.

Si vous souhaitez que la tâche de publication se produise ultérieurement, dans la page Publication, sélectionnez **[!UICONTROL Unique]**. Dans la liste déroulante, sélectionnez **[!UICONTROL Planifier pour plus tard]**. Utilisez le calendrier et le curseur de l’heure pour sélectionner un jour et une heure pour exécuter la tâche de publication.

### Créer une tâche de publication récurrente {#creating-a-recurring-publish-job}

Créez une tâche de publication récurrente en sélectionnant **[!UICONTROL Récurrente]** sur la page Publication.

Choisissez ensuite une option Répéter : **[!UICONTROL Quotidien]**, **[!UICONTROL Hebdomadaire]**, **[!UICONTROL Mensuel]** ou **[!UICONTROL Personnalisé]**, puis indiquez à quel moment la tâche de publication doit se répéter. Adobe Dynamic Media Classic présente des outils de calendrier pour la planification de la tâche de publication récurrente. Vous pouvez sélectionner l’option **[!UICONTROL Personnalisé]** et saisir une règle dans le champ Texte de la règle pour décrire un intervalle de tâches personnalisé.

Voir [Création d’un intervalle de temps de tâche de téléchargement ou de publication personnalisé](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

>[!NOTE]
>
>les tâches de publication (et de téléchargement) périodiques sont répertoriées sur la page Tâches. Vous pouvez modifier ou supprimer une tâche planifiée sous l’onglet Planifiée, sur la page Tâches.

### Options de publication avancées {#advanced-publish-options}

Vous pouvez afficher les options avancées sur la page Publication et choisir les options suivantes pour gérer une tâche de publication :

* **[!UICONTROL Publish To]** : pour publier des ressources uniquement sur un serveur spécifique, choisissez un type de serveur.

* **[!UICONTROL Publish]** : par défaut, Adobe Dynamic Media Classic publie uniquement les nouvelles ressources qui n’ont pas été publiées avant (option Nouveau depuis le dernier Publish ). Cependant, vous pouvez sélectionner **[!UICONTROL Publish complet]** afin de publier également les ressources qui ont été mises à jour ou modifiées depuis leur dernière publication. Sélectionnez **[!UICONTROL Complet avec données de recherche]** si vous publiez un catalogue électronique et souhaitez que les lecteurs puissent y effectuer des recherches par mot-clé.

* **[!UICONTROL Exécuter la tâche en tant que]** : sélectionnez un nom d’utilisateur dans la liste. Vous pouvez trier les tâches par nom d’utilisateur sur la page Tâches. En choisissant un nom, vous associez une tâche de publication à un utilisateur.

**[!UICONTROL Notification HTTP]** : entrez une URL pour déclencher les tâches de publication suivantes.

Voir [Utilisation d’une tâche de téléchargement ou de publication comme déclencheur](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger).)

## Annulation d’une tâche de publication {#canceling-a-publish-job}

Vous pouvez annuler une tâche de publication en cours. Par ailleurs, si vous êtes administrateur, vous pouvez annuler une tâche de publication en cours à partir de la page des tâches de l’entreprise.

Pour annuler une tâche de publication, accédez à la page Tâches et sélectionnez **[!UICONTROL Annuler]**. Dans l’onglet Planifié de la page Tâches, vous pouvez suspendre ou reprendre une tâche en désélectionnant ou en cochant la case dans la colonne Actif de la tâche.

>[!NOTE]
>
>Une fois la tâche de publication annulée, son état passe à &quot;arrêt&quot; jusqu’à ce que la tâche atteigne un point où elle peut s’arrêter en toute sécurité. L’arrêt d’une tâche de publication peut prendre un certain temps si la tâche est en train d’obtenir des données de la base de données.

## Ressources Publish manuellement {#manually-publishing-assets}

Vous pouvez publier des fichiers individuels manuellement au lieu de créer une tâche de publication. Lorsque vous publiez des visionneuses, telles qu’une visionneuse d’images ou de vidéos adaptatives, la visionneuse (ou &quot;parent&quot;) et tous les membres (ou &quot;enfants&quot;) de cette visionneuse sont publiés.

Les ressources non publiées sont indiquées dans l’interface utilisateur par une icône grise et ronde avec une barre oblique (état non publié), à gauche du nom de la ressource. Une fois le fichier publié, l’icône devient verte et une coche blanche s’affiche en son centre (état publié).

**Pour publier des ressources manuellement :**

1. Effectuez l’une des opérations suivantes :

   * En mode Affichage de la grille, Affichage par liste ou Affichage des détails, utilisez les méthodes standard de sélection des fichiers pour sélectionner un ou plusieurs fichiers non publiés.

     Dans la barre de navigation globale, accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Publish]**.

   * En mode Grille, Liste ou Détails, sélectionnez l’icône grise ronde avec une barre oblique, à gauche du nom de la ressource.

## Annulation manuelle de la publication des ressources {#manually-unpublishing-assets}

Vous pouvez annuler manuellement la publication de fichiers individuels. Lorsque vous annulez la publication d’ensembles, tels qu’une série d’échantillons ou un catalogue électronique, la série (ou &quot;parent&quot;) passe à l’état non publié. Cependant, les membres (ou &quot;enfants&quot;) de cet ensemble ne sont pas affectés ; au lieu de cela, ils conservent chacun leur état publié ou non publié existant.

Les ressources publiées sont indiquées dans l’interface utilisateur par une icône ronde et verte avec une coche blanche au centre (état publié), à gauche du nom de la ressource. Une fois la publication d’une ressource annulée, l’icône devient grise avec une barre oblique (état non publié),

**Pour annuler manuellement la publication de ressources :**

1. Effectuez l’une des opérations suivantes :

   * En mode Grille, Liste ou Détails, sélectionnez une ou plusieurs ressources publiées.

     Sur la barre de navigation globale, accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Annuler la publication]**.

   * En mode Grille, Liste ou Détails, sélectionnez l’icône en forme de coche ronde et verte située à gauche du nom de la ressource.

## Obtention de l’historique de publication d’une ressource {#getting-an-asset-s-publish-history}

La dernière date de publication d’une ressource s’affiche dans l’affichage des détails en haut du panneau. Pour plus d’informations sur l’historique de publication, ouvrez le panneau Historique et serveurs publiés dans la vue Détails. A partir de là, vous pouvez savoir quand le fichier a été publié et vers quels serveurs.

## Fichiers republiés et délais CDN {#republished-assets-and-cdn-delays}

Les ressources Adobe Dynamic Media Classic sont distribuées sur le réseau de diffusion de contenu (CDN). CDN est un système de serveurs informatiques reliés en réseau qui coopèrent de manière transparente pour diffuser des contenus, surtout des contenus multimédias volumineux, vers des utilisateurs finaux. Dans le système CDN, le contenu web est stocké dans des caches Web sur Internet (appelé réseau de cache de périphérie). Le contenu web est diffusé à partir des caches Web aux utilisateurs finaux afin de permettre des diffusions plus rapides.

La première fois qu’un utilisateur télécharge une page Web, les ressources sont diffusées sur un serveur de cache Web CDN. Ce serveur les stocke de sorte que, la prochaine fois qu’une personne se trouvant dans la même zone accédera à la page Web, le même contenu mis en cache sera diffusé plus rapidement. Le contenu étant plus proche de l’utilisateur final, il est livré plus vite. Le réseau de diffusion de contenu accélère l’affichage des pages Web. Il réduit les besoins en bande passante sur le serveur central dans la mesure où le contenu est diffusé à partir du réseau cache de périphérie, et non pas d’un serveur central à chaque fois.

Le contenu Adobe Dynamic Media Classic récemment publié est immédiatement disponible pour l’utilisateur final et remplit rapidement le réseau de cache de périphérie. Toutefois, le contenu récemment republié, c’est-à-dire les images portant le même nom que les images précédemment publiées sur un serveur d’images, ne sont pas mises à jour sur le réseau de diffusion de contenu pendant dix heures au maximum. À la place, les utilisateurs finaux voient ce qui se trouve dans un cache Web sur le réseau CDN. Pour cette raison, les ressources republiées d’Adobe Dynamic Media Classic ne semblent pas être destinées aux utilisateurs finaux pendant dix heures.

Si vous souhaitez que vos ressources d’image nouvellement republiées soient disponibles avant le délai de dix heures, vous pouvez vider les caches web sur le réseau de diffusion de contenu. Le vidage de ces caches Web supprime l’ancien contenu des caches Web CDN et le remplace par vos dernières ressources publiées.

Pour vider le cache, dans la barre de navigation globale, accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Invalider le CDN]**. Tous les fichiers sélectionnés sont supprimés du cache. Si aucun fichier de publication n’est disponible ou si vous n’êtes pas l’administrateur de la société, l’option Supprimer du réseau de redéfinition de contenu est désactivée.

>[!MORELIKETHIS]
>
>* [Vérifier les fichiers de tâche](checking-job-files.md)
>* [Modifier, supprimer, mettre en pause et reprendre des tâches récurrentes](checking-job-files.md#editing-deleting-pausing-and-resuming-recurring-jobs)
