---
title: Juurdepääs Intune ' i tingimustega
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807655"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="40aa1-102">Juurdepääs Intune ' i tingimustega</span><span class="sxs-lookup"><span data-stu-id="40aa1-102">Conditional Access with Intune</span></span>

<span data-ttu-id="40aa1-103">Intune  **' i**  kasutamine Intune ' i abil nõuab kolme toimingut.</span><span class="sxs-lookup"><span data-stu-id="40aa1-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="40aa1-104">Saate luua  **nõuetele vastavuse poliitika**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)), et määratleda sätted, mis peavad olema täidetud enne, kui seade on nõuetele vastavaks loetud.</span><span class="sxs-lookup"><span data-stu-id="40aa1-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="40aa1-105">Näiteks peab seadmel olema vähemalt 6-kohaline PIN-kood, enne kui seda loetakse nõuetele vastavaks.</span><span class="sxs-lookup"><span data-stu-id="40aa1-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="40aa1-106">Saate luua **tingimusjuurdepääsu poliitika**  , mis määratleb, milliseid ressursse kaitstakse, ja milliseid tingimusi tuleb nendele ressurssidele juurdepääsuks täita.</span><span class="sxs-lookup"><span data-stu-id="40aa1-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="40aa1-107">[Näiteks](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  peab seade olema ühilduv enne ettevõtte e-postile juurdepääsu.</span><span class="sxs-lookup"><span data-stu-id="40aa1-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="40aa1-108">Veenduge, et nii **nõuetele vastavuse poliitikad**  kui ka  **tingimusjuurdepääsu poliitikad**  on suunatud soovitud kasutajate rühmadele.</span><span class="sxs-lookup"><span data-stu-id="40aa1-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="40aa1-109">See võib nõuda Azure Active Directorys teatud kasutajate rühmade loomist.</span><span class="sxs-lookup"><span data-stu-id="40aa1-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="40aa1-110">**Kasulikud lingid:**</span><span class="sxs-lookup"><span data-stu-id="40aa1-110">**Helpful links:**</span></span>

[<span data-ttu-id="40aa1-111">Seadme nõuetele vastavuse ülevaade</span><span class="sxs-lookup"><span data-stu-id="40aa1-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="40aa1-112">Tõrkeotsing CA</span><span class="sxs-lookup"><span data-stu-id="40aa1-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="40aa1-113">Tõrkeotsingu poliitika</span><span class="sxs-lookup"><span data-stu-id="40aa1-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="40aa1-114">Meili (Exchange Online) ' i kaitsmiseks lubamatute seadmete kaudu juurdepääsu eest tuleb järgida mõlemat dokumenti.</span><span class="sxs-lookup"><span data-stu-id="40aa1-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="40aa1-115">E-posti kaitse kasutamine EAS-i kasutavates seadmetes</span><span class="sxs-lookup"><span data-stu-id="40aa1-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="40aa1-116">Meilikontode kaitsmine seadmete kaudu, mis kasutavad kaasaegseid autentimise kliente (nt Outlook)</span><span class="sxs-lookup"><span data-stu-id="40aa1-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)