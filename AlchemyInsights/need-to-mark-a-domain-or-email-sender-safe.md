---
title: Kas peate domeeni või meili saatja turvaliseks märkima?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: afc865a7b91036bd2d982e21dce059a87e109e3e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58319944"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Kas peate domeeni või meili saatja turvaliseks märkima?

- Turvaliste **saatjate loendite kasutamine pole soovitatav,** kuna see avab teie asutuse rämpsposti, andmepüügi ja tüssamisrünnakute jaoks.
- Kui aga kehtib ärinõue, soovitame **selleks** kasutada **[Flow reegleid.](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** Meie juhised tagavad saatja autentimise (kontrollib, et saatmisdomeeni ei tüssata). 
    **Märkus.** Me ei soovita turvaliste saatjate loendite abil valepositiivseid andmeid hallata, kuna rämpsposti filtreerimise erandid võivad teie asutuse avada turberünnetele. Kui teie kasutaja(d) saab valesti rämpsposti või rämpspostina märgitud sõnumeid, **[teatage sõnumitest ja failidest Microsoftile.](https://protection.office.com/reportsubmission)**
- seif Saatjaid, Outlook, Lubatud saatjate loend või lubatud domeeniloend  rämpspostitõrjepoliitikates, tuleks vältida, kuna saatjad väldivad kogu rämpsposti, tüssamis- ja andmepüügikaitset ning saatja autentimist (SPF, DKIM, DMARC). Seda meetodit on kõige parem kasutada ainult ajutiseks testimiseks.
- Valideerimise, et teatud meilisõnumite üleastamist rämpspostitõrje abil saab teha, kontrollimiseks kontrollige sõnumipäist "X-Forefront-Antispam-Report" (SFV:SFE, SFV:SKA, SFV:SKN), vt **[rämpspostitõrje sõnumipäised](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)**.
- Kuna Microsoft soovib meie kliente vaikimisi [kaitsta,](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions)ei rakendata mõnda rentniku alistamist ründevara ja suure usaldusväärsusega andmepüügile. Need alistamised on järgmised: o Lubatud saatjaloendid või lubatud domeeniloendid (rämpspostitõrjepoliitikad) o Outlook seif Saatjad o IP-lubamisloend (ühenduse filtreerimine) 
- Ainus alistamine, mis lubab suure usaldusväärsusega andmepüügisõnumil filtreerimist mööda hiilida, on Exchange (ehk transpordireeglid). Meilivooreeglite kasutamise kohta filtreerimise möödumiseks lugege teemat Meilivoo reeglite kasutamine sõnumites rämpsposti **[usaldustaseme (SCL) suurendamiseks.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)**