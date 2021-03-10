---
title: Tingimusjuurdepääsu kasutamine Intune ' i abil
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692976"
---
# <a name="using-conditional-access-with-intune"></a><span data-ttu-id="d2a02-102">Tingimusjuurdepääsu kasutamine Intune ' i abil</span><span class="sxs-lookup"><span data-stu-id="d2a02-102">Using Conditional Access with Intune</span></span>

<span data-ttu-id="d2a02-103">Intune ' i kasutamine Intune ' i abil nõuab kolme toimingut.</span><span class="sxs-lookup"><span data-stu-id="d2a02-103">Using Conditional Access with Intune requires 3 steps:</span></span>

- [<span data-ttu-id="d2a02-104">Saate luua nõuetele vastavuse poliitika, et määratleda sätted, mis peavad olema täidetud enne, kui seade on nõuetele vastavaks loetud. Näiteks peab seadmel olema vähemalt 6-kohaline PIN-kood, enne kui seda loetakse nõuetele vastavaks.</span><span class="sxs-lookup"><span data-stu-id="d2a02-104">Create a Compliance Policy to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [<span data-ttu-id="d2a02-105">Saate luua tingimusjuurdepääsu poliitika, mis määratleb, milliseid ressursse kaitstakse, ja milliseid tingimusi tuleb nendele ressurssidele juurdepääsuks täita. Näiteks peab seade olema ühilduv enne ettevõtte e-postile juurdepääsu.</span><span class="sxs-lookup"><span data-stu-id="d2a02-105">Create a Conditional Access Policy that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span>](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [<span data-ttu-id="d2a02-106">Veenduge, et nii nõuetele vastavuse poliitikad kui ka tingimusjuurdepääsu poliitikad on suunatud soovitud kasutajate rühmadele. See võib nõuda Azure Active Directorys teatud kasutajate rühmade loomist.</span><span class="sxs-lookup"><span data-stu-id="d2a02-106">Ensure both Compliance Policies and Conditional Access Policies are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[<span data-ttu-id="d2a02-107">Lugege lisateavet...</span><span class="sxs-lookup"><span data-stu-id="d2a02-107">Read more...</span></span>](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
