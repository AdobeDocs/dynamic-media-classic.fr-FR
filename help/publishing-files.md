---
title: 'Publication de fichiers '
description: Vous publiez vos fichiers sur les serveurs Dynamic Media Image Server. Vous pouvez publier des fichiers une seule fois ou organiser Dynamic Media Classic pour publier des fichiers selon un calendrier récurrent. Une fois vos fichiers publiés, vous en disposez pour les diffuser. Vous pouvez copier les appels d’URL de Dynamic Media Classic et les ajouter à votre site Web ou application.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
translation-type: tm+mt
source-git-commit: 2f7366a77c0fa5f3953721cdd5328123d9c2a052
workflow-type: tm+mt
source-wordcount: '1706'
ht-degree: 75%

---


# Publication de fichiers {#publishing-files}

Vous publiez vos fichiers sur les serveurs Dynamic Media Image Server. Vous pouvez publier des fichiers une seule fois ou organiser Dynamic Media Classic pour publier des fichiers selon un calendrier récurrent. Une fois vos fichiers publiés, vous en disposez pour les diffuser. Vous pouvez copier les appels d’URL de Dynamic Media Classic et les ajouter à votre site Web ou application.

Dynamic Media Classic prend désormais en charge la diffusion de toutes les images et vidéos sur HTTP/2. En d’autres termes, une URL publiée ou un code incorporé pour l’image ou la vidéo peut être intégré à toute application qui accepte une ressource hébergée. Cet actif publié est ensuite livré au moyen du protocole HTTP/2. Cette méthode de diffusion améliore la manière dont les navigateurs et les serveurs communiquent, ce qui permet de mieux répondre et de mieux charger les ressources Dynamic Media Classic. Voir [Diffusion HTTP2 de la FAQ sur le contenu](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/http2.html#dynamic).

## Publication après le téléchargement {#publish-after-uploading}

Fichiers dans un état publié ou non publié. Par défaut, tous les fichiers que vous téléchargez dans Dynamic Media Classic sont automatiquement marqués pour publication.

Pour plus d’informations, voir le [Instant Publish Notice PDF](/help/assets/rendering-instant-publish-notification.pdf).

Pour marquer des fichiers pour publication, utilisez les techniques suivantes :

* **Publier après le**
téléchargementSur la page de téléchargement, dans la partie inférieure, sélectionnez Publier après le téléchargement. La valeur par défaut est un état sélectionné.

* **Publier après le**
téléchargement Dans la boîte de dialogue Options de la tâche, sélectionnez Publier après le téléchargement. La valeur par défaut est un état sélectionné.

Certains fichiers « enfants » sont systématiquement marqués pour publication lorsque leurs parents le sont. Ce tableau dresse la liste des fichiers enfants automatiquement marqués pour publication.

| Elément (groupe) parent | Eléments (membre) enfants |
|--- |--- |
| Visionneuses d’images | Images dans la visionneuse. |
| Séries d’échantillons | Echantillons dans la visionneuse. |
| Visionneuses à 360° | Images dans la visionneuse. |
| Modèles | Images, pages et fichiers de modèle. |

Les images dérivées sont automatiquement marquées pour publication lorsque leurs images parentes sont publiées. Les images dérivées incluent les images que vous avez modifiées avec des options d’édition d’image. Vous pouvez voir ces images dérivées dans la vue de détail sous Version et dérivés.

## Création d’une tâche de publication  {#creating-a-publish-job}

Créez une tâche de publication pour publier des fichiers que vous avez téléchargés sur les serveurs Dynamic Media Classic, mais que vous avez choisi de ne pas publier automatiquement pour le moment. Vous pouvez réaliser une tâche de publication unique ou planifier la publication périodique de certaines tâches. Dynamic Media Classic offres propose des options de publication avancées pour des serveurs spécifiques et des options de republication de fichiers déjà publiés.

**Création d’une tâche de publication**

1. Sur la barre de navigation générale, cliquez sur **Publier**, 
1. Dans la boîte de dialogue Publier, choisissez s’il s’agit d’une tâche de publication ponctuelle ou périodique

   (voir les sections [Création d’une tâche de publication unique](publishing-files.md#creating_a_one_time_publish_job) et [Création d’une tâche de publication périodique](publishing-files.md#creating_a_recurring_publish_job)).

1. Entrez un nom de tâche.
1. (Facultatif) Affichez les options avancées, puis choisissez parmi elles 

   (voir [Options de publication avancées](publishing-files.md#advanced_publish_options)).

1. Cliquez sur **Lancer public.**

Dynamic Media Classic effectue le suivi des tâches de publication sur la page Tâches. Vous pouvez consulter les tâches de publication sur cette page.

>[!NOTE]
>
>les fichiers que vous republiez (vous les avez publiés auparavant) ne s’affichent pas immédiatement sur votre site Web en raison du mécanisme de mise en mémoire cache Web activé sur le réseau de diffusion de contenu (CDN) (voir [Fichiers republiés et délais CDN](publishing-files.md#republished_assets_and_cdn_delays)).

### Création d’une tâche de publication unique {#creating-a-one-time-publish-job}

Pour créer une tâche de publication unique, sélectionnez l’option Unique sur la page de publication.

Si vous souhaitez que la tâche de publication ait lieu à une date ultérieure, sélectionnez l’option Planifier pour plus tard dans le menu Quand. Puis, à l’aide du curseur de calendrier et d’heure, sélectionnez le jour et l’heure d’exécution de la publication.

### Création d’une tâche de publication périodique  {#creating-a-recurring-publish-job}

Pour créer une tâche de publication périodique, sélectionnez l’option Périodique sur la page de publication.

Puis, pour définir la périodicité de la tâche de publication, choisissez une option Répéter : Chaque jour, Une fois par semaine, Une fois par mois ou Personnalisé. Dynamic Media Classic propose des outils de calendrier pour la planification de la tâche de publication périodique. Vous pouvez choisir l’option Personnalisé, puis entrer une règle dans la zone Règle pour définir un intervalle de tâche personnalisé 

(voir [Création d’un intervalle de téléchargement ou de publication personnalisé](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval)).

>[!NOTE]
>
>les tâches de publication (et de téléchargement) périodiques sont répertoriées sur la page Tâches. Vous pouvez modifier ou supprimer une tâche planifiée sous l’onglet Planifiée, sur la page Tâches.

### Options de publication avancées {#advanced-publish-options}

Vous pouvez afficher les options avancées sur la page de publication et en choisir certaines pour gérer une tâche de publication :

* **Publier**
versChoisissez un type de serveur pour publier des fichiers uniquement sur un serveur spécifique et non sur tous les serveurs.

* ****
PublierPar défaut, Dynamic Media Classic publie uniquement les fichiers nouveaux qui n’ont pas été publiés auparavant (option Nouveau depuis la dernière publication). Cependant, vous pouvez choisir l’option Publication complète pour publier également les fichiers qui ont été mis à jour ou modifiés depuis leur dernière publication. Choisissez l’option Complet avec données de recherche si vous publiez un catalogue électronique et souhaitez que ses utilisateurs puissent y effectuer des recherches par mot-clé.

* **Exécuter la tâche**
en tant queChoisissez un nom d&#39;utilisateur dans la liste. Vous pouvez trier les tâches par nom d’utilisateur sur la page Tâches. En choisissant un nom, vous associez une tâche de publication à un utilisateur.

**Notification HTTPEntrez une URL pour déclencher les tâches de publication suivantes.**


(voir [Utilisation d’une tâche de téléchargement ou de publication comme déclencheur](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)).

## Annulation d’une tâche de publication  {#canceling-a-publish-job}

Vous pouvez annuler une tâche de publication en cours. Par ailleurs, si vous êtes administrateur, vous pouvez annuler une tâche de publication en cours à partir de la page des tâches de l’entreprise.

Pour annuler une tâche de publication, sur la page Tâches, cliquez sur Annuler. Dans l’onglet Planifiée de la page Tâches, vous pouvez interrompre ou reprendre une tâche en décochant/cochant la case située dans la colonne Actif de la tâche.

>[!NOTE]
>
>après avoir annulé une tâche de publication, son état devient « Arrêt en cours » tant qu’elle n’a pas atteint un point où elle peut s’arrêter en toute sécurité. L’arrêt d’une tâche de publication peut prendre un certain temps si la récupération des données dans la base de données est en cours.

## Publication manuelle de fichiers  {#manually-publishing-assets}

Vous pouvez publier des fichiers individuels manuellement au lieu de créer une tâche de publication. Lorsque vous publiez des visionneuses, comme une visionneuse d’images ou de vidéos adaptative, la visionneuse (ou « parent ») et tous les membres (ou « enfants ») dans cette visionneuse sont publiés.

Les fichiers non publiés sont indiqués dans l’interface utilisateur par une icône grise et ronde traversée d’une barre oblique (état non publié), à gauche du nom du fichier. Une fois le fichier publié, l’icône devient verte et une coche blanche s’affiche en son centre (état publié).

**Pour publier manuellement des fichiers**

1. Effectuez l’une des opérations suivantes :

   * En mode Affichage de la grille, Affichage par liste ou Affichage des détails, utilisez les méthodes standard de sélection des fichiers pour sélectionner un ou plusieurs fichiers non publiés.

      Sur la barre de navigation globale, cliquez sur **Fichier > Publier**.

   * En mode Affichage de la grille, Affichage par liste ou Affichage des détails, cliquez sur l’icône grise et ronde traversée d’une barre oblique, à gauche du nom du fichier.

## Annulation manuelle de la publication de fichiers  {#manually-unpublishing-assets}

Vous pouvez annuler manuellement la publication de fichiers individuels. Lorsque vous annulez la publication de visionneuses, comme une visionneuse de série d’échantillons ou un catalogue électronique, la visionneuse (ou « parent ») passe à l’état non publié. Toutefois, les membres (ou « enfants ») de cette visionneuse ne sont pas affectés : ils conservent en fait leur état existant publié ou non publié.

Les fichiers publiés sont indiqués dans l’interface utilisateur par une icône ronde et verte avec une coche blanche affichée en son centre (état publié), à gauche du nom du fichier. Suite à l’annulation de la publication d’un fichier, l’icône s’affiche en gris et traversée d’une barre oblique (état non publié),

**Pour annuler manuellement la publication de fichiers**

1. Effectuez l’une des opérations suivantes :

   * En mode Affichage de la grille, Affichage par liste ou Affichage des détails, sélectionnez un ou plusieurs fichiers publiés.

      Dans la barre de navigation globale, cliquez sur **Fichier > **Annuler la publication**.

   * En mode Affichage de la grille, Affichage par liste ou Affichage des détails, cliquez sur l’icône ronde marquée d’une coche verte située sur la gauche du nom du fichier.

## Récupération de l’historique de publication d’un fichier  {#getting-an-asset-s-publish-history}

La dernière date de publication d’un fichier apparaît dans la vue Affichage des détails située dans la partie supérieure du panneau. Vous pouvez obtenir des détails supplémentaires sur l’historique de publication dans le panneau Historique et serveurs publiés de la vue de détail. A partir de là, vous pouvez savoir quand le fichier a été publié et vers quels serveurs.

## Fichiers republiés et délais CDN {#republished-assets-and-cdn-delays}

Les ressources Dynamic Media Classic sont distribuées sur le réseau CDN (Content diffusion Network). CDN est un système de serveurs informatiques reliés en réseau qui coopèrent de manière transparente pour diffuser des contenus, surtout des contenus multimédias volumineux, vers des utilisateurs finaux. Dans le système CDN, le contenu Web est stocké dans des caches Web sur le réseau Internet (appelé réseau cache de périphérie). Le contenu Web est livré aux utilisateurs plus rapidement à partir de ces caches Web.

Lors du premier téléchargement d’une page Web, les fichiers correspondants sont envoyés à un serveur cache CDN pour y être stockés. Ainsi, au prochain accès de la page Web, le même contenu mis en cache pourra être acheminé plus rapidement à une personne située à proximité. Le contenu étant plus proche de l’utilisateur final, il est livré plus vite. Le système CDN accélère l’affichage des pages Web. Il réduit les besoins en bande passante sur le serveur central dans la mesure où le contenu est diffusé à partir du réseau cache de périphérie, et non pas d’un serveur central à chaque fois.

Le contenu Dynamic Media Classic récemment publié est immédiatement disponible pour l’utilisateur final et remplit rapidement le réseau de cache de périphérie. Néanmoins, le contenu venant d’être republié (à savoir des images portant exactement le même nom que les images précédemment publiées vers un serveur d’images) n’est actualisé sur le CDN qu’au bout de 10 heures, au maximum. En fait, l’utilisateur final n’a accès qu’au contenu du cache Web sur le réseau CDN. Pour cette raison, il est possible que les fichiers republiés dans Dynamic Media Classic ne s’affichent pas pour les utilisateurs finaux pendant dix heures.

Pour mettre à disposition des fichiers récemment republiés avant ce délai de 10 heures, vous pouvez vider les caches Web sur le CDN. Ce vidage aura pour effet de supprimer l’ancien contenu des caches Web CDN et de le remplacer par les derniers fichiers publiés.

Pour vider le cache, cliquez sur Fichier > Invalider sur le réseau de diffusion de contenu. Tous les fichiers sélectionnés sont supprimés du cache. Si aucun fichier de publication n’est disponible ou si vous n’êtes pas l’administrateur de la société, l’option Supprimer du réseau de redéfinition de contenu est désactivée.

>[!MORELIKETHIS]
>
>* [Vérification de fichiers de tâche](checking-job-files.md)
>* [Edition, suppression, interruption et reprise de tâches](checking-job-files.md#editing-deleting-pausing-and-resuming-recurring-jobs)

