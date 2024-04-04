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
source-git-commit: f054057d383b26e9088582f418f62504c3f327d8
workflow-type: tm+mt
source-wordcount: '1971'
ht-degree: 33%

---

<!-- UPDATE TOPIC AFTER DECEMBER 31, 2020!!!! -->

# Configuration de l’administration{#administration-setup}

Les écrans Configuration de l’administration permettent d’administrer les utilisateurs d’Adobe Dynamic Media Classic. Utilisez ces écrans pour permettre aux utilisateurs de travailler dans Adobe Dynamic Media Classic et de communiquer par e-mail avec les utilisateurs.

1. Pour accéder aux options Configuration de l’administration , accédez à **Configuration** > **Configuration personnelle** > **Configuration de l’administration**.

## Administration utilisateur {#user-administration}

Un rôle est attribué à tous les utilisateurs d’Adobe Dynamic Media Classic afin de déterminer leurs privilèges et leurs droits d’accès aux fonctionnalités d’Adobe Dynamic Media Classic. Les administrateurs définissent les différents rôles et responsabilités pour les entreprises auxquelles ils sont affectés.

En règle générale, Adobe Dynamic Media Classic configure le premier ensemble de sociétés et affecte un administrateur de société. L’administrateur de l’entreprise configure et administre ensuite les utilisateurs d’Adobe Dynamic Media Classic.

Adobe Dynamic Media Classic prend en charge plusieurs rôles utilisateur. Ces rôles peuvent accéder aux entreprises configurées pour Adobe Dynamic Media Classic :

<!-- **Adobe Dynamic Media Classic Administrator** Can view and administer all features in Adobe Dynamic Media Classic, as well as set up companies and add administrators and users. -->

**Utilisateur Adobe Dynamic Media Classic** Peuvent accéder aux entreprises auxquelles elles ont été assignées ; ne peuvent effectuer aucune tâche administrative.

**Administrateur de société Adobe Dynamic Media Classic** Peuvent visualiser et administrer uniquement leurs propres entreprises. Il peut également remplir toutes les fonctions d’administration, notamment l’ajout d’administrateurs et d’utilisateurs. Un administrateur d’entreprise peut ajouter un utilisateur aux comptes administrateur d’entreprise DMC. (Ce rôle est le rôle utilisateur par défaut.)

Une fois que vous avez ajouté un utilisateur, Adobe Dynamic Media Classic lui envoie un e-mail de bienvenue. Le message comprend un mot de passe et l’URL Adobe Dynamic Media Classic.

### Ajout d’un utilisateur ou d’un administrateur {#adding-a-user-or-administrator}

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Configuration de l’administration]** > **[!UICONTROL Administration des utilisateurs]**.
1. Sélectionner **[!UICONTROL Ajouter]**.
1. Saisissez le nom et l’adresse électronique de l’utilisateur ou de l’administrateur que vous souhaitez ajouter, puis sélectionnez **[!UICONTROL Suivant]**.

   >[!NOTE]
   >
   >Le caractère apostrophe (`'`) n’est pas autorisé dans les adresses électroniques.

1. Pour attribuer un rôle à l’utilisateur, sélectionnez une option Rôle .

   Voir [Rôles utilisateur et privilèges Adobe Dynamic Media Classic](administration-setup.md#user_administration).

1. Pour ajouter un utilisateur à une société, sélectionnez son nom.
1. Si vous souhaitez ajouter l’utilisateur à un groupe (si vous ajoutez un utilisateur ou un contributeur Media Portal), sélectionnez **[!UICONTROL Suivant]** et ajoutez l’utilisateur.
1. Sélectionner **[!UICONTROL Enregistrer]** pour terminer la configuration utilisateur.

   Après l’enregistrement, une invite demande si vous souhaitez ajouter un utilisateur à une autre société. Sélectionner **[!UICONTROL Ajouter]** si vous souhaitez ajouter l’utilisateur à une société.

   Tous les nouveaux utilisateurs reçoivent un mot de passe généré de manière aléatoire ; les utilisateurs doivent changer de mot de passe la première fois qu’ils se connectent à l’application de bureau Adobe Dynamic Media Classic.

   Un e-mail de bienvenue est envoyé aux utilisateurs une fois qu’ils ont été ajoutés. L’e-mail fournit un mot de passe temporaire et explique comment vous connecter à Adobe Dynamic Media Classic.

   Si l’utilisateur ne reçoit pas l’e-mail de bienvenue, demandez-lui d’accéder à la page de connexion Adobe Dynamic Media Classic (https://s7sps1.scene7.com), puis sélectionnez **[!UICONTROL Mot de passe oublié]**. Le mot de passe est réinitialisé et un nouveau courrier électronique est envoyé. Si l’utilisateur ne reçoit pas le courrier électronique et qu’il n’est pas placé dans le dossier du courrier indésirable, contactez le support technique.

   Lors de l’ajout de nouveaux utilisateurs de Media Portal, vous pouvez également accéder à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Administration des utilisateurs]**, puis sélectionnez **[!UICONTROL Télécharger la liste des utilisateurs]** et sélectionnez un fichier .csv ne contenant pas plus de 500 utilisateurs.

### Suppression d’un utilisateur {#delet-a-user}

Vous pouvez supprimer des utilisateurs d’Adobe Dynamic Media Classic en les rendant non valides. Les utilisateurs non valides sont supprimés du système et de tous les comptes.

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Configuration de l’administration]** > **[!UICONTROL Administration des utilisateurs]**.
1. Sélectionnez un utilisateur dans la liste, puis sélectionnez **[!UICONTROL Modifier]**.
1. Désélectionnez l’option Valide.
1. Sélectionner **[!UICONTROL Enregistrer]**.

