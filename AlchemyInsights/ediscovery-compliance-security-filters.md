---
title: Sisu otsingu/ekspordi ajal tulemeid ei tagastata
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
- "3200003"
- "7463"
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/14/2020
ms.locfileid: "49677683"
---
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="209bd-102">Sisu otsingu/ekspordi ajal tulemeid ei tagastata</span><span class="sxs-lookup"><span data-stu-id="209bd-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="209bd-103">Kui teil esineb järgmisi e-juurdluse stsenaariumeid, tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="209bd-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="209bd-104">Sisu otsimine/eksportimine ei tagasta andmeid ega ootamatuid andmeid</span><span class="sxs-lookup"><span data-stu-id="209bd-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="209bd-105">e-juurdluse otsing või eksport nurjub</span><span class="sxs-lookup"><span data-stu-id="209bd-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="209bd-106">See võib olla tingitud teatud nõuetele vastavuse turbe filtritest, mis olid häälestatud teatud administraatori poolt ja mida pole kõigile administraatoritele edastatud.</span><span class="sxs-lookup"><span data-stu-id="209bd-106">This may be caused due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="209bd-107">Selle probleemi lahendamiseks kontrollige, kas on olemas nõuetele vastavuse turbe filtrid, mis võivad põhjustada järgmisi probleeme.</span><span class="sxs-lookup"><span data-stu-id="209bd-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="209bd-108">Ühenduse loomine turbe ja ühilduvuse keskusega PowerShell</span><span class="sxs-lookup"><span data-stu-id="209bd-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="209bd-109">Käivitage järgmine Commandlets.</span><span class="sxs-lookup"><span data-stu-id="209bd-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="209bd-110">Lisateavet ühilduvuse turbe filtrite kohta leiate teemast [sisu otsimise õiguse filtreerimine](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span><span class="sxs-lookup"><span data-stu-id="209bd-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>
