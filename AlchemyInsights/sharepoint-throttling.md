---
title: SharePoint Online ' i ahendamine
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 9af4f09d50992c04a1f3d5a164093049a3ec3517
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931438"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="42ad6-102">SharePoint Online ' i ahendamine</span><span class="sxs-lookup"><span data-stu-id="42ad6-102">SharePoint Online throttling</span></span>

<span data-ttu-id="42ad6-103">**Oluline**: paljud SharePoint Online ' i ja OneDrive kliendid käivitada Business kriitilised rakendused teenuse, mis töötavad taustal.</span><span class="sxs-lookup"><span data-stu-id="42ad6-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="42ad6-104">Nende hulka kuuluvad sisu migratsioon, andmete kadu vältimine (DLP) ja backup lahendused.</span><span class="sxs-lookup"><span data-stu-id="42ad6-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="42ad6-105">Nendel enneolematul ajal me võtame meetmeid, et tagada SharePoint Online ' i ja OneDrive teenused on väga kättesaadav ja usaldusväärne oma kasutajatele, kes sõltuvad teenuse rohkem kui kunagi varem kaugtöö stsenaariume.</span><span class="sxs-lookup"><span data-stu-id="42ad6-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="42ad6-106">Selle eesmärgi toetuseks oleme rakendanud ranget ahendamise piiranguid taustal olevatele rakendustele (migratsioon, DLP ja backup lahendused) tööpäeval päeva jooksul.</span><span class="sxs-lookup"><span data-stu-id="42ad6-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="42ad6-107">Te peaksite ootama, et need rakendused saavutavad nende aegade jooksul väga piiratud läbilaskevõime.</span><span class="sxs-lookup"><span data-stu-id="42ad6-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="42ad6-108">Aga, õhtuti ja nädalavahetusel tundi piirkonna, teenus on valmis töötlema oluliselt suurem hulk taotlusi taustal apps.</span><span class="sxs-lookup"><span data-stu-id="42ad6-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="42ad6-109">**SharePoint Online ' i ahendamine**</span><span class="sxs-lookup"><span data-stu-id="42ad6-109">**SharePoint Online throttling**</span></span>

<span data-ttu-id="42ad6-110">SharePoint Online ' i kasutab ahendamine optimaalse jõudluse ja töökindluse SharePoint Online Service.</span><span class="sxs-lookup"><span data-stu-id="42ad6-110">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="42ad6-111">Ahendamine piirab kasutajate toimingute või samaaegsete kõnede (skripti või koodi) arvu, et vältida ressursside ülekasutamist.</span><span class="sxs-lookup"><span data-stu-id="42ad6-111">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="42ad6-112">Lisateabe saamiseks külastage allolevaid linke.</span><span class="sxs-lookup"><span data-stu-id="42ad6-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="42ad6-113">Vältige ahendamist või blokeeritud SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="42ad6-113">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="42ad6-114">Andmete migratsioon ja SPO ahendamine</span><span class="sxs-lookup"><span data-stu-id="42ad6-114">Data Migration and SPO Throttling </span></span>](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)

- [<span data-ttu-id="42ad6-115">SharePoint Online ja OneDrive ' i migreerimise kiirus</span><span class="sxs-lookup"><span data-stu-id="42ad6-115">SharePoint Online and OneDrive Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

 - [<span data-ttu-id="42ad6-116">SharePoint Online ' i ahendamise käsitsemiseks, kasutades eksponentsiaalselt tagasi välja</span><span class="sxs-lookup"><span data-stu-id="42ad6-116">Handle SharePoint Online throttling by using exponential back off</span></span>](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)

- [<span data-ttu-id="42ad6-117">Võimsuse planeerimine ja koormuse testimine SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="42ad6-117">Capacity planning and load testing SharePoint Online</span></span>](https://docs.microsoft.com/office365/enterprise/capacity-planning-and-load-testing-sharepoint-online)

