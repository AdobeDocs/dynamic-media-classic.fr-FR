---
title: Test des fichiers avant de les rendre publics
seo-title: Test des fichiers avant de les rendre publics
description: 'null'
seo-description: Découvrez comment tester des fichiers avant de les rendre publics.
uuid: 5e8f3bec-6cf1-408e-8ea1-aebde0012a70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: 52fadf99-7d11-46f7-8483-a9f87ffc2f67
translation-type: tm+mt
source-git-commit: 03ca030531f8d9fa0a6944bd5050e2c865adf5f5
workflow-type: tm+mt
source-wordcount: '1103'
ht-degree: 54%

---


# Test des fichiers avant de les rendre publics {#testing-assets-before-making-them-public}

Secure Testing vous permet de définir un environnement de test sécurisé et de créer des solutions B2B solides, basées sur un ensemble configurable de plages et d’adresses IP. Cette fonctionnalité vous permet de faire correspondre vos déploiements de Dynamic Media Classic avec l’architecture de votre gestion de contenu et de votre plateforme de commerce.

Avec Secure Testing, vous pouvez prévisualiser la version intermédiaire du site Web avec le contenu non publié.

Il se peut que vous préfériez créer un environnement intermédiaire plutôt que de publier des fichiers pour les raisons suivantes :

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

L’emplacement de la demande d’origine devant être confirmé, le trafic du service Secure Testing n’est pas acheminé par un réseau de distribution de contenu tel que le trafic public du serveur d’images de médias dynamiques. Les requêtes envoyées au service Secure Testing peuvent présenter une latence légèrement plus élevée que les serveurs d’images de médias dynamiques publics.

Les fichiers non publiés sont immédiatement disponibles à partir des services Secure Testing, sans avoir besoin d’être publiés. Cela vous permet d’effectuer un aperçu avant que les fichiers ne soient publiés dans leur serveur d’images destiné au public.

***remarque **: Les services Secure Testing tirent parti du serveur de catalogue configuré avec un contexte de publication interne. Par conséquent, si votre société est configurée pour publier sur Secure Testing, n’oubliez pas que tout fichier téléchargé dans Dynamic Media Classic devient immédiatement disponible sur les services Secure Testing. Cela est vrai pour les fichiers marqués ou non pour publication au moment du transfert.*

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
* Visionneuses de supports enrichis Standard Dynamic Media Classic.
* Pages JSP à la demande de Dynamic Media Classic.
* Contenu statique, par exemple fichiers PDF et vidéos servies progressivement.
* Diffusion vidéo en flux continu HTTP.
* Diffusion vidéo progressive.

Les types de fichiers suivants et les fonctionnalités suivantes ne sont actuellement pas pris en charge :

* Diffusion vidéo en flux continu RTMP
* Services UGC
* Impression en ligne
* Recherche d’informations ou de catalogue électronique dans Contenu multimédia dynamique

## Test du service Secure Testing {#testing-the-secure-testing-service}

Vous devez tester le service Secure Testing pour vous assurer qu’il fonctionne correctement.

Remarque : Si vous ne mentionnez aucune adresse IP sous Configuration > Configuration de la publication > Image Server > Tester Image Server si vous ajoutez une adresse IP uniquement, cette adresse IP pourra appeler les ressources et aucune autre adresse IP ne sera autorisée à effectuer les appels. Tant qu&#39;aucune IP n&#39;est mentionnée dans cette section, toutes les adresses IP sont autorisées à lancer des appels pour les ressources, et elles s&#39;afficheront.

**Préparation de votre compte**

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under “Prepare your account” 9/10/2012</p>

 -->

1. Contactez le support technique et demandez qu’il active Secure Testing dans votre compte.
1. Dans Dynamic Media Classic, cliquez sur **Configuration** > Configuration **de la** publication > Serveur **d’** images.
1. Dans la liste déroulante Contexte de publication de la page Publication sur hébergeur d’images, sélectionnez **Test de l&#39;hébergeur d&#39;images**.
1. Pour l’option Filtre d’adresse client, cliquez sur **Ajouter**.
1. Cochez la case permettant d’activer l’adresse, puis saisissez une adresse IP et un masque de sous-réseau dans les champs correspondants.

   >[!NOTE]
   >
   >Si vous ajoutez une seule adresse IP et un seul masque de réseau, cette adresse peut effectuer des appels de ressources. Toutefois, les autres adresses IP et masques réseau que vous ajoutez ne sont pas autorisés à effectuer des appels de ressources. Par conséquent, vous pouvez envisager de désactiver (désactiver) la case à cocher de l’étape ci-dessus pour désactiver la possibilité de spécifier une adresse IP et un masque réseau. Cela permet à *toutes les* adresses IP de passer des appels de ressources, et elles apparaîtront toutes.

1. Effectuez l’une des opérations suivantes :
   * Répétez les deux étapes précédentes pour ajouter d’autres adresses IP.
   * Passez à l’étape suivante.
1. En bas à gauche de la page Publication sur hébergeur d’images, cliquez sur **Enregistrer**. 
1. Téléchargez les images de votre choix dans votre compte Dynamic Media Classic.

   Voir [Transfert de fichiers](uploading-files.md#uploading_files).

1. Assurez-vous qu’une partie des images sont marquées pour publication et qu’une autre partie des images ne le sont pas, puis envoyez la tâche de publication.

   Voir [Publication](publishing-files.md#publishing_files).

1. Déterminez le nom de votre service Secure Testing en cliquant sur **Configuration** > **Configuration de l’application** > **Paramètres généraux**.
1. A la page Paramètres généraux de l’application, sous le groupe Serveurs, recherchez le nom indiqué à droite de **Test de contexte de publication du nom du serveur**.

Contactez le service à l’Adobe si le nom du serveur est absent ou si les URL vers le serveur ne fonctionnent pas.

**Préparation des variations de site Web**

Deux variations d’un site Web qui lie les fichiers publiés et non publiés sont nécessaires :

* Version publique - Liez des fichiers à l’aide de la syntaxe d’URL classique de Contenu multimédia dynamique.
* Version d’évaluation : liez les fichiers en utilisant la même syntaxe mais avec le nom du site Secure Testing.

**Exécution des tests**

Effectuez les tests suivants :

1. Vérifiez si les fichiers sont visibles de l’intérieur de votre réseau d’entreprise.

   Depuis le réseau d’entreprise identifié par la plage d’adresses IP précédemment définie, la version intermédiaire du site Web doit afficher toutes les images, qu’elles soient marquées pour publication ou non. Cela vous permet de tester sans rendre les images accidentellement disponibles avant approbation ou lancement du produit.

   Vérifiez que la version publique de votre site affiche les fichiers publiés comme vous l’avez déjà fait avec Dynamic Media Classic.

1. Depuis l’extérieur de votre réseau d’entreprise, vérifiez que les fichiers non publiés (c’est-à-dire, non marqués pour publication) sont protégés contre l’accès de tiers.

   Accédez votre réseau depuis l’extérieur (par exemple, depuis votre ordinateur personnel ou via une connexion 3G), puis vérifiez que la version publique du site affiche tous les fichiers publiés mais pas le contenu non publié.

   Confirmez que la version intermédiaire n’affiche aucun fichier, car vous accédez au service Secure Testing à partir d’une adresse IP non approuvée.

