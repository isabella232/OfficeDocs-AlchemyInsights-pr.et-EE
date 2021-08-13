---
title: Luba kasutajal sünkroonida isiklikku kontot töökontoga Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9127"
- "9004429"
ms.openlocfilehash: da435b37b689e97ca51ce5cf94eb7e7d71eb972060526989239310fac1460628
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813393"
---
# <a name="enable-a-user-to-sync-a-personal-account-with-the-work-account-in-microsoft-edge"></a>Luba kasutajal sünkroonida isiklikku kontot töökontoga Microsoft Edge

Veenduge, et vastate neile kriteeriumidele.

- Enterprise State Roaming on lubatud Azure Active Directory halduskeskuses, mis nõuab tellimuse Azure Active Directory Premium Enterprise Mobility + Security (EMS). Lisateavet leiate teemast Ettevõtte [oleku rändluse lubamine Azure Active Directory.](/azure/active-directory/devices/enterprise-state-roaming-enable)
- Täidetud on üks või mõlemad järgmistest kriteeriumidest.
    - Azure'i teabekaitse teenus on teie rentniku jaoks lubatud. Lisateavet leiate teemast [Azure Rights Managementi kaitse aktiveerimine Microsoft 365 halduskeskus.](/azure/information-protection/activate-office365)
    - Funktsioon Azure Active Directory Enterprise State Roaming (ESR) on lubatud mis tahes kasutaja või rentniku jaoks. Lisateavet leiate teemast Mis on [ettevõtte oleku rändlus?](/azure/active-directory/devices/enterprise-state-roaming-overview).

Kui AIP ja ESR on mõlemad keelatud, teavitab tõrketeade kasutajaid, et sünkroonimine pole nende kontode jaoks saadaval.
