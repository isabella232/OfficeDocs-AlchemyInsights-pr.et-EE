---
title: SharePoint Online ' i suvandite migreerimine
ms.author: pebaum
author: v-miegge
manager: v-cojank
ms.date: 11/04/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: c8c339c9-2e50-4daa-aa91-3eb5053e2bc6
ms.openlocfilehash: 830b39c51658cbc02f4be81acdfdf3b164a8df70
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932726"
---
# <a name="migrate-options-to-sharepoint-online"></a><span data-ttu-id="82118-102">SharePoint Online ' i suvandite migreerimine</span><span class="sxs-lookup"><span data-stu-id="82118-102">Migrate options to SharePoint Online</span></span>

<span data-ttu-id="82118-103">**Oluline**: paljud SharePoint Online ' i ja OneDrive kliendid käivitada Business kriitilised rakendused teenuse, mis töötavad taustal.</span><span class="sxs-lookup"><span data-stu-id="82118-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="82118-104">Nende hulka kuuluvad sisu migratsioon, andmete kadu vältimine (DLP) ja backup lahendused.</span><span class="sxs-lookup"><span data-stu-id="82118-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="82118-105">Nendel enneolematul ajal me võtame meetmeid, et tagada SharePoint Online ' i ja OneDrive teenused on väga kättesaadav ja usaldusväärne oma kasutajatele, kes sõltuvad teenuse rohkem kui kunagi varem kaugtöö stsenaariume.</span><span class="sxs-lookup"><span data-stu-id="82118-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="82118-106">Selle eesmärgi toetuseks oleme rakendanud ranget ahendamise piiranguid taustal olevatele rakendustele (migratsioon, DLP ja backup lahendused) tööpäeval päeva jooksul.</span><span class="sxs-lookup"><span data-stu-id="82118-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="82118-107">Te peaksite ootama, et need rakendused saavutavad nende aegade jooksul väga piiratud läbilaskevõime.</span><span class="sxs-lookup"><span data-stu-id="82118-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="82118-108">Aga, õhtuti ja nädalavahetusel tundi piirkonna, teenus on valmis töötlema oluliselt suurem hulk taotlusi taustal apps.</span><span class="sxs-lookup"><span data-stu-id="82118-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="82118-109">**Rände Valikud**</span><span class="sxs-lookup"><span data-stu-id="82118-109">**Migration options**</span></span>

<span data-ttu-id="82118-110">SharePoint Online ' i sisu migreerimiseks on saadaval erinevad suvandid, olenevalt teie teisaldamiseks vajavate failide suurusest ja kogusest, palun vaadake [siin asuvate](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online)suvandite loendit.</span><span class="sxs-lookup"><span data-stu-id="82118-110">There are different options available to migrate content to SharePoint Online, depending on the size and quantity of files you need to move, please see a list of options [located here](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span></span>

<span data-ttu-id="82118-111">Lisateavet sisu migreerimise kohta leiate alltoodud linkidest.</span><span class="sxs-lookup"><span data-stu-id="82118-111">For more information on content migration, please visit the links below.</span></span>

- [<span data-ttu-id="82118-112">SharePointi migreerimise tööriist</span><span class="sxs-lookup"><span data-stu-id="82118-112">Sharepoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)

- [<span data-ttu-id="82118-113">Migreerimise halduri alustamine</span><span class="sxs-lookup"><span data-stu-id="82118-113">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="82118-114">SharePoint Online ' i ja ODB migratsiooni kiirus</span><span class="sxs-lookup"><span data-stu-id="82118-114">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="82118-115">Vältige ahendamist või blokeeritud SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="82118-115">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="82118-116">SharePointi siirdamise hindamise tööriist (SMAT)</span><span class="sxs-lookup"><span data-stu-id="82118-116">SharePoint Migration Assessment Tool (SMAT)</span></span>](https://www.microsoft.com/download/details.aspx?id=53598&amp;751be11f-ede8-5a0c-058c-2ee190a24fa6=True)

<span data-ttu-id="82118-117">**Märkus**: praegu SharePointi migreerimise tööriist toetab ainult migreerimist SharePoint 2010 ja 2013.</span><span class="sxs-lookup"><span data-stu-id="82118-117">**Note**: Currently the SharePoint Migration tool only support migrations from SharePoint 2010  and 2013.</span></span> <span data-ttu-id="82118-118">Versioon 2016 või 2019 ei toetata sel ajal.</span><span class="sxs-lookup"><span data-stu-id="82118-118">Version 2016 or 2019 are not supported at this time.</span></span>
