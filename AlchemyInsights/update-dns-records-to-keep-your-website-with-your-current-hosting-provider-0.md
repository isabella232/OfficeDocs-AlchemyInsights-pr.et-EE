---
title: Värskendage DNS-i kirjeid, et hoida oma veebisait praeguse majutusteenuse pakkujaga.
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 1d8654bc2dfb9063d0203992d624285eb646027d
ms.sourcegitcommit: 78939b01579b626b147d356045a37aec1170c948
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47815781"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Värskendage DNS-i kirjeid, et hoida oma veebisait praeguse majutusteenuse pakkujaga.

1. Avage Microsoft 365 halduskeskus leht **Häälesta**  >  [Domeenid](https://admin.microsoft.com/Adminportal#/Domains) ja valige domeenide loendist domeen, mida kasutate oma veebisaidi jaoks.

2. Valige **+ Uus kohandatud kirje** ja sisestage järgmine tekst.

  - **DNS-i tüübi** sisestamiseks sisestage: **a (aadress)**

  - Tippige väljale **hosti nimi või pseudonüüm**järgmine tekst. **@**

  - **IP-aadressi**korral tippige veebisaidi staatiline IP-aadress, kus see on praegu majutatud (nt 172.16.140.1).

    See peab olema veebisaidi  *staatiline*  IP-aadress, mitte  *dünaamiline*  IP-aadress. Kontrolli saidil, kus teie veebisait on majutatud, et saaksite oma avaliku veebisaidi jaoks staatilise IP-aadressi.

3. Valige **Salvesta**.

Lisaks saate luua CNAME-kirje, mis aitab klientidel teie veebisaiti leida.
  
1. Valige **+ Uus kohandatud kirje** ja sisestage järgmine tekst.

  - **DNS-i tüübi** sisestamiseks sisestage: **CNAME (pseudonüüm)**

  - Tippige väljale **hosti nimi või pseudonüüm**järgmine tekst: **www**

  - **Punktide**saamiseks tippige oma veebisaidi täielik DOMEENINIMI (FQDN) (nt contoso.com).

2. Valige **Salvesta**.
