---
title: BitLockeri taasteklahvid
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 4e06e0e43b63836b9e9cf923e554dd474b82c671
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908811"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Juurdepääs BitLockeri taastevõtmetele

BitLockeri sätete Intune lõpp-punkti kaitse poliitika konfigureerimisel on võimalik määratleda, kas BitLockeri taasteteavet tuleks talletada Azure Active Directorys.

Kui see säte on konfigureeritud, salvestatud Taasteandmed peaks olema nähtav Intune admin osana seadme kirje andmed Intune Devices tera kahel viisil:

Seadmed-Azure AD seadmed-> "seade" või seadmed-> kõik seadmed-> "seade"-> taastevõtmed

Teise võimalusena, kui on administraatori juurdepääs seadme ise, taastevõti (Password) saab näha, käivitades laiendatud käsuviibalt järgmise käsu:

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
Kui seade krüptiti enne Intune ' i registreerimist, võib taastevõti olla seostatud "Microsofti kontoga" (MSA), mida kasutatakse OOBE-protsessi ajal seadmesse sisselogimiseks. Kui see oli nii, juurdepääsu https://onedrive.live.com/recoverykey ja sisselogimine, et MSA peaks näitama seadmeid, mille Taastevõtmete salvestati.
 
Kui seade on krüptitud konfiguratsiooni tulemusena domeeni põhinev rühmapoliitika kaudu, võib taasteteavet talletada on-premise Active Directory.
 

