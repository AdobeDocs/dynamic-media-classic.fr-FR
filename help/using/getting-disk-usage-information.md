---
title: Obtenir des informations sur l'utilisation du disque
description: Découvrez comment obtenir des informations sur l’utilisation du disque dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Admin,User
exl-id: 337a4681-ac9a-40d9-82e8-1999bbed980c
topic: Administration, Content Management
level: Intermediate
autotag-review: '2026-05-13T19:50:49.049Z'
TQID: 'https://experienceleague.adobe.com/g-mRoL2yYGRH-uFr2ACD2qOxBAGUlMMtKKuKtsv2pQk'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: df89051c2f5083cdf7ae39f978ab0bfc05230296
workflow-type: tm+mt
source-wordcount: 88
ht-degree: 34%

---

# Obtenir des informations sur l’utilisation du disque {#get-disk-usage-information}

Vous pouvez utiliser le paramètre `disk_info` pour récupérer des informations sur l’utilisation de l’espace disque, comme illustré dans l’exemple suivant :

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=d03b7e0b-c9dc-4c6c-af0b-419beeea1c63
```

Vous trouverez ci-après un exemple de réponse :

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content: Images</serviceName> 
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
| --- | --- | --- |
| op | Obligatoire | disk_info |
| shared_secret | Obligatoire | La clé qui est un secret partagé pour l’entreprise |

L’exemple de code suivant récupère des informations sur le disque :

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b9602
```
