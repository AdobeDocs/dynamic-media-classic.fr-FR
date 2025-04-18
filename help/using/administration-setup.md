---
title: Configuration de l’administration
description: Découvrez comment configurer la zone d’administration d’Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Admin
exl-id: 14e3d8be-f265-4cec-aa8e-19ef71526b68
topic: Administration
level: Intermediate
source-git-commit: dd799969ff9fd2638537254ae928a598eec627a3
workflow-type: tm+mt
source-wordcount: '1995'
ht-degree: 29%

---

<!-- UPDATE TOPIC AFTER DECEMBER 31, 2020!!!! -->

# Configuration de l’administration{#administration-setup}

Les écrans Configuration de l’administration permettent d’administrer les utilisateurs Adobe Dynamic Media Classic. Utilisez ces écrans pour permettre aux utilisateurs de travailler dans Adobe Dynamic Media Classic et de communiquer par e-mail avec d’autres utilisateurs.

1. Pour accéder aux options de configuration de l’administration, accédez à **Configuration** > **Configuration personnelle** > **Configuration de l’administration**.

## Administration des utilisateurs {#user-administration}

Un rôle déterminant leurs privilèges et droits d’accès aux fonctionnalités d’Adobe Dynamic Media Classic est attribué à tous les utilisateurs d’Adobe Dynamic Media Classic. Les administrateurs définissent les différents rôles et responsabilités pour les entreprises auxquelles ils sont affectés.

En règle générale, Adobe Dynamic Media Classic configure le premier ensemble de sociétés et affecte un administrateur d’entreprise. L’administrateur d’entreprise configure et administre ensuite les utilisateurs Adobe Dynamic Media Classic.

Adobe Dynamic Media Classic prend en charge plusieurs rôles utilisateur. Ces rôles peuvent accéder aux sociétés configurées pour Adobe Dynamic Media Classic :

<!-- **Adobe Dynamic Media Classic Administrator** Can view and administer all features in Adobe Dynamic Media Classic, as well as set up companies and add administrators and users. -->

**Utilisateur Adobe Dynamic Media Classic** peut accéder aux sociétés auxquelles il a été affecté ; ne peut effectuer aucune tâche administrative.

**Administrateur d’entreprise Adobe Dynamic Media Classic** peut afficher et administrer uniquement ses propres entreprises. Il peut également remplir toutes les fonctions d’administration, notamment l’ajout d’administrateurs et d’utilisateurs. Un administrateur d’entreprise peut ajouter un utilisateur aux comptes d’administration de la société DMC. (Ce rôle est le rôle utilisateur par défaut.)

Une fois que vous avez ajouté un utilisateur, Adobe Dynamic Media Classic lui envoie un message électronique de bienvenue. Le message comprend un mot de passe et l’URL d’Adobe Dynamic Media Classic.

### Ajouter un utilisateur, une utilisatrice ou un administrateur {#adding-a-user-or-administrator}

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Configuration de l’administration]** > **[!UICONTROL Administration des utilisateurs]**.
1. Sélectionnez **[!UICONTROL Ajouter]**.
1. Saisissez le nom et l’adresse e-mail de l’utilisateur ou de l’administrateur que vous souhaitez ajouter, puis sélectionnez **[!UICONTROL Suivant]**.

   >[!NOTE]
   >
   >Le caractère apostrophe (`'`) n’est pas autorisé dans les adresses e-mail.

