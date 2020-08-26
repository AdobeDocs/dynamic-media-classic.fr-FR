---
title: Configuration de l’administration
seo-title: Configuration de l’administration
description: 'null'
seo-description: Découvrez comment configurer la zone d’administration de Dynamic Media Classic.
uuid: 16ba9fed-b5c6-4991-83b3-8d7d7129013a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 3c9ee4ec-dd37-498d-98d6-1339b80177ff
translation-type: tm+mt
source-git-commit: 1ee586fab6a4e10a946848fd079438ade38490d9
workflow-type: tm+mt
source-wordcount: '1945'
ht-degree: 64%

---


<!-- UPDATE TOPIC AFTER DECEMBER 31, 2020!!!! -->

# Configuration de l’administration{#administration-setup}

Les écrans Configuration de l’administration permettent d’administrer les utilisateurs de Dynamic Media Classic. Utilisez ces écrans pour permettre aux utilisateurs de travailler dans Dynamic Media Classic et de communiquer par e-mail avec les utilisateurs.

1. To access Administration Setup options, click **Setup** > **Personal Setup** > **Administration Setup**.

## Administration utilisateur {#user-administration}

Tous les utilisateurs de Dynamic Media Classic se voient attribuer un rôle qui détermine leurs privilèges et droits d’accès aux fonctionnalités de Dynamic Media Classic. Les administrateurs définissent les différents rôles et responsabilités pour les entreprises auxquelles ils sont affectés.

En règle générale, Dynamic Media Classic configure le premier ensemble de sociétés et affecte un administrateur de société. L’administrateur de société configure et administre ensuite les utilisateurs de Dynamic Media Classic.

Dynamic Media Classic prend en charge plusieurs rôles d’utilisateur. Ces rôles peuvent accéder aux sociétés configurées pour Dynamic Media Classic :

<!-- **Adobe Dynamic Media Classic Administrator** Can view and administer all features in Dynamic Media Classic, as well as set up companies and add administrators and users. -->

**adobe de l’utilisateur** Dynamic Media Classic peut accéder aux sociétés auxquelles ils ont été affectés ; ne peuvent pas exercer de fonctions administratives.

**adobe Dynamic Media Classic Société Admin** peut vue et administrer uniquement leurs propres sociétés. Il peut également remplir toutes les fonctions d’administration, notamment l’ajout d’administrateurs et d’utilisateurs. Un administrateur de Société peut ajouter un utilisateur aux comptes d’administration de société DMC. (Ce rôle est le rôle utilisateur par défaut.)

Après avoir ajouté un utilisateur, Dynamic Media Classic lui envoie un e-mail de bienvenue. Le message comprend un mot de passe et l’URL de Dynamic Media Classic.

### Ajout d’un utilisateur ou d’un administrateur {#adding-a-user-or-administrator}

1. Cliquez sur Configuration > Configuration de l’application > Configuration de l’administration > Administration utilisateur.
1. Cliquez sur Ajouter.
1. Entrez le nom et l’adresse électronique de l’utilisateur ou de l’administrateur à ajouter, puis cliquez sur Suivant.

   >[!NOTE]
   >
   >le caractère apostrophe (’) n’est pas autorisé dans les adresses électroniques.

