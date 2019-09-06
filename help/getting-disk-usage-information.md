---
title: Obtention d’informations sur l’utilisation du disque
seo-title: Obtention d’informations sur l’utilisation du disque
description: 'null'
seo-description: Découvrez comment obtenir des informations sur l'utilisation du disque.
uuid: 01361693-53 d 0-4072-b 7 c 3-f 284631 d 28 cf
contentOwner: admin
content-type: référence
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
discoiquuid: 6763546 d -83 c 4-42 dc -879 f -6 bbfc 8 b 56482
translation-type: tm+mt
source-git-commit: 75f006fd81b0fe2dad5479cdd98e45eaada46b2a

---


# Obtention d’informations sur l’utilisation du disque {#getting-disk-usage-information}

Vous pouvez utiliser le paramètre `disk_info` pour récupérer des informations sur l’utilisation de l’espace disque d’une société, comme indiqué dans l’exemple suivant :

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=d03b7e0b-c9dc-4c6c-af0b-419beeea1c63
```

Vous trouverez ci-après un exemple de réponse :

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>disk_info</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>Disk Information for d03b7e0b-c9dc-4c6c-af0b-419beeea1c63</title> 
            <message>Total Space available = 1395402342400 bytes. Total Space used = 0 bytes.</message> 
        </response> 
    </user_generated_content> 
</scene7>
```

Vous pouvez utiliser les champs suivants dans la chaîne de requête d’URL pour obtenir des informations sur l’utilisation du disque :

| Paramètre de l’URL | Obligatoire ou facultatif | Valeur |
|--- |--- |--- |
| op | Obligatoire | disk_info |
| shared_secret | Obligatoire | La clé de secret partagé de l’entreprise |

L’exemple de code suivant permet d’obtenir des informations sur le disque pour l’entreprise000 :

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b9602
```