1. Pour attribuer un rôle à l’utilisateur, choisissez une option de rôle.

   Voir [Rôles et privilèges d’utilisateur Adobe Dynamic Media Classic](administration-setup.md#user_administration).

1. Pour ajouter un utilisateur à une société, sélectionnez un nom de société.
1. Si vous souhaitez ajouter l’utilisateur à un groupe (si vous ajoutez un utilisateur ou un contributeur du portail multimédia), sélectionnez **[!UICONTROL Suivant]** et ajoutez l’utilisateur.
1. Sélectionnez **[!UICONTROL Enregistrer]** pour terminer la configuration de l’utilisateur.

   Après l’enregistrement, une invite demande si vous souhaitez ajouter un utilisateur à une autre société. Sélectionnez **[!UICONTROL Ajouter]** si vous souhaitez ajouter l’utilisateur à une entreprise.

   Un mot de passe généré de manière aléatoire est attribué à tous les nouveaux utilisateurs. Ceux-ci doivent modifier leur mot de passe la première fois qu’ils se connectent à l’application de bureau Adobe Dynamic Media Classic.

   Un e-mail de bienvenue est envoyé aux utilisateurs une fois qu’ils ont été ajoutés. Cet e-mail fournit un mot de passe temporaire et explique comment se connecter à Adobe Dynamic Media Classic.

   Si l’utilisateur ne reçoit pas l’e-mail de bienvenue, demandez-lui d’accéder à la page de connexion d’Adobe Dynamic Media Classic (https://s7sps1.scene7.com) et de sélectionner **[!UICONTROL Mot de passe oublié]**. Le mot de passe est réinitialisé et un nouveau courrier électronique est envoyé. Si l’utilisateur ne reçoit pas le courrier électronique et qu’il n’est pas placé dans le dossier du courrier indésirable, contactez le support technique.

   Lors de l’ajout d’utilisateurs au portail multimédia, vous pouvez également accéder à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Administration des utilisateurs]**, puis sélectionner **[!UICONTROL Charger la liste des utilisateurs]** et sélectionner un fichier .csv ne contenant pas plus de 500 utilisateurs.

### Suppression d’un utilisateur {#delet-a-user}

Vous pouvez supprimer des utilisateurs d’Adobe Dynamic Media Classic en les rendant non valides. Les utilisateurs non valides sont supprimés du système et de tous les comptes.

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Configuration de l’administration]** > **[!UICONTROL Administration des utilisateurs]**.
1. Sélectionnez un utilisateur dans la liste, puis sélectionnez **[!UICONTROL Modifier]**.
1. Désélectionnez l’option Valide.
1. Sélectionnez **[!UICONTROL Enregistrer]**.

### Activer ou désactiver des utilisateurs {#activating-or-deactivating-users}

Les utilisateurs désactivés n’ont plus le droit d’accéder au compte indiqué en haut du menu Sélectionner le compte auquel accéder.

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Configuration de l’administration]** > **[!UICONTROL Administration des utilisateurs]**.
1. Dans la liste des utilisateurs, sélectionnez ou désélectionnez l’option **[!UICONTROL Actif]** en regard du nom de l’utilisateur.

### Modification des informations de l’utilisateur {#editing-user-information}

Les informations sur l’utilisateur que vous pouvez modifier dépendent de votre rôle en tant qu’administrateur et du rôle de l’utilisateur dont vous souhaitez modifier les informations. Les options qui apparaissent en grisé (non disponibles) ne sont pas modifiables.

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Configuration de l’administration]** > **[!UICONTROL Administration des utilisateurs]**.
1. Sélectionnez un utilisateur dans la liste, puis sélectionnez **[!UICONTROL Modifier]**.
1. Sélectionnez l’entrée dans le tableau qui indique la société pour laquelle vous essayez de modifier les autorisations ou l’accès, puis sélectionnez **[!UICONTROL Gérer la société]**.
1. Sélectionnez le rôle de l’utilisateur.
1. Si vous souhaitez modifier l’appartenance à un groupe de l’utilisateur (si vous modifiez ou ajoutez un utilisateur ou un contributeur du portail multimédia), sélectionnez **[!UICONTROL Suivant]** et modifiez l’appartenance à un groupe.
1. Sélectionnez **[!UICONTROL Enregistrer]**.

### Filtrage et tri de la liste des utilisateurs {#filtering-and-sorting-the-user-list}

Vous pouvez filtrer et trier la liste des utilisateurs afin de localiser les utilisateurs. Tous les utilisateurs figurant dans tous les comptes que vous gérez sont répertoriés dans la liste des utilisateurs, quel que soit le compte sélectionné dans le menu Sélectionner le compte auquel accéder.

Vous pouvez utiliser les techniques de filtrage de liste d’utilisateurs suivantes :

