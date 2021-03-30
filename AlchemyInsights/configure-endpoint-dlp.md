---
title: Lõppseadmete andmelekketõkestuse konfigureerimine
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402416"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="b776f-102">Lõppseadmete andmelekketõkestuse konfigureerimine</span><span class="sxs-lookup"><span data-stu-id="b776f-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="b776f-103">Microsofti lõppseadmete andmelekketõkestuse funktsioon lubab teil DLP kaitset ja seirevõimalusi laiendada ka Windows 10 seadmetes leiduvale delikaatsele teabele.</span><span class="sxs-lookup"><span data-stu-id="b776f-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="b776f-104">Pärast seda, kui seadmed on seadmehalduses registreeritud, saate luua DLP-poliitikad üksustega tehtavate kaitsetoimingute jõustamiseks.</span><span class="sxs-lookup"><span data-stu-id="b776f-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="b776f-105">Tegevuse-uurijat saab kasutada tegevuste kontrollimiseks delikaatse teabe asjus.</span><span class="sxs-lookup"><span data-stu-id="b776f-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="b776f-106">Lisateavet leiate artiklist [Seadmete kasutuselevõtt seadmehalduses](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="b776f-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="b776f-107">Lõppseadmete andmelekketõkestuse kasutuselevõtuks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="b776f-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="b776f-108">Veenduge, et teil oleks asjakohaste SKU-de / tellimuste litsentsid.</span><span class="sxs-lookup"><span data-stu-id="b776f-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="b776f-109">Lisateavet leiate artiklist [SKU-de / tellimuste litsentsid](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="b776f-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="b776f-110">Kontrollige üle seadmehalduse lubamise, kasutuselevõtulehele juurdepääsu või seadmeseire sisse- ja väljalülitamise õigused.</span><span class="sxs-lookup"><span data-stu-id="b776f-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="b776f-111">Lisateavet leiate artiklist [Õigused](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="b776f-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="b776f-112">Seadmete kasutuselevõtuks seadmehalduses täitke seadmete kasutuselevõtu juhised.</span><span class="sxs-lookup"><span data-stu-id="b776f-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="b776f-113">Kui te ei näe M365 vastavuskeskuse jaotises **Sätted** seadmete kasutuselevõtu (eelversiooni) sätet, siis veenduge, et teil oleksid olemas eespool viidatud vajalikud litsentsid ja õigused.</span><span class="sxs-lookup"><span data-stu-id="b776f-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="b776f-114">Lisateavet leiate artiklist [Seadmete kasutuselevõtt](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="b776f-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="b776f-115">Delikaatsete üksuste kaitsmiseks looge DLP-poliitikad.</span><span class="sxs-lookup"><span data-stu-id="b776f-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="b776f-116">Lisateavet leiate artiklist [Lõppseadmete andmelekketõkestuse poliitika stsenaariumid](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="b776f-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span></span>

<span data-ttu-id="b776f-117">Lisateavet Microsofti lõppseadmete andmelekketõkestuse kohta leiate artiklist [Microsoft 365 lõppseadmete andmelekketõkestuse (eelversioon) teave](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="b776f-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="b776f-118">**Olulised andmete kogumise juhised, kui vaja on kasutajatuge**</span><span class="sxs-lookup"><span data-stu-id="b776f-118">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="b776f-119">Laadige siit alla MDATP Client Analyzeri eelversioon: [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer").</span><span class="sxs-lookup"><span data-stu-id="b776f-119">Download MDATP Client Analyzer Preview from [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span></span>
2. <span data-ttu-id="b776f-120">Käivitage tööriist administraatorina käsuviibaaknas:</span><span class="sxs-lookup"><span data-stu-id="b776f-120">Run the tool as Admin from the cmd window:</span></span>
3. <span data-ttu-id="b776f-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span><span class="sxs-lookup"><span data-stu-id="b776f-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span></span>
4. <span data-ttu-id="b776f-122">Kui teil palutakse sisestada jälitusteabe kogumise kestus minututes, sisestage stsenaariumi käitamiseks vajalik aeg minutites.</span><span class="sxs-lookup"><span data-stu-id="b776f-122">When prompted with “Enter the number of minutes to collect traces: ", enter the number of minutes that are required to run the scenario</span></span>
5. <span data-ttu-id="b776f-123">Käivitage stsenaarium.</span><span class="sxs-lookup"><span data-stu-id="b776f-123">Run the scenario</span></span>

<span data-ttu-id="b776f-124">Koguge tugiagendile edastamiseks vajalik väljund-ZIP-fail.</span><span class="sxs-lookup"><span data-stu-id="b776f-124">Collect the Zip file output to be given to the Support agent.</span></span>
