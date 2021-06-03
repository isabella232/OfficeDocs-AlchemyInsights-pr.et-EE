---
title: Lõpp-punkti DLP pole kasutaja seadmesse juurutatud
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731410"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a><span data-ttu-id="e703e-102">Lõpp-punkti DLP pole kasutaja seadmesse juurutatud</span><span class="sxs-lookup"><span data-stu-id="e703e-102">Endpoint DLP not deployed to user's device</span></span>

<span data-ttu-id="e703e-103">Kui sätte Lõpp-punkti andmete kaotsimineku vältimine (DLP) pole kasutaja seadmele rakendatud, veenduge, et vastate neile nõuetele.</span><span class="sxs-lookup"><span data-stu-id="e703e-103">If the Endpoint data loss prevention (DLP) setting has not applied to a user's device, confirm you meet these requirements:</span></span>

- <span data-ttu-id="e703e-104">Windows 10 on installitud x64 järk 1809 või uuem versioon.</span><span class="sxs-lookup"><span data-stu-id="e703e-104">Windows 10 x64 build 1809 or later is installed on the device.</span></span>
- <span data-ttu-id="e703e-105">Ründevaratõrje klientversioon 4.18.2009.7 või uuem versioon on installitud.</span><span class="sxs-lookup"><span data-stu-id="e703e-105">Anti-malware client version 4.18.2009.7 or later is installed.</span></span>
- <span data-ttu-id="e703e-106">Seade on **üks** järgmistest.</span><span class="sxs-lookup"><span data-stu-id="e703e-106">The device is **one** of these:</span></span>
    
    - <span data-ttu-id="e703e-107">Azure Active Directory (Azure AD) on ühendatud</span><span class="sxs-lookup"><span data-stu-id="e703e-107">Azure Active Directory (Azure AD) joined</span></span>
    - <span data-ttu-id="e703e-108">Hübriid-Azure AD-ga liidetud</span><span class="sxs-lookup"><span data-stu-id="e703e-108">Hybrid Azure AD joined</span></span>
    - <span data-ttu-id="e703e-109">AAD registreeritud</span><span class="sxs-lookup"><span data-stu-id="e703e-109">AAD registered</span></span>

- <span data-ttu-id="e703e-110">Poliitikatoimingute jõustamiseks veenduge, et Chromium Edge'i brauser on installitud lõpp-punkti seadmesse.</span><span class="sxs-lookup"><span data-stu-id="e703e-110">To enforce policy actions, make sure Microsoft Chromium Edge browser is installed on the endpoint device.</span></span>

<span data-ttu-id="e703e-111">Lisateavet Lõpp-punkti DLP juurutamise kohta leiate teemast [Lõpp-punkti andmete kaotsimineku vältimisega alustamine.](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)</span><span class="sxs-lookup"><span data-stu-id="e703e-111">For additional requirements for deploying Endpoint DLP, see [Get started with Endpoint data loss prevention](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).</span></span>