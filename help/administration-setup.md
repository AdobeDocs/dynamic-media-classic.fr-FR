---
title: Configuration de l’administration
seo-title: Configuration de l’administration
description: 'null'
seo-description: Découvrez comment configurer la zone d'administration de Dynamic Media Classic.
uuid: 16 ba 9 fed-b 5 c 6-4991-83 b 3-8 d 7 d 7129013 a
contentOwner: admin
content-type: référence
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
discoiquuid: 3 c 9 ee 4 ec-dd 37-498 d -98 d 6-1339 b 80177 ff
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Configuration de l’administration{#administration-setup}

Les écrans Configuration de l’administration sont destinés à la gestion des utilisateurs de Scene7 Publishing System. Utilisez ces écrans pour permettre aux utilisateurs de travailler dans Scene7 Publishing System et pour communiquer par e-mail avec eux.

1. To access Administration Setup options, click **Setup** &gt; **Personal Setup** &gt; **Administration Setup**.

## Administration utilisateur {#user-administration}

Tous les utilisateurs de Media Classic Classic se voient attribuer un rôle qui détermine leurs privilèges et droits d'accès aux fonctionnalités de Scene 7 Publishing System. Les administrateurs définissent les différents rôles et responsabilités pour les entreprises auxquelles ils sont affectés.

En général, Dynamic Media Classic configure le premier ensemble d'entreprises et affecte un administrateur d'entreprise. L’administrateur de l’entreprise configure et gère alors les utilisateurs de Scene7 Publishing System.

Scene7 Publishing System prend en charge trois rôles utilisateur. Ces trois rôles donnent accès à des entreprises configurées pour Scene7 Publishing System :

**L'administrateur SPS** peut afficher et gérer toutes les fonctionnalités de Scene 7 Publishing System, mais aussi configurer des entreprises et ajouter des administrateurs et des utilisateurs.

**L'administrateur d'entreprise** peut afficher et gérer uniquement ses propres entreprises. Il peut également remplir toutes les fonctions d’administration, notamment l’ajout d’administrateurs et d’utilisateurs. L’Administrateur d’entreprise peut ajouter un utilisateur aux comptes d’administration SPS de l’entreprise. (Ce rôle est le rôle utilisateur par défaut.)

**Les utilisateurs** SPS peuvent accéder aux entreprises auxquelles ils ont été affectés ; ne peut pas effectuer de tâches administratives.

Une fois que vous avez ajouté un utilisateur, Scene7 Publishing System lui envoie un e-mail de bienvenue. Ce message comporte un mot de passe et l’URL de Scene7 Publishing System.

### Ajout d’un utilisateur ou d’un administrateur {#adding-a-user-or-administrator}

1. Cliquez sur Configuration &gt; Configuration de l’application &gt; Configuration de l’administration &gt; Administration utilisateur.
1. Cliquez sur Ajouter.
1. Entrez le nom et l’adresse électronique de l’utilisateur ou de l’administrateur à ajouter, puis cliquez sur Suivant.

   >[!NOTE]
   >
   >le caractère apostrophe (’) n’est pas autorisé dans les adresses électroniques.

1. Choisissez une option de rôle pour attribuer un rôle à l’utilisateur.

   Voir [Rôles utilisateur Classic Media Classic et privilèges](administration-setup.md#user_administration).

1. Sélectionnez un nom de société pour ajouter un utilisateur à une entreprise.
1. Si vous souhaitez ajouter l’utilisateur à un groupe (si vous ajoutez un utilisateur ou un contributeur au portail multimédia), cliquez sur Suivant et ajoutez l’utilisateur.
1. Cliquez sur le bouton Enregistrer pour terminer la configuration de l’utilisateur.

   Après l’enregistrement, une invite demande si vous souhaitez ajouter un utilisateur à une autre société. Cliquez sur Ajouter si vous souhaitez ajouter l’utilisateur à une société.

   Un mot de passe est attribué de manière aléatoire à tous les nouveaux utilisateurs. Les utilisateurs doivent changer le mot de passe lors de leur première connexion au système Scene7 Publishing System.

   Un e-mail de bienvenue est envoyé aux utilisateurs une fois qu’ils ont été ajoutés. Ce message électronique indique un mot de passe provisoire et explique la procédure à suivre pour se connecter à Scene7 Publishing System.

   Si l'utilisateur ne reçoit pas le courriel de bienvenue, demandez-lui de se connecter à la page de connexion SPS (https://s7sps1.scene7.com), puis cliquez sur Mot de passe oublié. Le mot de passe est réinitialisé et un nouveau courrier électronique est envoyé. Si l’utilisateur ne reçoit pas le courrier électronique et qu’il n’est pas placé dans le dossier du courrier indésirable, contactez le support technique.

   Lorsque vous ajoutez de nouveaux utilisateurs du portail multimédia, vous pouvez également accéder à Configuration &gt;Configuration de l’application &gt; Administration utilisateur, puis cliquer sur Télécharger liste utilisateur et sélectionner un fichier .csv contenant 500 utilisateurs maximum.

### Suppression d’un utilisateur {#deleting-a-user}

Vous pouvez supprimer des utilisateurs de Scene7 Publishing System en les rendant non valides. Les utilisateurs non valides sont supprimés du système et de tous les comptes.

1. Cliquez sur **Configuration** &gt; **Configuration de l’application** &gt; **Configuration de l’administration** &gt; **Administration utilisateur**.
1. Sélectionnez un utilisateur dans la liste, puis cliquez sur **Modifier**.
1. Désélectionnez l’option Valide.
1. Cliquez sur **Enregistrer**.

### Activation ou désactivation d’utilisateurs {#activating-or-deactivating-users}

Les utilisateurs désactivés n’ont plus le droit d’accéder au compte indiqué en haut du menu Sélectionner le compte auquel accéder.

1. Cliquez sur **Configuration** &gt; **Configuration de l’application** &gt; **Configuration de l’administration** &gt; **Administration utilisateur**.
1. Dans la liste des utilisateurs, activez ou désactivez l’option Actif en regard du nom de l’utilisateur.

### Modification des informations utilisateur {#editing-user-information}

Les informations sur l’utilisateur que vous pouvez modifier dépendent de votre rôle en tant qu’administrateur et du rôle de l’utilisateur dont vous souhaitez modifier les informations. Les options qui apparaissent en grisé (non disponibles) ne sont pas modifiables.

1. Allez à **Configuration** &gt; **Configuration de l’application** &gt; **Configuration de l’administration** &gt; **Administration utilisateur**.
1. Sélectionnez l’utilisateur, puis cliquez sur **Modifier**.
1. Sélectionnez l’entrée dans le tableau qui affiche l’entreprise dont vous essayez de modifier les autorisations ou l’accès, puis cliquez sur le lien Gérer l’entreprise.
1. Sélectionnez le rôle de l’utilisateur.
1. Si vous souhaitez modifier le groupe de l’utilisateur (si vous modifiez ou ajoutez un utilisateur ou un contributeur au portail multimédia), cliquez sur Suivant et modifiez l’appartenance au groupe.
1. Cliquez sur **Enregistrer**.

### Filtrage et tri de la liste des utilisateurs {#filtering-and-sorting-the-user-list}

Vous pouvez filtrer et trier la liste des utilisateurs afin de localiser les utilisateurs. Tous les utilisateurs figurant dans tous les comptes que vous gérez sont répertoriés dans la liste des utilisateurs, quel que soit le compte sélectionné dans le menu Sélectionner le compte auquel accéder.

Vous pouvez utiliser les techniques de filtrage suivantes :

**Filtrage par groupe** Sélectionnez le menu Par groupe et choisissez une option pour restreindre la liste aux utilisateurs d'un groupe.

**Filtrer par rôle utilisateur** Sélectionnez le menu Par rôle utilisateur et choisissez une option pour restreindre la liste aux utilisateurs ou aux administrateurs de types différents.

**Filtrer par nom de champ** Sélectionnez l'option Activer le filtre par champ. Sélectionnez ensuite le menu Par nom de champ, puis choisissez une colonne pour filtrer la liste. Sélectionnez ensuite le menu Filtrer par caractère, puis choisissez une lettre. La liste est filtrée en fonction d’une des colonnes selon la lettre que vous avez choisie. Désélectionnez l’option Activer le filtre par champ pour afficher la liste complète.

**Filtrage des utilisateurs non valides** Désélectionnez l'option Inclure non valide. Les résultats de la recherche affichent uniquement les utilisateurs présents dans le système. Les utilisateurs non valides ont été supprimés du système et des comptes que vous gérez.

**Tri par en-tête de colonne** Cliquez sur un en-tête pour trier tous les utilisateurs par état, par ordre alphabétique par prénom, nom ou courrier électronique, par rôle utilisateur ou par état valide/non valide.

Si les utilisateurs sont trop nombreux, vous pouvez limiter la taille de la liste en sélectionnant le menu Taille liste max., puis en choisissant une valeur.

### Liaison d'une identité utilisateur IMS à un compte utilisateur IPS Dynamic Media Classic {#linking-an-ims-user-identity-to-a-scene-ips-user-account}

Vous pouvez lier une identité utilisateur Adobe IMS à un compte utilisateur IPS Dynamic Media Classic afin que vous puissiez utiliser la connexion unique (SSO) pour ouvrir une session et lancer Scene 7 Publishing System depuis Adobe Marketing Cloud.

1. Adobe aurait déjà configuré votre compte avec une organisation Adobe Marketing Cloud et l'a lié à votre contexte de produit Scene 7 Publishing System. Si cette configuration n'est pas encore effectuée ou si vous ne savez pas si elle a été effectuée, contactez le service à la clientèle Adobe.

   Une fois la configuration terminée, vous pouvez vous connecter à Adobe Marketing Cloud et associer votre identité Adobe Marketing Cloud à votre compte utilisateur Classic Media Classic en procédant comme suit.

1. Dans Adobe Marketing Cloud, accédez aux paramètres de votre compte.
1. Cliquez **sur Gérer les organisations**.
1. Cliquez **sur Lier le compte** ou **Obtenir un accès**.
1. Sélectionnez **Experience Manager**, puis entrez vos informations d'identification.

   Vos informations d'identification incluent la région de votre entreprise IPS, votre adresse électronique et votre mot de passe.

1. Cliquez **sur Lier**.
1. Lorsque le lien est défini, vous pouvez lancer Scene 7 Publishing System à partir d'Adobe Marketing Cloud, ou vous pouvez le lancer directement.

   Effectuez l’une des opérations suivantes :

   * Pour lancer Dynamic Media Classic depuis Adobe Marketing Cloud, dans le rail gauche d'Adobe Marketing Cloud, cliquez **sur Solutions** &gt; **Experience Manager**. Sous la carte Dynamic Media Classic, cliquez **sur Lancer**.
   * Pour vous connecter à Scene 7 Publishing System directement à l'aide de vos informations d'identification IMS, utilisez le site Web suivant :

      https://s7spsN.scene7.com/IpsWeb?ims=1

      Remplacez « N » dans le chemin ci-dessus par le nombre correspondant à votre région d'entreprise IPS. C'est-à-dire N = 1 pour l'Amérique du Nord ; 3 pour EMEA ; ou 5 pour JAPAC.

## Bande passante et stockage {#bandwidth-storage}

Les administrateurs SPS peuvent consulter des rapports de bande passante, de stockage et d’erreurs pour les entreprises qu’ils gèrent. Ces rapports sont disponibles sur l’écran Bande passante et stockage. 

Pour ouvrir cet écran, cliquez sur Configuration &gt; Configuration personnelle. Développez Configuration de l’administration, puis cliquez sur Bande passante et stockage.

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

**Demandes d'image** pour les images.

**Demandes de** requêtes miniatures pour les images d'échantillon ou d'alternative dans les visionneuses.

**Demandes de masques** pour les images renvoyant des masques d'échelle de gris.

**Demandes d'image de demande** de mosaïque de visionneuse chargées par une visionneuse.

**Demandes de rendu** d'image de demande d'objet Vnt qui renvoient une image avec des objets spécifiés dans les vignettes demandées.

**Demandes de rendu** d'image Vnt Demande de rendu qui renvoient des informations relatives aux vignettes demandées.

>[!NOTE]
>
>le rapport Diffusion de vidéo en flux continu s’applique uniquement aux vidéos diffusées en flux continu. Il ne rend nullement compte des vidéos en cours de visionnage.

### Génération d’un rapport {#generating-a-report}

Pour générer un rapport de bande passante, stockage, contenu de l’image, domaine, diffusion en flux continu de vidéo ou contenu de la vidéo :

1. Sélectionnez Configuration &gt; Configuration personnelle.
1. Développez Configuration de l’administration, puis cliquez sur Bande passante et stockage.
1. Cliquez sur un onglet : Bande passante, Stockage, Contenu de l’image, Domaine, Diffusion vidéo en flux continu ou Contenu vidéo.

   Voir [Types de rapports](administration-setup.md#types_of_reports).

### Affichage des données de différentes manières {#viewing-data-in-different-ways}

Après avoir généré un rapport sur la page Bande passante et stockage, vous pouvez choisir des options pour l’affichage des informations. Vous pouvez choisir le mode de présentation des informations, afficher les informations dans un tableau ou une grille de données et indiquer une période pour la capture des informations. En mode Affichage des données, vous pouvez également trier les informations et réorganiser les colonnes.

**Affichage des données dans un graphique ou une grille de données** Cliquez sur l'option Affichage du tableau pour afficher les données dans un graphique ; Cliquez sur l'option Vue des données pour afficher les données dans une grille de données.

**Choix d'un type de présentation du rapport** Dans le menu Type de rapport, choisissez Résumé, Quotidien ou Mensuel pour organiser les données sous forme de résumé, par jour ou par mois. Tous les rapports ne proposent pas cette option.

**Spécification d'une période** Choisissez des options pour définir une période pour votre rapport, puis cliquez sur Mettre à jour après avoir défini une période :

**Période prédéfinie** Dans le menu Rapport prédéfini, choisissez une option. Par exemple, choisissez Le mois dernier pour capturer les données du mois précédent.

**Période personnalisée** Dans le menu Rapport prédéfini, sélectionnez Personnalisé. Choisissez ensuite une date dans le menu Mois de début (ou Date de début) et une date dans le menu Nombre de mois (ou Nombre de jours). Pour les rapports de domaine ou de contenu vidéo, vous pouvez choisir une date de début et une date de fin spécifiques pour la capture des informations du rapport.

**Tri des données (vue des données uniquement)** Pour trier les informations d'une colonne, cliquez sur l'en-tête de la colonne. Cliquez une nouvelle fois pour effectuer le tri dans l’ordre décroissant.

**Réorganisation des colonnes (vue des données uniquement)** Pour déplacer une colonne vers un autre emplacement sur la grille de données, faites glisser son en-tête.

### Exportation et impression des rapports {#exporting-and-printing-reports}

Après avoir généré un rapport, vous pouvez exporter ses données pour une utilisation dans des feuilles de calcul et d’autres applications. Vous pouvez également imprimer des rapports.

**Exportation des données de rapport** dans la vue Données, triez et organisez les données selon vos besoins. Ouvrez ensuite le menu Exporter et choisissez un format : Délimité par une tabulation, Séparé par des virgules ou Format HTML. Les données sont copiées dans le Presse-papiers au format choisi. Vous pouvez à présent coller les données dans une feuille de calcul ou une application.

**Imprimer un rapport** cliquez sur Imprimer, choisissez les options voulues dans la boîte de dialogue Imprimer, puis cliquez sur OK.

## Erreurs d’image {#image-errors}

Les administrateurs SPS peuvent générer des rapports d’erreurs d’image. Un rapport d’erreurs d’image fournit la liste des 20 erreurs d’image les plus fréquentes sur les dernières 24 heures, pour l’entreprise à laquelle vous êtes actuellement connecté. Pour générer un rapport d’erreurs d’image, procédez comme suit :

1. Choisissez Configuration &gt; Configuration personnelle.
1. Développez Configuration de l’administration, puis cliquez sur Erreurs d’image.
1. (Facultatif) Utilisez l’une des méthodes suivantes :

   * Cliquez sur un en-tête pour trier les erreurs selon les informations de l’en-tête. Par défaut, les erreurs sont triées par nombre d’occurrences, du plus élevé au moins élevé.
   * Placez le curseur sur le champ Réponse d’une erreur pour afficher le message d’erreur correspondant.
   * Placez le curseur sur le champ URL ou sur le champ Référent pour afficher le lien pointant vers l’image ou le site Web référent.
   * Cliquez sur Copier l’URL de la colonne URL pour copier le lien pointant vers l’image. Vous pouvez coller ce lien dans un navigateur pour accéder à l’image et étudier l’erreur.
   * Cliquez sur Copier l’URL de la colonne Référent pour copier le lien pointant vers le site Web référent.

Les erreurs s’affichent pour la société à laquelle vous êtes actuellement connecté. Les informations suivantes sont indiquées pour chaque erreur :

**ID d'ID** d'image pour l'image de fin.

**Heure La** période de la première fois que l'erreur a été signalée à la dernière fois que l'erreur a été signalée, au cours des dernières 24 heures.

**Compter** le nombre d'erreurs signalées sur l'image.

**Réponse** Le message d'erreur spécifique. Les erreurs sont soit 4xx soit 5xx.

**URL** Répertorie l'URL de l'image sur Scene 7.

**Référent** Spécifie l'URL du site Web d'où provient la demande initiale. Le référant peut être n’importe quel site Web contenant un lien vers l’image.

Les colonnes URL et Référent disposent de boutons Copier l’URL qui permettent de simplifier les tests.
