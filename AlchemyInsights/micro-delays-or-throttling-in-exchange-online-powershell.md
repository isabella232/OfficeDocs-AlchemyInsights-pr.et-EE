---
title: Mikro viivitused või ahendamine Exchange Online PowerShellis
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702122"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="9d4db-102">Mikro viivitused või ahendamine Exchange Online PowerShellis</span><span class="sxs-lookup"><span data-stu-id="9d4db-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="9d4db-103">Exchange Online’is skriptide ja cmdlet-käskude käitamisel võite näha hoiatusi „Mikro viivitus rakendatud“ või viivitusi.</span><span class="sxs-lookup"><span data-stu-id="9d4db-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="9d4db-104">Siin on mõned soovitused selle lahendamiseks.</span><span class="sxs-lookup"><span data-stu-id="9d4db-104">Here are a few suggestions how to solve this:</span></span>

- <span data-ttu-id="9d4db-105">Rentniku PowerShelli ahendamise poliitikate leevendamiseks käivitage meie diagnostika.</span><span class="sxs-lookup"><span data-stu-id="9d4db-105">Please run our diagnostics to relax your tenant's PowerShell throttling policies.</span></span> <span data-ttu-id="9d4db-106">See lahendus lahendab probleemi kõige rohkem.</span><span class="sxs-lookup"><span data-stu-id="9d4db-106">This solution will solve the problem for most.</span></span>
- <span data-ttu-id="9d4db-107">Kui probleem ei lahene, kasutage [Exchange Online v2 PowerShelli](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)moodulit, mis sisaldab REST API-l põhinevaid CMDlets'i ja on oluliselt rohkem esinejad.</span><span class="sxs-lookup"><span data-stu-id="9d4db-107">If issue still not solved, use the [Exchange Online v2 PowerShell module](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="9d4db-108">See võib olla suurepärane lahendus paljudele cmdleti hankimise käskude, mida sageli kasutatakse.</span><span class="sxs-lookup"><span data-stu-id="9d4db-108">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="9d4db-109">Kui teil on vaja kasutada CMDlets'i, mida v2 moodul ei hõlma, lugege teemat [PowerShelli](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)cmdlet-käskude käitamine suure hulga kasutajate jaoks Office 365-s, mis räägib powerShelli ahendamise piirangutest Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="9d4db-109">If you need to use CMDlets that are not covered in the v2 module, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around PowerShell throttling limits in Exchange Online.</span></span>
