---
title: Sisu otsing tulemeid
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680643"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="891c6-102">Sisu otsingu/ekspordi tulemeid ei kuvata</span><span class="sxs-lookup"><span data-stu-id="891c6-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="891c6-103">Sisu otsimisega/ekspordiga seotud probleemid võivad olla tingitud teatud nõuetele vastavuse turbe filtrist, mis on häälestatud teatud administraatori poolt ja mitte edastama seda kõigile administraatoritele.</span><span class="sxs-lookup"><span data-stu-id="891c6-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="891c6-104">Selle probleemi lahendamiseks kontrollige, kas selle põhjuseks võib olla mõni nõuetele vastav turvamise filtrid.</span><span class="sxs-lookup"><span data-stu-id="891c6-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="891c6-105">Ühenduse loomine turbe ja ühilduvuse keskusega PowerShell</span><span class="sxs-lookup"><span data-stu-id="891c6-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="891c6-106">Käivitage järgmine Commandlets.</span><span class="sxs-lookup"><span data-stu-id="891c6-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="891c6-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="891c6-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="891c6-108">Get-ComplianceSecurityFilter-organisatsioon $org</span><span class="sxs-lookup"><span data-stu-id="891c6-108">Get-ComplianceSecurityFilter -Organization $org</span></span>