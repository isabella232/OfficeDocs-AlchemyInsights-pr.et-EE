---
title: Probleemid SharePoint Online ' i andmete migreerimine
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "1885"
ms.openlocfilehash: b53a98480bab48497274c7358f7e606caa477f5a
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931690"
---
# <a name="issues-while-migrating-data-to-sharepoint-online"></a><span data-ttu-id="65b22-102">Probleemid SharePoint Online ' i andmete migreerimine</span><span class="sxs-lookup"><span data-stu-id="65b22-102">Issues while migrating data to SharePoint Online</span></span>

<span data-ttu-id="65b22-103">**Oluline**: paljud SharePoint Online ' i ja OneDrive kliendid käivitada Business kriitilised rakendused teenuse, mis töötavad taustal.</span><span class="sxs-lookup"><span data-stu-id="65b22-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="65b22-104">Nende hulka kuuluvad sisu migratsioon, andmete kadu vältimine (DLP) ja backup lahendused.</span><span class="sxs-lookup"><span data-stu-id="65b22-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="65b22-105">Nendel enneolematul ajal me võtame meetmeid, et tagada SharePoint Online ' i ja OneDrive teenused on väga kättesaadav ja usaldusväärne oma kasutajatele, kes sõltuvad teenuse rohkem kui kunagi varem kaugtöö stsenaariume.</span><span class="sxs-lookup"><span data-stu-id="65b22-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="65b22-106">Selle eesmärgi toetuseks oleme rakendanud ranget ahendamise piiranguid taustal olevatele rakendustele (migratsioon, DLP ja backup lahendused) tööpäeval päeva jooksul.</span><span class="sxs-lookup"><span data-stu-id="65b22-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="65b22-107">Te peaksite ootama, et need rakendused saavutavad nende aegade jooksul väga piiratud läbilaskevõime.</span><span class="sxs-lookup"><span data-stu-id="65b22-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="65b22-108">Aga, õhtuti ja nädalavahetusel tundi piirkonna, teenus on valmis töötlema oluliselt suurem hulk taotlusi taustal apps.</span><span class="sxs-lookup"><span data-stu-id="65b22-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="65b22-109">**Üle 100TB andmete migreerimine**</span><span class="sxs-lookup"><span data-stu-id="65b22-109">**Migrating over 100TB of data**</span></span>

<span data-ttu-id="65b22-110">Tundub, et olete migreerimine üle 100TB andmeid SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="65b22-110">It appears you are migrating over 100TB of data to SharePoint Online.</span></span> <span data-ttu-id="65b22-111">Palun järgige alltoodud samme, et saaksime teid aidata nii ruttu kui võimalik.</span><span class="sxs-lookup"><span data-stu-id="65b22-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="65b22-112">Valige **Uus teenuspäring**ja seejärel **Uus teenuspäring**.</span><span class="sxs-lookup"><span data-stu-id="65b22-112">Select **New Service Request**, and then **New Service Request**.</span></span> 
2. <span data-ttu-id="65b22-113">Jätke tiitel ja kirjeldus **SharePointi migreerimise üle 100TB**.</span><span class="sxs-lookup"><span data-stu-id="65b22-113">Leave the title and description as **SharePoint migration over 100TB**.</span></span>
3. <span data-ttu-id="65b22-114">Kui pilet on esitatud, värskendage seda järgmise teabega:</span><span class="sxs-lookup"><span data-stu-id="65b22-114">Once the ticket has been submitted, please update it with the following information:</span></span> 

    - <span data-ttu-id="65b22-115">Teie migratsiooni hinnanguline suurus.</span><span class="sxs-lookup"><span data-stu-id="65b22-115">Estimated size of your migration.</span></span>
    - <span data-ttu-id="65b22-116">Hinnang, millal soovite oma migreerimise käivitada ja lõpule viia.</span><span class="sxs-lookup"><span data-stu-id="65b22-116">An estimate of when you would like to start and complete your migration.</span></span>
    - <span data-ttu-id="65b22-117">Kirjeldage, kus olete oma sisu migreerimine (nt SharePoint Server, kast, GDrive, failide osad jne).</span><span class="sxs-lookup"><span data-stu-id="65b22-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>


  

