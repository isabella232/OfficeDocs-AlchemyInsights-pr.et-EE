---
title: Rentniku poliitika lahendamine (toimingu alistamine)
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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745879"
---
# <a name="fix-tenant-policy-action-override"></a>Rentniku poliitika lahendamine (toimingu alistamine)

See sõnum mõjutas teie rentniku rämpsposti poliitikat. Poliitika läbivaatamiseks tehke järgmist.

1. Minge [Office 365 turbe & nõuetele vastavuse keskusse](https://go.microsoft.com/fwlink/p/?linkid=2077143)ja seejärel valige **ohustatud halduse**  >  **poliitika**  >  [anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Kontrollige, kas **poliitika allikas** viitab järgmistele teemale:  **Add-Xheader/ModifySubject/ümbersuunamine/DELETE/ei toimingu/Salakoopia sõnum**

    Kui see on nii, siis kontrollige, kas vahekaardil **kohandatud** kuvatakse sõnumiga mõjutatud poliitika sätted. On võimalik, et kõik Exchange Online ' i kaitstud kliendid rakendasid sõnumile **normi** .

Lisateavet rämpsmeili filtri poliitikate konfigureerimise kohta leiate teemast [rämpsmeili filtri poliitikate konfigureerimine](https://go.microsoft.com/fwlink/?linkid=2101431).
