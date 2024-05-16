---
title: Suppression d’une ressource d’image pixellisée chargée
description: Découvrez comment supprimer une ressource chargée dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: User
exl-id: d845bcb2-f914-4727-8df2-049dc172f266
topic: Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '136'
ht-degree: 33%

---

# Supprimer un fichier téléchargé{#deleting-an-uploaded-asset}

Vous pouvez utiliser la variable `delete` dans ce format pour supprimer une ressource :

```as3
https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

Vous trouverez ci-après un exemple de réponse à une suppression de fichier d’image réussie :

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content: Images</serviceName> 
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
| `shared_secret` | Obligatoire | Clé qui est un secret partagé pour la société. |
| `image_name` | Obligatoire | Nom de la ressource à supprimer. |

<!-- <li>For Vector:fxg_name</li> -->

>[!IMPORTANT]
>
>À compter du 1er mai 2023, les ressources UGC dans Dynamic Media pourront être utilisées pendant 60 jours à compter de la date de téléchargement. Au bout de 60 jours, les ressources seront supprimées.

>[!NOTE]
>
>La prise en charge des ressources d’image vectorielle UGC nouvelles ou existantes dans Adobe Dynamic Media Classic s’est terminée le 30 septembre 2021.

**Exemple d’URL d’image :**

`https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

<!-- **Sample vector URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=delete&shared_secret=2160a8fa-cec6-45ba-8d59- ca595f6d2b47& &fxg_name=8875744.fxg` -->
