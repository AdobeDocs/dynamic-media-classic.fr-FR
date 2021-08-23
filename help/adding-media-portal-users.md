---
title: Ajout et gestion des utilisateurs de Media Portal
description: Découvrez comment ajouter et gérer des utilisateurs Media Portal dans Dynamic Media Classic.
uuid: 96d4103c-6428-4ce1-b9e4-231599304f27
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 5e933045-ce1a-41b9-ba8b-2151c396b7a2
feature: Dynamic Media Classic,Collaboration,Gestion des ressources
role: Admin,User
exl-id: 9590c53c-fd38-4bf2-b723-cd7369702364
source-git-commit: 1d30c98b76ebe78ff60bae87bd112de7a577182d
workflow-type: tm+mt
source-wordcount: '1018'
ht-degree: 58%

---

# Ajout et gestion des utilisateurs de Media Portal{#adding-and-managing-media-portal-users}

En tant qu’administrateur, vous pouvez ajouter et gérer des utilisateurs, définir s’ils peuvent modifier leur mot de passe, modifier les informations utilisateur et télécharger des listes d’utilisateurs. Ces tâches sont accomplies à partir de l’écran Administration utilisateur. Pour accéder à cet écran, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Configuration de l’administration]** > **[!UICONTROL Administration des utilisateurs]**.

>[!NOTE]
>
>avant d’ajouter des utilisateurs, configurez des groupes chargés de les administrer. Le portail multimédia ne vous laisse pas ajouter un utilisateur sans l’affecter à un ou plusieurs groupes. Pour plus d’informations, voir [Création et gestion des groupes Media Portal](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

## Administration des mots de passe Media Portal {#handling-media-portal-passwords}

Lorsque leur inscription est validée, les utilisateurs, les contributeurs et les contributeurs-utilisateurs du portail multimédia reçoivent un message électronique de bienvenue dans lequel figure un mot de passe. Les administrateurs peuvent déterminer si les utilisateurs du portail multimédia sont autorisés à modifier ce mot de passe.

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration du portail multimédia]** > **[!UICONTROL Paramètres généraux]**.
1. Dans la page Paramètres généraux, sélectionnez ou désélectionnez l’option **[!UICONTROL Autoriser l’utilisateur Media Portal à modifier le mot de passe]**.
1. Sélectionnez **[!UICONTROL Enregistrer]**.

>[!NOTE]
>
>Les utilisateurs du portail multimédia autorisés à modifier des mots de passe peuvent le faire en sélectionnant **[!UICONTROL Configuration]** > **[!UICONTROL Configuration personnelle]** et en modifiant les mots de passe dans l’écran Configuration personnelle .

