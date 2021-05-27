---
title: Näidikud ei tööta Edge'i brauseris
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676239"
---
# <a name="indicators-dont-work-using-edge-browser"></a><span data-ttu-id="88e1a-102">Näidikud ei tööta Edge'i brauseris</span><span class="sxs-lookup"><span data-stu-id="88e1a-102">Indicators don't work using Edge browser</span></span>

<span data-ttu-id="88e1a-103">Pärast näidiku loomist ei pea Edge (Smartscreen) seda austama.</span><span class="sxs-lookup"><span data-stu-id="88e1a-103">After you created an Indicator, it's not honored by Edge (Smartscreen).</span></span> <span data-ttu-id="88e1a-104">Lisateavet leiate teemast [IPde ja URL-ide/domeenide näidikute loomine.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="88e1a-104">For more information, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>

## <a name="step-1-ensure-the-following"></a><span data-ttu-id="88e1a-105">1. juhis. Veenduge, et</span><span class="sxs-lookup"><span data-stu-id="88e1a-105">Step 1: Ensure the following</span></span>

- <span data-ttu-id="88e1a-106">Veenduge, et indikaator on õige (IP/URL-is ei ole kirjavigu, õige toiming, õiged RBAC-rühmad).</span><span class="sxs-lookup"><span data-stu-id="88e1a-106">Verify that the indicator is correct (no typos in IP/URL, correct action, the correct RBAC groups).</span></span>
- <span data-ttu-id="88e1a-107">Võimaliku latentsuse arvesse miseks oodake pärast näidiku loomist vähemalt 2 tundi.</span><span class="sxs-lookup"><span data-stu-id="88e1a-107">Wait the minimum 2 hours after creating the indicator to take into account any possible latency.</span></span>
- <span data-ttu-id="88e1a-108">Veenduge, et süsteem(id) on microsoft Defenderi lõpp-punkti jaoks sisse logitud.</span><span class="sxs-lookup"><span data-stu-id="88e1a-108">Confirm that the system(s) are onboarded to Microsoft Defender for Endpoint.</span></span>
- <span data-ttu-id="88e1a-109">Veenduge, et süsteem(id) saaks pilveteenusega suhelda.</span><span class="sxs-lookup"><span data-stu-id="88e1a-109">Verify that system(s) can communicate with the Cloud.</span></span>
- <span data-ttu-id="88e1a-110">Kontrollige, kas Smartscreen on lubatud ja kasutatav, kui avate [testimissaidi.](https://demo.smartscreen.msft.net)</span><span class="sxs-lookup"><span data-stu-id="88e1a-110">Verify that Smartscreen is enabled and reachable by going to the [test site](https://demo.smartscreen.msft.net).</span></span>

## <a name="step-2-troubleshoot-the-potential-issue"></a><span data-ttu-id="88e1a-111">2. juhis. Võimaliku probleemi tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="88e1a-111">Step 2: Troubleshoot the potential issue</span></span>

- <span data-ttu-id="88e1a-112">Veenduge, et klient vastaks nõuetele.</span><span class="sxs-lookup"><span data-stu-id="88e1a-112">Make sure the client meets the requirements.</span></span> <span data-ttu-id="88e1a-113">Lisateavet leiate teemast [IPde ja URL-ide/domeenide jaoks näidikute loomine.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="88e1a-113">For details, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>
- <span data-ttu-id="88e1a-114">Veenduge, et kasutate Edge'i brauseri uusimat versiooni.</span><span class="sxs-lookup"><span data-stu-id="88e1a-114">Make sure you're running the latest version of the Edge browser.</span></span> <span data-ttu-id="88e1a-115">Uusima versiooni kohta leiate teavet teemast [Microsoft Edge versioon.](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)</span><span class="sxs-lookup"><span data-stu-id="88e1a-115">To find out the latest version, see [Find out which version of Microsoft Edge you have](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span></span>
- <span data-ttu-id="88e1a-116">Taaskäivitage Edge'i brauser.</span><span class="sxs-lookup"><span data-stu-id="88e1a-116">Restart the Edge browser.</span></span>
- <span data-ttu-id="88e1a-117">Liikuge saidile, mille jaoks olete näidiku häälestanud.</span><span class="sxs-lookup"><span data-stu-id="88e1a-117">Navigate to the site for which you have setup an indicator.</span></span> <span data-ttu-id="88e1a-118">Kui sait ei kuvata ootuspäraselt, jätkake 3. juhise kasutamist.</span><span class="sxs-lookup"><span data-stu-id="88e1a-118">If the site does not appear as expected, continue to Step 3.</span></span> 

## <a name="step-3-collect-data"></a><span data-ttu-id="88e1a-119">3. juhis: andmete kogumine</span><span class="sxs-lookup"><span data-stu-id="88e1a-119">Step 3: Collect data</span></span>

- <span data-ttu-id="88e1a-120">Koguge **MDEClientAnalyzeri diagnostikaandmeid.**</span><span class="sxs-lookup"><span data-stu-id="88e1a-120">Collect **MDEClientAnalyzer** diagnostic data.</span></span> <span data-ttu-id="88e1a-121">Juhised leiate teemast Microsoft Defender for Endpoint'ile [sisseldumisseadmetega seotud probleemid.](issues-with-onboarding-machines.md)</span><span class="sxs-lookup"><span data-stu-id="88e1a-121">For instructions, see [Issues with onboarding machines to Microsoft Defender for Endpoint](issues-with-onboarding-machines.md).</span></span>
- <span data-ttu-id="88e1a-122">Kui teil on mugav Fiddleri jälitust installida ja koguda, lugege [teemat Telerik Fiddler](http://www.telerik.com/fiddler).</span><span class="sxs-lookup"><span data-stu-id="88e1a-122">If you are comfortable installing and collecting a Fiddler trace, see [Telerik Fiddler](http://www.telerik.com/fiddler).</span></span>
- <span data-ttu-id="88e1a-123">Kui eelistate Microsofti tugiteenuste juhiseid, valige tugiteenuse juhtumi avamiseks allpool ikoon Tugi.</span><span class="sxs-lookup"><span data-stu-id="88e1a-123">If you prefer guidance from Microsoft Support, select the Support icon below to open a support case.</span></span>