* **Filtrer par groupe** : sélectionnez le menu **[!UICONTROL Par groupe]** et choisissez une option pour limiter la liste aux utilisateurs d’un groupe.

* **Filtrer par rôle d’utilisateur** : sélectionnez le menu **[!UICONTROL Par rôle d’utilisateur]** et choisissez une option pour limiter la liste aux utilisateurs ou administrateurs de différents types.

* **Filtrer par nom de champ** : sélectionnez **[!UICONTROL Activer le filtrage par champ]**. Sélectionnez ensuite le menu **[!UICONTROL Par nom de champ]**, choisissez une colonne pour filtrer la liste, puis sélectionnez le menu Filtrer les caractères et choisissez une lettre. La liste est filtrée sur l’une des colonnes par la lettre que vous avez choisie. Pour afficher la liste complète, désélectionnez l’option **[!UICONTROL Activer le filtrage par champ]**.

* **Filtrer les utilisateurs non valides** : désélectionnez **[!UICONTROL Inclure non valide]**. Les résultats de la recherche affichent uniquement les utilisateurs présents dans le système. Des utilisateurs non valides ont été supprimés du système et des comptes que vous administrez.

* **Trier par en-tête de colonne** : sélectionnez un en-tête pour trier tous les utilisateurs par statut, par ordre alphabétique de prénom, de nom ou d’adresse e-mail. Ou, triez-les par rôle d’utilisateur ou par statut valide/non valide.

Si les utilisateurs sont trop nombreux, vous pouvez limiter la taille de la liste en sélectionnant le menu Taille liste max., puis en choisissant une valeur.

<!-- CQDOC-16690 TOPIC REMOVED AS PER JIRA TICKET INSTRUCTIONS ### Linking an IMS user identity to an Adobe Dynamic Media Classic IPS user account {#linking-an-ims-user-identity-to-a-scene-ips-user-account}

You can link an Adobe IMS user identity to an Adobe Dynamic Media Classic IPS user account so you can use SSO (Single Sign On) to log on and launch Scene7 Publishing System from within Adobe Marketing Cloud.

1. Adobe should already have setup your account with an Adobe Marketing Cloud organization and linked it to your Scene7 Publishing System product context. If this setup is not yet done or you are unsure if it has been done, contact Adobe Customer Care.

   When the setup is complete, you can can log on to Adobe Marketing Cloud and link your Adobe Marketing Cloud identity to your Adobe Dynamic Media Classic user account by doing the following.

1. In Adobe Marketing Cloud, navigate to your account settings.
1. Select **Manage Organizations**.
1. Select **Link Account** or **Get Access**.
1. Select **Experience Manager**, and then type your credentials.

   Your credentials include your IPS company region, email address, and password.

1. Select **Link**.
1. When the link is set, you can launch Scene7 Publishing System from within Adobe Marketing Cloud, or you can launch it directly.

   Do one of the following:

    * To launch Adobe Dynamic Media Classic from within Adobe Marketing Cloud, in the left rail of Adobe Marketing Cloud, select **Solutions** > **Experience Manager**. Under the Adobe Dynamic Media Classic card, select **Launch**.
    * To log on to Scene7 Publishing System directly using your IMS credentials, use the following website:

      https://s7spsN.scene7.com/IpsWeb?ims=1

      Replace "N" in the above path with the number for your IPS company region. That is, N = 1 for North America; 3 for EMEA; or 5 for JAPAC.
 -->

## Bande passante et stockage {#bandwidth-storage}

Les administrateurs d’Adobe Dynamic Media Classic peuvent générer de la bande passante, du stockage et d’autres types de rapports pour les sociétés qu’ils administrent. Ces rapports sont disponibles sur la page Bande passante et stockage .

Pour ouvrir cette page, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration personnelle]**. Développez **[!UICONTROL Configuration de l’administration]**, puis sélectionnez **[!UICONTROL Bande passante et stockage]**.

### Types de rapports {#types-of-reports}

Le tableau suivant décrit les rapports que vous pouvez générer à partir de la page Bande passante et stockage :

