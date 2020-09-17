---
title: Tõrge SpamHaus poolt blokeeritud meilisõnumite saatmisel
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783799"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Tõrge meilisõnumi saatmisel: kliendi host on SpamHaus abil blokeeritud

Sõnumi saatnud IP-aadress on [SpamHaus](https://go.microsoft.com/fwlink/p/?linkid=123245)-i omanikule kuuluval ploki loendis. Põhjused, miks SpamHaus on blokeeritud, hõlmavad ka ohustatud kontosid, avaliku IP-aadressi ühiskasutusse antud ohustatud seadmeid ja Interneti-teenuse pakkuja (ISP) poliitikaid. Võimalikud parandused on järgmised.
  
- Blokeeritud sissetulevatele sõnumitele, kus saate määrata allika meiliserveri, peate tuvastama põhjuse ja eemaldama ploki SpamHaus veebisaidilt.

- Blokeeritud sissetulevatele sõnumitele, kus allika IP-aadress kuulub kellelegi teisele, peab aadressi omanik eemaldama ploki SpamHaus veebisaidilt. Kui IP-aadress asub poliitikate blokeerimise loendis (PBL), saab omanik määrata teistsuguse staatilise IP-aadressi või eemaldada aadressi PBL.

- Microsoftiga ühendatud domeeni blokeeritud Väljaminevatele sõnumitele saate selle tõrketeate, kui sõnumeid marsruuditakse kolmanda osapoole teenuse kaudu. Saate kasutada WHOIS-otsingu tööriista, et leida blokeeritud IP-aadressi omanik.