### Activation ou désactivation d’utilisateurs {#activating-or-deactivating-users}

Les utilisateurs désactivés n’ont plus le droit d’accéder au compte indiqué en haut du menu Sélectionner le compte auquel accéder.

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Configuration de l’administration]** > **[!UICONTROL Administration des utilisateurs]**.
1. Dans la liste des utilisateurs, sélectionnez ou désélectionnez l’option **[!UICONTROL Actif]** en regard du nom de l’utilisateur.

### Modification des informations de l’utilisateur {#editing-user-information}

Les informations sur l’utilisateur que vous pouvez modifier dépendent de votre rôle en tant qu’administrateur et du rôle de l’utilisateur dont vous souhaitez modifier les informations. Les options qui apparaissent en grisé (non disponibles) ne sont pas modifiables.

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Configuration de l’administration]** > **[!UICONTROL Administration des utilisateurs]**.
1. Sélectionnez un utilisateur dans la liste, puis sélectionnez **[!UICONTROL Modifier]**.
1. Sélectionnez l’entrée dans le tableau qui indique la société pour laquelle vous essayez de modifier les autorisations ou l’accès, puis sélectionnez **[!UICONTROL Gérer l’entreprise]**.
1. Sélectionnez le rôle de l’utilisateur.
1. Si vous souhaitez modifier l’appartenance au groupe de l’utilisateur (si vous modifiez ou ajoutez un utilisateur ou un contributeur Media Portal), sélectionnez **[!UICONTROL Suivant]** et modifiez l’appartenance au groupe.
1. Sélectionner **[!UICONTROL Enregistrer]**.

### Filtrage et tri de la liste des utilisateurs {#filtering-and-sorting-the-user-list}

Vous pouvez filtrer et trier la liste des utilisateurs afin de localiser les utilisateurs. Tous les utilisateurs figurant dans tous les comptes que vous gérez sont répertoriés dans la liste des utilisateurs, quel que soit le compte sélectionné dans le menu Sélectionner le compte auquel accéder.

Vous pouvez utiliser les techniques de filtrage par liste d’utilisateurs suivantes :

* **Filtrage par groupe** - Sélectionnez la variable **[!UICONTROL Par groupe]** et choisissez une option pour limiter la liste aux utilisateurs d’un groupe.

* **Filtrage par rôle d’utilisateur** - Sélectionnez la variable **[!UICONTROL Par rôle d’utilisateur]** et choisissez une option pour limiter la liste aux utilisateurs ou aux administrateurs de différents types.

* **Filtrer par nom de champ** - Sélectionner **[!UICONTROL Activer le filtre par champ]**. Sélectionnez ensuite le **[!UICONTROL Par nom de champ]** , choisissez une colonne pour filtrer la liste, sélectionnez le menu Filtrer les caractères et choisissez une lettre. La liste est filtrée sur l’une des colonnes par la lettre choisie. Pour afficher la liste complète, désélectionnez l’option **[!UICONTROL Activer le filtre par champ]** .

* **Filtrage des utilisateurs non valides** - Désélectionner **[!UICONTROL Inclure non valide]**. Les résultats de la recherche affichent uniquement les utilisateurs présents dans le système. Les utilisateurs non valides ont été supprimés du système et des comptes que vous administrez.

