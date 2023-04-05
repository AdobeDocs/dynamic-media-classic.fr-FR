---
title: Suppression d’une ressource d’image pixellisée chargée
description: Découvrez comment supprimer une ressource chargée dans Adobe Dynamic Media Classic.
uuid: edd2b688-c377-4be1-ba16-d2dd2e6f716d
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: dd338c8c-06c6-44d5-8493-dc2087eeeafb
feature: Dynamic Media Classic
role: User
exl-id: d845bcb2-f914-4727-8df2-049dc172f266
source-git-commit: e235cdf331a1366ea81bd609e4e264c0c2cd8264
workflow-type: tm+mt
source-wordcount: '133'
ht-degree: 51%

---

# Supprimer un fichier téléchargé{#deleting-an-uploaded-asset}

Vous pouvez utiliser le paramètre `delete` dans ce format pour supprimer un fichier :

```as3
https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

Vous trouverez ci-après un exemple de réponse à une suppression de fichier d’image réussie :

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>delete</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>Delete request for1442564.tif</title> 
            <message>Your file was successfully deleted</message> 
        </response> 
    </user_generated_content> 
</scene7>
```

Vous pouvez utiliser les champs suivants dans la chaîne de requête d’URL pour supprimer un fichier :

| Paramètre de l’URL | Obligatoire ou facultatif | Valeur |
| --- | --- | --- |
| `op` | Obligatoire | supprimer |
| `shared_secret` | Obligatoire | La clé de secret partagé de l’entreprise. |
| `image_name` | Obligatoire | Nom du fichier à supprimer. |

<!-- <li>For Vector:fxg_name</li> -->

>[!IMPORTANT]
>
>À compter du 1er mai 2023, les ressources de pixellisation UGC dans Dynamic Media Classic seront disponibles jusqu’à 60 jours à compter de la date de chargement. Au bout de 60 jours, les ressources seront supprimées.

>[!NOTE]
>
>La prise en charge des ressources d’image vectorielle UGC nouvelles ou existantes dans Adobe Dynamic Media Classic s’est terminée le 30 septembre 2021.

**Exemple d’URL d’image :**

`https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

<!-- **Sample vector URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=delete&shared_secret=2160a8fa-cec6-45ba-8d59- ca595f6d2b47& &fxg_name=8875744.fxg` -->
