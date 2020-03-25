---
title: SharePointi migreerimise ahendamine 503 tõrked
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931654"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a><span data-ttu-id="6635b-102">SharePointi migreerimise ahendamine 503 tõrked</span><span class="sxs-lookup"><span data-stu-id="6635b-102">SharePoint migration throttling with 503 errors</span></span>

<span data-ttu-id="6635b-103">**Oluline**: paljud SharePoint Online ' i ja OneDrive kliendid käivitada Business kriitilised rakendused teenuse, mis töötavad taustal.</span><span class="sxs-lookup"><span data-stu-id="6635b-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="6635b-104">Nende hulka kuuluvad sisu migratsioon, andmete kadu vältimine (DLP) ja backup lahendused.</span><span class="sxs-lookup"><span data-stu-id="6635b-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="6635b-105">Nendel enneolematul ajal me võtame meetmeid, et tagada SharePoint Online ' i ja OneDrive teenused on väga kättesaadav ja usaldusväärne oma kasutajatele, kes sõltuvad teenuse rohkem kui kunagi varem kaugtöö stsenaariume.</span><span class="sxs-lookup"><span data-stu-id="6635b-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="6635b-106">Selle eesmärgi toetuseks oleme rakendanud ranget ahendamise piiranguid taustal olevatele rakendustele (migratsioon, DLP ja backup lahendused) tööpäeval päeva jooksul.</span><span class="sxs-lookup"><span data-stu-id="6635b-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="6635b-107">Te peaksite ootama, et need rakendused saavutavad nende aegade jooksul väga piiratud läbilaskevõime.</span><span class="sxs-lookup"><span data-stu-id="6635b-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="6635b-108">Aga, õhtuti ja nädalavahetusel tundi piirkonna, teenus on valmis töötlema oluliselt suurem hulk taotlusi taustal apps.</span><span class="sxs-lookup"><span data-stu-id="6635b-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="6635b-109">**503 tõrked, kui migreerimine SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="6635b-109">**503 errors when migrating to SharePoint Online**</span></span>

<span data-ttu-id="6635b-110">Tundub, et migreerite SharePoint Online ' i ja saate 503 tõrked.</span><span class="sxs-lookup"><span data-stu-id="6635b-110">It appears you are migrating to SharePoint Online and receiving 503 errors.</span></span> <span data-ttu-id="6635b-111">Palun järgige alltoodud samme, et saaksime teid aidata nii ruttu kui võimalik.</span><span class="sxs-lookup"><span data-stu-id="6635b-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="6635b-112">Klõpsake nuppu **Kontakt tugiteenja**seejärel **uue teenuse taotlus**.</span><span class="sxs-lookup"><span data-stu-id="6635b-112">Click **Contact Support**, and then **New Service Request**.</span></span>
2. <span data-ttu-id="6635b-113">Pealkirja ja kirjeldus, tippige **SharePointi migreerimise ahendamine koos 503**.</span><span class="sxs-lookup"><span data-stu-id="6635b-113">For the title and description, type **SharePoint Migration Throttling with 503**.</span></span>
3. <span data-ttu-id="6635b-114">Kui pilet on esitatud, värskendage seda järgmise teabega:</span><span class="sxs-lookup"><span data-stu-id="6635b-114">Once the ticket has been submitted, please update it with the following information:</span></span>
    - <span data-ttu-id="6635b-115">Kui palju jäänud migratsioon (näiteks kui palju TBs?).</span><span class="sxs-lookup"><span data-stu-id="6635b-115">How much left of migration (for example, how many TBs?).</span></span>
    - <span data-ttu-id="6635b-116">Migratsiooni algus-ja lõppkuupäev.</span><span class="sxs-lookup"><span data-stu-id="6635b-116">Migration start and end date.</span></span>
    - <span data-ttu-id="6635b-117">Kirjeldage, kus olete oma sisu migreerimine (nt SharePoint Server, kast, GDrive, failide osad jne).</span><span class="sxs-lookup"><span data-stu-id="6635b-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>
    - <span data-ttu-id="6635b-118">Kas hinnata ahendamisvigade arvu (nt x-Throttle tunnis?) ja millal see ahendamine juhtus.</span><span class="sxs-lookup"><span data-stu-id="6635b-118">Estimate the number of throttling errors (for example, x throttle per hour?) and when did the throttling happen.</span></span>
    - <span data-ttu-id="6635b-119">Millist siirdustööriista kasutate (nt SPMT või ShareGate).</span><span class="sxs-lookup"><span data-stu-id="6635b-119">Which migration tool you are using (for example, SPMT or ShareGate).</span></span>


