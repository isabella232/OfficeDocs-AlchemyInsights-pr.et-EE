---
title: E-juurdluse tõrkeotsing sisaldab tõrkeid
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676147"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a><span data-ttu-id="9bf29-102">E-juurdluse tõrkeotsing sisaldab tõrkeid</span><span class="sxs-lookup"><span data-stu-id="9bf29-102">Troubleshooting ediscovery holds errors</span></span>

<span data-ttu-id="9bf29-103">Kas teil on probleeme e-juurdlusega?</span><span class="sxs-lookup"><span data-stu-id="9bf29-103">Experiencing issues with eDiscovery holds?</span></span> <span data-ttu-id="9bf29-104">Siin on mõned head tavad, mida kaaluda.</span><span class="sxs-lookup"><span data-stu-id="9bf29-104">Here are some best practices to consider:</span></span>

- <span data-ttu-id="9bf29-105">Kontrollige ootel jaotusolekut.</span><span class="sxs-lookup"><span data-stu-id="9bf29-105">Check the hold distribution status.</span></span>  <span data-ttu-id="9bf29-106">Kui olek **on Sees (Ootel) või** Väljas **(Ootel),** oodake, kuni ootel jaotus on lõpule viidud.</span><span class="sxs-lookup"><span data-stu-id="9bf29-106">If status is **On (Pending)** or **Off (Pending)**, wait for hold distribution to complete.</span></span>
- <span data-ttu-id="9bf29-107">E-juurdluse värskenduste ühendamine ühekordse hulgitaotlusena, mitte iga tehingu poliitika korduva värskendamise asemel.</span><span class="sxs-lookup"><span data-stu-id="9bf29-107">Merge eDiscovery hold updates into a single bulk request instead of updating the policy repeatedly for each transaction.</span></span>
- <span data-ttu-id="9bf29-108">Käivitage Set-CaseHoldPolicy <policyname> -RetryDistribution turbe- ja vastavuskeskuse PowerShellis.</span><span class="sxs-lookup"><span data-stu-id="9bf29-108">Run Set-CaseHoldPolicy <policyname> -RetryDistribution in the Security and Compliance Center Powershell.</span></span> <span data-ttu-id="9bf29-109">Lisateavet leiate teemast [Ühendus Security & PowerShell](/powershell/exchange/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="9bf29-109">For details, see [Connect to Security & Compliance Center PowerShell](/powershell/exchange/connect-to-scc-powershell).</span></span>

<span data-ttu-id="9bf29-110">Nende sätete ja täiendavate e-juurdluse leevendamise ja lahendamise parimate tavade kontrolli juhised leiate teemast [E-juurdluse ootel](/microsoft-365/compliance/hold-distribution-errors)oleku tõrgete tõrkeotsing.</span><span class="sxs-lookup"><span data-stu-id="9bf29-110">For steps to check these settings and additional best practices for mitigating and resolving eDiscovery holds issues, see [Troubleshoot eDiscovery hold errors](/microsoft-365/compliance/hold-distribution-errors).</span></span>
<span data-ttu-id="9bf29-111">Lisateavet muude levinud e-juurdluse probleemide tõrkeotsingu kohta leiate teemast [Levinuma](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)e-juurdluse probleemide juurdlus, tõrkeotsing ja lahendamine.</span><span class="sxs-lookup"><span data-stu-id="9bf29-111">For info about troubleshooting other common eDiscovery issues, see [Investigate, troubleshoot, and resolve common eDiscovery issues](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span></span>
