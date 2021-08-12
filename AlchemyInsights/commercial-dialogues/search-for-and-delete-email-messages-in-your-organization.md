---
title: Ettevõttes meilisõnumite otsimine ja kustutamine
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: bd25d9bb2af8114786503e129de105c9a0f602c98b206f01770605d1957e3a1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948879"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Ettevõttes meilisõnumite otsimine ja kustutamine

Tehke järgmist.

1. Kui te pole üldadministraator, tuleb teie konto otsimiseks lisada **e-juurdluse halduri** rollirühma või **vastavusotsingu haldusrolli.** Sõnumite kustutamiseks peate liituma organisatsioonihalduse rollirühma või **otsingu-** ja **puhastushalduse rolliga.** Nende rollide õigused määratakse turbe- [& vastavuskeskuses.](https://protection.office.com)
2. [Kustutava sõnumi](https://docs.microsoft.com/office365/securitycompliance/content-search) otsimiseks looge sisuotsing.
3. [Ühendus security & Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell). Kui kasutate MFA-d, lugege järgmisi juhiseid: Ühendus security [& Compliance Center PowerShell multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Sõnumi kustutamine: käivitage `New-ComplianceSearchAction` sõnumi kustutamiseks cmdlet-käsk. Kustutatud sõnumid teisaldatakse kasutaja taastatavate üksuste kausta. Näitekäsku leiate teemast [3. juhis: sõnumi kustutamine.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
