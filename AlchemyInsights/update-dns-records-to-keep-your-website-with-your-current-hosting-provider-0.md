---
title: Värskendada DNS-kirjete hoida oma veebilehel koos oma praeguse hosting teenust
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: a79302259e294ea5bf3b1d29393a412edb27a388
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28285428"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Värskendada DNS-kirjete hoida oma veebilehel koos oma praeguse hosting teenust

1. Leheküljel [Domeenid](https://portal.office.com/adminportal/home#/Domains) domeenide loendis Valige domeen, mida kasutate oma veebilehel, ja seejärel valige paan Dokumendihaldus **DNS-i sätted** . 
    
2. Valige **+ uue kohandatud kirje** ja tippige järgmine: 
    
  - Sisestage **DNS-i tüüp** : **(aadress)**
    
  - **Hosti nimi või pseudonüüm**, tippige järgmine:**@**
    
  - **IP-aadress**tippige veebisaidi, kus on praegu majutatud (näiteks 172.16.140.1) staatiline IP-aadress. 
    
    See peab olema koduleht, mitte *dünaamilise* IP-aadressi *staatilise* IP-aadressi. Kohas, kus teie koduleheküljel on hostitud veendumaks, et avaliku veebisaidi staatilisi IP-aadressi saamiseks pöörduge. 
    
3. Valige **Salvesta**. 
    
Lisaks saate luua CNAME-kirje aitab kasutajatel leida oma veebilehel.
  
1. Valige **+ uue kohandatud kirje** ja tippige järgmine: 
    
  - Sisestage **DNS-i tüüp** : **CNAME (pseudonüüm)**
    
  - **Hosti nimi või pseudonüüm**, tippige järgmine: **www**
    
  - **Punktid aadressile**, tippige domeeni nimi (FQDN) oma veebilehel (nt contoso.com). 
    
2. Valige **Salvesta**. 
    

