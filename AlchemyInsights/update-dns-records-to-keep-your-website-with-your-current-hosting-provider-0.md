---
title: Värskendage DNS-kirjete hoida oma kodulehel praeguse hosting pakkuja
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
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665756"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Värskendage DNS-kirjete hoida oma kodulehel praeguse hosting pakkuja

1. Microsoft 365 halduskeskus, lehele **setup**  >  [Domeenid](https://portal.office.com/adminportal/home#/Domains) ja domeenide loendis Valige domeen, mida kasutate oma veebilehel.

2. Valige **+ Uus kohandatud kirje** ja sisestage järgmine:

  - Sisestage **DNS-i tüüp** : **a (aadress)**

  - **Hosti nime või pseudonüümi**, tippige järgmine:**@**

  - **IP-aadressi**puhul tippige oma veebisaidi staatiline IP-aadress, kus see praegu majutatud (nt 172.16.140.1).

    See peab olema *staatiline* IP-aadress veebilehel, mitte *dünaamiline* IP-aadress. Kontrollige saiti, kus teie veebisait on majutatud veendumaks, et saate oma avaliku veebisaidi jaoks staatilise IP-aadressi.

3. Valige **Salvesta**.

Lisaks saate luua CNAME-kirje, et aidata klientidel teie veebisaiti leida.
  
1. Valige **+ Uus kohandatud kirje** ja sisestage järgmine:

  - Sisestage **DNS-i tüüp** : **CNAME (alias)**

  - **Hosti nime või pseudonüümi**, tippige järgmine: **www**

  - **Aadressi punktide käsitlemiseks**tippige oma veebisaidile täielik DOMEENINIMI (FQDN) (nt contoso.com).

2. Valige **Salvesta**.
