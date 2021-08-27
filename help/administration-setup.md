---
title: Configuration de l’administration
description: Découvrez comment configurer la zone d’administration d’Adobe Dynamic Media Classic.
uuid: 16ba9fed-b5c6-4991-83b3-8d7d7129013a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 3c9ee4ec-dd37-498d-98d6-1339b80177ff
feature: Dynamic Media Classic
role: Admin
exl-id: 14e3d8be-f265-4cec-aa8e-19ef71526b68
source-git-commit: ad5270545be502d3aaabba574353787622ab0445
workflow-type: tm+mt
source-wordcount: '1966'
ht-degree: 36%

---

<!-- UPDATE TOPIC AFTER DECEMBER 31, 2020!!!! -->

# Configuration de l’administration{#administration-setup}

Les écrans Configuration de l’administration permettent d’administrer les utilisateurs d’Adobe Dynamic Media Classic. Utilisez ces écrans pour permettre aux utilisateurs de travailler dans Adobe Dynamic Media Classic et de communiquer par e-mail avec les utilisateurs.

1. Pour accéder aux options Configuration de l’administration, accédez à **Configuration** > **Configuration personnelle** > **Configuration de l’administration**.

## Administration utilisateur {#user-administration}

Tous les utilisateurs d’Adobe Dynamic Media Classic se voient attribuer un rôle qui détermine leurs privilèges et droits d’accès aux fonctionnalités d’Adobe Dynamic Media Classic. Les administrateurs définissent les différents rôles et responsabilités pour les entreprises auxquelles ils sont affectés.

En règle générale, Adobe Dynamic Media Classic configure le premier ensemble d’entreprises et affecte un administrateur d’entreprise. L’administrateur de l’entreprise configure et administre ensuite les utilisateurs d’Adobe Dynamic Media Classic.

Adobe Dynamic Media Classic prend en charge plusieurs rôles d’utilisateur. Ces rôles peuvent accéder aux entreprises configurées pour Adobe Dynamic Media Classic :

<!-- **Adobe Dynamic Media Classic Administrator** Can view and administer all features in Adobe Dynamic Media Classic, as well as set up companies and add administrators and users. -->

**Adobe** Utilisateur Dynamic Media Classic Peut accéder aux entreprises auxquelles elles ont été affectées ; ne peuvent pas effectuer de tâches administratives.

**Adobe Dynamic Media Classic Company** AdminPeut afficher et administrer uniquement leurs propres entreprises. Il peut également remplir toutes les fonctions d’administration, notamment l’ajout d’administrateurs et d’utilisateurs. Un administrateur d’entreprise peut ajouter un utilisateur aux comptes administrateur d’entreprise DMC. (Ce rôle est le rôle utilisateur par défaut.)

Une fois que vous avez ajouté un utilisateur, Adobe Dynamic Media Classic lui envoie un e-mail de bienvenue. Le message comprend un mot de passe et l’URL Adobe Dynamic Media Classic.

### Ajout d’un utilisateur ou d’un administrateur {#adding-a-user-or-administrator}

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Configuration de l’administration]** > **[!UICONTROL Administration des utilisateurs]**.
1. Sélectionnez **[!UICONTROL Ajouter]**.
1. Saisissez le nom et l’adresse email de l’utilisateur ou de l’administrateur que vous souhaitez ajouter, puis sélectionnez **[!UICONTROL Suivant]**.

   >[!NOTE]
   >
   >Le caractère apostrophe (`‘`) n’est pas autorisé dans les adresses électroniques.

