---
title: SharePointi siirdamise tööriista probleemide ja tõrgete tõrkeotsing
ms.author: v-miegge
author: v-miegge
manager: v-cojank
ms.date: 10/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3178"
ms.assetid: ''
ms.openlocfilehash: f9f5694b1d88bccebdc5448d5629ea5120c52511
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931114"
---
# <a name="troubleshooting-sharepoint-migration-tool-issues-and-errors"></a><span data-ttu-id="2ae1c-102">SharePointi siirdamise tööriista probleemide ja tõrgete tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="2ae1c-102">Troubleshooting SharePoint Migration Tool issues and errors</span></span>

<span data-ttu-id="2ae1c-103">**Oluline**: paljud SharePoint Online ' i ja OneDrive kliendid käivitada Business kriitilised rakendused teenuse, mis töötavad taustal.</span><span class="sxs-lookup"><span data-stu-id="2ae1c-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="2ae1c-104">Nende hulka kuuluvad sisu migratsioon, andmete kadu vältimine (DLP) ja backup lahendused.</span><span class="sxs-lookup"><span data-stu-id="2ae1c-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="2ae1c-105">Nendel enneolematul ajal me võtame meetmeid, et tagada SharePoint Online ' i ja OneDrive teenused on väga kättesaadav ja usaldusväärne oma kasutajatele, kes sõltuvad teenuse rohkem kui kunagi varem kaugtöö stsenaariume.</span><span class="sxs-lookup"><span data-stu-id="2ae1c-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="2ae1c-106">Selle eesmärgi toetuseks oleme rakendanud ranget ahendamise piiranguid taustal olevatele rakendustele (migratsioon, DLP ja backup lahendused) tööpäeval päeva jooksul.</span><span class="sxs-lookup"><span data-stu-id="2ae1c-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="2ae1c-107">Te peaksite ootama, et need rakendused saavutavad nende aegade jooksul väga piiratud läbilaskevõime.</span><span class="sxs-lookup"><span data-stu-id="2ae1c-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="2ae1c-108">Aga, õhtuti ja nädalavahetusel tundi piirkonna, teenus on valmis töötlema oluliselt suurem hulk taotlusi taustal apps.</span><span class="sxs-lookup"><span data-stu-id="2ae1c-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="2ae1c-109">**Levinud probleemid ja tõrked**</span><span class="sxs-lookup"><span data-stu-id="2ae1c-109">**Common issues and errors**</span></span>

<span data-ttu-id="2ae1c-110">SharePoint Migration Tool (SPMT) kasutamisel võib ilmneda mõned levinud probleemid ja tõrked.</span><span class="sxs-lookup"><span data-stu-id="2ae1c-110">You may encounter some common issues and errors when using the SharePoint Migration Tool (SPMT).</span></span> <span data-ttu-id="2ae1c-111">Lisateabe saamiseks lugege allolevaid linke.</span><span class="sxs-lookup"><span data-stu-id="2ae1c-111">Please reference the links below for more information.</span></span>

* [<span data-ttu-id="2ae1c-112">Levinud SPMT probleemide ja tõrgete tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="2ae1c-112">Troubleshooting common SPMT issues and errors</span></span>](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
* [<span data-ttu-id="2ae1c-113">SPMT installimise probleemide tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="2ae1c-113">Troubleshooting SPMT install issues</span></span>](https://docs.microsoft.com/sharepointmigration/spmt-install-issues)