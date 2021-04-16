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
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792128"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Kas peate domeeni või meili saatja turvaliseks märkima?

- Turvaliste **saatjate loendite kasutamine pole soovitatav,** kuna see avab teie asutuse rämpsposti, andmepüügi ja tüssamisrünnakute jaoks.
- Kui aga on olemas ärinõue, **soovitame selleks** kasutada **[meilivoo](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** reegleid. Meie juhised tagavad saatja autentimise (kontrollib, et saatmisdomeeni ei tüssata). **Märkus.** Me ei soovita turvaliste saatjate loendite abil valepositiivseid andmeid hallata, kuna rämpsposti filtreerimise erandid võivad teie asutuse avada turberünnetele. Kui teie kasutaja(d) saavad valesti rämpsposti või rämpspostina märgitud sõnumeid, **[teatage sõnumitest ja failidest Microsoftile.](https://protection.office.com/reportsubmission)**
- Turvaliste saatjate kasutamist Outlookis, lubatud saatjate loendit  või lubatud domeeniloendit rämpspostitõrjepoliitikates tuleks vältida, kuna saatjad väldivad kogu rämpsposti, tüssamis- ja andmepüügikaitset ning saatja autentimist (SPF, DKIM, DMARC). Seda meetodit on kõige parem kasutada ainult ajutiseks testimiseks.
