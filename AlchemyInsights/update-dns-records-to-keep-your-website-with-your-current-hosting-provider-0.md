---
title: Värskendage DNS-i kirjeid, et hoida oma veebisaiti praeguse majutusteenuse pakkuja juures
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: f868ce25d68f61da30d2db4de88aa83675c97857b3c1371cf2039e0b03895a64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007678"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Värskendage DNS-i kirjeid, et hoida oma veebisaiti praeguse majutusteenuse pakkuja juures

1. Avage Microsoft 365 halduskeskus lehel **Domeenide** häälestamine ja valige domeenide loendis domeen, mida  >  [](https://admin.microsoft.com/Adminportal#/Domains) oma veebisaidi jaoks kasutate.

2. Valige **+ Uus kohandatud kirje** ja sisestage järgmine teave.

  - **DNS-i tüübi jaoks** **sisestage: A (Aadress)**

  - Tippige **väljale Hosti nimi või Pseudonüüm** järgmine tekst. **@**

  - **Tippige IP-aadressi** jaoks oma veebisaidi staatiline IP-aadress, kus seda praegu majutatakse (nt 172.16.140.1).

    See peab olema veebisaidi  *staatiline*  IP-aadress, mitte  *dünaamiline*  IP-aadress. Kontrollige veebisaiti, kus teie veebisaiti majutatakse, veendumaks, et saate oma avaliku veebisaidi jaoks staatilise IP-aadressi.

3. Valige **Salvesta**.

Lisaks saate luua CNAME-kirje, et aidata klientidel teie veebisaiti leida.
  
1. Valige **+ Uus kohandatud kirje** ja sisestage järgmine teave.

  - **DNS-i tüübi jaoks** **sisestage: CNAME (Pseudonüüm)**

  - Hostinime **või pseudonüümi** korral tippige järgmine tekst: **www**

  - Tippige väljale Points to address (Points **to address)** oma veebisaidi täielik domeeninimi (FQDN) (nt contoso.com).

2. Valige **Salvesta**.
