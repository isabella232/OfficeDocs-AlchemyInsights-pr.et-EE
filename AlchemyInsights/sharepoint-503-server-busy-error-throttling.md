---
title: SharePoint Online ' i ahendamine
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931222"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="612fc-102">SharePoint Online ' i ahendamine</span><span class="sxs-lookup"><span data-stu-id="612fc-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="612fc-103">**Oluline**: paljud SharePoint Online ' i ja OneDrive kliendid käivitada Business kriitilised rakendused teenuse, mis töötavad taustal.</span><span class="sxs-lookup"><span data-stu-id="612fc-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="612fc-104">Nende hulka kuuluvad sisu migratsioon, andmete kadu vältimine (DLP) ja backup lahendused.</span><span class="sxs-lookup"><span data-stu-id="612fc-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="612fc-105">Nendel enneolematul ajal me võtame meetmeid, et tagada SharePoint Online ' i ja OneDrive teenused on väga kättesaadav ja usaldusväärne oma kasutajatele, kes sõltuvad teenuse rohkem kui kunagi varem kaugtöö stsenaariume.</span><span class="sxs-lookup"><span data-stu-id="612fc-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="612fc-106">Selle eesmärgi toetuseks oleme rakendanud ranget ahendamise piiranguid taustal olevatele rakendustele (migratsioon, DLP ja backup lahendused) tööpäeval päeva jooksul.</span><span class="sxs-lookup"><span data-stu-id="612fc-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="612fc-107">Te peaksite ootama, et need rakendused saavutavad nende aegade jooksul väga piiratud läbilaskevõime.</span><span class="sxs-lookup"><span data-stu-id="612fc-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="612fc-108">Aga, õhtuti ja nädalavahetusel tundi piirkonna, teenus on valmis töötlema oluliselt suurem hulk taotlusi taustal apps.</span><span class="sxs-lookup"><span data-stu-id="612fc-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="612fc-109">**503 server on hõivatud tõrge**</span><span class="sxs-lookup"><span data-stu-id="612fc-109">**503 server is busy error**</span></span>

<span data-ttu-id="612fc-110">Kasutajad võivad saada 503 server on hõivatud tõrge katsel navigeerida SharePointi või OneDrive saidid.</span><span class="sxs-lookup"><span data-stu-id="612fc-110">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="612fc-111">See tõrge võib põhjustada ahendamine jooksul SharePointi teenus.</span><span class="sxs-lookup"><span data-stu-id="612fc-111">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="612fc-112">SharePoint Online ' i kasutab ahendamine optimaalse jõudluse ja töökindluse SharePoint Online Service.</span><span class="sxs-lookup"><span data-stu-id="612fc-112">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="612fc-113">Ahendamine piirab kasutajate toimingute või samaaegsete kõnede (skripti või koodi) arvu, et vältida ressursside ülekasutamist.</span><span class="sxs-lookup"><span data-stu-id="612fc-113">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="612fc-114">Ahendamise kohta lisateabe saamiseks [Vältige saada ahendatud või blokeeritud SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="612fc-114">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="612fc-115">Kui arvate, et see tõrge ei ole seotud ahendamine, saate kontrollida, kas on aktiivne hooldus esineb teie rentniku navigeerides [sõnumikeskus](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="612fc-115">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="612fc-116">Lõpuks, veenduge, et külastate [teenuse tervis](https://portal.office.com/adminportal/home#/servicehealth) lehte, et kontrollida mis tahes teateid/intsidente, mis võivad tekkida.</span><span class="sxs-lookup"><span data-stu-id="612fc-116">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

