---
title: Rakenduse kaitsmise poliitika
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/22/2020
ms.locfileid: "45423595"
---
# <a name="application-protection-policy"></a><span data-ttu-id="83152-102">Rakenduse kaitsmise poliitika</span><span class="sxs-lookup"><span data-stu-id="83152-102">Application protection policy</span></span>

<span data-ttu-id="83152-103">Kui olete rakenduse Protection Policy (APP) uus, lugege teemat [rakenduse kaitsepoliitika ülevaade](https://docs.microsoft.com/intune/apps/app-protection-policy).</span><span class="sxs-lookup"><span data-stu-id="83152-103">If you're new to Application protection policy (APP), check out the [App protection policies overview](https://docs.microsoft.com/intune/apps/app-protection-policy).</span></span>

<span data-ttu-id="83152-104">RAKENDUSE kasutamise alustamiseks vaadake teemat [rakenduse kaitsmise poliitikate loomine ja määramine](https://docs.microsoft.com/intune/app-protection-policies).</span><span class="sxs-lookup"><span data-stu-id="83152-104">To start using APP, see [How to create and assign app protection policies](https://docs.microsoft.com/intune/app-protection-policies).</span></span>

<span data-ttu-id="83152-105">Application Protection Policy nõuded:</span><span class="sxs-lookup"><span data-stu-id="83152-105">Application protection policy requirements:</span></span>

- <span data-ttu-id="83152-106">Kasutajal on Intune või EMS litsents.</span><span class="sxs-lookup"><span data-stu-id="83152-106">User has an Intune or EMS license.</span></span>
- <span data-ttu-id="83152-107">Kasutaja kuulub rakenduste kaitse poliitikate sihtrühma.</span><span class="sxs-lookup"><span data-stu-id="83152-107">User belongs to a group targeted by application protection policies.</span></span>
- <span data-ttu-id="83152-108">Ainult üks ettevõtte kasutaja on seadmesse sisse logitud kaitstud rakendustes.</span><span class="sxs-lookup"><span data-stu-id="83152-108">Only one corporate user is signed into protected apps on a device.</span></span>
- <span data-ttu-id="83152-109">Rakendus on rakendanud [INTUNE SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span><span class="sxs-lookup"><span data-stu-id="83152-109">The application has implemented the [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span></span> <span data-ttu-id="83152-110">SDK-ga toetatud rakenduste loendi leiate teemast [Microsoft Intune ' i kaitstud rakendused](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span><span class="sxs-lookup"><span data-stu-id="83152-110">For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span></span>

<span data-ttu-id="83152-111">Poliitika rakendub pärast seda, kui ülaltoodud nõuetele vastav kasutaja kirjutab sisse Intune SDK toega rakenduse.</span><span class="sxs-lookup"><span data-stu-id="83152-111">Policies apply after a user who meets the above requirements signs into an Intune SDK enabled app.</span></span> <span data-ttu-id="83152-112">Lihtsaim viis määrata, kas poliitika on rakendatud, nõutakse, et kasutaja määraks poliitikas PIN-koodi.</span><span class="sxs-lookup"><span data-stu-id="83152-112">The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy.</span></span> 

<span data-ttu-id="83152-113">Lisateavet leiate järgmisest teemast.</span><span class="sxs-lookup"><span data-stu-id="83152-113">For more information, see:</span></span>

[<span data-ttu-id="83152-114">RAKENDUSE/MAM tõrkeotsingu KKK</span><span class="sxs-lookup"><span data-stu-id="83152-114">APP/MAM troubleshooting FAQ</span></span>](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[<span data-ttu-id="83152-115">Rakenduse Protection Policy setup kinnitamine</span><span class="sxs-lookup"><span data-stu-id="83152-115">How to validate your app protection policy setup</span></span>](https://docs.microsoft.com/intune/app-protection-policies-validate)

[<span data-ttu-id="83152-116">Rakenduse kaitsmise poliitikate kohaletoimetamise ajastuse mõistmine</span><span class="sxs-lookup"><span data-stu-id="83152-116">Understand App Protection Policy delivery timing</span></span>](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[<span data-ttu-id="83152-117">Rakenduse kaitsmise poliitikate jälgimine</span><span class="sxs-lookup"><span data-stu-id="83152-117">How to monitor app protection policies</span></span>](https://docs.microsoft.com/intune/app-protection-policies-monitor)