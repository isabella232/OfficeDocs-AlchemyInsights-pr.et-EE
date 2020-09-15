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
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="87ebb-102">Juurdepääs BitLockeri taastevõti</span><span class="sxs-lookup"><span data-stu-id="87ebb-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="87ebb-103">Kui konfigureerite BitLockeri sätteid Intune Endpoint Protection Policy, on võimalik määratleda, kas BitLockeri taasteparool tuleks talletada Azure Active Directorys.</span><span class="sxs-lookup"><span data-stu-id="87ebb-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="87ebb-104">Kui see säte on konfigureeritud, peaks talletatud andmete taastamise andmed olema nähtavad Intune ' i administraatorile osana seadme kirje andmeid Intune Devices Blade kahel viisil:</span><span class="sxs-lookup"><span data-stu-id="87ebb-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="87ebb-105">Seadmed – Azure AD seadmed – > "seade" või seadmed – > kõik seadmed – > "Device"-> taastevõtme</span><span class="sxs-lookup"><span data-stu-id="87ebb-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="87ebb-106">Kui seadmele on installitud ka administratiivne juurdepääs, kuvatakse taastevõti (parool) kõrgenenud käsuviiba kaudu järgmine käsk:</span><span class="sxs-lookup"><span data-stu-id="87ebb-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="87ebb-107">Kui seade krüptiti enne sisselogimist Intune ' is, võis taastevõti olla seostatud "Microsofti kontoga" (MK), mida kasutati OOBE-protsessi ajal seadmesse sisse logimiseks.</span><span class="sxs-lookup"><span data-stu-id="87ebb-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="87ebb-108">Kui see oli nii,  https://onedrive.live.com/recoverykey tuleks selle MSA-ga sisse logida ja sisse logida, et kuvada seadmed, mille taastevõti on talletatud.</span><span class="sxs-lookup"><span data-stu-id="87ebb-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="87ebb-109">Kui seade oli krüptitud rühmapoliitika kaudu konfigureerimise tulemusena krüptitud, võib süsteemitaaste teavet talletada kohapealses Active Directorys.</span><span class="sxs-lookup"><span data-stu-id="87ebb-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