* **Tri par en-tête de colonne** - Sélectionnez un en-tête pour trier tous les utilisateurs selon leur état, par ordre alphabétique de prénom, nom ou adresse électronique, par rôle d’utilisateur ou par statut valide/non valide.

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

Les administrateurs Adobe Dynamic Media Classic peuvent générer des rapports de bande passante, de stockage et d’autres types pour les entreprises qu’ils gèrent. Ces rapports sont disponibles sur la page Bande passante et stockage .

Pour ouvrir cette page, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration personnelle]**. Développer **[!UICONTROL Configuration de l’administration]**, puis sélectionnez **[!UICONTROL Bande passante et stockage]**.

### Types de rapports {#types-of-reports}

Le tableau suivant décrit les rapports que vous pouvez générer à partir de la page Bande passante et stockage :

| Rapport | Informations | Utilité |
|:--- |:--- |:--- |
| Bande passante | Utilisation de la bande passante par entreprise | Observe l’utilisation de la bande passante par entreprise dans un intervalle de temps spécifié afin de définir des schémas de trafic. |
| Stockage | Utilisation de l’espace de stockage | Observe la quantité de données téléchargées par une entreprise. |
| Contenu de l’image | Nombre de demandes d’images par type | Observe le nombre de demandes et le volume pour différents types d’images. |
| Domaine | Nombre de demandes d’URL par domaine | Observe l’utilisation des images en fonction du domaine de la demande d’image pour une entreprise spécifique. (Adobe Dynamic Media Classic peut fournir plusieurs domaines par compte. Pour plus d’informations, contactez l’assistance technique.) |
| Diffusion de vidéo en flux continu | Utilisation de la bande passante pour la diffusion de vidéo en flux continu | Observe l’utilisation de la diffusion de vidéo en flux continu par entreprise dans un intervalle de temps spécifié afin de définir des schémas de trafic. |
| Contenu vidéo | Temps de lecture de différentes vidéos | Détermine quelles sont les vidéos les plus visionnées et les moins visionnées. |

Le rapport Contenu de l’image fournit des informations sur les requêtes pour les types d’image suivants :

* **Demande d’image** - Demandes d’images.

* **Demande de miniature** - Demandes d’échantillon ou d’images de remplacement dans les visionneuses.

* **Masquer la requête** - Demandes d’images renvoyant des masques en niveaux de gris.

* **Requête de mosaïque de visionneuse** - Demandes d’image chargées par une visionneuse.

* **Requête D’Objet Vnt** - Demandes de rendu d’image qui renvoient une image avec des objets spécifiés dans les vignettes demandées.

* **Requête Infos Vnt** - Demandes de rendu d’image qui renvoient des informations relatives aux vignettes demandées.

>[!NOTE]
>
>le rapport Diffusion de vidéo en flux continu s’applique uniquement aux vidéos diffusées en flux continu. Il ne suit pas l’affichage des vidéos progressives.

### Générer un rapport {#generating-a-report}

