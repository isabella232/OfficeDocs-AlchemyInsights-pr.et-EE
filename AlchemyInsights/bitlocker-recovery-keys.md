---
title: BitLockeri taastevõti
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 7c56e68cf303939d8e7d4ee0a7301e367ecfe9f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685882"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Juurdepääs BitLockeri taastevõti

Kui konfigureerite BitLockeri sätteid Intune Endpoint Protection Policy, on võimalik määratleda, kas BitLockeri taasteparool tuleks talletada Azure Active Directorys.

Kui see säte on konfigureeritud, peaks talletatud andmete taastamise andmed olema nähtavad Intune ' i administraatorile osana seadme kirje andmeid Intune Devices Blade kahel viisil:

Seadmed – Azure AD seadmed – > "seade" või seadmed – > kõik seadmed – > "Device"-> taastevõtme

Kui seadmele on installitud ka administratiivne juurdepääs, kuvatakse taastevõti (parool) kõrgenenud käsuviiba kaudu järgmine käsk:

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
Kui seade krüptiti enne sisselogimist Intune ' is, võis taastevõti olla seostatud "Microsofti kontoga" (MK), mida kasutati OOBE-protsessi ajal seadmesse sisse logimiseks. Kui see oli nii,  https://onedrive.live.com/recoverykey tuleks selle MSA-ga sisse logida ja sisse logida, et kuvada seadmed, mille taastevõti on talletatud.
 
Kui seade oli krüptitud rühmapoliitika kaudu konfigureerimise tulemusena krüptitud, võib süsteemitaaste teavet talletada kohapealses Active Directorys.
 