1. Choisissez une option de rôle pour attribuer un rôle à l’utilisateur.

   Voir Rôles utilisateur et privilèges [Dynamic Media Classic](administration-setup.md#user_administration).

1. Sélectionnez un nom de société pour ajouter un utilisateur à une entreprise.
1. Si vous souhaitez ajouter l’utilisateur à un groupe (si vous ajoutez un utilisateur ou un contributeur au portail multimédia), cliquez sur Suivant et ajoutez l’utilisateur.
1. Cliquez sur le bouton Enregistrer pour terminer la configuration de l’utilisateur.

   Après l’enregistrement, une invite demande si vous souhaitez ajouter un utilisateur à une autre société. Cliquez sur Ajouter si vous souhaitez ajouter l’utilisateur à une société.

   Tous les nouveaux utilisateurs se voient attribuer un mot de passe généré de manière aléatoire ; les utilisateurs doivent changer de mot de passe lors de leur première connexion à Dynamic Media Classic.

   Un e-mail de bienvenue est envoyé aux utilisateurs une fois qu’ils ont été ajoutés. Ce message électronique indique un mot de passe provisoire et explique la procédure à suivre pour se connecter à Scene7 Publishing System.

   Si l’utilisateur ne reçoit pas le courrier électronique de bienvenue, demandez-lui d’accéder à la page de connexion à Dynamic Media Classic (https://s7sps1.scene7.com), puis de cliquer sur Mot de passe oublié. Le mot de passe est réinitialisé et un nouveau courrier électronique est envoyé. Si l’utilisateur ne reçoit pas le courrier électronique et qu’il n’est pas placé dans le dossier du courrier indésirable, contactez le support technique.

   Lorsque vous ajoutez de nouveaux utilisateurs du portail multimédia, vous pouvez également accéder à Configuration >Configuration de l’application > Administration utilisateur, puis cliquer sur Télécharger liste utilisateur et sélectionner un fichier .csv contenant 500 utilisateurs maximum.

### Suppression d’un utilisateur {#deleting-a-user}

Vous pouvez supprimer des utilisateurs de Dynamic Media Classic en les rendant non valides. Les utilisateurs non valides sont supprimés du système et de tous les comptes.

1. Cliquez sur **Configuration** > **Configuration de l’application** > **Configuration de l’administration** > **Administration utilisateur**.
1. Sélectionnez un utilisateur dans la liste, puis cliquez sur **Modifier**.
1. Désélectionnez l’option Valide.
1. Cliquez sur **Enregistrer**.

### Activation ou désactivation d’utilisateurs {#activating-or-deactivating-users}

Les utilisateurs désactivés n’ont plus le droit d’accéder au compte indiqué en haut du menu Sélectionner le compte auquel accéder.

1. Cliquez sur **Configuration** > **Configuration de l’application** > **Configuration de l’administration** > **Administration utilisateur**.
1. Dans la liste des utilisateurs, activez ou désactivez l’option Actif en regard du nom de l’utilisateur.

### Modification des informations utilisateur {#editing-user-information}

Les informations sur l’utilisateur que vous pouvez modifier dépendent de votre rôle en tant qu’administrateur et du rôle de l’utilisateur dont vous souhaitez modifier les informations. Les options qui apparaissent en grisé (non disponibles) ne sont pas modifiables.

1. Allez à **Configuration** > **Configuration de l’application** > **Configuration de l’administration** > **Administration utilisateur**.
1. Sélectionnez l’utilisateur, puis cliquez sur **Modifier**.
1. Sélectionnez l’entrée dans le tableau qui affiche l’entreprise dont vous essayez de modifier les autorisations ou l’accès, puis cliquez sur le lien Gérer l’entreprise.
1. Sélectionnez le rôle de l’utilisateur.
1. Si vous souhaitez modifier le groupe de l’utilisateur (si vous modifiez ou ajoutez un utilisateur ou un contributeur au portail multimédia), cliquez sur Suivant et modifiez l’appartenance au groupe.
1. Cliquez sur **Enregistrer**.

### Filtrage et tri de la liste des utilisateurs {#filtering-and-sorting-the-user-list}

Vous pouvez filtrer et trier la liste des utilisateurs afin de localiser les utilisateurs. Tous les utilisateurs figurant dans tous les comptes que vous gérez sont répertoriés dans la liste des utilisateurs, quel que soit le compte sélectionné dans le menu Sélectionner le compte auquel accéder.

Vous pouvez utiliser les techniques de filtrage suivantes :

**Filtrer par groupe** Sélectionnez le menu Par groupe et choisissez une option pour restreindre la liste aux utilisateurs d’un groupe.

**Filtrer par rôle** utilisateur Sélectionnez le menu Par rôle utilisateur et choisissez une option pour restreindre la liste aux utilisateurs ou aux administrateurs de différents types.

**Filtrer par nom** de champ Sélectionnez l’option Activer le filtre par champ. Sélectionnez ensuite le menu Par nom de champ, puis choisissez une colonne pour filtrer la liste. Sélectionnez ensuite le menu Filtrer par caractère, puis choisissez une lettre. La liste est filtrée en fonction d’une des colonnes selon la lettre que vous avez choisie. Désélectionnez l’option Activer le filtre par champ pour afficher la liste complète.

**Filtrer les utilisateurs** non valides Désélectionnez l’option Inclure les utilisateurs non valides. Les résultats de la recherche affichent uniquement les utilisateurs présents dans le système. Les utilisateurs non valides ont été supprimés du système et des comptes que vous gérez.

**Tri par en-tête** de colonne Cliquez sur un en-tête pour trier tous les utilisateurs selon leur état, par ordre alphabétique de prénom, de nom ou de courriel, selon leur rôle ou selon leur statut valide/non valide.

Si les utilisateurs sont trop nombreux, vous pouvez limiter la taille de la liste en sélectionnant le menu Taille liste max., puis en choisissant une valeur.

<!-- CQDOC-16690 TOPIC REMOVED AS PER JIRA TICKET INSTRUCTIONS ### Linking an IMS user identity to a Dynamic Media Classic IPS user account {#linking-an-ims-user-identity-to-a-scene-ips-user-account}

You can link an Adobe IMS user identity to a Dynamic Media Classic IPS user account so you can use SSO (Single Sign On) to log on and launch Scene7 Publishing System from within Adobe Marketing Cloud.

1. Adobe should already have setup your account with an Adobe Marketing Cloud organization and linked it to your Scene7 Publishing System product context. If this setup is not yet done or you are unsure if it has been done, contact Adobe Customer Care.

   When the setup is complete, you can can log on to Adobe Marketing Cloud and link your Adobe Marketing Cloud identity to your Dynamic Media Classic user account by doing the following.

1. In Adobe Marketing Cloud, navigate to your account settings.
1. Click **Manage Organizations**.
1. Click **Link Account** or **Get Access**.
1. Select **Experience Manager**, and then type your credentials.

   Your credentials include your IPS company region, email address, and password.

1. Click **Link**.
1. When the link is set, you can launch Scene7 Publishing System from within Adobe Marketing Cloud, or you can launch it directly.

   Do one of the following:

    * To launch Dynamic Media Classic from within Adobe Marketing Cloud, in the left rail of Adobe Marketing Cloud, click **Solutions** &gt; **Experience Manager**. Under the Dynamic Media Classic card, click **Launch**.
    * To log on to Scene7 Publishing System directly using your IMS credentials, use the following website:

      https://s7spsN.scene7.com/IpsWeb?ims=1

      Replace “N” in the above path with the number for your IPS company region. That is, N = 1 for North America; 3 for EMEA; or 5 for JAPAC.
 -->

## Bande passante et stockage {#bandwidth-storage}

Les administrateurs de Dynamic Media Classic peuvent générer de la bande passante, des enregistrements et d’autres types de rapports pour les sociétés qu’ils gèrent. Ces rapports sont disponibles sur l’écran Bande passante et stockage. 

Pour ouvrir cet écran, cliquez sur Configuration > Configuration personnelle. Développez Configuration de l’administration, puis cliquez sur Bande passante et stockage.

### Types de rapports {#types-of-reports}

Le tableau suivant décrit les rapports que vous pouvez générer à partir de l’écran Bande passante et stockage :

| Rapport | Informations | Utilité |
|:--- |:--- |:--- |
| Bande passante | Utilisation de la bande passante par entreprise | Observe l’utilisation de la bande passante par entreprise dans un intervalle de temps spécifié afin de définir des schémas de trafic. |
| Stockage | Utilisation de l’espace de stockage | Observe la quantité de données téléchargées par une entreprise. |
| Contenu de l’image | Nombre de demandes d’images par type | Observe le nombre de demandes et le volume pour différents types d’images. |
| Domaine | Nombre de demandes d’URL par domaine | Observe l’utilisation des images en fonction du domaine de la demande d’image pour une entreprise spécifique. (Dynamic Media Classic peut fournir plusieurs domaines par compte. Pour plus d’informations, contactez l’assistance technique.) |
| Diffusion de vidéo en flux continu | Utilisation de la bande passante pour la diffusion de vidéo en flux continu | Observe l’utilisation de la diffusion de vidéo en flux continu par entreprise dans un intervalle de temps spécifié afin de définir des schémas de trafic. |
| Contenu vidéo | Temps de lecture de différentes vidéos | Détermine quelles sont les vidéos les plus visionnées et les moins visionnées. |


Le rapport Contenu de l’image fournit des informations sur les requêtes pour les types d’image suivants :

**Demande** d’image Demandes d’images pour les images.

**Demande** de miniature Demandes d’échantillons ou d’images de remplacement dans les visionneuses.

**Requête** de masquage Demandes d’images renvoyant des masques en niveaux de gris.

**Requête** d’image de mosaïque de visionneuse chargée par une visionneuse.

**Demande** d’objet Vnt Demandes d’image Demandes de rendu qui renvoient une image avec des objets spécifiés dans les vignettes demandées.

**Demande** d’informations Vnt Demandes d’image qui renvoient des informations sur les vignettes demandées.

>[!NOTE]
>
>le rapport Diffusion de vidéo en flux continu s’applique uniquement aux vidéos diffusées en flux continu. Il ne rend nullement compte des vidéos en cours de visionnage.

### Génération d’un rapport {#generating-a-report}

Pour générer un rapport de bande passante, stockage, contenu de l’image, domaine, diffusion en flux continu de vidéo ou contenu de la vidéo :

1. Sélectionnez Configuration > Configuration personnelle.
1. Développez Configuration de l’administration, puis cliquez sur Bande passante et stockage.
1. Cliquez sur un onglet : Bande passante, Stockage, Contenu de l’image, Domaine, Diffusion vidéo en flux continu ou Contenu vidéo.

   Voir [Types de rapports](administration-setup.md#types_of_reports).

### Affichage des données de différentes manières {#viewing-data-in-different-ways}

Après avoir généré un rapport sur la page Bande passante et stockage, vous pouvez choisir des options pour l’affichage des informations. Vous pouvez choisir le mode de présentation des informations, afficher les informations dans un tableau ou une grille de données et indiquer une période pour la capture des informations. En mode Affichage des données, vous pouvez également trier les informations et réorganiser les colonnes.

**Affichage des données dans un graphique ou une grille** de données Cliquez sur l&#39;option Vue du graphique pour vue des données dans un graphique ; cliquez sur l’option Vue de données pour vue des données dans une grille de données.

**Choisir un type** de présentation de rapport Dans le menu Type de rapport, choisissez Résumé, Quotidien ou Mensuel pour organiser les données sous forme de résumé, par jour ou par mois. Tous les rapports ne proposent pas cette option.

**Spécification d&#39;une période** Choisissez des options pour définir une période pour votre rapport, puis cliquez sur Mettre à jour après avoir défini une période :

**Période** prédéfinie Dans le menu Rapport prédéfini, sélectionnez une option. Par exemple, choisissez Le mois dernier pour capturer les données du mois précédent.

**Période** personnalisée Dans le menu Rapport prédéfini, choisissez Personnalisé. Choisissez ensuite une date dans le menu Mois de début (ou Date de début) et une date dans le menu Nombre de mois (ou Nombre de jours). Pour les rapports de domaine ou de contenu vidéo, vous pouvez choisir une date de début et une date de fin spécifiques pour la capture des informations du rapport.

**Tri des données (vue de données uniquement)** Pour trier les informations d’une colonne, cliquez sur son en-tête. Cliquez une nouvelle fois pour effectuer le tri dans l’ordre décroissant.

**Réorganisation des colonnes (vue de données uniquement)** Pour déplacer une colonne vers un autre emplacement de la grille de données, faites glisser son en-tête.

### Exportation et impression des rapports {#exporting-and-printing-reports}

Après avoir généré un rapport, vous pouvez exporter ses données pour une utilisation dans des feuilles de calcul et d’autres applications. Vous pouvez également imprimer des rapports.

**Exportation de données** de rapport Dans la vue de données, triez et disposez les données selon vos besoins. Ouvrez ensuite le menu Exporter et choisissez un format : Délimité par une tabulation, Séparé par des virgules ou Format HTML. Les données sont copiées dans le Presse-papiers au format choisi. Vous pouvez à présent coller les données dans une feuille de calcul ou une application.

**Impression d&#39;un rapport** Cliquez sur Imprimer, choisissez les options de votre choix dans la boîte de dialogue Imprimer, puis cliquez sur OK.

## Erreurs d’image {#image-errors}

Les administrateurs de Dynamic Media Classic peuvent générer des rapports d’erreurs d’image. Un rapport d’erreurs d’image fournit la liste des 20 erreurs d’image les plus fréquentes sur les dernières 24 heures, pour l’entreprise à laquelle vous êtes actuellement connecté. Pour générer un rapport d’erreurs d’image, procédez comme suit :

1. Choisissez Configuration > Configuration personnelle.
1. Développez Configuration de l’administration, puis cliquez sur Erreurs d’image.
1. (Facultatif) Utilisez l’une des méthodes suivantes :

   * Cliquez sur un en-tête pour trier les erreurs selon les informations de l’en-tête. Par défaut, les erreurs sont triées par nombre d’occurrences, du plus élevé au moins élevé.
   * Placez le curseur sur le champ Réponse d’une erreur pour afficher le message d’erreur correspondant.
   * Placez le curseur sur le champ URL ou sur le champ Référent pour afficher le lien pointant vers l’image ou le site Web référent.
   * Cliquez sur Copier l’URL de la colonne URL pour copier le lien pointant vers l’image. Vous pouvez coller ce lien dans un navigateur pour accéder à l’image et étudier l’erreur.
   * Cliquez sur Copier l’URL de la colonne Référent pour copier le lien pointant vers le site Web référent.

Les erreurs s’affichent pour la société à laquelle vous êtes actuellement connecté. Les informations suivantes sont indiquées pour chaque erreur :

**ID** d’image pour l’image incriminée.

**Heure** Période de la première fois que l’erreur a été signalée à la dernière fois que l’erreur a été signalée, au cours des dernières 24 heures.

**Nombre** Nombre d’erreurs signalées sur l’image.

**Réponse** Message d&#39;erreur spécifique. Les erreurs sont soit 4xx soit 5xx.

**Les URL** Liste l’URL de l’image sur Scene7.

**Parrain** Spécifie l’URL du site Web d’où provient la demande initiale. Le référant peut être n’importe quel site Web contenant un lien vers l’image.

Les colonnes URL et Référent disposent de boutons Copier l’URL qui permettent de simplifier les tests.
