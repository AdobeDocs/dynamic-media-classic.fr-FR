---
title: Ajout et gestion des utilisateurs de Media Portal
description: Découvrez comment ajouter et gérer des utilisateurs Media Portal dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: 9590c53c-fd38-4bf2-b723-cd7369702364
topic: Administration
level: Intermediate
source-git-commit: bb229047c0c9b3855453ea15dcd1f9754bc65cef
workflow-type: tm+mt
source-wordcount: '1008'
ht-degree: 50%

---

# Ajout et gestion des utilisateurs de Media Portal{#adding-and-managing-media-portal-users}

En tant qu’administrateur, vous pouvez ajouter et gérer des utilisateurs, définir s’ils peuvent modifier leur mot de passe, modifier les informations utilisateur et télécharger des listes d’utilisateurs. Ces tâches sont accomplies à partir de l’écran Administration utilisateur. Pour accéder à cet écran, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Configuration de l’administration]** > **[!UICONTROL Administration des utilisateurs]**.

>[!NOTE]
>
>avant d’ajouter des utilisateurs, configurez des groupes chargés de les administrer. Media Portal permet d’ajouter un utilisateur en l’affectant à un ou plusieurs groupes. Pour plus d’informations, voir [Création et gestion des groupes Media Portal](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

## Administration des mots de passe Media Portal {#handling-media-portal-passwords}

Lorsque leur inscription est validée, les utilisateurs, les contributeurs et les contributeurs-utilisateurs du portail multimédia reçoivent un message électronique de bienvenue dans lequel figure un mot de passe. Les administrateurs peuvent déterminer si les utilisateurs du portail multimédia sont autorisés à modifier ce mot de passe.

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de Media Portal]** > **[!UICONTROL Paramètres généraux]**.
1. Dans la page Paramètres généraux, sélectionnez ou désélectionnez l’option **[!UICONTROL Autoriser l’utilisateur Media Portal à modifier le mot de passe]**.
1. Sélectionner **[!UICONTROL Enregistrer]**.

>[!NOTE]
>
>Les utilisateurs du portail multimédia autorisés à modifier des mots de passe peuvent le faire en sélectionnant **[!UICONTROL Configuration]** > **[!UICONTROL Configuration personnelle]** et la modification des mots de passe dans l’écran Configuration personnelle .

