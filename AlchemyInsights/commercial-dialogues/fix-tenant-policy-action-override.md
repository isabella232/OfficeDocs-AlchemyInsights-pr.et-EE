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
ms.openlocfilehash: 157baa1f1e3f48b47ba07b8c6d446f8e081a4ad24b7d48f50c4fc5af5518cdd6
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896071"
---
# <a name="fix-tenant-policy-action-override"></a>Rentnikupoliitika parandus (toimingu alistamine)

Üks teie rämpspostitõrje poliitikatest mõjutas seda sõnumit. Poliitikate läbivaatamiseks tehke järgmist.

1. Avage Microsoft 365 Defender portaal jaotises Poliitikad & Meilipoliitikad & Reeglid <https://security.microsoft.com/>  \>  \>  \>  ohupoliitikad Rämpspostitõrje. 

   Otse rämpspostitõrje **poliitikate lehele minemiseks** kasutage funktsiooni <https://security.microsoft.com/antispam> .

2. Valige **lehel Rämpspostitõrje poliitika** poliitika, klõpsates poliitika nime **(Tüüp** on  Kohandatud rämpspostivastane poliitika või **Nimi** on rämpspostitõrje sissetulev **poliitika (vaikesäte).**
3. Klõpsake kuvatavas üksikasja hüpikmenüüs **jaotises Toimingud** nuppu **Redigeeri toiminguid.**
4.  Vaadake jaotises **Sõnumitoimingud** üle rämpsposti, suure usaldusväärsusega **rämpsposti,** **andmepüügi** ja suure usaldusväärsusega andmepüügi otsused, et näha, kas on valitud mõni järgmistest väärtustest.
   - **X-päise lisamine**
   - **Valmis teemarida tekstiga**
   - **Sõnumi ümbersuunamine meiliaadressile**
   - **Kustuta sõnum**
   - **Toiming puudub**

   Võimalik, et kõigile klientidele **rakendatud standardsätted** Exchange Online'i kaitseteenus mõjutasid sõnumit.

Lisateavet leiate teemast [Rämpspostitõrjepoliitikate konfigureerimine EOP-s.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies)