1. Pour attribuer un rôle à l’utilisateur, sélectionnez une option Rôle .

   Voir [Adobe des rôles utilisateur et des privilèges Dynamic Media Classic](administration-setup.md#user_administration).

1. Pour ajouter un utilisateur à une société, sélectionnez son nom.
1. Si vous souhaitez ajouter l’utilisateur à un groupe (si vous ajoutez un utilisateur ou un contributeur Media Portal), sélectionnez **[!UICONTROL Suivant]** et ajoutez l’utilisateur.
1. Sélectionnez **[!UICONTROL Enregistrer]** pour terminer la configuration de l’utilisateur.

   Après l’enregistrement, une invite demande si vous souhaitez ajouter un utilisateur à une autre société. Sélectionnez **[!UICONTROL Ajouter]** si vous souhaitez ajouter l’utilisateur à une société.

   Tous les nouveaux utilisateurs reçoivent un mot de passe généré de manière aléatoire ; Les utilisateurs doivent changer de mot de passe la première fois qu’ils se connectent à l’application de bureau Dynamic Media Classic Adobe.

   Un e-mail de bienvenue est envoyé aux utilisateurs une fois qu’ils ont été ajoutés. L’e-mail fournit un mot de passe temporaire et explique comment vous connecter à Adobe Dynamic Media Classic.

   Si l’utilisateur ne reçoit pas l’e-mail de bienvenue, demandez-lui d’accéder à la page de connexion d’Adobe Dynamic Media Classic (https://s7sps1.scene7.com), puis sélectionnez **[!UICONTROL Mon mot de passe oublié]**. Le mot de passe est réinitialisé et un nouveau courrier électronique est envoyé. Si l’utilisateur ne reçoit pas le courrier électronique et qu’il n’est pas placé dans le dossier du courrier indésirable, contactez le support technique.

   Lors de l’ajout de nouveaux utilisateurs Media Portal, vous pouvez également accéder à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Administration des utilisateurs]**, sélectionner **[!UICONTROL Télécharger la liste des utilisateurs]** et sélectionner un fichier .csv ne contenant pas plus de 500 utilisateurs.

### Suppression d’un utilisateur {#deleting-a-user}

Vous pouvez supprimer des utilisateurs d’Adobe Dynamic Media Classic en les rendant non valides. Les utilisateurs non valides sont supprimés du système et de tous les comptes.

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Configuration de l’administration]** > **[!UICONTROL Administration des utilisateurs]**.
1. Sélectionnez un utilisateur dans la liste, puis **[!UICONTROL Modifier]**.
1. Désélectionnez l’option Valide.
1. Sélectionnez **[!UICONTROL Enregistrer]**.

### Activation ou désactivation d’utilisateurs {#activating-or-deactivating-users}

Les utilisateurs désactivés n’ont plus le droit d’accéder au compte indiqué en haut du menu Sélectionner le compte auquel accéder.

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Configuration de l’administration]** > **[!UICONTROL Administration des utilisateurs]**.
1. Dans la liste des utilisateurs, sélectionnez ou désélectionnez l’option **[!UICONTROL Principale]** en regard du nom de l’utilisateur.

### Modification des informations de l’utilisateur {#editing-user-information}

Les informations sur l’utilisateur que vous pouvez modifier dépendent de votre rôle en tant qu’administrateur et du rôle de l’utilisateur dont vous souhaitez modifier les informations. Les options qui apparaissent en grisé (non disponibles) ne sont pas modifiables.

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Configuration de l’administration]** > **[!UICONTROL Administration des utilisateurs]**.
1. Sélectionnez un utilisateur dans la liste, puis **[!UICONTROL Modifier]**.
1. Sélectionnez l’entrée dans le tableau qui indique la société pour laquelle vous essayez de modifier les autorisations ou l’accès, puis sélectionnez **[!UICONTROL Gérer la société]**.
1. Sélectionnez le rôle de l’utilisateur.
1. Si vous souhaitez modifier l’appartenance au groupe de l’utilisateur (si vous modifiez ou ajoutez un utilisateur ou contributeur Media Portal), sélectionnez **[!UICONTROL Suivant]** et modifiez l’appartenance au groupe.
1. Sélectionnez **[!UICONTROL Enregistrer]**.

### Filtrage et tri de la liste des utilisateurs {#filtering-and-sorting-the-user-list}

Vous pouvez filtrer et trier la liste des utilisateurs afin de localiser les utilisateurs. Tous les utilisateurs figurant dans tous les comptes que vous gérez sont répertoriés dans la liste des utilisateurs, quel que soit le compte sélectionné dans le menu Sélectionner le compte auquel accéder.

Vous pouvez utiliser les techniques de filtrage suivantes :

* **Filtrer par groupe**  : sélectionnez le menu  **[!UICONTROL Par]** groupe et choisissez une option pour restreindre la liste aux utilisateurs d’un groupe.

* **Filtrer par rôle utilisateur**  : sélectionnez  **[!UICONTROL Par rôle utilisateur]** Rolemenu et choisissez une option pour restreindre la liste aux utilisateurs ou administrateurs de différents types.

