---
title: Test des fichiers avant de les rendre publics
seo-title: Test des fichiers avant de les rendre publics
description: 'null'
seo-description: Découvrez comment tester des fichiers avant de les rendre publics.
uuid: 5 e 8 f 3 bec -6 cf 1-408 e -8 ea 1-aebde 0012 a 70
contentOwner: admin
content-type: référence
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/upload_ and_ publish_ assets
discoiquuid: 52 fadf 99-7 d 11-46 f 7-8483-a 9 f 87 ffc 2 f 67
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Test des fichiers avant de les rendre publics {#testing-assets-before-making-them-public}

Secure Testing vous permet de définir un environnement de test sécurisé et de créer des solutions B2B solides, basées sur un ensemble configurable de plages et d’adresses IP. Cette fonctionnalité vous permet de faire correspondre vos déploiements Dynamic Media Classic avec l'architecture de votre gestion de contenu et de votre plate-forme de commerce.

Avec Secure Testing, vous pouvez prévisualiser la version intermédiaire du site Web avec le contenu non publié.

Il se peut que vous préfériez créer un environnement intermédiaire plutôt que de publier des fichiers pour les raisons suivantes :

* Aperçu des sites Web avant lancement public (site Web intermédiaire).
* Servir les fichiers qui nécessitent un accès restreint, tels que les catalogues électroniques qui affichent des prix dans une application Web B2B.
* Utiliser des fichiers se trouvant derrière un pare-feu dans le cadre du système de gestion des informations sur le produit, d’une application de service d’assistance à la clientèle, d’un site de formation, etc.

>[!NOTE]
>
>Secure Testing n’a pas d’incidence sur l’accès au Scene7 Publishing System. La sécurité de SPS reste cohérente et requiert les informations d’identification habituelles pour accéder à SPS et aux services Web associés.

## Comment fonctionne Secure Testing {#how-secure-testing-works}

La plupart des entreprises gèrent leur Internet derrière un pare-feu. L’accès à Internet est possible via certaines routes et généralement via une plage limitée d’adresses IP publiques.

Sur votre réseau d'entreprise, vous pouvez déterminer votre adresse IP publique à l'aide de sites Web tels que https://whatismyip.com ou demander ces informations auprès de votre organisation informatique.

Avec Secure Testing, Dynamic Media Classic établit un serveur d'images dédié pour les environnements d'évaluation ou les applications internes. Toute requête sur ce serveur vérifie l’adresse IP d’origine. Si la requête entrante n’est pas incluse dans la liste approuvée des adresses IP, une réponse d’échec est renvoyée. L'administrateur d'entreprise Dynamic Media Classic configure la liste approuvée des adresses IP pour l'environnement Secure Testing de leur entreprise.

Puisque l'emplacement de la requête d'origine doit être confirmé, le trafic du service Secure Testing n'est pas acheminé via un réseau de distribution de contenu tel que le trafic Public Dynamic Media Image Server. Les requêtes au service Secure Testing peuvent présenter une latence légèrement plus élevée par rapport aux serveurs d'images dynamiques publiques.

Les fichiers non publiés sont immédiatement disponibles à partir des services Secure Testing, sans avoir besoin d’être publiés. Cela vous permet d’effectuer un aperçu avant que les fichiers ne soient publiés dans leur serveur d’images destiné au public.

***remarque**: Les services Secure Testing tirent parti du serveur de catalogue configuré avec un contexte de publication interne. Par conséquent, si votre entreprise a été configurée pour publier sur Secure Testing, n’oubliez pas que les fichiers transférés vers Scene7 Publishing System deviennent immédiatement disponibles dans les services Secure Testing. Cela est vrai pour les fichiers marqués ou non pour publication au moment du transfert.*

Les services Secure Testing prennent actuellement en charge les types de ressource et les fonctionnalités suivants :

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Added videos to list below 9/11/2012. Moved “Render Server requests” from unsupported to supported, listed below on 3/15/2016 as per email from Cynthia March 11, 2016)</p>

 -->

