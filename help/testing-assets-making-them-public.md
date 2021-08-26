---
title: Test des fichiers avant de les rendre publics
description: Découvrez comment tester les ressources avant de les rendre publiques.
uuid: 5e8f3bec-6cf1-408e-8ea1-aebde0012a70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: 52fadf99-7d11-46f7-8483-a9f87ffc2f67
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: fd78d535-391e-43eb-a8aa-25fa6c2885cb
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '1036'
ht-degree: 37%

---

# Test des fichiers avant de les rendre publics {#testing-assets-before-making-them-public}

Le test sécurisé vous permet de définir un environnement de test sécurisé et de créer une solution B2B robuste, basée sur un ensemble configurable d’adresses IP et de plages. Cette fonctionnalité vous permet de faire correspondre vos déploiements Dynamic Media Classic Adobe à l’architecture de votre système de gestion de contenu et de fonctionnement.

Avec Secure Testing, vous pouvez prévisualiser la version intermédiaire du site Web avec le contenu non publié.

Si vous le souhaitez, créez un environnement d’évaluation plutôt que de rendre les ressources publiques disponibles pour les raisons suivantes :

* Aperçu des sites Web avant lancement public (site Web intermédiaire).
* Servir les fichiers qui nécessitent un accès restreint, tels que les catalogues électroniques qui affichent des prix dans une application Web B2B.
* Utiliser des fichiers se trouvant derrière un pare-feu dans le cadre du système de gestion des informations sur le produit, d’une application de service d’assistance à la clientèle, d’un site de formation, etc.

>[!NOTE]
>
>Le test sécurisé n’affecte pas l’accès à Adobe Dynamic Media Classic. La sécurité d’Adobe Dynamic Media Classic reste cohérente et nécessite les informations d’identification habituelles pour accéder à Adobe Dynamic Media Classic et aux services Web associés.

## Comment fonctionne Secure Testing {#how-secure-testing-works}

La plupart des entreprises gèrent leur Internet derrière un pare-feu. L’accès à Internet est possible via certaines routes et généralement via une plage limitée d’adresses IP publiques.

À partir du réseau de votre entreprise, vous pouvez déterminer votre adresse IP publique à l’aide de sites web tels que https://whatismyip.com ou demander ces informations à votre service informatique d’entreprise.

Avec le test sécurisé, Adobe Dynamic Media Classic établit un serveur d’images dédié pour les environnements d’évaluation ou les applications internes. Toute requête sur ce serveur vérifie l’adresse IP d’origine. Si la requête entrante n’est pas incluse dans la liste approuvée des adresses IP, une réponse d’échec est renvoyée. L’administrateur d’entreprise Adobe Dynamic Media Classic configure la liste approuvée des adresses IP pour l’environnement de test sécurisé de l’entreprise.

L’emplacement de la requête d’origine devant être confirmé, le trafic du service Secure Testing n’est pas acheminé via un réseau de distribution de contenu tel que le trafic du serveur d’images Dynamic Media public. Les demandes au service Secure Testing présentent une latence légèrement plus élevée que les serveurs d’images Dynamic Media publics.

Les fichiers non publiés sont immédiatement disponibles à partir des services Secure Testing, sans avoir besoin d’être publiés. Ainsi, vous pouvez exécuter un aperçu avant que les ressources ne soient publiées sur leur serveur d’images public.

>[!NOTE]
>
>Les services de test sécurisé utilisent le serveur de catalogue configuré avec un contexte de publication interne. Par conséquent, si votre entreprise est configurée pour publier vers le test sécurisé, toutes les ressources chargées dans Adobe Dynamic Media Classic sont immédiatement disponibles sur les services de test sécurisé. Cette fonctionnalité est vraie que les ressources soient marquées pour publication au moment du téléchargement ou non.

Les services Secure Testing prennent actuellement en charge les types et fonctionnalités de ressources suivants :

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Added videos to list below 9/11/2012. Moved “Render Server requests” from unsupported to supported, listed below on 3/15/2016 as per email from Cynthia March 11, 2016)</p>

 -->

* Images.
* Vignettes (demandes de seveur Render Server).
* Requêtes de serveur de rendu (prises en charge, mais doivent être demandées explicitement par le client).
* Visionneuses, dont visionneuses d’images, catalogue électronique, visionneuses de rendu et de supports.
* Visionneuses de médias riches Dynamic Media Classic standard Adobe.
* Adobe des pages JSP Dynamic Media Classic On Demand.
* Contenu statique, par exemple fichiers PDF et vidéos servies progressivement.
* Diffusion vidéo en flux continu HTTP.
* Diffusion vidéo progressive.