* **Filtrer par nom de champ**  : sélectionnez  **[!UICONTROL Activer le filtre par champ]**. Sélectionnez ensuite le menu **[!UICONTROL Par nom de champ]**, choisissez une colonne pour filtrer la liste, sélectionnez le menu Filtrer les caractères et choisissez une lettre. La liste est filtrée en fonction d’une des colonnes selon la lettre que vous avez choisie. Pour afficher la liste complète, désélectionnez l’option **[!UICONTROL Activer le filtre par champ]** .

* **Filtrer les utilisateurs non valides**  - Désélectionnez  **[!UICONTROL Inclure non valide]**. Les résultats de la recherche affichent uniquement les utilisateurs présents dans le système. Les utilisateurs non valides ont été supprimés du système et des comptes que vous gérez.

* **Tri par en-tête**  de colonne : sélectionnez un en-tête pour trier tous les utilisateurs selon leur état, par ordre alphabétique de prénom, nom ou adresse électronique, par rôle d’utilisateur ou par statut valide/non valide.

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

      Replace “N” in the above path with the number for your IPS company region. That is, N = 1 for North America; 3 for EMEA; or 5 for JAPAC.
 -->

## Bande passante et stockage {#bandwidth-storage}

Les administrateurs d’Adobe Dynamic Media Classic peuvent générer de la bande passante, du stockage et d’autres types de rapports pour les entreprises qu’ils gèrent. Ces rapports sont disponibles sur la page Bande passante et stockage .

Pour ouvrir cette page, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration personnelle]**. Développez **[!UICONTROL Configuration de l’administration]**, puis sélectionnez **[!UICONTROL Bande passante et stockage]**.

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

* **Demande d’image**  : demandes d’images.

* **Demande de miniature**  : demandes d’échantillon ou d’images de remplacement dans les visionneuses.

* **Requête de masque**  : demandes d’images renvoyant des masques en niveaux de gris.

* **Requête de mosaïque de visionneuse**  : demandes d’image chargées par une visionneuse.

* **Demande d’objet Vnt**  : demandes de rendu d’image qui renvoient une image avec des objets spécifiés dans les vignettes demandées.

* **Demande d’informations sur le Vnt**  : demandes de rendu d’image qui renvoient des informations relatives aux vignettes demandées.

>[!NOTE]
>
>le rapport Diffusion de vidéo en flux continu s’applique uniquement aux vidéos diffusées en flux continu. Il ne rend nullement compte des vidéos en cours de visionnage.

### Générer un rapport {#generating-a-report}

