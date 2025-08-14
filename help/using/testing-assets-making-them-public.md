---
title: Tester les ressources avant leur publication
description: Découvrez comment tester des ressources dans Adobe Dynamic Media Classic avant de les rendre publiques.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: fd78d535-391e-43eb-a8aa-25fa6c2885cb
topic: Content Management
level: Intermediate
source-git-commit: 29752cf9eca0fc9bb760c721e1c3dc8e4ef912c3
workflow-type: tm+mt
source-wordcount: '1061'
ht-degree: 19%

---

# Tester les ressources avant leur publication {#testing-assets-before-making-them-public}

Secure Testing vous permet de définir un environnement de test sécurisé et de créer une solution B2B robuste, basée sur un ensemble configurable d’adresses IP et de plages. Cette fonctionnalité vous permet de faire correspondre vos déploiements Adobe Dynamic Media Classic avec l’architecture de votre système de gestion de contenu et de votre système d’entreprise.

Avec Secure Testing, vous pouvez prévisualiser la version intermédiaire du site Web avec le contenu non publié.

Si vous le souhaitez, vous pouvez créer un environnement d’évaluation plutôt que de rendre les ressources disponibles publiquement, pour les raisons suivantes :

* Aperçu des sites Web avant lancement public (site Web intermédiaire).
* Fournir des ressources nécessitant un accès restreint, telles que des catalogues électroniques qui affichent les prix dans une application Web B2B.
* Utilisez des ressources derrière un pare-feu dans le cadre d’un système de gestion de l’information sur les produits, d’une application de service client, d’un site de formation, etc.

>[!NOTE]
>
>Secure Testing n’affecte pas l’accès à Adobe Dynamic Media Classic. La sécurité d’Adobe Dynamic Media Classic reste cohérente et requiert les informations d’identification habituelles pour accéder à Adobe Dynamic Media Classic et aux services web associés.

## Comment fonctionne Secure Testing {#how-secure-testing-works}

La plupart des entreprises gèrent leur Internet derrière un pare-feu. L’accès à Internet est possible via certaines routes et généralement via une plage limitée d’adresses IP publiques.

À partir du réseau de votre entreprise, vous pouvez déterminer votre adresse IP publique à l’aide de sites web tels que [https://www.whatismyip.com](https://www.whatismyip.com/) ou demander ces informations à votre service informatique d’entreprise.

Grâce à Secure Testing, Adobe Dynamic Media Classic établit un serveur d’images dédié pour les environnements d’évaluation ou les applications internes. Toute requête sur ce serveur vérifie l’adresse IP d’origine. Si la requête entrante ne figure pas dans la liste approuvée des adresses IP, une réponse d’échec est renvoyée. L’administrateur d’entreprise d’Adobe Dynamic Media Classic configure la liste approuvée des adresses IP pour l’environnement Secure Testing de l’entreprise.

Comme l’emplacement de la requête originale doit être confirmé, le trafic du service Secure Testing n’est pas acheminé via un réseau de distribution de contenu comme le trafic du serveur d’images Dynamic Media public. Les requêtes effectuées auprès du service Secure Testing présentent une latence légèrement plus élevée par rapport aux serveurs d’images Dynamic Media publics.

Les fichiers non publiés sont immédiatement disponibles à partir des services Secure Testing, sans avoir besoin d’être publiés. Ainsi, vous pouvez exécuter un aperçu avant la publication des ressources sur leur serveur d’images public.

>[!NOTE]
>
>Les services Secure Testing utilisent le serveur de catalogue configuré avec un contexte de publication interne. Par conséquent, si votre société est configurée pour publier sur Secure Testing, toutes les ressources chargées dans Adobe Dynamic Media Classic sont immédiatement disponibles sur les services Secure Testing. Cette fonctionnalité s’applique que les ressources soient marquées ou non pour publication au moment du chargement.

Les services Secure Testing prennent actuellement en charge les types de ressources et fonctionnalités suivants :

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Added videos to list below 9/11/2012. Moved "Render Server requests" from unsupported to supported, listed below on 3/15/2016 as per email from Cynthia March 11, 2016)</p>

 -->

* Images.
* Vignettes (demandes de seveur Render Server).
* Requêtes du serveur de rendu (prises en charge, mais le client doit le demander explicitement).
* Visionneuses, dont visionneuses d’images, catalogue électronique, visionneuses de rendu et de supports.
* Visionneuses de médias riches Adobe Dynamic Media Classic standard.
* Pages JSP d’Adobe Dynamic Media Classic OnDemand.
* Contenu statique, par exemple fichiers PDF et vidéos servies progressivement.
* Diffusion vidéo en flux continu HTTP.
* Diffusion vidéo progressive.

Les types de fichiers suivants et les fonctionnalités suivantes ne sont actuellement pas pris en charge :