## Ajout d’un utilisateur Media Portal {#adding-a-media-portal-user}

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Configuration de l’administration]** > **[!UICONTROL Administration des utilisateurs]**.
1. Sur la page Administration des utilisateurs, sélectionnez **Ajouter**.
1. Dans la boîte de dialogue Ajouter un utilisateur, dans le panneau Informations sur l’utilisateur, saisissez le prénom, le nom et l’adresse électronique de l’utilisateur, puis sélectionnez **[!UICONTROL Suivant]**.
1. Dans le panneau Entreprise/Fonction, dans la liste déroulante des entreprises, sélectionnez une ou plusieurs entreprises pour l’utilisateur.
1. Dans la liste Rôle, sélectionnez un rôle Media Portal, puis **[!UICONTROL Suivant]**.

   Voir [Rôles utilisateur du portail multimédia](media-portal-user-roles.md#media_portal_user_roles).

1. Dans le panneau des Groupes d’accès, sélectionnez un ou plusieurs groupes.

   Voir [Création et gestion des groupes Media Portal](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

1. (Facultatif) Sélectionnez **[!UICONTROL Paramètres d’e-mail]** pour choisir des paramètres d’e-mail différents des paramètres par défaut.

   Voir [Définition du message de l’e-mail de bienvenue pour les utilisateurs du portail multimédia](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users).

1. Sélectionnez **[!UICONTROL Ajouter un utilisateur]**.

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
| Rôle utilisateur | MediaPortalAdminMediaPortalUserMediaPortalContributorMediaPortalContributorContributorUser |
| Groupes | Liste d’une ou de plusieurs attributions de groupe de compte pour chaque utilisateur, séparées par des virgules. Vous définissez le groupe en y ajoutant le nom du compte en préfixe, séparé par une barre oblique (/). Par exemple, PortalCo/IT, où PortalCo correspond au compte et IT au groupe du compte PortalCo. |

L’exemple de feuille de calcul ci-dessous montre la disposition d’un fichier CSV :

| Prénom | Nom | E-mail | Mot de passe | Rôle utilisateur | Groupes |
|--- |--- |--- |--- |--- |--- |
| Parc | Kat | `prairiek@company.com` | bienvenue | MediaPortalAdmin | PortalCo/IT,PortalCo/Admin |
| Rick | Broad | `rickb@myco.com` | bienvenue | Utilisateur du portail multimédia | PortalCo/MktgGroup, PortalCo/test |

### Téléchargement du fichier CSV {#uploading-the-csv-file}

1. Ouvrez l’écran de configuration de l’administration utilisateur.
1. Sélectionnez **[!UICONTROL Transférer la liste des utilisateurs]**.
1. Dans la boîte de dialogue Select File to Upload (Sélectionner un fichier à télécharger), sélectionnez le fichier CSV, puis **[!UICONTROL Open]** (Ouvrir).

Chaque utilisateur de la liste est automatiquement ajouté aux groupes spécifiés Un message de bienvenue est envoyé à chacun d’eux.

>[!NOTE]
>
>si le fichier CSV n’a pas été correctement mis en forme, le message d’erreur suivant s’affiche : « Une erreur est survenue pendant le traitement du fichier CSV téléchargé. Veuillez vérifier que les données du fichier sont valides ». En outre, si le fichier CSV contient un utilisateur IP ou IPS existant, cet utilisateur n’est pas ajouté à la liste des utilisateurs.

## Génération d’une liste d’utilisateurs du portail multimédia disponible à la sélection {#generating-a-selectable-list-of-media-portal-users}

Vous pouvez afficher les noms et les adresses e-mail des utilisateurs du portail multimédia dans une fenêtre contextuelle. Cette liste est utile pour couper et coller des noms d’utilisateur et des adresses qui seront utilisés à l’extérieur du portail multimédia.

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Configuration de l’administration]** > **[!UICONTROL Administration des utilisateurs]**.
1. Dans la liste déroulante **[!UICONTROL Par rôle d’utilisateur]** , choisissez le nom d’un rôle d’utilisateur du portail multimédia, puis sélectionnez **[!UICONTROL Actualiser]** pour afficher les noms d’une classe d’utilisateurs du portail multimédia.
1. Sélectionnez **[!UICONTROL Liste contextuelle]**. Copiez et collez cette liste.

## Définition du message de l’e-mail de bienvenue pour les utilisateurs du portail multimédia {#setting-up-the-welcome-e-mail-message-for-media-portal-users}

Vous pouvez envoyer un e-mail de bienvenue à tous les nouveaux utilisateurs, contributeurs et contributeurs-utilisateurs du portail multimédia. Vous pouvez configurer ce message électronique ou indiquer à Dynamic Media Classic de ne pas l’envoyer.

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Configuration de l’administration]** > **[!UICONTROL Administration des utilisateurs]**.
1. Dans l’écran Configuration de l’administration des utilisateurs, sélectionnez **[!UICONTROL Paramètres des emails]**.
1. Dans la boîte de dialogue Paramètres d’e-mail, définissez les paramètres suivants à votre convenance :

   * **[!UICONTROL Envoyer un courrier électronique]**  : désélectionnez cette option si vous ne souhaitez pas informer les nouveaux utilisateurs par courrier électronique que vous les avez inscrits.

   * **[!UICONTROL Mot de passe par défaut]**  : saisissez un mot de passe temporaire pour les nouveaux utilisateurs ou laissez le champ vide pour que Dynamic Media Classic génère des mots de passe aléatoires. Les utilisateurs sont invités à modifier leurs mots de passe la première fois qu’ils se connectent.

   * **[!UICONTROL URL de remplacement]**  : saisissez une URL différente de celle par défaut si vos utilisateurs accèdent à Dynamic Media Classic par le biais d’une autre URL.

## Autres tâches de gestion des utilisateurs {#other-user-management-tasks}

L’écran de configuration de l’administration utilisateur vous permet d’effectuer les tâches suivantes :

* **[!UICONTROL Filtrer et trier la liste]**  des utilisateurs - Filtrez la liste des utilisateurs du portail multimédia pour localiser les utilisateurs.

* **[!UICONTROL Supprimer des utilisateurs]**  : supprimez un utilisateur de la liste.

* **[!UICONTROL Activer et désactiver des utilisateurs]**  : empêche un utilisateur d’accéder à des dossiers.

* **[!UICONTROL Modifier les informations sur l’utilisateur]**  : renseignez les informations à jour sur un utilisateur.

* **[!UICONTROL Créer des champs]**  définis par l’utilisateur : créez des champs de métadonnées personnalisés définis par l’utilisateur afin qu’ils vous aident à organiser les ressources dans Dynamic Media Classic. Les champs peuvent également être activés ou désactivés, le cas échéant.

(Voir [Champs définis par l’utilisateur](application-setup.md#user_defined_fields).)
