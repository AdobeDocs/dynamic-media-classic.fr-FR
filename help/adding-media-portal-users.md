---
title: Ajout et gestion des utilisateurs du portail multimédia
seo-title: Ajout et gestion des utilisateurs du portail multimédia
description: 'null'
seo-description: Découvrez comment ajouter et gérer les utilisateurs du portail multimédia
uuid: 96 d 4103 c -6428-4 ce 1-b 9 e 4-231599304 f 27
contentOwner: admin
content-type: référence
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/media_ portal
discoiquuid: 5 e 933045-ce 1 a -41 b 9-ba 8 b -2151 c 396 b 7 a 2
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Ajout et gestion des utilisateurs du portail multimédia{#adding-and-managing-media-portal-users}

En tant qu’administrateur, vous pouvez ajouter et gérer des utilisateurs, définir s’ils peuvent modifier leur mot de passe, modifier les informations utilisateur et télécharger des listes d’utilisateurs. Ces tâches sont accomplies à partir de l’écran Administration utilisateur. Pour accéder à cet écran, choisissez **Configuration** &gt; **Configuration de l’application** &gt; **Configuration de l’administration** &gt; **Administration utilisateur**.

>[!NOTE]
>
>avant d’ajouter des utilisateurs, configurez des groupes chargés de les administrer. Le portail multimédia ne vous laisse pas ajouter un utilisateur sans l’affecter à un ou plusieurs groupes. Pour plus d’informations, voir [Création et gestion des groupes du portail multimédia](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

## Gestion des mots de passe du portail multimédia {#handling-media-portal-passwords}

Lorsque leur inscription est validée, les utilisateurs, les contributeurs et les contributeurs-utilisateurs du portail multimédia reçoivent un message électronique de bienvenue dans lequel figure un mot de passe. Les administrateurs peuvent déterminer si les utilisateurs du portail multimédia sont autorisés à modifier ce mot de passe.

1. Cliquez sur **Configuration** &gt; **Configuration de Media Portal** &gt; **Paramètres généraux**.
1. Dans la page Paramètres généraux, sélectionnez ou désélectionnez l’option **Autoriser l’utilisateur Media Portal à modifier le mot de passe**.
1. Cliquez sur **Enregistrer**.

>[!NOTE]
>
>les utilisateurs du portail multimédia autorisés à modifier leur mot de passe peuvent procéder à cette modification en cliquant sur **Configuration** &gt; **Configuration personnelle**, puis en modifiant le mot de passe dans l’écran Configuration personnelle.

## Ajout d’un utilisateur au portail multimédia {#adding-a-media-portal-user}

1. Cliquez sur **Configuration** &gt; **Configuration de l’application** &gt; **Configuration de l’administration** &gt; **Administration utilisateur**.
1. Sur la page Administration utilisateur, cliquez sur **Ajouter**.
1. Dans la boîte de dialogue Ajouter un utilisateur, dans le panneau Informations utilisateur, entrez les prénom, nom et adresse électronique de l’utilisateur, puis cliquez sur **Suivant**.
1. Dans le panneau Entreprise/Fonction, dans la liste déroulante des entreprises, sélectionnez une ou plusieurs entreprises pour l’utilisateur.
1. Dans la liste des fonctions, sélectionnez une fonction du portail multimédia, puis cliquez sur **Suivant**.

   Voir [Rôles utilisateur du portail multimédia](media-portal-user-roles.md#media_portal_user_roles).

1. Dans le panneau des Groupes d’accès, sélectionnez un ou plusieurs groupes.

   Voir [Création et gestion des groupes du portail multimédia](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

1. (Facultatif) Cliquez sur **Paramètres d’e-mail** pour choisir d’autres paramètres d’e-mail dans les paramètres par défaut.

   Voir [Définition du message de l’e-mail de bienvenue pour les utilisateurs du portail multimédia](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users).

1. Cliquez sur **Ajouter un utilisateur**.

Une fois que vous avez ajouté un utilisateur, le portail multimédia lui envoie un e-mail de bienvenue. Le message comprend un mot de passe temporaire et l’URL du portail multimédia.

## Téléchargement d’une liste d’utilisateurs du portail multimédia {#uploading-a-media-portal-user-list}

Si vous devez ajouter de nombreux utilisateurs, vous pouvez télécharger une liste d’utilisateurs. Ceux-ci seront automatiquement ajoutés au compte sélectionné.

Créez la liste d’utilisateurs au format de fichier CSV (valeurs séparées par des virgules). Une fois la liste téléchargée, les utilisateurs y figurant sont automatiquement ajoutés au compte avec leurs attributions de groupe. Un e-mail de bienvenue est envoyé à chaque nouvel utilisateur, avec un lien vers le portail multimédia et un mot de passe temporaire.

### Création du fichier CSV {#creating-the-csv-file}

Créez un fichier CSV (nom_de_fichier.csv) conforme au format et aux champs suivants. La première ligne du fichier doit contenir les en-têtes de colonne indiqués dans ce tableau. Vous pouvez trier ces colonnes selon vos souhaits. Toutes les colonnes sont obligatoires.

| Nom de la colonne | Description |
|--- |--- |
| Prénom | Contient le prénom. |
| Nom | Contient le nom. |
| E-mail | Contient une adresse de messagerie valide. |
| Mot de passe | Contient une chaîne de mot de passe sensible à la casse. |
| Rôle utilisateur | Mediaportaladminmediaportalusermediaportalcontributormediaportalcontributoruser |
| Groupes | Liste d’une ou de plusieurs attributions de groupe de compte pour chaque utilisateur, séparées par des virgules. Vous définissez le groupe en y ajoutant le nom du compte en préfixe, séparé par une barre oblique (/). Par exemple, PortalCo/IT, où PortalCo correspond au compte et IT au groupe du compte PortalCo. |

L’exemple de feuille de calcul ci-dessous montre la disposition d’un fichier CSV :

| Prénom | Nom | E-mail | Mot de passe | Rôle utilisateur | Groupes |
|--- |--- |--- |--- |--- |--- |
| Peter | Peterson | `petep@company.com` | bienvenue | MediaPortalAdmin | PortalCo/IT,PortalCo/Admin |
| Kevin | Marks | `kevinm@myco.com` | bienvenue | Utilisateur du portail multimédia | PortalCo/MktgGroup, PortalCo/test |


### Téléchargement du fichier CSV {#uploading-the-csv-file}

1. Ouvrez l’écran de configuration de l’administration utilisateur.
1. Cliquez sur **Télécharger liste utilisateurs**.
1. Dans la boîte de dialogue Sélectionner un fichier à télécharger, sélectionnez le fichier CSV, puis cliquez sur **Ouvrir**.

Chaque utilisateur de la liste est automatiquement ajouté aux groupes spécifiés Un message de bienvenue est envoyé à chacun d’eux.

>[!NOTE]
si le fichier CSV n’a pas été correctement mis en forme, le message d’erreur suivant s’affiche : « Une erreur est survenue pendant le traitement du fichier CSV téléchargé. Veuillez vérifier que les données du fichier sont valides ». En outre, si le fichier CSV contient un utilisateur IP ou IPS existant, cet utilisateur n’est pas ajouté à la liste des utilisateurs.

## Génération d’une liste d’utilisateurs du portail multimédia disponible à la sélection {#generating-a-selectable-list-of-media-portal-users}

Vous pouvez afficher les noms et les adresses e-mail des utilisateurs du portail multimédia dans une fenêtre contextuelle. Cette liste est utile pour couper et coller des noms d’utilisateur et des adresses qui seront utilisés à l’extérieur du portail multimédia.

1. Cliquez sur **Configuration** &gt; **Configuration de l’application** &gt; **Configuration de l’administration** &gt; **Administration utilisateur**.
1. Dans la liste **Par rôle utilisateur**, choisissez le nom d’un rôle utilisateur du portail multimédia, puis cliquez sur **Actualiser** afin d’afficher uniquement les noms d’une seule catégorie d’utilisateurs du portail multimédia.
1. Cliquez sur **Liste contextuelle** pour ouvrir la fenêtre contextuelle. Vous pouvez copier et coller cette liste.

## Définition du message de l’e-mail de bienvenue pour les utilisateurs du portail multimédia {#setting-up-the-welcome-e-mail-message-for-media-portal-users}

Vous pouvez envoyer un e-mail de bienvenue à tous les nouveaux utilisateurs, contributeurs et contributeurs-utilisateurs du portail multimédia. Vous pouvez configurer ce message électronique ou indiquer à Dynamic Media Classic de ne pas l'envoyer.

1. Choisissez **Configuration** &gt; **Configuration de l’application** &gt; **Configuration de l’administration** &gt; **Administration utilisateur**.
1. In the User Administration Setup screen, click **Email Settings**.
1. Dans la boîte de dialogue Paramètres d’e-mail, définissez les paramètres suivants à votre convenance :

   **Envoyer un courrier électronique** Désélectionnez cette option si vous ne souhaitez pas envoyer par e-mail aux nouveaux utilisateurs un e-mail que vous leur avez ajouté.

   **Mot de passe par défaut** Saisissez un mot de passe temporaire pour les nouveaux utilisateurs ou laissez le champ vide pour que Dynamic Media Classic génère des mots de passe aléatoires. Les utilisateurs sont invités à modifier leur mot de passe lors de la première connexion.

   **URL de remplacement** Saisissez une URL différente de la valeur par défaut si vos utilisateurs accèdent à Dynamic Media Classic via une autre URL.

## Autres tâches de gestion des utilisateurs {#other-user-management-tasks}

L’écran de configuration de l’administration utilisateur vous permet d’effectuer les tâches suivantes :

**Filtrage et tri de la liste des utilisateurs** Filtrez la liste des utilisateurs du portail multimédia pour localiser les utilisateurs. (voir Filtrage et tri de la liste des utilisateurs).

**Supprimer les utilisateurs** Supprimez un utilisateur de la liste. (voir Suppression d’un utilisateur.

**Activer et désactiver les utilisateurs** Suspendez un utilisateur de l'accès aux dossiers. (voir Activation et désactivation d’utilisateurs).

**Modifier les informations** de l'utilisateur Saisissez des informations à jour sur un utilisateur. (voir Modification des informations de l’utilisateur).

**Création de champs définis par l'utilisateur** Créez des champs de métadonnées personnalisés définis par l'utilisateur pour organiser les fichiers dans Scene 7 Publishing System. Les champs peuvent également être activés ou désactivés, le cas échéant.

(Voir [Champs définis par l’utilisateur](application-setup.md#user_defined_fields).)
