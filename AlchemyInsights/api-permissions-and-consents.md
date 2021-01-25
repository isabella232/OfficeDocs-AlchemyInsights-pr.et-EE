---
title: API load ja nõusolek
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974373"
---
# <a name="api-permissions-and-consent"></a>API load ja nõusolek

Microsoft Identity platformiga integreeritud rakendused järgivad loa mudelit, mis annab kasutajatele ja administraatoritele ülevaate sellest, kuidas andmeid saab kasutada. Loa mudeli rakendamine on Microsofti identiteedi platvormi lõpp-punktis uuendatud. See muudab viisi, kuidas rakendus peab Microsoft Identity platformiga suhtlema. [Microsofti identiteedi platvormi lõpp-punktides olevad load ja nõusolek](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) hõlmavad selle loa mudeli põhimõisteid (sh ulatused, load ja nõusolek).

[Azure Active Directory (AZURE ad) nõusoleku raamistiku](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) abil on lihtne arendada mitme rentniku veebirakendust ja kohalikku klientrakendust. Need rakendused lubavad sisse logida kasutaja kontodelt Azure AD rentniku jaoks, mis erineb rakenduse registreerimisest. Lisaks on võimalik, et lisaks oma veebirakendusliidestele on neil vaja juurde pääseda ka veebi API-de (nt Microsoft Graph API) (Microsoft 365 Azure AD, Intune ' i ja teenuste jaoks) ning muude Microsofti teenuste API-de jaoks.

