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
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657925"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="4aaa1-102">Lõppseadmete andmelekketõkestuse konfigureerimine</span><span class="sxs-lookup"><span data-stu-id="4aaa1-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="4aaa1-103">Microsofti lõppseadmete andmelekketõkestuse funktsioon lubab teil DLP kaitset ja seirevõimalusi laiendada ka Windows 10 seadmetes leiduvale delikaatsele teabele.</span><span class="sxs-lookup"><span data-stu-id="4aaa1-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="4aaa1-104">Pärast seda, kui seadmed on seadmehalduses registreeritud, saate luua DLP-poliitikad üksustega tehtavate kaitsetoimingute jõustamiseks.</span><span class="sxs-lookup"><span data-stu-id="4aaa1-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="4aaa1-105">Tegevuse-uurijat saab kasutada tegevuste kontrollimiseks delikaatse teabe asjus.</span><span class="sxs-lookup"><span data-stu-id="4aaa1-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="4aaa1-106">Lisateavet leiate artiklist [Seadmete kasutuselevõtt seadmehalduses](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="4aaa1-106">For more info, see [Onboarding devices into device management](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="4aaa1-107">Lõppseadmete andmelekketõkestuse kasutuselevõtuks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="4aaa1-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="4aaa1-108">Veenduge, et teil oleks asjakohaste SKU-de / tellimuste litsentsid.</span><span class="sxs-lookup"><span data-stu-id="4aaa1-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="4aaa1-109">Lisateavet leiate artiklist [SKU-de / tellimuste litsentsid](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="4aaa1-109">For more info, see [SKU/subscriptions licensing](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="4aaa1-110">Kontrollige üle seadmehalduse lubamise, kasutuselevõtulehele juurdepääsu või seadmeseire sisse- ja väljalülitamise õigused.</span><span class="sxs-lookup"><span data-stu-id="4aaa1-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="4aaa1-111">Lisateavet leiate artiklist [Õigused](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="4aaa1-111">For more info, see [Permissions](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="4aaa1-112">Seadmete kasutuselevõtuks seadmehalduses täitke seadmete kasutuselevõtu juhised.</span><span class="sxs-lookup"><span data-stu-id="4aaa1-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="4aaa1-113">Lisateavet leiate artiklist [Seadmete kasutuselevõtt](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="4aaa1-113">For more info, see [Onboarding devices](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="4aaa1-114">Delikaatsete üksuste kaitsmiseks looge DLP-poliitikad.</span><span class="sxs-lookup"><span data-stu-id="4aaa1-114">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="4aaa1-115">Lisateavet leiate artiklist [Lõppseadmete andmelekketõkestuse poliitika stsenaariumid](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="4aaa1-115">For info, see [Endpoint DLP policy scenarios](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="4aaa1-116">Lisateavet Microsofti lõppseadmete andmelekketõkestuse kohta leiate artiklist [Microsoft 365 lõppseadmete andmelekketõkestuse (eelversioon) teave](/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="4aaa1-116">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="4aaa1-117">**Olulised andmete kogumise juhised, kui vaja on kasutajatuge**</span><span class="sxs-lookup"><span data-stu-id="4aaa1-117">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="4aaa1-118">Laadige [alla MDATP kliendi analüsaatori eelvaade.](https://aka.ms/betamdatpanalyzer)</span><span class="sxs-lookup"><span data-stu-id="4aaa1-118">Download [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span></span>
1. <span data-ttu-id="4aaa1-119">Käivitage tööriist administraatorina käsuviibaaknas:</span><span class="sxs-lookup"><span data-stu-id="4aaa1-119">Run the tool as Admin from the cmd window:</span></span>

    <span data-ttu-id="4aaa1-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span><span class="sxs-lookup"><span data-stu-id="4aaa1-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span></span>

1. <span data-ttu-id="4aaa1-121">Kui kuvatakse teade **Sisestage jälituste** kogumiseks minutite arv: sisestage stsenaariumi käivitamiseks vajalik minutite arv.</span><span class="sxs-lookup"><span data-stu-id="4aaa1-121">When prompted with **Enter the number of minutes to collect traces:**, enter the number of minutes required to run the scenario.</span></span>
1. <span data-ttu-id="4aaa1-122">Käivitage stsenaarium.</span><span class="sxs-lookup"><span data-stu-id="4aaa1-122">Run the scenario.</span></span>

<span data-ttu-id="4aaa1-123">Koguge zip-faili väljund tugiagendile andmiseks.</span><span class="sxs-lookup"><span data-stu-id="4aaa1-123">Collect the Zip file output to give to the Support agent.</span></span>
