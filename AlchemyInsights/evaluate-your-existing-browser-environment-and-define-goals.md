---
title: Olemasoleva brauseri keskkonna väärtustamine ja eesmärkide määratlemine
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9141"
- "9005291"
ms.openlocfilehash: 5b03d188aa78be83928cf262f1d86f3f933c85ab
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693001"
---
# <a name="evaluate-your-existing-browser-environment-and-define-goals"></a><span data-ttu-id="67928-102">Olemasoleva brauseri keskkonna väärtustamine ja eesmärkide määratlemine</span><span class="sxs-lookup"><span data-stu-id="67928-102">Evaluate your existing browser environment and define goals</span></span>

<span data-ttu-id="67928-103">Võttes aega, et mõista oma praegust brauseri olekut ja projekti visiooni, tagab kõigi projekti sidusrühmade vastavusseviimise ja töötab sama eesmärgi poole.</span><span class="sxs-lookup"><span data-stu-id="67928-103">Taking time to understand your current browser state and project vision ensures all project stakeholders are aligned and are working toward the same goal.</span></span> <span data-ttu-id="67928-104">Tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="67928-104">Follow these steps:</span></span>

1. <span data-ttu-id="67928-105">Määratlege praegune olek.</span><span class="sxs-lookup"><span data-stu-id="67928-105">Define your current state.</span></span> <span data-ttu-id="67928-106">Kaaluge järgmist.</span><span class="sxs-lookup"><span data-stu-id="67928-106">Consider the following:</span></span>
- <span data-ttu-id="67928-107">Milliseid brausereid teie keskkonnas praegu kasutatakse?</span><span class="sxs-lookup"><span data-stu-id="67928-107">Which browsers are currently deployed in your environment?</span></span>
- <span data-ttu-id="67928-108">Milline brauser on määratud vaikebrauseriks?</span><span class="sxs-lookup"><span data-stu-id="67928-108">Which browser is set as the default browser?</span></span>
- <span data-ttu-id="67928-109">Kas teil on vaja mõne rakenduse jaoks kasutada Internet Explorerit?</span><span class="sxs-lookup"><span data-stu-id="67928-109">Do you need to use Internet Explorer for some of your apps?</span></span>
- <span data-ttu-id="67928-110">Kas kasutate Enterprise ' i režiimi saitide loendit, et konfigureerida Internet Explorerit juba täna?</span><span class="sxs-lookup"><span data-stu-id="67928-110">Do you use an Enterprise Mode Site List to configure Internet Explorer today?</span></span>
- <span data-ttu-id="67928-111">Millised OS-i platvormid (nt Windows 10 ja macOS) toetavad teie keskkonna tuge?</span><span class="sxs-lookup"><span data-stu-id="67928-111">Which OS platforms, such as Windows 10 and macOS, does your environment support?</span></span>
- <span data-ttu-id="67928-112">Milliseid halduse tööriistu te brauseri haldamiseks kasutate?</span><span class="sxs-lookup"><span data-stu-id="67928-112">Which management tools do you use for browser management?</span></span>
- <span data-ttu-id="67928-113">Kes vastutab brauseri häälestamise ja haldamise eest?</span><span class="sxs-lookup"><span data-stu-id="67928-113">Who's responsible for browser configuration and management?</span></span>
- <span data-ttu-id="67928-114">Mis on brauseri ühilduvuse valideerimise protsess?</span><span class="sxs-lookup"><span data-stu-id="67928-114">What's the process for validating browser compatibility?</span></span>
2. <span data-ttu-id="67928-115">Saate määratleda juurutuse eesmärgid.</span><span class="sxs-lookup"><span data-stu-id="67928-115">Define the goals for your deployment.</span></span> <span data-ttu-id="67928-116">Pidage meeles järgmisi asju.</span><span class="sxs-lookup"><span data-stu-id="67928-116">Keep the following things in mind:</span></span>
- <span data-ttu-id="67928-117">Kas soovite [määrata Microsoft Edge](https://docs.microsoft.com/DeployEdge/edge-default-browser)' i vaikebrauseriks?</span><span class="sxs-lookup"><span data-stu-id="67928-117">Do you want to [set Microsoft Edge as your default browser](https://docs.microsoft.com/DeployEdge/edge-default-browser)?</span></span>
- <span data-ttu-id="67928-118">Kas soovite peita Microsoft Edge ' i pärandi versiooni või soovite [selle kasutajatele kättesaadavaks jätta](https://docs.microsoft.com/DeployEdge/microsoft-edge-sysupdate-access-old-edge)?</span><span class="sxs-lookup"><span data-stu-id="67928-118">Do you want to hide the legacy version of Microsoft Edge or do you want to [leave it available for users](https://docs.microsoft.com/DeployEdge/microsoft-edge-sysupdate-access-old-edge)?</span></span>
- <span data-ttu-id="67928-119">Kuidas [konfigureerida Microsoft Edge](https://docs.microsoft.com/DeployEdge/configure-microsoft-edge)' i?</span><span class="sxs-lookup"><span data-stu-id="67928-119">How will you [configure Microsoft Edge](https://docs.microsoft.com/DeployEdge/configure-microsoft-edge)?</span></span>
- <span data-ttu-id="67928-120">Milliseid funktsioone on teie algse juurutuse osana oluline konfigureerida?</span><span class="sxs-lookup"><span data-stu-id="67928-120">What features are critical to configure as part of your initial deployment?</span></span>
- <span data-ttu-id="67928-121">Mis on mis tahes tuvastatud ühilduvuse või konfiguratsiooni probleemide lahendamise protsess?</span><span class="sxs-lookup"><span data-stu-id="67928-121">What is the process for addressing any identified compatibility or configuration issues?</span></span>
3. <span data-ttu-id="67928-122">Saate teada, milliste funktsioonide eeltingimusi soovite kasutada, näiteks:</span><span class="sxs-lookup"><span data-stu-id="67928-122">Understand the prerequisites for features you might want to use, such as:</span></span>
- [<span data-ttu-id="67928-123">Windows Defenderi rakenduse valvur</span><span class="sxs-lookup"><span data-stu-id="67928-123">Windows Defender Application Guard</span></span>](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-application-guard/reqs-md-app-guard)
- [<span data-ttu-id="67928-124">Internet Exploreri režiim</span><span class="sxs-lookup"><span data-stu-id="67928-124">Internet Explorer mode</span></span>](https://docs.microsoft.com/DeployEdge/edge-ie-mode)
- [<span data-ttu-id="67928-125">Autentimine ja sünkroonimine</span><span class="sxs-lookup"><span data-stu-id="67928-125">Authentication and sync</span></span>](https://docs.microsoft.com/DeployEdge/microsoft-edge-security-identity)

<span data-ttu-id="67928-126">Kui olete need juhised täitnud, olete valmis alustama oma juurutamise strateegia kavandamist.</span><span class="sxs-lookup"><span data-stu-id="67928-126">After you complete these steps, you're ready to start planning your deployment strategy.</span></span>