| Rapport | Informations | Utilité |
| --- | --- | --- |
| Bande passante | | **IMPORTANT** : l’onglet Bande passante n’est plus pris en charge. Bien qu’elles apparaissent toujours dans l’interface utilisateur, les données de bande passante ne sont pas disponibles et toutes les valeurs s’affichent sous la forme `0`. |
| Stockage | Utilisation de l’espace de stockage | Effectuez le suivi de la quantité de données téléchargées par l’entreprise. |
| Contenu de l’image | Affiche le nombre total d’accès et le volume de diffusion d’images, répartis par type et sous-type de requête. | Effectuez le suivi du nombre de requêtes et du volume pour différents types d’images, y compris les mesures provenant de ressources non vidéo. |
| Domaine | Nombre de demandes d’URL par domaine | Observe l’utilisation des images en fonction du domaine de la demande d’image pour une entreprise spécifique. (Adobe Dynamic Media Classic peut fournir plusieurs domaines par compte. Pour plus d’informations, contactez l’assistance technique.) |
| Diffusion de vidéo en flux continu | Utilisation de la bande passante pour la diffusion de vidéo en flux continu | Observe l’utilisation de la diffusion de vidéo en flux continu par entreprise dans un intervalle de temps spécifié afin de définir des schémas de trafic. |
| Contenu vidéo | Temps de lecture de différentes vidéos | Détermine quelles sont les vidéos les plus visionnées et les moins visionnées. |

Le rapport Contenu de l’image fournit des informations sur les requêtes pour les types d’image suivants :

* **Demande d’image** : demandes d’images.

* **Demande de miniature** : demandes d’échantillon ou d’images de remplacement dans les visionneuses.

* **Requête de masque** : requêtes d’images renvoyant des masques en niveaux de gris.

* **Demande de mosaïque de visionneuse** : demandes d’image chargées par une visionneuse.

* **Demande d’objet VNT** : demandes de rendu d’image qui renvoient une image avec des objets spécifiés dans les vignettes demandées.

* **Demande d’informations VNT** : demandes de rendu d’image qui renvoient des informations concernant les vignettes demandées.

>[!NOTE]
>
>le rapport Diffusion de vidéo en flux continu s’applique uniquement aux vidéos diffusées en flux continu. Il ne suit pas le visionnage des vidéos progressives.

### Générer un rapport {#generating-a-report}

