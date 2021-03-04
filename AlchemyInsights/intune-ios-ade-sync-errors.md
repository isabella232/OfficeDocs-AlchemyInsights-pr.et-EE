---
title: Apple ' i automaatse liitumise sünkroonimise tõrked
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448918"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="3f8da-102">Apple ' i automaatse liitumise sünkroonimise tõrked</span><span class="sxs-lookup"><span data-stu-id="3f8da-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="3f8da-103">"Oleme tuvastanud, et teil on üks või mitu ADE/DEP tõendit, mis on tõrke olekus.</span><span class="sxs-lookup"><span data-stu-id="3f8da-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="3f8da-104">Kui tõrketeade on lahendatud iga mõjutatud tõendi korral, siis ei tööta funktsioon ADE ootuspäraselt. ".</span><span class="sxs-lookup"><span data-stu-id="3f8da-104">Until the error state is resolved for each affected token, the ADE functionality will not work as expected.”.</span></span>

<span data-ttu-id="3f8da-105">See tõrge võib ilmneda mitmel viisil (sh:</span><span class="sxs-lookup"><span data-stu-id="3f8da-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="3f8da-106">Seadmeid ei pruugita sünkroonida tegevuspõhise juhtimise/ASM abil</span><span class="sxs-lookup"><span data-stu-id="3f8da-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="3f8da-107">Registreerimise profiili ülesanded võivad ebaõnnestuda</span><span class="sxs-lookup"><span data-stu-id="3f8da-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="3f8da-108">Seadmeid ei pruugita lõpule viia, kuna ADE registreerimine õnnestus</span><span class="sxs-lookup"><span data-stu-id="3f8da-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="3f8da-109">Kontrollige, kas jaotises **seadmed > Registreeri seadmed > Apple ' i liitumise > registreerimise programmi märkidega** sünkroonitud tõrge.</span><span class="sxs-lookup"><span data-stu-id="3f8da-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens**.</span></span>

<span data-ttu-id="3f8da-110">Sünkroonimise tõrke mõni levinumaid põhjusi on praeguse tõendi aegumine.</span><span class="sxs-lookup"><span data-stu-id="3f8da-110">One of the most common causes of sync error is expiration of the current token.</span></span> <span data-ttu-id="3f8da-111">Paljudel juhtudel lahendab mõjutatud tõendi pikendamise probleemi.</span><span class="sxs-lookup"><span data-stu-id="3f8da-111">In many cases,renewal of the affected token will resolve the issue.</span></span>

<span data-ttu-id="3f8da-112">Kui mõni teie märkidest on aegunud, lugege järgmisi dokumente, mis aitavad teil neid vastavalt vajadusele uuendada.</span><span class="sxs-lookup"><span data-stu-id="3f8da-112">If one or more of your tokens has expired,  see the following documentation to help you renew them as appropriate:</span></span>

[<span data-ttu-id="3f8da-113">Automatiseeritud seadme registreerimise loa pikendamine</span><span class="sxs-lookup"><span data-stu-id="3f8da-113">Renew an Automated Device Enrollment token</span></span>](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

<span data-ttu-id="3f8da-114">Lisaks saate vaadata järgmisi dokumente, et näha võimalikke ümbervahendusi muude tõrgete korral, mis põhjustavad märkide sünkroonimise tõrkeid.</span><span class="sxs-lookup"><span data-stu-id="3f8da-114">In addition, you can see the following documentation to see potential remediations for other errors causing token synchronization failures:</span></span>

[<span data-ttu-id="3f8da-115">Autojuhtimise/ASM sünkroonimise tõrked iOS-i/iPadOS ja macOS ' i automaatse registreerimise märkide korral</span><span class="sxs-lookup"><span data-stu-id="3f8da-115">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[<span data-ttu-id="3f8da-116">Autojuhtimise/ASM sünkroonimise tõrked iOS-i/iPadOS ja macOS ' i automaatse registreerimise märkide korral</span><span class="sxs-lookup"><span data-stu-id="3f8da-116">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