* Recherche catalogue électronique ou informations Adobe Dynamic Media Classic
* Diffusion vidéo en flux continu RTMP
* Impression en ligne
* Services UGC (contenu créé par l’utilisateur)

>[!IMPORTANT]
>
>La prise en charge des ressources d’images vectorielles UGC nouvelles ou existantes dans Adobe Dynamic Media Classic a pris fin le 30 septembre 2021.

## Tester le service Secure Testing {#testing-the-secure-testing-service}

Testez le service Secure Testing afin de vous assurer qu’il fonctionne comme prévu.

<!-- >[!NOTE]
>
>*If you do not mention any IPs under **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]** > **[!UICONTROL Test Image Service]***: If you add an IP only, that IP is able to call the assets and no other IP are allowed to make the calls. As long there is no IP mentioned under that section, all IPs are allowed to make the calls for the assets, and they show up. -->

### Préparation de votre compte

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under "Prepare your account" 9/10/2012</p>

 -->

1. Contactez l’assistance clientèle d’Adobe et demandez-lui d’activer Secure Testing sur votre compte.
1. Dans Adobe Dynamic Media Classic, sur la barre de navigation générale, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de la publication]** > **[!UICONTROL Serveur d’images]**.
1. Sur la page Publication du serveur d’images, dans la liste déroulante **[!UICONTROL `Publish Context`]**, sélectionnez **[!UICONTROL Test de l’hébergeur d’images]**.
1. Pour l’option Filtre d’adresse client, sélectionnez **[!UICONTROL Ajouter]**.
1. Cochez la case pour que l’adresse soit activée (activée), puis saisissez une adresse IP et un masque de réseau dans les champs de texte respectifs.

   >[!NOTE]
   >
   >Si vous ajoutez une seule adresse IP et un masque de réseau, cette adresse peut effectuer des appels de ressources. Cependant, les autres adresses IP et masques de réseau que vous ajoutez ne sont pas autorisés à effectuer des appels de ressources. Ainsi, envisagez de désactiver (désactiver) la case à cocher de l’étape ci-dessus pour désactiver la possibilité de spécifier une adresse IP et un masque de réseau. Cela permet à *toutes* les adresses IP d’effectuer des appels de ressources, et elles s’affichent toutes.

1. Effectuez l’une des opérations suivantes :
   * Répétez les deux étapes précédentes si vous devez ajouter d’autres adresses IP.
   * Passez à l’étape suivante.
1. Dans le coin inférieur gauche de la page Publication du serveur d’images, sélectionnez **[!UICONTROL Enregistrer]**
1. Chargez les images souhaitées dans votre compte Adobe Dynamic Media Classic.

   Voir [Charger des fichiers](uploading-files.md#uploading_files).

1. Assurez-vous que certaines des images sont marquées pour publication et d’autres ne le sont pas, puis soumettez la tâche de publication.

   Voir [Publication de fichiers](publishing-files.md#publishing_files).

1. Déterminez le nom de votre service Secure Testing en accédant à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Paramètres généraux]**.
1. A la page Paramètres généraux de l’application, sous le groupe Serveurs, recherchez le nom indiqué à droite de **[!UICONTROL Test de contexte de publication du nom du serveur]**.

Contactez l’Assistance Adobe si le nom du serveur est manquant ou si les URL du serveur ne fonctionnent pas.

### Préparation des variations de site Web

Deux variations d’un site Web qui lie les fichiers publiés et non publiés sont nécessaires :

* Version publique : liez les ressources à l’aide de la syntaxe traditionnelle de l’URL Adobe Dynamic Media Classic.
* Version intermédiaire : liez les ressources en utilisant la même syntaxe, mais avec le nom du site de test sécurisé.

### Exécution des tests

Effectuez les tests suivants :

1. Vérifiez si les fichiers sont visibles de l’intérieur de votre réseau d’entreprise.

   Depuis le réseau d’entreprise identifié par la plage d’adresses IP définie précédemment, la version intermédiaire du site web affiche toutes les images, qu’elles soient marquées pour la publication ou non. Ainsi, vous pouvez tester sans rendre accidentellement les images disponibles avant l’approbation de l’aperçu ou le lancement du produit.

   Vérifiez que la version publique de votre site affiche les ressources publiées comme vous l’avez déjà fait avec Adobe Dynamic Media Classic.

1. Depuis l’extérieur de votre réseau d’entreprise, vérifiez que les ressources non publiées (c’est-à-dire non marquées pour la publication) sont protégées contre l’accès par des tiers.

   Accédez à votre réseau depuis l’extérieur (depuis votre ordinateur personnel ou via une connexion 3G, par exemple), puis vérifiez que la version publique du site affiche toutes les ressources publiées, mais aucun contenu dépublié.

   Confirmez que la version intermédiaire n’affiche aucun fichier, car vous accédez au service Secure Testing à partir d’une adresse IP non approuvée.
