---
title: Apple ' i automaatse liitumise sünkroonimise tõrked
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714737"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="2a9fc-102">Apple ' i automaatse liitumise sünkroonimise tõrked</span><span class="sxs-lookup"><span data-stu-id="2a9fc-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="2a9fc-103">"Oleme tuvastanud, et teil on üks või mitu ADE/DEP tõendit, mis on tõrke olekus.</span><span class="sxs-lookup"><span data-stu-id="2a9fc-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="2a9fc-104">Kuni tõrke olekuks on lahendatud iga mõjutatud tõendi korral, ei tööta funktsioon ADE sama ".</span><span class="sxs-lookup"><span data-stu-id="2a9fc-104">Until the error state is resolved for each affected token, the ADE functionality will not work for the same”.</span></span>

<span data-ttu-id="2a9fc-105">See tõrge võib ilmneda mitmel viisil (sh:</span><span class="sxs-lookup"><span data-stu-id="2a9fc-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="2a9fc-106">Seadmeid ei pruugita sünkroonida tegevuspõhise juhtimise/ASM abil</span><span class="sxs-lookup"><span data-stu-id="2a9fc-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="2a9fc-107">Registreerimise profiili ülesanded võivad ebaõnnestuda</span><span class="sxs-lookup"><span data-stu-id="2a9fc-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="2a9fc-108">Seadmeid ei pruugita lõpule viia, kuna ADE registreerimine õnnestus</span><span class="sxs-lookup"><span data-stu-id="2a9fc-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="2a9fc-109">Kui soovite, et jaotises **seadmed > Registreeri seadmed > Apple ' i registreerimiseks >** registreerimiseks ette nähtud sünkroonimise tõrked ja vaadake üle järgmised dokumendid, et näha võimalikke tervendamist.</span><span class="sxs-lookup"><span data-stu-id="2a9fc-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens** and review the following documentation to see any potential remediation:</span></span>

[<span data-ttu-id="2a9fc-110">Autojuhtimise/ASM sünkroonimise tõrked iOS-i/iPadOS ja macOS ' i automaatse registreerimise märkide korral</span><span class="sxs-lookup"><span data-stu-id="2a9fc-110">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