* Images.
* Vignettes (demandes de seveur Render Server).
* Demandes de serveur de rendu (pris en charge, mais doivent être explicitement demandées par le client).
* Visionneuses, dont visionneuses d’images, catalogue électronique, visionneuses de rendu et de supports.
* Visionneuses de médias enrichis standard Media Classic.
* Pages JSP Dynamic Media Classic ondemand.
* Contenu statique, par exemple fichiers PDF et vidéos servies progressivement.
* Diffusion vidéo en flux continu HTTP.
* Diffusion vidéo progressive.

Les types de fichiers suivants et les fonctionnalités suivantes ne sont actuellement pas pris en charge :

* Diffusion vidéo en flux continu RTMP
* Services UGC
* Impression en ligne
* Informations sur le contenu multimédia dynamique ou recherche de catalogue électronique

## Test du service Secure Testing {#testing-the-secure-testing-service}

Vous devez tester le service Secure Testing pour vous assurer qu’il fonctionne correctement.

**Préparation de votre compte**

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under “Prepare your account” 9/10/2012</p>

 -->

1. Contactez le support technique et demandez qu’il active Secure Testing dans votre compte.
1. Dans Scene7 Publishing System, cliquez sur **Configuration** &gt; **Configuration personnelle** &gt; **Image Server**.
1. Dans la liste déroulante Contexte de publication de la page Publication sur hébergeur d’images, sélectionnez **Test de l'hébergeur d'images**.
1. Pour l’option Filtre d’adresse client, cliquez sur **Ajouter**.
1. Cochez la case permettant d’activer l’adresse, puis saisissez une adresse IP et un masque de sous-réseau dans les champs correspondants.
1. Répétez les deux étapes précédentes pour ajouter d’autres adresses IP. Sinon, passez à l’étape suivante.
1. En bas à gauche de la page Publication sur hébergeur d’images, cliquez sur **Enregistrer**. 
1. Transférez les images souhaitées vers votre compte Scene7 Publishing System.

   Voir [Transfert de fichiers](uploading-files.md#uploading_files).

1. Assurez-vous qu’une partie des images sont marquées pour publication et qu’une autre partie des images ne le sont pas, puis envoyez la tâche de publication.

   Voir [Publication](publishing-files.md#publishing_files).

1. Déterminez le nom de votre service Secure Testing en cliquant sur **Configuration** &gt; **Configuration de l’application** &gt; **Paramètres généraux**.
1. A la page Paramètres généraux de l’application, sous le groupe Serveurs, recherchez le nom indiqué à droite de **Test de contexte de publication du nom du serveur**.

Contactez l’assistance technique si le nom de serveur est manquant ou si des URL vers le serveur ne fonctionnent pas.

**Préparation des variations de site Web**

Deux variations d’un site Web qui lie les fichiers publiés et non publiés sont nécessaires :

* Version publique : Liaison de fichiers à l'aide de la syntaxe d'URL classique de Media Classic classique
* Version intermédiaire : liez les fichiers en utilisant la même syntaxe mais avec le nom du site Secure Testing

**Exécution des tests**

Effectuez les tests suivants :

1. Vérifiez si les fichiers sont visibles de l’intérieur de votre réseau d’entreprise.

   Depuis le réseau d’entreprise identifié par la plage d’adresses IP précédemment définie, la version intermédiaire du site Web doit afficher toutes les images, qu’elles soient marquées pour publication ou non. Cela vous permet de tester sans rendre les images accidentellement disponibles avant approbation ou lancement du produit.

   Vérifiez que la version publique de votre site affiche les fichiers publiés comme précédemment avec Dynamic Media Classic.

1. Depuis l’extérieur de votre réseau d’entreprise, vérifiez que les fichiers non publiés (c’est-à-dire, non marqués pour publication) sont protégés contre l’accès de tiers.

   Accédez votre réseau depuis l’extérieur (par exemple, depuis votre ordinateur personnel ou via une connexion 3G), puis vérifiez que la version publique du site affiche tous les fichiers publiés mais pas le contenu non publié.

   Confirmez que la version intermédiaire n’affiche aucun fichier, car vous accédez au service Secure Testing à partir d’une adresse IP non approuvée.