Pour générer un rapport de bande passante, stockage, contenu de l’image, domaine, diffusion en flux continu de vidéo ou contenu de la vidéo :

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration personnelle]**.
1. Développez Configuration de l’administration, puis sélectionnez **[!UICONTROL Bande passante et stockage]**.
1. Sélectionnez un onglet : **[!UICONTROL Bande passante]**, **[!UICONTROL Stockage]**, **[!UICONTROL Contenu de l’image]**, **[!UICONTROL Domaine]**, **[!UICONTROL Diffusion en continu de vidéos]**, ou **[!UICONTROL Contenu vidéo]**.

   Voir [Types de rapports](administration-setup.md#types_of_reports).

### Affichage des données de différentes manières {#viewing-data-in-different-ways}

Après avoir généré un rapport sur la page Bande passante et stockage, vous pouvez choisir des options pour l’affichage des informations. Vous pouvez choisir le mode de présentation des informations, afficher les informations dans un tableau ou une grille de données et indiquer une période pour la capture des informations. En mode Affichage des données, vous pouvez également trier les informations et réorganiser les colonnes.

* **Affichage des données dans un graphique ou une grille de données** - Sélectionner **[!UICONTROL Affichage du graphique]** pour afficher les données dans un graphique ; sélectionnez **[!UICONTROL Vue des données]** pour afficher les données dans une grille de données.

* **Choisissez un type de présentation de rapport** - Dans le menu Type de rapport, sélectionnez **[!UICONTROL Résumé]**, **[!UICONTROL Qualité]**, ou **[!UICONTROL Mensuel]** pour organiser les données sous forme de résumé, par jour ou par mois. Tous les rapports ne proposent pas cette option.

* **Définition d’une période** - Choisissez des options pour définir une période pour votre rapport, puis sélectionnez **[!UICONTROL Mettre à jour]** après avoir défini une période :

* **Période prédéfinie** - Dans le menu Rapport prédéfini , sélectionnez une option. Par exemple, choisissez Le mois dernier pour capturer les données du mois précédent.

* **Période personnalisée** - Dans le menu Rapport prédéfini, sélectionnez **[!UICONTROL Personnalisé]**. Sélectionnez ensuite une date sur la page **[!UICONTROL Mois de début]** (ou **[!UICONTROL Date de début]**) et une date dans le menu Nombre de mois (ou Nombre ou Jours) . Pour les rapports de domaine ou de contenu vidéo, vous pouvez choisir une date de début et une date de fin spécifiques pour la capture des informations du rapport.

* **Tri des données (vue Données uniquement)** - Pour trier les informations sur une colonne, sélectionnez l’en-tête de la colonne. Sélectionnez à nouveau pour trier dans l’ordre décroissant.

* **Réorganiser les colonnes (vue Données uniquement)** - Pour déplacer une colonne vers un autre emplacement de la grille de données, faites glisser son en-tête.

### Exporter et imprimer des rapports {#exporting-and-printing-reports}

Après avoir généré un rapport, vous pouvez exporter ses données pour une utilisation dans des feuilles de calcul et d’autres applications. Vous pouvez également imprimer des rapports.

* **Exporter les données de rapport** - Dans la vue Données, triez et organisez les données selon vos besoins. Ouvrez ensuite le **[!UICONTROL Exporter]** et choisissez un format : **[!UICONTROL Délimité par tabulation]**, **[!UICONTROL Séparée par une virgule]**, ou **[!UICONTROL HTML formaté]**. Les données sont copiées dans le Presse-papiers au format que vous choisissez. Vous pouvez à présent coller les données dans une feuille de calcul ou une application.

* **Imprimer un rapport** - Sélectionner **[!UICONTROL Imprimer]**, choisissez les options de votre choix dans la boîte de dialogue Imprimer, puis sélectionnez **[!UICONTROL OK]**.

## Erreurs d’image {#image-errors}

Les administrateurs Adobe Dynamic Media Classic peuvent générer des rapports d’erreurs d’image. Un rapport d’erreurs d’image fournit la liste des 20 erreurs d’image les plus fréquentes sur les dernières 24 heures, pour l’entreprise à laquelle vous êtes actuellement connecté. Pour générer un rapport d’erreur d’image, procédez comme suit :

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration personnelle]**.
1. Développez Configuration de l’administration, puis sélectionnez **[!UICONTROL Erreurs d’image]**.
1. (Facultatif) Utilisez l’une des méthodes suivantes :

   * Pour trier les erreurs selon les informations d’en-tête, sélectionnez un en-tête. Par défaut, les erreurs sont triées par nombre d’occurrences, du plus élevé au moins élevé.
   * Placez le curseur sur le champ Réponse d’une erreur pour afficher le message d’erreur correspondant.
   * Pour afficher le lien vers l’image ou la page web du référent, placez le curseur sur le champ URL ou le champ Référent .
   * Pour copier le lien vers l’image, sélectionnez **[!UICONTROL URL de copie d’URL]**. Vous pouvez coller ce lien dans un navigateur pour accéder à l’image et étudier l’erreur.
   * Pour copier le lien vers la page web du référent, sélectionnez **[!UICONTROL URL de copie de référent]**.

Les erreurs affichées concernent la société à laquelle vous êtes actuellement connecté. Les informations suivantes sont indiquées pour chaque erreur :

* **ID d’image** - Identifiant de l’image offensante.

* **Heure** - La période de la première fois où l’erreur a été signalée à la dernière fois où l’erreur a été signalée, au cours des dernières 24 heures.

* **Count** - Nombre d’erreurs signalées sur l’image.

* **Réponse** - Message d’erreur spécifique. Les erreurs sont soit 4xx soit 5xx.

* **URL** - Répertorie l’URL de l’image sur Adobe Dynamic Media Classic.

* **Référent** : indique l’URL du site web d’où provient la requête initiale. Le référant peut être n’importe quel site Web contenant un lien vers l’image.

Les colonnes URL et Référent disposent de boutons Copier l’URL qui permettent de simplifier les tests.
