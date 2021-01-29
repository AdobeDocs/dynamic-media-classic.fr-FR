---
title: Suppression d’un fichier téléchargé
description: Découvrez comment supprimer un fichier téléchargé.
uuid: edd2b688-c377-4be1-ba16-d2dd2e6f716d
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: dd338c8c-06c6-44d5-8493-dc2087eeeafb
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '94'
ht-degree: 88%

---


# Suppression d’un fichier téléchargé{#deleting-an-uploaded-asset}

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
|--- |--- |--- |
| op | Obligatoire | supprimer |
| shared_secret | Obligatoire | La clé de secret partagé de l’entreprise. |
| <ul><li>Pour les images:image_name</li><li>Pour les fichiers vectoriels :fxg_name</li></ul> | Obligatoire | Nom du fichier à supprimer. |

**Exemple d’URL d’image :**

`https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

**Exemple d’URL de fichier vectoriel :**

`https://s7ugc1.scene7.com/ugc/vector?op=delete&shared_secret=2160a8fa-cec6-45ba-8d59- ca595f6d2b47& &fxg_name=8875744.fxg`