Pour générer un rapport de bande passante, stockage, contenu de l’image, domaine, diffusion en flux continu de vidéo ou contenu de la vidéo :

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration personnelle]**.
1. Développez Administration et configuration, puis sélectionnez **[!UICONTROL Bande passante et stockage]**.
1. Sélectionnez un onglet : **[!UICONTROL Bande passante]**, **[!UICONTROL Stockage]**, **[!UICONTROL Contenu d’image]**, **[!UICONTROL Domaine]**, **[!UICONTROL Diffusion vidéo]** ou **[!UICONTROL Contenu vidéo]**.

   Voir [Types de rapports](administration-setup.md#types_of_reports).

### Affichage des données de différentes manières {#viewing-data-in-different-ways}

Après avoir généré un rapport sur la page Bande passante et stockage, vous pouvez choisir des options pour l’affichage des informations. Vous pouvez choisir le mode de présentation des informations, afficher les informations dans un tableau ou une grille de données et indiquer une période pour la capture des informations. En mode Affichage des données, vous pouvez également trier les informations et réorganiser les colonnes.

* **Afficher les données dans un graphique ou une grille de données** : sélectionnez **[!UICONTROL Vue du graphique]** pour afficher les données dans un graphique ; sélectionnez **[!UICONTROL Vue des données]** pour afficher les données dans une grille de données.

* **Choisissez un type de présentation de rapport** : dans le menu Type de rapport, sélectionnez **[!UICONTROL Résumé]**, **[!UICONTROL Quotidien]** ou **[!UICONTROL Mensuel]** pour organiser les données sous forme de résumé, par jour ou par mois. Tous les rapports ne proposent pas cette option.

* **Définir une période** : sélectionnez les options permettant de définir une période pour votre rapport, puis sélectionnez **[!UICONTROL Mettre à jour]** après avoir défini une période :

* **Période prédéfinie** : dans le menu Rapport prédéfini, sélectionnez une option. Par exemple, choisissez Le mois dernier pour capturer les données du mois précédent.

* **Période personnalisée** : dans le menu Rapport prédéfini, sélectionnez **[!UICONTROL Personnalisé]**. Choisissez ensuite une date dans le menu **[!UICONTROL Mois de début]** (ou **[!UICONTROL Date de début]**) et une date dans le menu # de mois (ou # ou Jours). Pour les rapports de domaine ou de contenu vidéo, vous pouvez choisir une date de début et une date de fin spécifiques pour la capture des informations du rapport.

* **Trier les données (vue de données uniquement)** : trier les informations dans une colonne. Sélectionnez l’en-tête de la colonne. Sélectionnez à nouveau pour trier par ordre décroissant.

* **Réorganiser les colonnes (vue de données uniquement)** : pour déplacer une colonne vers un autre emplacement sur la grille de données, faites glisser son en-tête.

### Exporter et imprimer des rapports {#exporting-and-printing-reports}

Après avoir généré un rapport, vous pouvez exporter ses données pour une utilisation dans des feuilles de calcul et d’autres applications. Vous pouvez également imprimer des rapports.

* **Exporter les données du rapport** : dans la vue Données, triez et organisez les données selon vos besoins. Ouvrez ensuite le menu **[!UICONTROL Exporter]** et choisissez un format : **[!UICONTROL Délimité par des tabulations]**, **[!UICONTROL Séparé par des virgules]** ou **[!UICONTROL Formaté en HTML]**. Les données sont copiées dans le Presse-papiers au format choisi. Vous pouvez à présent coller les données dans une feuille de calcul ou une application.

* **Imprimer un rapport** : sélectionnez **[!UICONTROL Imprimer]**, choisissez les options souhaitées dans la boîte de dialogue Imprimer, puis sélectionnez **[!UICONTROL OK]**.

## Erreurs d’image {#image-errors}

Les administrateurs Adobe Dynamic Media Classic peuvent générer des rapports d’erreur d’image. Un rapport d’erreurs d’image fournit la liste des 20 erreurs d’image les plus fréquentes sur les dernières 24 heures, pour l’entreprise à laquelle vous êtes actuellement connecté. Pour générer un rapport d’erreur d’image, procédez comme suit :

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration personnelle]**.
1. Développez Administration Configuration, puis sélectionnez **[!UICONTROL Erreurs d’image]**.
1. (Facultatif) Utilisez l’une des méthodes suivantes :

   * Pour trier les erreurs en fonction des informations d’en-tête, sélectionnez un en-tête. Par défaut, les erreurs sont triées par nombre d’occurrences, du plus élevé au moins élevé.
   * Placez le curseur sur le champ Réponse d’une erreur pour afficher le message d’erreur correspondant.
   * Pour voir le lien vers l’image ou la page Web du référent, déplacez le curseur sur le champ URL ou le champ Référent .
   * Pour copier le lien vers l’image réelle, sélectionnez **[!UICONTROL URL de copie]**. Vous pouvez coller ce lien dans un navigateur pour accéder à l’image et étudier l’erreur.
   * Pour copier le lien vers la page Web du référent, sélectionnez **[!UICONTROL URL de copie du référent]**.

Les erreurs affichées concernent la société à laquelle vous êtes actuellement connecté. Les informations suivantes sont indiquées pour chaque erreur :

* **Identifiant de l’image** : identifiant de l’image incriminée.

* **Heure** : période entre la première fois où l’erreur a été signalée et la dernière fois où l’erreur a été signalée, au cours des dernières 24 heures.

* **Nombre** : nombre d’erreurs signalées sur l’image.

* **Réponse** : message d’erreur spécifique. Les erreurs sont soit 4xx soit 5xx.

* **URLs** : répertorie l’URL de l’image sur Adobe Dynamic Media Classic.

* **Référent** : indique l’URL du site Web d’où provient la demande initiale. Le référent peut être n’importe quel site web comportant un lien vers l’image.

Les colonnes URL et Référent disposent de boutons Copier l’URL qui permettent de simplifier les tests.
