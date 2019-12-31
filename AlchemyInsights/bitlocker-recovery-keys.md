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
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="552ac-102">Juurdepääs BitLockeri taastevõtmetele</span><span class="sxs-lookup"><span data-stu-id="552ac-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="552ac-103">BitLockeri sätete Intune lõpp-punkti kaitse poliitika konfigureerimisel on võimalik määratleda, kas BitLockeri taasteteavet tuleks talletada Azure Active Directorys.</span><span class="sxs-lookup"><span data-stu-id="552ac-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="552ac-104">Kui see säte on konfigureeritud, salvestatud Taasteandmed peaks olema nähtav Intune admin osana seadme kirje andmed Intune Devices tera kahel viisil:</span><span class="sxs-lookup"><span data-stu-id="552ac-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="552ac-105">Seadmed-Azure AD seadmed-> "seade" või seadmed-> kõik seadmed-> "seade"-> taastevõtmed</span><span class="sxs-lookup"><span data-stu-id="552ac-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="552ac-106">Teise võimalusena, kui on administraatori juurdepääs seadme ise, taastevõti (Password) saab näha, käivitades laiendatud käsuviibalt järgmise käsu:</span><span class="sxs-lookup"><span data-stu-id="552ac-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="552ac-107">Kui seade krüptiti enne Intune ' i registreerimist, võib taastevõti olla seostatud "Microsofti kontoga" (MSA), mida kasutatakse OOBE-protsessi ajal seadmesse sisselogimiseks.</span><span class="sxs-lookup"><span data-stu-id="552ac-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="552ac-108">Kui see oli nii, juurdepääsu https://onedrive.live.com/recoverykey ja sisselogimine, et MSA peaks näitama seadmeid, mille Taastevõtmete salvestati.</span><span class="sxs-lookup"><span data-stu-id="552ac-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="552ac-109">Kui seade on krüptitud konfiguratsiooni tulemusena domeeni põhinev rühmapoliitika kaudu, võib taasteteavet talletada on-premise Active Directory.</span><span class="sxs-lookup"><span data-stu-id="552ac-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

