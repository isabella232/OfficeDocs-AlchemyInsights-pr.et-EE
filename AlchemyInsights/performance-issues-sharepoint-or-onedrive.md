---
title: Jõudluse probleemid – SharePoint või OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771897"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="e4c41-102">SharePointi või OneDrive ' i aeglased, kättesaamatud või kättesaamatud mitme kasutaja jaoks</span><span class="sxs-lookup"><span data-stu-id="e4c41-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="e4c41-103">SharePointis või OneDrive ' is võivad olla aeglased, kättesaamatud või kättesaamatud või kuvada mitu põhjust teenust kättesaamatuks või 503 tõrkeks.</span><span class="sxs-lookup"><span data-stu-id="e4c41-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="e4c41-104">Kui teie SharePointi või OneDrive ' i sait on mitme kasutaja jaoks aeglane või hilinenud, võib esineda ajutine teenus, kus kasutajad saavad SharePointi saitidele või OneDrive ' i sisule juurdepääsul kasutada ajutisi viivitusi või navigeerimine.</span><span class="sxs-lookup"><span data-stu-id="e4c41-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="e4c41-105">Kontrollige [teenuse tervise armatuurlauda](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , et näha, kas teie ettevõte on mõjutatud.</span><span class="sxs-lookup"><span data-stu-id="e4c41-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="e4c41-106">Kui proovite liikuda SharePointi või OneDrive ' i saitidele, võivad kasutajad saada *503 serveriga hõivatud* tõrke.</span><span class="sxs-lookup"><span data-stu-id="e4c41-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="e4c41-107">Selle tõrke põhjuseks võib olla SharePointi teenuse ahendamine.</span><span class="sxs-lookup"><span data-stu-id="e4c41-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="e4c41-108">SharePoint Online kasutab SharePoint Online’i teenuste optimaalse jõudluse ja töökindluse säilitamiseks ahendamist.</span><span class="sxs-lookup"><span data-stu-id="e4c41-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="e4c41-109">Ahendamine piirab kasutajate toimingute või samaaegsete kõnede arvu (skripti või koodi poolt), et ennetada ressursside ülekasutamist.</span><span class="sxs-lookup"><span data-stu-id="e4c41-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="e4c41-110">Lisateavet ahendamise kohta leiate artiklist [SharePoint Online ' is ahendamise või blokeerimise vältimine](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="e4c41-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="e4c41-111">Kui teil ilmneb väike jõudlus **klassikalise** või **moodsa** SharePointi saidi või lehega, kasutage lehtede analüüsimiseks [lehte diagnostilist tööriista](https://aka.ms/perftool) .</span><span class="sxs-lookup"><span data-stu-id="e4c41-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="e4c41-112">Kui teil on endiselt üldine aegluse, vaadake selle artikli allosas olevaid ressursse: [SharePoint Online ' i jõudluse häälestamise tutvustus](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="e4c41-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  