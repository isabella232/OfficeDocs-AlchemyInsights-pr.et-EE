---
title: Lõpp-punkti DLP konfigureerimine
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 039c8f78c5896b66eab5763fb0bbddd3f0b06f2d
ms.sourcegitcommit: 1dada930649a2625eb6d15910b2bfd5e1e00e5b6
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/03/2020
ms.locfileid: "46555129"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="a0aa1-102">Lõpp-punkti DLP konfigureerimine</span><span class="sxs-lookup"><span data-stu-id="a0aa1-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="a0aa1-103">Microsoft Endpoint DLP võimaldab teil Windows 10 seadmetes tundlikku teavet laiendada DLP kaitse ja jälgimise võimalustest.</span><span class="sxs-lookup"><span data-stu-id="a0aa1-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="a0aa1-104">Kui seadmed on seadme haldusse sisse lülitatud, saate üksustele kaitsemeetmete rakendamiseks luua DLP poliitika.</span><span class="sxs-lookup"><span data-stu-id="a0aa1-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="a0aa1-105">Tegevuste Explorerit saab kasutada tundlike üksuste tegevuse jälgimiseks.</span><span class="sxs-lookup"><span data-stu-id="a0aa1-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="a0aa1-106">Lisateavet leiate teemast [seadmete juhtimine seadme haldusse](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="a0aa1-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="a0aa1-107">Lõpp-punkti DLP alustamiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="a0aa1-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="a0aa1-108">Veenduge, et teil oleks sobiv SKU/tellimused litsentseeritud.</span><span class="sxs-lookup"><span data-stu-id="a0aa1-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="a0aa1-109">Lisateavet leiate teemast [SKU/tellimused litsentseerimine](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="a0aa1-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="a0aa1-110">Kontrollige, kas teil on vaja seadmete halduse lubamiseks, juurdepääsuks lehel või lülitage sisse/välja seadme jälgimine.</span><span class="sxs-lookup"><span data-stu-id="a0aa1-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="a0aa1-111">Lisateavet leiate teemast [permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="a0aa1-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="a0aa1-112">Seadmete juhtimine seadme juhtimiseks, järgides seadmete protseduuri.</span><span class="sxs-lookup"><span data-stu-id="a0aa1-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="a0aa1-113">Kui te ei leia jaotises M365 nõuetele vastavat seadet (eelvaade **), veenduge**, et teil on eespool viidatud vastav litsents ja load.</span><span class="sxs-lookup"><span data-stu-id="a0aa1-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="a0aa1-114">Lisateavet leiate teemast [seadmete](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices)sisselogimine.</span><span class="sxs-lookup"><span data-stu-id="a0aa1-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="a0aa1-115">Saate luua DLP poliitikaid, et kaitsta oma tundlikke üksusi.</span><span class="sxs-lookup"><span data-stu-id="a0aa1-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="a0aa1-116">Lisateavet leiate teemast [lõpp-punkti DLP poliitika stsenaariumid](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="a0aa1-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="a0aa1-117">Lisateavet Microsofti lõpp-punkti DLP kohta leiate teemast teave [microsoft 365 lõpp-punkti andmete kaotsimineku vältimise kohta (eelvaade)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="a0aa1-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>