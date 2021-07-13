---
title: Väljaminevate kattekaustade
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/08/2021
ms.locfileid: "53381633"
---
# <a name="outbound-relay-pool"></a>Väljaminevate kattekaustade

Microsoft muudab konfiguratsiooni meilisõnumite edastamiseks või edasisaatmiseks Microsoft 365. Teatud stsenaariumides sõnumeid edastatakse või edastatakse Microsoft 365 kaudu, kasutades spetsiaalset releekausta. Releekausta abil saadetud sõnumid võivad olla adressaadi rämpspostikaustas. Lisateavet leiate teemast [Väljaminevate tarnete kaustu](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

Releekausta kasutamise vältimiseks veenduge, et edasi saadetud/edastatud sõnumid vastaksid ühele järgmistest kriteeriumidest.

- Väljamineva saatja on rentniku aktsepteeritud domeen.
- Saatjapoliitika raamistik (SPF) möödub, kui sõnum jõuab Microsoft 365.
- DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.
 
Ülaltoodud kriteeriumidele vastavad sõnumid ei edastata releekausta kaudu.

Kui teie domeeni MX-kirje on suunatud kolmandale osapoolele või asutusesisesele serverile, kasutage täiustatud filtreerimist, et veenduda, kas SPF-i valideerimine on sissetulevate meilisõnumite jaoks õige ja et vältida meilisõnumite saatmist läbi releekausta.

**Kuidas saame teada, kas me oleme releekausta mõjul?**

Kui teie edastatud või edastatud meilisõnumid kasutavad ühte ülaltoodud kriteeriumidest, ei edastata sõnumeid läbi releekausta. Kui aga sõnum saadetakse releekausta kaudu, on väljamineva meili serveri IP vahemikus 40.95.0.0/16 ja väljamineva meili serveri nimi **sisaldab nime rly.**

