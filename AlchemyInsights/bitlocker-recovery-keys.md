---
title: Bitlockeri taastevõtmed
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: f71fae0aabda3fc48f20d5ea1e6909475f0c17ff5cdf98b58b1403bd2e291c19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54060060"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Juurdepääs BitLockeri taastevõtmetele

Bitlockeri sätete konfigureerimisel Intune'i lõpp-punkti kaitsepoliitikas on võimalik määratleda, kas Bitlockeri taasteteavet tuleks talletada Azure Active Directory.

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

Kui olete konfigureerinud lõpp-punkti kaitsepoliitika, et talletada taastevõti Azure Active Directory'is, kuid konkreetse seadme võtit pole üles laaditud, saate üleslaadimise käivitada, pöörates selle seadme taastevõtit MEM-i konsooli kaudu. Lisateavet leiate teemast [BitLockeri taastevõtmete pööramine.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)

