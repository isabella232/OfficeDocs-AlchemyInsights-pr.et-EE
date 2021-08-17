---
title: Säilituspoliitikad Exchange halduskeskuses ei tööta
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 6652ad5fc1691e1d5a4293d81f3a649f23ec38f18c8ed9fe06665628a901d13e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074928"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Säilituspoliitikad Exchange halduskeskuses

Kui soovite, et käivitame allpool nimetatud sätete automaatsed kontrollid, valige selle lehe ülaservas nupp < ja sisestage säilituspoliitikatega seotud probleemidega kasutaja meiliaadress.

Kui teil on probleeme Exchange halduskeskuse säilituspoliitikatega, mis ei rakenda postkastidele või üksustele, mis ei teisalda arhiivipostkasti, kontrollige järgmist.

**Juurpõhjused:**

- **Hallatud** kaustaabimees ei ole kasutaja postkasti töötlenud. Hallatava kausta abiline proovib töödelda iga postkasti teie pilvepõhises organisatsioonis üks kord seitsme päeva jooksul.

  **Lahendus:** Käivitage hallatud kaustaabimees.

- **Säilituspeetus** on **postkastis** lubatud. Kui postkast on paigutatud säilitusapeetusse, siis selle aja jooksul postkasti säilituspoliitikat ei töödelda.

  **Lahendus:** Kontrollige säilitussätte olekut ja värskendage seda vastavalt vajadusele. Lisateavet leiate teemast [Postkasti säilituse ootel hoidmine.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)
 
**Märkus.** Kui postkast on väiksem kui 10 MB, ei töötle hallatava kausta abiline postkasti automaatselt.
 
Lisateavet halduskeskuse säilituspoliitikate Exchange leiate järgmisest teemast.

- [Säilitussildid ja säilituspoliitikad](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Säilituspoliitika rakendumine postkastidele või](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) [säilitussiltide lisamine või eemaldamine](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Postkasti paigutatud ootel salvestatud ootele pandud tüübi tuvastamine](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
