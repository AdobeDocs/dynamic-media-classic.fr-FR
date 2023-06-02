---
title: Publication de fichiers
description: "Découvrez comment publier vos ressources sur les serveurs d’images Dynamic Media. Vous pouvez publier des ressources ponctuellement ou organiser Adobe Dynamic Media Classic pour les publier selon une planification récurrente. Une fois vos fichiers publiés, vous en disposez pour les diffuser. Vous pouvez copier les appels d’URL d’Adobe Dynamic Media Classic et les ajouter à votre site web ou à votre application."
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 91b73a09-c5b5-4001-b36f-6bebe65717ff
source-git-commit: 358284e6c9888e5188bec35eb7b5408563a71bad
workflow-type: tm+mt
source-wordcount: '1729'
ht-degree: 45%

---

# Publication de fichiers{#publishing-files}

Vous publiez vos ressources sur les serveurs d’images Dynamic Media. Vous pouvez publier des ressources ponctuellement ou organiser Adobe Dynamic Media Classic pour les publier selon une planification récurrente. Une fois vos fichiers publiés, vous en disposez pour les diffuser. Vous pouvez copier les appels d’URL d’Adobe Dynamic Media Classic et les ajouter à votre site web ou à votre application.

Adobe Dynamic Media Classic prend désormais en charge la diffusion de toutes les images et vidéos sur HTTP/2. En d’autres termes, une URL publiée ou un code incorporé pour l’image ou la vidéo peut être intégré à toute application qui accepte une ressource hébergée. Cette ressource publiée est ensuite diffusée au moyen du protocole HTTP/2. Cette méthode de remise améliore la communication entre les navigateurs et les serveurs, ce qui permet de bénéficier de meilleurs temps de réponse et de chargement de toutes vos ressources Adobe Dynamic Media Classic. Voir [FAQ sur la diffusion de contenu HTTP2](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/http2.html#dynamic).

## Publication après le téléchargement {#publish-after-uploading}

Fichiers dans un état publié ou non publié. Par défaut, toutes les ressources que vous chargez dans Adobe Dynamic Media Classic sont automatiquement marquées pour publication.

Pour plus d’informations, voir [PDF Instant Publish Notice](/help/assets/rendering-instant-publish-notification.pdf).

Pour marquer des fichiers pour publication, utilisez les techniques suivantes :

* **[!UICONTROL Publier après le téléchargement]** - Sur la page Télécharger, près du bas, sélectionnez **[!UICONTROL Publier après le téléchargement]**. La valeur par défaut est un état sélectionné.

* **[!UICONTROL Publier après le téléchargement]** - Dans la boîte de dialogue Options de tâche, sélectionnez **[!UICONTROL Publier après le téléchargement]**. La valeur par défaut est un état sélectionné.

Certains fichiers « enfants » sont systématiquement marqués pour publication lorsque leurs parents le sont. Ce tableau dresse la liste des fichiers enfants automatiquement marqués pour publication.

| Elément (groupe) parent | Eléments (membre) enfants |
| --- | --- |
| Visionneuses d’images | Images dans la visionneuse. |
| Série d’échantillons | Echantillons dans la visionneuse. |
| Visionneuses à 360° | Images dans la visionneuse. |
| Modèles | Images, pages et fichiers de modèle. |

Les images dérivées sont automatiquement marquées pour publication lorsque leurs images parentes sont publiées. Les images dérivées incluent les images que vous avez modifiées avec des options d’édition d’image. Vous pouvez voir ces images dérivées dans la vue Détails sous Créé et dérivés.

## Création d’une tâche de publication {#creating-a-publish-job}

Créez une tâche de publication pour publier les ressources que vous avez chargées sur les serveurs Adobe Dynamic Media Classic, mais que vous ne souhaitez pas encore publier automatiquement. Vous pouvez effectuer une tâche de publication ponctuelle ou planifier la réexécution régulière des tâches. Adobe Dynamic Media Classic propose des options de publication avancées pour la publication sur des serveurs spécifiques et des options pour la republication de ressources qui ont déjà été publiées.

**Création d’une tâche de publication:**

1. Dans la barre de navigation globale, sélectionnez **[!UICONTROL Publier]**.
1. Dans la boîte de dialogue Publier, choisissez s’il s’agit d’une tâche de publication ponctuelle ou périodique

   Voir [Création d’une tâche de publication unique](publishing-files.md#creating_a_one_time_publish_job) et [Création d’une tâche de publication récurrente](publishing-files.md#creating_a_recurring_publish_job).

1. Entrez un nom de tâche.
1. (Facultatif) Affichez les options avancées, puis choisissez parmi elles 

   (voir [Options de publication avancées](publishing-files.md#advanced_publish_options)).

1. Sélectionner **[!UICONTROL Envoyer la publication]**.

Adobe Dynamic Media Classic effectue le suivi des tâches de publication sur la page Tâches. Vous pouvez consulter les tâches de publication sur cette page.

>[!NOTE]
>
>Les ressources que vous republiez (vous les avez publiées auparavant) n’apparaissent pas immédiatement sur votre site web en raison du mécanisme de mise en cache web sur le réseau de diffusion de contenu (CDN). (voir [Fichiers republiés et délais CDN](publishing-files.md#republished_assets_and_cdn_delays)).

### Création d’une tâche de publication unique {#creating-a-one-time-publish-job}

Créez une tâche de publication unique en sélectionnant l’option **[!UICONTROL Unique]** sur la page Publier .

Si vous souhaitez que la tâche de publication se produise ultérieurement, sélectionnez dans la page Publier . **[!UICONTROL Unique]**, puis sélectionnez **[!UICONTROL Planifier ultérieurement]** menu déroulant. Utilisez le calendrier et le curseur de l’heure pour sélectionner un jour et une heure pour exécuter la tâche de publication.

### Création d’une tâche de publication récurrente {#creating-a-recurring-publish-job}

Créez une tâche de publication récurrente en sélectionnant **[!UICONTROL Récurrente]** sur la page Publier .

Choisissez ensuite l’option Répéter de **[!UICONTROL Quotidien]**, **[!UICONTROL Hebdomadaire]**, **[!UICONTROL Mensuel]** ou **[!UICONTROL Personnalisé]**, puis indiquez quand la tâche de publication doit se répéter. Adobe Dynamic Media Classic présente des outils de calendrier pour la planification de la tâche de publication récurrente. Vous pouvez sélectionner **[!UICONTROL Personnalisé]** et saisissez une règle dans le champ Texte de la règle pour décrire un intervalle de tâche personnalisé.

Voir [Création d’un intervalle de temps de tâche de téléchargement ou de publication personnalisé](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

>[!NOTE]
>
>les tâches de publication (et de téléchargement) périodiques sont répertoriées sur la page Tâches. Vous pouvez modifier ou supprimer une tâche planifiée sous l’onglet Planifiée, sur la page Tâches.

### Options de publication avancées {#advanced-publish-options}

Vous pouvez afficher les options avancées sur la page de publication et en choisir certaines pour gérer une tâche de publication :

* **[!UICONTROL Publier sur]** - Pour publier des ressources uniquement sur un serveur spécifique, choisissez un type de serveur.

* **[!UICONTROL Publier]** - Par défaut, Adobe Dynamic Media Classic publie uniquement les nouvelles ressources qui n’ont pas été publiées avant (option Nouveau depuis la dernière publication ). Vous pouvez toutefois sélectionner **[!UICONTROL Publication complète]** pour publier également les ressources qui ont été mises à jour ou modifiées depuis leur dernière publication. Sélectionner **[!UICONTROL Complet avec données de recherche]** si vous publiez un catalogue électronique et souhaitez que les lecteurs puissent y effectuer des recherches par mot-clé.

* **[!UICONTROL Exécuter la tâche en tant que]** - Sélectionnez un nom d’utilisateur dans la liste. Vous pouvez trier les tâches par nom d’utilisateur sur la page Tâches. En choisissant un nom, vous associez une tâche de publication à un utilisateur.

**[!UICONTROL Notification HTTP]** - Entrez une URL pour déclencher les tâches de publication suivantes.

Voir [Utilisation d’une tâche de téléchargement ou de publication comme déclencheur](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger).)

## Annulation d’une tâche de publication {#canceling-a-publish-job}

Vous pouvez annuler une tâche de publication en cours. Par ailleurs, si vous êtes administrateur, vous pouvez annuler une tâche de publication en cours à partir de la page des tâches de l’entreprise.

Pour annuler une tâche de publication, accédez à la page Tâches et sélectionnez **[!UICONTROL Annuler]**. Dans l’onglet Planifiée de la page Tâches, vous pouvez interrompre ou reprendre une tâche en décochant/cochant la case située dans la colonne Actif de la tâche.

>[!NOTE]
>
>après avoir annulé une tâche de publication, son état devient « Arrêt en cours » tant qu’elle n’a pas atteint un point où elle peut s’arrêter en toute sécurité. L’arrêt d’une tâche de publication peut prendre un certain temps si la récupération des données dans la base de données est en cours.

## Publication manuelle de ressources {#manually-publishing-assets}

Vous pouvez publier des fichiers individuels manuellement au lieu de créer une tâche de publication. Lorsque vous publiez des visionneuses, comme une visionneuse d’images ou de vidéos adaptative, la visionneuse (ou « parent ») et tous les membres (ou « enfants ») dans cette visionneuse sont publiés.

Les ressources non publiées sont indiquées dans l’interface utilisateur par une icône grise et ronde avec une barre oblique (état non publié), à gauche du nom de la ressource. Une fois le fichier publié, l’icône devient verte et une coche blanche s’affiche en son centre (état publié).

**Pour publier manuellement des fichiers:**

1. Effectuez l’une des opérations suivantes :

   * En mode Affichage de la grille, Affichage par liste ou Affichage des détails, utilisez les méthodes standard de sélection des fichiers pour sélectionner un ou plusieurs fichiers non publiés.

      Dans la barre de navigation globale, accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Publier]**.

   * En mode Grille, Liste ou Détails, sélectionnez l’icône grise ronde avec une barre oblique, à gauche du nom de la ressource.

## Annulation manuelle de la publication des ressources {#manually-unpublishing-assets}

Vous pouvez annuler manuellement la publication de fichiers individuels. Lorsque vous annulez la publication de visionneuses, comme une visionneuse de série d’échantillons ou un catalogue électronique, la visionneuse (ou « parent ») passe à l’état non publié. Toutefois, les membres (ou « enfants ») de cette visionneuse ne sont pas affectés : ils conservent en fait leur état existant publié ou non publié.

Les fichiers publiés sont indiqués dans l’interface utilisateur par une icône ronde et verte avec une coche blanche affichée en son centre (état publié), à gauche du nom du fichier. Une fois la publication d’une ressource annulée, l’icône devient grise avec une barre oblique (état non publié),

**Pour annuler manuellement la publication de fichiers:**

1. Effectuez l’une des opérations suivantes :

   * En mode Grille, Liste ou Détails, sélectionnez une ou plusieurs ressources publiées.

      Dans la barre de navigation globale, accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Annuler la publication]**.

   * En mode Grille, Liste ou Détails, sélectionnez l’icône en forme de coche ronde et verte située à gauche du nom de la ressource.

## Obtention de l’historique de publication d’une ressource {#getting-an-asset-s-publish-history}

La dernière date de publication d’une ressource s’affiche dans l’affichage des détails en haut du panneau. Pour plus d’informations sur l’historique de publication, ouvrez le panneau Historique et serveurs publiés dans la vue Détails. A partir de là, vous pouvez savoir quand le fichier a été publié et vers quels serveurs.

## Fichiers republiés et délais CDN {#republished-assets-and-cdn-delays}

Les ressources Adobe Dynamic Media Classic sont distribuées sur le réseau de diffusion de contenu (CDN). CDN est un système de serveurs informatiques reliés en réseau qui coopèrent de manière transparente pour diffuser des contenus, surtout des contenus multimédias volumineux, vers des utilisateurs finaux. Dans le système CDN, le contenu Web est stocké dans des caches Web sur le réseau Internet (appelé réseau cache de périphérie). Le contenu web est diffusé à partir des caches web aux utilisateurs finaux afin de permettre des diffusions plus rapides.

Lors du premier téléchargement d’une page Web, les fichiers correspondants sont envoyés à un serveur cache CDN pour y être stockés. Ainsi, au prochain accès de la page Web, le même contenu mis en cache pourra être acheminé plus rapidement à une personne située à proximité. Le contenu étant plus proche de l’utilisateur final, il est livré plus vite. Le système CDN accélère l’affichage des pages Web. Il réduit les besoins en bande passante sur le serveur central dans la mesure où le contenu est diffusé à partir du réseau cache de périphérie, et non pas d’un serveur central à chaque fois.

Le contenu Adobe Dynamic Media Classic récemment publié est immédiatement disponible pour l’utilisateur final et remplit rapidement le réseau de cache de périphérie. Néanmoins, le contenu venant d’être republié (à savoir des images portant exactement le même nom que les images précédemment publiées vers un serveur d’images) n’est actualisé sur le CDN qu’au bout de 10 heures, au maximum. En fait, l’utilisateur final n’a accès qu’au contenu du cache Web sur le réseau CDN. Pour cette raison, les ressources republiées d’Adobe Dynamic Media Classic ne semblent pas être destinées aux utilisateurs finaux pendant dix heures.

Pour mettre à disposition des fichiers récemment republiés avant ce délai de 10 heures, vous pouvez vider les caches Web sur le CDN. Ce vidage aura pour effet de supprimer l’ancien contenu des caches Web CDN et de le remplacer par les derniers fichiers publiés.

Pour vider le cache, dans la barre de navigation globale, accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Invalider le réseau de diffusion de contenu]**. Tous les fichiers sélectionnés sont supprimés du cache. Si aucun fichier de publication n’est disponible ou si vous n’êtes pas l’administrateur de la société, l’option Supprimer du réseau de redéfinition de contenu est désactivée.

>[!MORELIKETHIS]
>
>* [Vérification des fichiers de tâche](checking-job-files.md)
>* [Modification, suppression, pause et reprise de tâches récurrentes](checking-job-files.md#editing-deleting-pausing-and-resuming-recurring-jobs)

