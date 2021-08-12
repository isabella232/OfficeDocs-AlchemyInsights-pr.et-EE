---
title: Rämpspostihausi blokeeritud meilisõnumite saatmisel ilmnes tõrge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8372032e19bd2ebaf3ba8cc8e87f19ef3e2edf1e607b1739a919f6dcc443cd97
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946711"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Meilisõnumite saatmisel ilmnes tõrge: Rämpspostihausi abil blokeeritud klientarvuti host

Sõnumi saatnud IP-aadress asub rämpspostisaatjale omases [blokeerimisloendis.](https://go.microsoft.com/fwlink/p/?linkid=123245) Rämpspostihausi blokeerimise põhjused on näiteks ohustatud kontod, avaliku IP-aadressiga ohustatud masinad ja Interneti-teenuse pakkuja (ISP) poliitikad. Võimalikud parandused on järgmised.
  
- Blokeeritud sissetulevate sõnumite korral, kus saate lähtemeiliserverit juhtida, peate määrama põhjuse ja eemaldama blokeerimise Rämpspostikeskuse veebisaidilt.

- Blokeeritud sissetulevate sõnumite korral, mille lähte-IP-aadress kuulub kellelegi teisele, peab aadressi omanik blokeerima Rämpspostihausi veebisaidilt. Kui IP-aadress on poliitikaplokkide loendis (PBL), saab omanik määrata muu staatilise IP-aadressi või eemaldada aadressi PBL-ist.

- Microsoftiga ühendatud blokeeritud väljaminevate sõnumite korral saate selle tõrketeate, kui sõnumid marsruuditakse kolmanda osapoole teenuse kaudu. Blokeeritud IP-aadressi omaniku leidmiseks saate kasutada WHOIS-otsingutööriista.
