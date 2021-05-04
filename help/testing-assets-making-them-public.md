---
title: Test des fichiers avant de les rendre publics
description: Découvrez comment tester des fichiers avant de les rendre publics.
uuid: 5e8f3bec-6cf1-408e-8ea1-aebde0012a70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: 52fadf99-7d11-46f7-8483-a9f87ffc2f67
feature: Dynamic Media Classic,Gestion des ressources
role: Business Practitioner
exl-id: fd78d535-391e-43eb-a8aa-25fa6c2885cb
translation-type: tm+mt
source-git-commit: 1beb30b9eda4487dcd549034906079dee0b3149a
workflow-type: tm+mt
source-wordcount: '1027'
ht-degree: 37%

---

# Test des fichiers avant de les rendre publics {#testing-assets-before-making-them-public}

Secure Testing vous permet de définir un environnement de test sécurisé et de créer une solution B2B robuste, basée sur un ensemble configurable d’adresses et de plages IP. Cette fonctionnalité vous permet d’associer vos déploiements Dynamic Media Classic à l’architecture de votre gestion de contenu et de votre système d’entreprise.

Avec Secure Testing, vous pouvez prévisualiser la version intermédiaire du site Web avec le contenu non publié.

Si vous le souhaitez, créez un environnement d’évaluation plutôt que de rendre les ressources publiques pour les raisons suivantes :

* Aperçu des sites Web avant lancement public (site Web intermédiaire).
* Servir les fichiers qui nécessitent un accès restreint, tels que les catalogues électroniques qui affichent des prix dans une application Web B2B.
* Utiliser des fichiers se trouvant derrière un pare-feu dans le cadre du système de gestion des informations sur le produit, d’une application de service d’assistance à la clientèle, d’un site de formation, etc.

>[!NOTE]
>
>Secure Testing n’affecte pas l’accès à Dynamic Media Classic. La sécurité de Dynamic Media Classic reste cohérente et requiert les informations d’identification habituelles pour accéder à Dynamic Media Classic et aux services Web connexes.

## Comment fonctionne Secure Testing {#how-secure-testing-works}

La plupart des entreprises gèrent leur Internet derrière un pare-feu. L’accès à Internet est possible via certaines routes et généralement via une plage limitée d’adresses IP publiques.

Sur votre réseau d’entreprise, vous pouvez déterminer votre adresse IP publique à l’aide de sites Web tels que https://whatismyip.com ou demander ces informations à votre service informatique d’entreprise.

Avec Secure Testing, Dynamic Media Classic établit un serveur d’images dédié pour les environnements d’évaluation ou les applications internes. Toute requête sur ce serveur vérifie l’adresse IP d’origine. Si la requête entrante n’est pas incluse dans la liste approuvée des adresses IP, une réponse d’échec est renvoyée. L’administrateur de la Société Dynamic Media Classic configure la liste approuvée des adresses IP pour l’environnement Secure Testing de leur société.

L’emplacement de la requête d’origine devant être confirmé, le trafic du service Secure Testing n’est pas acheminé via un réseau de distribution de contenu tel que le trafic public du serveur Dynamic Media Image Server. Les requêtes envoyées au service Secure Testing présentent une latence légèrement plus élevée que les serveurs Dynamic Media Image Server publics.

Les fichiers non publiés sont immédiatement disponibles à partir des services Secure Testing, sans avoir besoin d’être publiés. Ainsi, vous pouvez exécuter une prévisualisation avant que les fichiers ne soient publiés sur leur serveur d’images accessible au public.

>[!NOTE]
>
>Les services Secure Testing utilisent le serveur de catalogue configuré avec un contexte de publication interne. Par conséquent, si votre société est configurée pour publier sur Secure Testing, les ressources transférées dans Dynamic Media Classic deviennent immédiatement disponibles sur les services Secure Testing. Cette fonctionnalité est vraie, que les ressources soient marquées pour publication au moment du téléchargement ou non.

Les services Secure Testing prennent actuellement en charge les types et fonctionnalités de ressources suivants :

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Added videos to list below 9/11/2012. Moved “Render Server requests” from unsupported to supported, listed below on 3/15/2016 as per email from Cynthia March 11, 2016)</p>

 -->

* Images.
* Vignettes (demandes de seveur Render Server).
* Demandes Render Server (prises en charge, mais doivent être demandées explicitement par le client).
* Visionneuses, dont visionneuses d’images, catalogue électronique, visionneuses de rendu et de supports.
* Visionneuses de médias enrichis Dynamic Media Classic standard.
* Pages JSP à la demande Dynamic Media Classic.
* Contenu statique, par exemple fichiers PDF et vidéos servies progressivement.
* Diffusion vidéo en flux continu HTTP.
* Diffusion vidéo progressive.

