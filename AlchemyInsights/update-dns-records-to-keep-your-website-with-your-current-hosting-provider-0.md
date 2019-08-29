---
title: Värskendada DNS-kirjete hoida oma veebilehel koos oma praeguse hosting teenust
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 7bd36c3954d12d3ee4ac624a2f827d8e5cd88082
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665756"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Värskendada DNS-kirjete hoida oma veebilehel koos oma praeguse hosting teenust

1. Minge Microsoft 365 administreerimiskeskuses **Seadistus** > [domeenide](https://portal.office.com/adminportal/home#/Domains) lehekülg ja domeenide loendis valige domeeni kasutamisel oma veebilehel.

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
