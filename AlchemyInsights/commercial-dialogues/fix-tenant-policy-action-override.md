---
title: Rentnikupoliitika parandus (toimingu alistamine)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ee45e86a143719914f7a7917730d7e840e90625f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326793"
---
# <a name="fix-tenant-policy-action-override"></a>Rentnikupoliitika parandus (toimingu alistamine)

Üks teie rämpspostitõrje poliitikatest mõjutas seda sõnumit. Poliitikate läbivaatamiseks tehke järgmist.

1. Avage Microsoft 365 Defender portaal jaotises Poliitikad <https://security.microsoft.com/> **& Meil&** koostööpoliitikad & Reeglid \>  \>  \>  ohupoliitikad  Rämpspostitõrje.

   Otse rämpspostitõrje **poliitikate lehele minemiseks** kasutage funktsiooni <https://security.microsoft.com/antispam> .

2. Lehel **Rämpspostitõrje poliitikad** poliitika valimiseks klõpsake poliitika nime (**Tüüp** on  Kohandatud rämpspostivastane poliitika või **Nimi** on rämpspostivastane sissetulev **poliitika (vaikesäte).**
3. Klõpsake kuvatavas üksikasja hüpikmenüüs **jaotises Toimingud** nuppu **Redigeeri toiminguid.**
4.  Vaadake jaotises **Sõnumitoimingud** üle rämpsposti, suure usaldusväärsusega **rämpsposti,** **andmepüügi** ja suure usaldusväärsusega andmepüügi otsused, et näha, kas on valitud mõni järgmistest väärtustest.
   - **X-päise lisamine**
   - **Valmis teemarida tekstiga**
   - **Sõnumi ümbersuunamine meiliaadressile**
   - **Kustuta sõnum**
   - **Toiming puudub**

   Võimalik, et kõigile klientidele **rakendatud standardsätted** Exchange Online'i kaitseteenus mõjutasid sõnumit.

Lisateavet leiate teemast [Rämpspostitõrjepoliitikate konfigureerimine EOP-s.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies)
