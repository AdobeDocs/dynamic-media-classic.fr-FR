---
title: Publier des fichiers
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

# Publier des fichiers{#publishing-files}

Vous publiez vos ressources sur les serveurs d’images Dynamic Media. Vous pouvez publier des ressources sur une base unique ou demander à Adobe Dynamic Media Classic de les publier selon un calendrier récurrent. Une fois vos fichiers publiés, vous en disposez pour les diffuser. Vous pouvez copier les appels d’URL d’Adobe Dynamic Media Classic et les ajouter à votre site web ou à votre application.

Adobe Dynamic Media Classic prend désormais en charge la diffusion de toutes les images et vidéos via HTTP/2. En d’autres termes, une URL publiée ou un code intégré pour l’image ou la vidéo peut être intégré à toute application qui accepte une ressource hébergée. Cette ressource publiée utilise le protocole HTTP/2 pour la diffuser. Cette méthode de diffusion améliore la communication entre les navigateurs et les serveurs, ce qui permet d’obtenir de meilleurs temps de réponse et de chargement pour toutes vos ressources Adobe Dynamic Media Classic. Voir la [HTTP2 FAQ sur la diffusion de contenu](https://experienceleague.adobe.com/fr/docs/experience-manager-65/content/assets/dynamic/http2).

## Publication après le téléchargement {#publish-after-uploading}

Fichiers dans un état publié ou non publié. Par défaut, toutes les ressources que vous chargez dans Adobe Dynamic Media Classic sont automatiquement marquées pour publication.

Pour plus d’informations, voir [Avis de publication instantanée PDF](/help/using/assets/rendering-instant-publish-notification.pdf).

Utilisez les techniques suivantes pour marquer les ressources en vue de leur publication :

* **[!UICONTROL Publier après le chargement]** : sur la page Charger, près du bas, sélectionnez **[!UICONTROL Publier après le chargement]**. La valeur par défaut est un état sélectionné.

* **[!UICONTROL Publier après le chargement]** : dans la boîte de dialogue Options de la tâche, sélectionnez **[!UICONTROL Publier après le chargement]**. La valeur par défaut est un état sélectionné.

Certains fichiers « enfants » sont systématiquement marqués pour publication lorsque leurs parents le sont. Ce tableau répertorie les ressources enfants qui sont automatiquement marquées pour publication.

| Elément (groupe) parent | Eléments (membre) enfants |
| --- | --- |
| Visionneuses d’images | Images dans la visionneuse. |
| Série d’échantillons | Echantillons dans la visionneuse. |
| Visionneuses à 360° | Images dans la visionneuse. |
| Modèles | Fichiers modèles, pages et images. |

Les images dérivées sont également automatiquement marquées pour publication lorsque leurs images parentes sont en cours de publication. Les images dérivées incluent les images que vous avez modifiées avec des options d’édition d’image. Vous pouvez voir ces images dérivées dans la vue détaillée sous Créés et dérivés.

## Création d’un traitement de publication {#creating-a-publish-job}

Créez une tâche de publication pour publier les ressources que vous avez chargées sur les serveurs Adobe Dynamic Media Classic mais que vous ne souhaitez pas encore publier automatiquement. Vous pouvez effectuer une tâche de publication unique ou planifier des tâches récurrentes. Adobe Dynamic Media Classic propose des options de publication avancées pour la publication sur des serveurs spécifiques, ainsi que des options pour republier des ressources déjà publiées.

**Pour créer une tâche de publication, procédez comme suit**

1. Sur la barre de navigation générale, sélectionnez **[!UICONTROL Publier]**.
1. Dans la boîte de dialogue Publication, choisissez si vous souhaitez une tâche de publication ponctuelle ou récurrente.

   Voir [Création d’une tâche de publication unique](publishing-files.md#creating_a_one_time_publish_job) et [Création d’une tâche de publication récurrente](publishing-files.md#creating_a_recurring_publish_job).

1. Entrez un nom de tâche.
1. (Facultatif) Affichez les options avancées, puis choisissez parmi elles 

   (voir [Options de publication avancées](publishing-files.md#advanced_publish_options)).

1. Sélectionnez **[!UICONTROL Envoyer la publication]**.

Adobe Dynamic Media Classic effectue le suivi des tâches de publication sur la page Tâches . Vous pouvez consulter les tâches de publication sur cette page.

>[!NOTE]
>
>Les Assets que vous avez republiées (vous les avez déjà publiées) n’apparaissent pas immédiatement sur votre site web en raison du mécanisme de mise en cache web sur le réseau de diffusion de contenu (CDN). (voir [Fichiers republiés et délais CDN](publishing-files.md#republished_assets_and_cdn_delays)).

### Création d’une tâche de publication unique {#creating-a-one-time-publish-job}

Créez une tâche de publication ponctuelle en sélectionnant l’option **[!UICONTROL Une seule fois]** sur la page Publication .

Si vous souhaitez que la tâche de publication se produise ultérieurement, dans la page Publication, sélectionnez **[!UICONTROL Une fois]**. Dans la liste déroulante, sélectionnez **[!UICONTROL Planifier pour plus tard]**. Utilisez le calendrier et le curseur Heure pour sélectionner un jour et une heure d’exécution de la tâche de publication.

### Créer une tâche de publication récurrente {#creating-a-recurring-publish-job}

Créez une tâche de publication récurrente en sélectionnant **[!UICONTROL Récurrent]** sur la page Publication .

Choisissez ensuite l’option Répéter de **[!UICONTROL Quotidien]**, **[!UICONTROL Hebdomadaire]**, **[!UICONTROL Mensuel]** ou **[!UICONTROL Personnalisé]**, puis indiquez à quel moment vous souhaitez que la tâche de publication se répète. Adobe Dynamic Media Classic présente les outils de calendrier pour la planification de la tâche de publication récurrente. Vous pouvez sélectionner l’option **[!UICONTROL Personnalisé]** et saisir une règle dans le champ de texte Règle pour décrire un intervalle de tâche personnalisé.

Voir [&#x200B; Création d’un intervalle personnalisé de chargement ou de publication](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

>[!NOTE]
>
>les tâches de publication (et de téléchargement) périodiques sont répertoriées sur la page Tâches. Vous pouvez modifier ou supprimer une tâche planifiée sous l’onglet Planifiée, sur la page Tâches.

### Options de publication avancées {#advanced-publish-options}

Vous pouvez afficher les options avancées sur la page Publication et choisir les options suivantes pour gérer une tâche de publication :

* **[!UICONTROL Publier vers]** : pour publier des ressources uniquement sur un serveur spécifique, choisissez un type de serveur.

* **[!UICONTROL Publier]** : par défaut, Adobe Dynamic Media Classic publie uniquement les ressources qui sont nouvelles et qui n’ont pas été publiées auparavant (option Nouveau depuis la dernière publication ). Cependant, vous pouvez sélectionner **[!UICONTROL Publication complète]** afin de publier également les ressources qui ont été mises à jour ou modifiées depuis leur dernière publication. Sélectionnez **[!UICONTROL Complet avec données de recherche]** si vous publiez un catalogue électronique et que vous souhaitez que les lecteurs puissent le rechercher par mot-clé.

* **[!UICONTROL Exécuter le travail en tant que]** : sélectionnez un nom d’utilisateur dans la liste. Vous pouvez trier les tâches par nom d’utilisateur sur la page Tâches. En choisissant un nom, vous associez une tâche de publication à un utilisateur.

**[!UICONTROL Notification HTTP]** : saisissez une URL pour déclencher les tâches de publication suivantes.

Voir [Utiliser une tâche de chargement ou de publication comme déclencheur](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger).)

## Annuler une tâche de publication {#canceling-a-publish-job}

Vous pouvez annuler une tâche de publication en cours. Par ailleurs, si vous êtes administrateur, vous pouvez annuler une tâche de publication en cours à partir de la page des tâches de l’entreprise.

Pour annuler une tâche de publication, accédez à la page Tâches et sélectionnez **[!UICONTROL Annuler]**. Dans l’onglet Planifié de la page Tâches, vous pouvez suspendre ou reprendre une tâche en désactivant ou en cochant la case située dans la colonne Actif de la tâche.

>[!NOTE]
>
>Après l’annulation d’une tâche de publication, son statut passe à « arrêt » jusqu’à ce que la tâche atteigne un point où elle peut s’arrêter en toute sécurité. L’arrêt d’une tâche de publication peut prendre un certain temps si la tâche est en cours d’obtention des données de la base de données.

## Publication manuelle de ressources {#manually-publishing-assets}

Vous pouvez publier des fichiers individuels manuellement au lieu de créer une tâche de publication. Lorsque vous publiez des visionneuses, telles qu’une visionneuse d’images ou une visionneuse de vidéos adaptative, la visionneuse (ou la visionneuse « parente ») et tous ses membres (ou ses « enfants ») sont publiés.

Les ressources dépubliées sont indiquées dans l’interface utilisateur par une icône ronde grise barrée d’une barre oblique (statut dépublié), à gauche du nom de la ressource. Une fois le fichier publié, l’icône devient verte et une coche blanche s’affiche en son centre (état publié).

**Pour publier les ressources manuellement, procédez comme suit**

1. Effectuez l’une des opérations suivantes :

   * En mode Affichage de la grille, Affichage par liste ou Affichage des détails, utilisez les méthodes standard de sélection des fichiers pour sélectionner un ou plusieurs fichiers non publiés.

     Sur la barre de navigation générale, accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Publier]**.

   * Dans la vue Grille, Liste ou Détails, sélectionnez l’icône grise et ronde entourée d’une barre oblique, située à gauche du nom de la ressource.

## Dépublication manuelle de ressources {#manually-unpublishing-assets}

Vous pouvez annuler manuellement la publication de fichiers individuels. Lorsque vous dépubliez des visionneuses, telles qu’une visionneuse d’échantillons ou un catalogue électronique, la visionneuse (ou le « parent ») passe elle-même à l’état dépublié. Toutefois, les membres (ou « enfants ») de cet ensemble ne sont pas affectés. Ils conservent chacun leur état publié ou dépublié existant.

Les ressources publiées sont signalées dans l’interface utilisateur par une icône ronde verte avec une coche blanche au centre (statut publié), à gauche du nom de la ressource. Une fois la dépublication d’une ressource effectuée, l’icône devient grise et est barrée d’une barre oblique (statut dépublié).

**Pour dépublier des ressources manuellement, procédez comme suit**

1. Effectuez l’une des opérations suivantes :

   * Dans la vue Grille, Liste ou Détails, sélectionnez une ou plusieurs ressources publiées.

     Sur la barre de navigation générale, accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Dépublier]**.

   * Dans la vue Grille, Liste ou Détails, sélectionnez l’icône en forme de coche ronde verte à gauche du nom de la ressource.

## Obtention de l’historique de publication d’une ressource {#getting-an-asset-s-publish-history}

La dernière date de publication d’une ressource s’affiche dans l’affichage des détails en haut du panneau. Pour plus d’informations sur l’historique de publication, ouvrez le panneau Historique et serveurs publiés dans l’affichage des détails. A partir de là, vous pouvez savoir quand le fichier a été publié et vers quels serveurs.

## Fichiers republiés et délais CDN {#republished-assets-and-cdn-delays}

Les ressources Adobe Dynamic Media Classic sont distribuées sur le réseau de diffusion de contenu (CDN). CDN est un système de serveurs informatiques reliés en réseau qui coopèrent de manière transparente pour diffuser des contenus, surtout des contenus multimédias volumineux, vers des utilisateurs finaux. Dans le système CDN, le contenu Web est stocké dans des caches Web sur Internet (appelé réseau de cache Edge). Le contenu web est diffusé à partir des caches web vers les utilisateurs finaux afin de permettre des diffusions plus rapides.

La première fois qu’une personne télécharge une page web, les ressources sont diffusées à un serveur de cache web CDN. Ce serveur les stocke de sorte que la prochaine fois qu’une personne se trouvant dans la même zone accédera à la page web, le même contenu mis en cache sera diffusé plus rapidement. Le contenu étant plus proche de l’utilisateur final, il est livré plus vite. Le réseau de diffusion de contenu accélère l’affichage des pages web. Il réduit les besoins en bande passante sur le serveur central dans la mesure où le contenu est diffusé à partir du réseau cache de périphérie, et non pas d’un serveur central à chaque fois.

Le contenu Adobe Dynamic Media Classic nouvellement publié est immédiatement disponible pour l’utilisateur final et renseigne rapidement le réseau de cache Edge. Cependant, le contenu nouvellement republié, c’est-à-dire les images portant le même nom que les images précédemment publiées sur un serveur d’images, ne sera pas mis à jour sur le réseau CDN pendant une durée maximale de dix heures. Au lieu de cela, les utilisateurs finaux voient ce qui se trouve dans un cache Web sur le réseau CDN. Pour cette raison, les ressources republiées par Adobe Dynamic Media Classic n’apparaissent pas aux utilisateurs finaux pendant dix heures.

Si vous souhaitez que vos ressources d’images nouvellement republiées soient disponibles avant ce délai de dix heures, vous pouvez vider les caches Web sur le réseau CDN. Le vidage de ces caches web supprime l’ancien contenu des caches web du réseau CDN et le remplace par vos ressources publiées le plus récemment.

Pour vider le cache, sur la barre de navigation globale, accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Invalider sur le réseau de diffusion de contenu]**. Tous les fichiers sélectionnés sont supprimés du cache. Si aucun fichier de publication n’est disponible ou si vous n’êtes pas l’administrateur de la société, l’option Supprimer du réseau de redéfinition de contenu est désactivée.

>[!MORELIKETHIS]
>
>* [Vérifier les fichiers de traitement](checking-job-files.md)
>* [Modifier, supprimer, suspendre et reprendre les tâches récurrentes](checking-job-files.md#editing-deleting-pausing-and-resuming-recurring-jobs)