## Ajout d’un utilisateur Media Portal {#adding-a-media-portal-user}

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Configuration de l’administration]** > **[!UICONTROL Administration des utilisateurs]**.
1. Sur la page Administration des utilisateurs, sélectionnez **Ajouter**.
1. Dans le **[!UICONTROL `Add User`]** dans le panneau Informations utilisateur, saisissez le prénom, le nom et l’adresse électronique de l’utilisateur, puis sélectionnez **[!UICONTROL Suivant]**.
1. Dans le panneau Entreprise/Fonction, dans la liste déroulante des entreprises, sélectionnez une ou plusieurs entreprises pour l’utilisateur.
1. Dans la liste Rôle, sélectionnez un rôle Media Portal, puis sélectionnez **[!UICONTROL Suivant]**.

   Voir [Rôles utilisateur du portail multimédia](media-portal-user-roles.md#media_portal_user_roles).

1. Dans le panneau des Groupes d’accès, sélectionnez un ou plusieurs groupes.

   Voir [Création et gestion des groupes Media Portal](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

1. (Facultatif) Sélectionnez **[!UICONTROL Paramètres de messagerie électronique]** pour sélectionner des paramètres d’email différents des paramètres par défaut.

   Voir [Définition du message de l’e-mail de bienvenue pour les utilisateurs du portail multimédia](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users).

1. Sélectionner **[!UICONTROL Ajouter un utilisateur]**.

Une fois que vous avez ajouté un utilisateur, le portail multimédia lui envoie un e-mail de bienvenue. Le message comprend un mot de passe temporaire et l’URL du portail multimédia.

## Téléchargement d’une liste d’utilisateurs du portail multimédia {#uploading-a-media-portal-user-list}

Si vous devez ajouter de nombreux utilisateurs, vous pouvez télécharger une liste d’utilisateurs. Ceux-ci seront automatiquement ajoutés au compte sélectionné.

Créez la liste d’utilisateurs au format de fichier CSV (valeurs séparées par des virgules). Une fois la liste téléchargée, les utilisateurs y figurant sont automatiquement ajoutés au compte avec leurs attributions de groupe. Un e-mail de bienvenue est envoyé à chaque nouvel utilisateur, avec un lien vers le portail multimédia et un mot de passe temporaire.

### Création du fichier CSV {#create-the-csv-file}

Créez un fichier CSV (nom_de_fichier.csv) conforme au format et aux champs suivants. La première ligne du fichier doit contenir les en-têtes de colonne indiqués dans ce tableau. Vous pouvez trier ces colonnes selon vos souhaits. Toutes les colonnes sont obligatoires.

| Nom de la colonne | Description |
|--- |--- |
| Prénom | Contient le prénom. |
| Nom | Contient le nom. |
| E-mail | Contient une adresse de messagerie valide. |
| Mot de passe | Contient une chaîne de mot de passe sensible à la casse. |
| Rôle utilisateur | MediaPortalAdminMediaPortalUserMediaPortalContributorMediaPortalContributorContributorUser |
| Groupes | Liste d’une ou de plusieurs attributions de groupe de compte pour chaque utilisateur, séparées par des virgules. Vous définissez le groupe en y ajoutant le nom du compte en préfixe, séparé par une barre oblique (/). Par exemple, PortalCo/IT, où PortalCo correspond au compte et IT au groupe du compte PortalCo. |

L’exemple de feuille de calcul ci-dessous montre la disposition d’un fichier CSV :

| Prénom | Nom | E-mail | Mot de passe | Rôle utilisateur | Groupes |
|--- |--- |--- |--- |--- |--- |
| Granite | Kat | `prairiek@company.com` | bienvenue | MediaPortalAdmin | PortalCo/IT, PortalCo/Admin |
| Rick | Broad | `rickb@myco.com` | bienvenue | Utilisateur du portail multimédia | PortalCo/MktgGroup, PortalCo/test |

### Téléchargement du fichier CSV {#uploading-the-csv-file}

1. Ouvrez l’écran de configuration de l’administration utilisateur.
1. Sélectionner **[!UICONTROL Télécharger la liste des utilisateurs]**.
1. Dans la boîte de dialogue Select File to Upload (Sélectionner un fichier à télécharger), sélectionnez le fichier CSV, puis sélectionnez **[!UICONTROL Ouvrir]**.

Chaque utilisateur de la liste est automatiquement ajouté aux groupes spécifiés. Un message de bienvenue est envoyé à chacun d’eux.

>[!NOTE]
>
>Si le fichier CSV n’a pas été correctement formaté, le message d’erreur suivant s’affiche : &quot;Une erreur s’est produite lors du traitement du fichier CSV transféré. Vérifiez que le contenu du fichier contient des données valides.&quot; En outre, si le fichier CSV contient un utilisateur IP ou IPS existant, l’utilisateur n’est pas ajouté à la liste des utilisateurs.

## Génération d’une liste d’utilisateurs du portail multimédia disponible à la sélection {#generating-a-selectable-list-of-media-portal-users}

Vous pouvez afficher les noms et les adresses e-mail des utilisateurs du portail multimédia dans une fenêtre contextuelle. Cette liste est utile pour couper et coller des noms d’utilisateur et des adresses qui seront utilisés à l’extérieur du portail multimédia.

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Configuration de l’administration]** > **[!UICONTROL Administration des utilisateurs]**.
1. Dans le **[!UICONTROL Par rôle d’utilisateur]** , choisissez le nom d’un rôle d’utilisateur Media Portal, puis sélectionnez **[!UICONTROL Actualiser]** pour afficher les noms d’une classe d’utilisateurs Media Portal.
1. Sélectionner **[!UICONTROL Liste déroulante]**. Copiez et collez cette liste.

## Définition du message de l’e-mail de bienvenue pour les utilisateurs du portail multimédia {#setting-up-the-welcome-e-mail-message-for-media-portal-users}

Vous pouvez envoyer un e-mail de bienvenue à tous les nouveaux utilisateurs, contributeurs et contributeurs-utilisateurs du portail multimédia. Vous pouvez configurer ce message électronique ou indiquer à Adobe Dynamic Media Classic de ne pas l’envoyer.

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Configuration de l’administration]** > **[!UICONTROL Administration des utilisateurs]**.
1. Dans l’écran Configuration de l’administration utilisateur, sélectionnez **[!UICONTROL Paramètres de messagerie électronique]**.
1. Dans la boîte de dialogue Paramètres d’e-mail, définissez les paramètres suivants à votre convenance :

   * **[!UICONTROL Envoyer un courrier électronique]**: désélectionnez cette option pour informer les nouveaux utilisateurs par e-mail que vous les avez inscrits.

   * **[!UICONTROL Mot de passe par défaut]**: saisissez un mot de passe temporaire pour les nouveaux utilisateurs ou laissez le champ vide pour qu’Adobe Dynamic Media Classic génère des mots de passe aléatoires. Les utilisateurs sont invités à modifier leurs mots de passe la première fois qu’ils se connectent.

   * **[!UICONTROL URL de remplacement]**: saisissez une URL différente de celle par défaut si vos utilisateurs accèdent à Adobe Dynamic Media Classic via une autre URL.

## Autres tâches de gestion des utilisateurs {#other-user-management-tasks}

L’écran de configuration de l’administration utilisateur vous permet d’effectuer les tâches suivantes :

* **[!UICONTROL Filtrage et tri de la liste des utilisateurs]**: filtrez la liste des utilisateurs de Media Portal pour localiser les utilisateurs.

* **[!UICONTROL Suppression d’utilisateurs]**: supprime un utilisateur de la liste.

* **[!UICONTROL Activation et désactivation des utilisateurs]**: empêche un utilisateur d’accéder aux dossiers.

* **[!UICONTROL Modification des informations utilisateur]**: saisissez les informations les plus récentes sur un utilisateur.

* **[!UICONTROL Création de champs définis par l’utilisateur]**: créez des champs de métadonnées personnalisés définis par l’utilisateur afin qu’ils vous aident à organiser les ressources dans Adobe Dynamic Media Classic. Les champs peuvent également être activés ou désactivés, le cas échéant.

(Voir [Champs définis par l’utilisateur](application-setup.md#user_defined_fields).)