Pour générer un rapport de bande passante, stockage, contenu de l’image, domaine, diffusion en flux continu de vidéo ou contenu de la vidéo :

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration personnelle]**.
1. Développez Configuration de l’administration, puis sélectionnez **[!UICONTROL Bande passante et stockage]**.
1. Sélectionnez un onglet : **[!UICONTROL Bande passante]**, **[!UICONTROL Stockage]**, **[!UICONTROL Contenu de l’image]**, **[!UICONTROL Domaine]**, **[!UICONTROL Diffusion vidéo en continu]** ou **[!UICONTROL Contenu vidéo]**.

   Voir [Types de rapports](administration-setup.md#types_of_reports).

### Affichage des données de différentes manières {#viewing-data-in-different-ways}

Après avoir généré un rapport sur la page Bande passante et stockage, vous pouvez choisir des options pour l’affichage des informations. Vous pouvez choisir le mode de présentation des informations, afficher les informations dans un tableau ou une grille de données et indiquer une période pour la capture des informations. En mode Affichage des données, vous pouvez également trier les informations et réorganiser les colonnes.

* **Afficher les données dans un graphique ou une grille de données**  : sélectionnez  **[!UICONTROL Affichage du graphique]** pour afficher les données dans un graphique. sélectionnez  **[!UICONTROL Visionneuse de données]** pour afficher les données dans une grille de données.

* **Choisissez un type de présentation de rapport**  : dans le menu Type de rapport, sélectionnez  **[!UICONTROL Résumé]**,  **[!UICONTROL Quotidien]** ou  **** Mois pour organiser les données sous forme de synthèse, par jour ou par mois. Tous les rapports ne proposent pas cette option.

* **Spécifiez une période**  : choisissez des options pour définir une période pour votre rapport, puis sélectionnez  **** Mettre à jour après avoir défini une période :

* **Période prédéfinie**  : dans le menu Rapport prédéfini, sélectionnez une option. Par exemple, choisissez Le mois dernier pour capturer les données du mois précédent.

* **Période personnalisée**  : dans le menu Rapport prédéfini, sélectionnez  **[!UICONTROL Personnalisé]**. Choisissez ensuite une date dans le menu **[!UICONTROL Début du mois]** (ou **[!UICONTROL Date de début]**) et une date dans le menu # ou Jours (Nombre de mois). Pour les rapports de domaine ou de contenu vidéo, vous pouvez choisir une date de début et une date de fin spécifiques pour la capture des informations du rapport.

* **Tri des données (vue des données uniquement)**  : pour trier les informations sur une colonne, sélectionnez l’en-tête de la colonne. Sélectionnez à nouveau pour trier dans l’ordre décroissant.

* **Réorganiser les colonnes (vue Données uniquement)**  : pour déplacer une colonne vers un autre emplacement de la grille de données, faites glisser son en-tête.

### Exporter et imprimer des rapports {#exporting-and-printing-reports}

Après avoir généré un rapport, vous pouvez exporter ses données pour une utilisation dans des feuilles de calcul et d’autres applications. Vous pouvez également imprimer des rapports.

* **Exporter les données**  du rapport : dans la vue Données, triez et organisez les données selon vos besoins. Ouvrez ensuite le menu **[!UICONTROL Export]** et choisissez un format : **[!UICONTROL Tabulation délimitée]**, **[!UICONTROL Virgule séparée]** ou **[!UICONTROL Format HTML]**. Les données sont copiées dans le Presse-papiers au format choisi. Vous pouvez à présent coller les données dans une feuille de calcul ou une application.

* **Imprimer un rapport**  : sélectionnez  **[!UICONTROL Imprimer]**, choisissez les options de votre choix dans la boîte de dialogue Imprimer, puis sélectionnez  **[!UICONTROL OK]**.

## Erreurs d’image {#image-errors}

Les administrateurs d’Adobe Dynamic Media Classic peuvent générer des rapports d’erreur d’image. Un rapport d’erreurs d’image fournit la liste des 20 erreurs d’image les plus fréquentes sur les dernières 24 heures, pour l’entreprise à laquelle vous êtes actuellement connecté. Pour générer un rapport d’erreur d’image, procédez comme suit :

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration personnelle]**.
1. Développez Configuration de l’administration, puis sélectionnez **[!UICONTROL Erreurs d’image]**.
1. (Facultatif) Utilisez l’une des méthodes suivantes :

   * Pour trier les erreurs selon les informations d’en-tête, sélectionnez un en-tête. Par défaut, les erreurs sont triées par nombre d’occurrences, du plus élevé au moins élevé.
   * Placez le curseur sur le champ Réponse d’une erreur pour afficher le message d’erreur correspondant.
   * Pour afficher le lien vers l’image ou la page web du référent, placez le curseur sur le champ URL ou le champ Référent .
   * Pour copier le lien vers l’image, sélectionnez **[!UICONTROL URL Copier l’URL]**. Vous pouvez coller ce lien dans un navigateur pour accéder à l’image et étudier l’erreur.
   * Pour copier le lien vers la page web du référent, sélectionnez **[!UICONTROL URL de copie du référent]**.

Les erreurs s’affichent pour la société à laquelle vous êtes actuellement connecté. Les informations suivantes sont indiquées pour chaque erreur :

* **ID d’image**  : ID de l’image offensante.

* **Heure**  : période de la première fois où l’erreur a été signalée à la dernière fois où l’erreur a été signalée, au cours des dernières 24 heures.

* **Comptage**  : nombre d’erreurs signalées sur l’image.

* **Réponse**  : message d’erreur spécifique. Les erreurs sont soit 4xx soit 5xx.

* **URL**  : répertorie l’URL de l’image sur Adobe Dynamic Media Classic.

* **Référent**  : indique l’URL du site web d’où provient la requête initiale. Le référant peut être n’importe quel site Web contenant un lien vers l’image.

Les colonnes URL et Référent disposent de boutons Copier l’URL qui permettent de simplifier les tests.