Les types de fichiers suivants et les fonctionnalités suivantes ne sont actuellement pas pris en charge :

* Diffusion vidéo en flux continu RTMP
* Services UGC
* Impression en ligne
* Adobe Dynamic Media Classic Info ou recherche eCatalog

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

1. Contactez l’assistance clientèle d’Adobe et demandez-lui d’activer le test sécurisé sur votre compte.
1. Dans Adobe Dynamic Media Classic, dans la barre de navigation globale, cliquez sur **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de la publication]** > **[!UICONTROL Serveur d’images]**.
1. Sur la page Publication sur hébergeur d’images, dans la liste déroulante **[!UICONTROL Contexte de publication]**, sélectionnez **[!UICONTROL Test de la diffusion d’images]**.
1. Pour l’option Filtre d’adresse client, cliquez sur **[!UICONTROL Ajouter]**.
1. Cochez la case pour activer l’adresse, puis saisissez une adresse IP et un masque de réseau dans les champs de texte respectifs.

   >[!NOTE]
   >
   >Si vous ajoutez une seule adresse IP et un seul masque de réseau, cette adresse peut effectuer des appels de ressources. Toutefois, les autres adresses IP et masques réseau que vous ajoutez ne sont pas autorisées à effectuer des appels de ressources. Par conséquent, envisagez de désactiver (désactiver) la case à cocher à l’étape ci-dessus pour désactiver la possibilité de spécifier une adresse IP et un masque de réseau. Cela permet de *toutes les* adresses IP de lancer des appels de ressources, et elles s’affichent toutes.

1. Effectuez l’une des opérations suivantes :
   * Répétez les deux étapes précédentes si vous devez ajouter d’autres adresses IP.
   * Passez à l’étape suivante.
1. En bas à gauche de la page Publication sur hébergeur d’images, cliquez sur **[!UICONTROL Enregistrer]**
1. Chargez les images souhaitées dans votre compte Dynamic Media Classic Adobe.

   Voir [Transfert de fichiers](uploading-files.md#uploading_files).

1. Assurez-vous qu’une partie des images sont marquées pour publication et qu’une autre partie des images ne le sont pas, puis envoyez la tâche de publication.

   Voir [Publication](publishing-files.md#publishing_files).

1. Déterminez le nom de votre service Secure Testing en cliquant sur **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Paramètres généraux]**.
1. A la page Paramètres généraux de l’application, sous le groupe Serveurs, recherchez le nom indiqué à droite de **[!UICONTROL Test de contexte de publication du nom du serveur]**.

Contactez le service à l’Adobe si le nom du serveur est manquant ou si les URL vers le serveur ne fonctionnent pas.

### Préparation des variations de site Web

Deux variations d’un site Web qui lie les fichiers publiés et non publiés sont nécessaires :

* Version publique - Liez des ressources à l’aide de votre syntaxe d’URL classique Adobe Dynamic Media Classic.
* Version intermédiaire : liez les ressources en utilisant la même syntaxe mais avec le nom du site de test sécurisé.

### Exécution des tests

Effectuez les tests suivants :

1. Vérifiez si les fichiers sont visibles de l’intérieur de votre réseau d’entreprise.

   Depuis le réseau d’entreprise identifié par la plage d’adresses IP définie précédemment, la version intermédiaire du site web affiche toutes les images, qu’elles soient marquées pour publication ou non. Ainsi, vous pouvez tester sans rendre les images disponibles accidentellement avant l’approbation de l’aperçu ou le lancement du produit.

   Vérifiez que la version publique de votre site affiche les ressources publiées comme vous l’avez déjà fait avec Adobe Dynamic Media Classic.

1. Depuis l’extérieur de votre réseau d’entreprise, vérifiez que les fichiers non publiés (c’est-à-dire, non marqués pour publication) sont protégés contre l’accès de tiers.

   Accédez votre réseau depuis l’extérieur (par exemple, depuis votre ordinateur personnel ou via une connexion 3G), puis vérifiez que la version publique du site affiche tous les fichiers publiés mais pas le contenu non publié.

   Confirmez que la version intermédiaire n’affiche aucun fichier, car vous accédez au service Secure Testing à partir d’une adresse IP non approuvée.