Les types de fichiers suivants et les fonctionnalités suivantes ne sont actuellement pas pris en charge :

* Diffusion vidéo en flux continu RTMP
* Services UGC
* Impression en ligne
* Recherche Dynamic Media Classic Info ou catalogue électronique

## Test du service Secure Testing {#testing-the-secure-testing-service}

Testez le service Secure Testing pour vous assurer qu’il fonctionne comme prévu.

<!-- >[!NOTE]
>
>*If you do not mention any IPs under **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]** > **[!UICONTROL Test Image Service]*** - If you add an IP only, that IP is able to call the assets and no other IP are allowed to make the calls. As long there is no IP mentioned under that section, all IPs are allowed to make the calls for the assets, and they show up. -->

### Préparation de votre compte

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under “Prepare your account” 9/10/2012</p>

 -->

1. Contactez le service à la clientèle d’Adobe et demandez-lui d’activer Secure Testing sur votre compte.
1. Dans Dynamic Media Classic, sur la barre de navigation globale, cliquez sur **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de la publication]** > **[!UICONTROL Image Server]**.
1. Sur la page Publication sur hébergeur d’images, dans la liste déroulante **[!UICONTROL Contexte de publication]**, sélectionnez **[!UICONTROL Test Image Serving]**.
1. Pour l’option Filtre d’adresse client, cliquez sur **[!UICONTROL Ajouter]**.
1. Activez la case à cocher pour que l’adresse soit activée, puis entrez une adresse IP et un masque de réseau dans les champs de texte respectifs.

   >[!NOTE]
   >
   >Si vous ajoutez une seule adresse IP et un seul masque de réseau, cette adresse peut effectuer des appels de ressources. Toutefois, les autres adresses IP et masques réseau que vous ajoutez ne sont pas autorisés à effectuer des appels de ressources. Par conséquent, pensez à désactiver (désactiver) la case à cocher de l’étape ci-dessus pour désactiver la possibilité de spécifier une adresse IP et un masque de réseau. Cela permet à *toutes les* adresses IP de passer des appels de ressources, et elles s&#39;affichent toutes.

1. Effectuez l’une des opérations suivantes :
   * Répétez les deux étapes précédentes si vous devez ajouter d’autres adresses IP.
   * Passez à l’étape suivante.
1. Dans le coin inférieur gauche de la page Publication sur hébergeur d’images, cliquez sur **[!UICONTROL Enregistrer]**.
1. Téléchargez les images de votre choix sur votre compte Dynamic Media Classic.

   Voir [Transfert de fichiers](uploading-files.md#uploading_files).

1. Assurez-vous qu’une partie des images sont marquées pour publication et qu’une autre partie des images ne le sont pas, puis envoyez la tâche de publication.

   Voir [Publication](publishing-files.md#publishing_files).

1. Déterminez le nom de votre service Secure Testing en cliquant sur **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Paramètres généraux]**.
1. A la page Paramètres généraux de l’application, sous le groupe Serveurs, recherchez le nom indiqué à droite de **[!UICONTROL Test de contexte de publication du nom du serveur]**.

Contactez le service à l’Adobe si le nom du serveur est absent ou si les URL vers le serveur ne fonctionnent pas.

### Préparation des variations de site Web

Deux variations d’un site Web qui lie les fichiers publiés et non publiés sont nécessaires :

* Version publique - Liez des fichiers à l’aide de votre syntaxe d’URL classique Dynamic Media Classic.
* Version d’évaluation : liez les fichiers en utilisant la même syntaxe mais avec le nom du site Secure Testing.

### Exécution des tests

Effectuez les tests suivants :

1. Vérifiez si les fichiers sont visibles de l’intérieur de votre réseau d’entreprise.

   Depuis le réseau d’entreprise identifié par la plage d’adresses IP précédemment définie, la version intermédiaire du site Web affiche toutes les images, marquées ou non pour publication. Ainsi, vous pouvez tester sans rendre accidentellement les images disponibles avant l’approbation de la prévisualisation ou le lancement du produit.

   Confirmez que la version publique de votre site affiche les fichiers publiés comme vous l’avez vu précédemment avec Dynamic Media Classic.

1. Depuis l’extérieur de votre réseau d’entreprise, vérifiez que les fichiers non publiés (c’est-à-dire, non marqués pour publication) sont protégés contre l’accès de tiers.

   Accédez votre réseau depuis l’extérieur (par exemple, depuis votre ordinateur personnel ou via une connexion 3G), puis vérifiez que la version publique du site affiche tous les fichiers publiés mais pas le contenu non publié.

   Confirmez que la version intermédiaire n’affiche aucun fichier, car vous accédez au service Secure Testing à partir d’une adresse IP non approuvée.
