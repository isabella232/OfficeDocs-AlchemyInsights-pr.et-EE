---
title: Bitlockeri taastevõtmed
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
ms.openlocfilehash: 8708ed76f6abe81582823c8af89db8fffef9a3c5
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505064"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Juurdepääs BitLockeri taastevõtmetele

Bitlockeri sätete konfigureerimisel Intune'i lõpp-punkti kaitse poliitikas on võimalik määratleda, kas Bitlockeri taasteteavet tuleks talletada Azure Active Directorys.

Kui see säte on konfigureeritud, peaksid salvestatud taasteandmed olema Intune'i administraatorile intune'i seadmete tera seadmekirje andmete osana nähtavad kahel viisil.

Seadmed – Azure AD-seadmed -> "Seade" VÕI Seadmed -> Kõik seadmed -> "Seade" -> Taastevõtmed

Teise võimalusena, kui seadmele on administraatorijuurdepääs, saab taastevõtit (parooli) vaadata, käivitades administraatoriõigustega käsuviiba kaudu järgmise käsu:

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
Kui seade oli enne Intune'is registreerumist krüptitud, võib taastevõti olla seostatud "Microsofti kontoga" (MSA), mida kasutati seadmesse SISSE logimiseks OOBE-protsessi käigus. Sel juhul peaks selle MSA-le juurdepääsemisel ja sellega sisselogimisel olema näha seadmed,  https://onedrive.live.com/recoverykey mille taastevõtmed talletati.
 
Kui seade on domeenipõhise rühmapoliitika kaudu konfigureerimise tulemusena krüptitud, võidakse taasteteave talletada siseses Active Directorys.

Kui olete konfigureerinud lõpp-punkti kaitsepoliitika Azure Active Directory taastevõtme talletamiseks, kuid konkreetse seadme võtit pole üles laaditud, saate üleslaadimise käivitada, pöörates selle seadme taastevõtit MEM-konsooli kaudu. Lisateavet leiate teemast [BitLockeri taastevõtmete pööramine.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)

