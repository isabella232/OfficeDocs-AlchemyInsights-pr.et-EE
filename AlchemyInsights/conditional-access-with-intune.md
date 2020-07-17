---
title: Tingimuslik juurdepääs Intune'iga
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931426"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="9e542-102">Tingimuslik juurdepääs Intune'iga</span><span class="sxs-lookup"><span data-stu-id="9e542-102">Conditional Access with Intune</span></span>

<span data-ttu-id="9e542-103">**Tingimusjuurdepääsu** kasutamine Intune'iga nõuab kolme etappi.</span><span class="sxs-lookup"><span data-stu-id="9e542-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="9e542-104">Looge **vastavuspoliitika** [(Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)), et määratleda sätted, mis peavad olema täidetud enne seadme nõuetele vastavust.</span><span class="sxs-lookup"><span data-stu-id="9e542-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="9e542-105">Näiteks peab seadmel olema vähemalt 6-kohaline viik, enne kui seda loetakse nõuetele vastavaks.</span><span class="sxs-lookup"><span data-stu-id="9e542-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="9e542-106">Looge **tingimusjuurdepääsu poliitika,** mis määratleb, milliseid ressursse kaitstakse ja millised tingimused peavad nendele ressurssidele juurdepääsuks olema täidetud.</span><span class="sxs-lookup"><span data-stu-id="9e542-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="9e542-107">[Näiteks](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) seade peab olema ühilduv enne juurdepääsu ettevõtte e-posti.</span><span class="sxs-lookup"><span data-stu-id="9e542-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="9e542-108">Veenduge, et nii **vastavuspoliitika** kui ka **tingimusjuurdepääsu poliitika** on suunatud soovitud kasutajarühmadele.</span><span class="sxs-lookup"><span data-stu-id="9e542-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="9e542-109">See võib nõuda teatud kasutajate rühmade loomine Azure Active Directorys.</span><span class="sxs-lookup"><span data-stu-id="9e542-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="9e542-110">**Kasulikud lingid:**</span><span class="sxs-lookup"><span data-stu-id="9e542-110">**Helpful links:**</span></span>

[<span data-ttu-id="9e542-111">Seadme vastavuse ülevaade</span><span class="sxs-lookup"><span data-stu-id="9e542-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="9e542-112">Ca tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="9e542-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="9e542-113">Tõrkeotsingu poliitika</span><span class="sxs-lookup"><span data-stu-id="9e542-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="9e542-114">Meili (Exchange Online'i) kaitsmiseks mitteühilduvate seadmete juurdepääsu eest tuleb järgida mõlemat dokumenti.</span><span class="sxs-lookup"><span data-stu-id="9e542-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="9e542-115">EAS-i abil e-posti juurdepääsu kaitsmine seadmete eest</span><span class="sxs-lookup"><span data-stu-id="9e542-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="9e542-116">Kaitske e-posti juurdepääsu seadmetest, mis kasutavad kaasaegseid autentimiskliente nagu Outlook</span><span class="sxs-lookup"><span data-stu-id="9e542-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)