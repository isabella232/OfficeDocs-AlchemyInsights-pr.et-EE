---
title: Jõudlusprobleemid-SharePoint või OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068394"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="84eb6-102">SharePointi või OneDrive ' i aeglane, juurdepääsetav või mitmele kasutajale kättesaamatu</span><span class="sxs-lookup"><span data-stu-id="84eb6-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="84eb6-103">SharePoint või OneDrive võib olla aeglane, kättesaamatu või pole saadaval või võib kuvada teenuse kättesaamatuks või 503 tõrked mitmel põhjusel:</span><span class="sxs-lookup"><span data-stu-id="84eb6-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="84eb6-104">Kui teie SharePointi või OneDrive ' i sait on aeglane või viibib mitu kasutajat, võib olla ajutine teenuse probleem, kus kasutajad kogevad vahelduva viivitusi või navigeerimine tõrked SharePointi saitide või OneDrive ' i sisu kasutamisel.</span><span class="sxs-lookup"><span data-stu-id="84eb6-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="84eb6-105">Kontrollige [teenuse tervise armatuurlauda](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , et näha, kas teie organisatsioon on mõjutatud.</span><span class="sxs-lookup"><span data-stu-id="84eb6-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="84eb6-106">Kasutajad võivad saada *503 server on hõivatud* tõrge katsel navigeerida SharePointi või OneDrive saidid.</span><span class="sxs-lookup"><span data-stu-id="84eb6-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="84eb6-107">See tõrge võib põhjustada ahendamine jooksul SharePointi teenus.</span><span class="sxs-lookup"><span data-stu-id="84eb6-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="84eb6-108">SharePoint Online ' i kasutab ahendamine optimaalse jõudluse ja töökindluse SharePoint Online Service.</span><span class="sxs-lookup"><span data-stu-id="84eb6-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="84eb6-109">Ahendamine piirab kasutajate toimingute või samaaegsete kõnede (skripti või koodi) arvu, et vältida ressursside ülekasutamist.</span><span class="sxs-lookup"><span data-stu-id="84eb6-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="84eb6-110">Ahendamise kohta lisateabe saamiseks [Vältige saada ahendatud või blokeeritud SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="84eb6-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="84eb6-111">Kui teil on aeglane **klassikaline** või **kaasaegne** SharePointi saidi või lehe, kasutada [lehe diagnostika tööriista](https://aka.ms/perftool) lehtede analüüsimiseks.</span><span class="sxs-lookup"><span data-stu-id="84eb6-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="84eb6-112">Kui teil on endiselt üldine aeglane jõudlus, vaadake selle artikli allosas ressursid: [Sissejuhatus jõudluse häälestamine SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="84eb6-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  