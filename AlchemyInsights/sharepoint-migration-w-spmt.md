---
title: SharePointi migratsioon koos SPMT-ga
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "2594"
ms.openlocfilehash: e7719d1fc6dda0d5bd340775219401dade2933fe
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931546"
---
# <a name="sharepoint-migration-with-spmt"></a><span data-ttu-id="adb63-102">SharePointi migratsioon koos SPMT-ga</span><span class="sxs-lookup"><span data-stu-id="adb63-102">SharePoint Migration with SPMT</span></span>

<span data-ttu-id="adb63-103">**Oluline**: paljud SharePoint Online ' i ja OneDrive kliendid käivitada Business kriitilised rakendused teenuse, mis töötavad taustal.</span><span class="sxs-lookup"><span data-stu-id="adb63-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="adb63-104">Nende hulka kuuluvad sisu migratsioon, andmete kadu vältimine (DLP) ja backup lahendused.</span><span class="sxs-lookup"><span data-stu-id="adb63-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="adb63-105">Nendel enneolematul ajal me võtame meetmeid, et tagada SharePoint Online ' i ja OneDrive teenused on väga kättesaadav ja usaldusväärne oma kasutajatele, kes sõltuvad teenuse rohkem kui kunagi varem kaugtöö stsenaariume.</span><span class="sxs-lookup"><span data-stu-id="adb63-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="adb63-106">Selle eesmärgi toetuseks oleme rakendanud ranget ahendamise piiranguid taustal olevatele rakendustele (migratsioon, DLP ja backup lahendused) tööpäeval päeva jooksul.</span><span class="sxs-lookup"><span data-stu-id="adb63-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="adb63-107">Te peaksite ootama, et need rakendused saavutavad nende aegade jooksul väga piiratud läbilaskevõime.</span><span class="sxs-lookup"><span data-stu-id="adb63-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="adb63-108">Aga, õhtuti ja nädalavahetusel tundi piirkonna, teenus on valmis töötlema oluliselt suurem hulk taotlusi taustal apps.</span><span class="sxs-lookup"><span data-stu-id="adb63-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="adb63-109">**SharePointi migreerimise tööriist**</span><span class="sxs-lookup"><span data-stu-id="adb63-109">**SharePoint Migration Tool**</span></span>

<span data-ttu-id="adb63-110">Mõeldud kasutamiseks migreerimist alates väikseim kogum faile suuremahuline ettevõtte migratsioon, SharePoint Migration Tool võimaldab teil edastada oma andmeid pilve ja ära uusim koostöö, intelligentsus, ja turvalisuse lahendusi Office 365.</span><span class="sxs-lookup"><span data-stu-id="adb63-110">Designed to be used for migrations ranging from the smallest set of files to a large scale enterprise migration, the SharePoint Migration Tool will allow you to transfer your information to the cloud and take advantage of the newest collaboration, intelligence, and security solutions with Office 365.</span></span>

- [<span data-ttu-id="adb63-111">Laadige alla ja installige SharePointi migreerimise tööriist</span><span class="sxs-lookup"><span data-stu-id="adb63-111">Download and install the SharePoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)
- [<span data-ttu-id="adb63-112">Levinud SPMT probleemide ja tõrgete tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="adb63-112">Troubleshooting common SPMT issues and errors</span></span>](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
- [<span data-ttu-id="adb63-113">SPMT installimise probleemide tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="adb63-113">Troubleshooting SPMT installation issues</span></span>](https://docs.microsoft.com/sharepointmigration/spmt-install-issues#troubleshooting-spmt-installation-issues)
