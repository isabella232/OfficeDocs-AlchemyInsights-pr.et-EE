---
title: SharePointi migreerimisjõudlus
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "2700"
ms.openlocfilehash: 812444589d5a5bf766bbc6f466077d4ca829d79f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932000"
---
# <a name="sharepoint-migration-performance"></a><span data-ttu-id="fa5ab-102">SharePointi migreerimisjõudlus</span><span class="sxs-lookup"><span data-stu-id="fa5ab-102">SharePoint migration performance</span></span>

<span data-ttu-id="fa5ab-103">**Tähtis.** Paljud SharePoint Online’i ja OneDrive’i kliendid käitavad äriks olulisi rakendusi teenuses, mis töötab taustal.</span><span class="sxs-lookup"><span data-stu-id="fa5ab-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="fa5ab-104">Nende hulka kuuluvad sisu migreerimine, andmelekketõkestus (DLP) ja varunduslahendused.</span><span class="sxs-lookup"><span data-stu-id="fa5ab-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="fa5ab-105">Praegusel ootamatul ajal teeme kõik selleks, et SharePoint Online’i ja OneDrive’i teenused jääksid püsivalt kättesaadavaks ja töökindlaks kasutajate jaoks, kes sõltuvad kaugtööd tehes teenusest rohkem kui kunagi varem.</span><span class="sxs-lookup"><span data-stu-id="fa5ab-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="fa5ab-106">Selle eesmärgi toetamiseks oleme taustrakenduste (migreerimine, DLP ja varunduslahendused) jaoks tööpäevadel päevasel ajal kehtestanud rangemad ahendamispiirangud.</span><span class="sxs-lookup"><span data-stu-id="fa5ab-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="fa5ab-107">Eeldatavasti on neil rakendustel nendel aegadel väga piiratud läbilaskevõime.</span><span class="sxs-lookup"><span data-stu-id="fa5ab-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="fa5ab-108">Aga piirkonna õhtustel aegadel ja nädalavahetustel on teenus valmis töötlema palju suuremat hulka taustrakendustest pärit taotlusi.</span><span class="sxs-lookup"><span data-stu-id="fa5ab-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="fa5ab-109">**Migreerimise jõudlus**</span><span class="sxs-lookup"><span data-stu-id="fa5ab-109">**Migration performance**</span></span>

<span data-ttu-id="fa5ab-110">Migreerimise jõudlust võivad mõjutada võrgutaristu, failimaht, migreerimiskellaaeg ja ahendamine.</span><span class="sxs-lookup"><span data-stu-id="fa5ab-110">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling.</span></span> <span data-ttu-id="fa5ab-111">Kõigi nende tegurite mõistmine aitab teil plaanida oma migreerimisprotsessi ja tagada suurim tõhusus.</span><span class="sxs-lookup"><span data-stu-id="fa5ab-111">Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

<span data-ttu-id="fa5ab-112">Lisateabe saamiseks klõpsake allolevaid linke.</span><span class="sxs-lookup"><span data-stu-id="fa5ab-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="fa5ab-113">Sharepoint Online’i ja ODB migreerimise kiirus</span><span class="sxs-lookup"><span data-stu-id="fa5ab-113">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="fa5ab-114">Ahendamise või blokeerimise vältimine SharePoint Online’is</span><span class="sxs-lookup"><span data-stu-id="fa5ab-114">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="fa5ab-115">SharePointi migreerimistööriista allalaadimine ja installimine</span><span class="sxs-lookup"><span data-stu-id="fa5ab-115">Download and install the SharePoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)
