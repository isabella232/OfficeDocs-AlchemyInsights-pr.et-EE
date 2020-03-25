---
title: Rohkem infot DLP probleemid
ms.author: pebaum
author: pebaum
manager: laurawi
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2447"
- "3200001"
ms.openlocfilehash: 6525cee0555f1ae67b7d4e32445b9a1537d4a804
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932690"
---
# <a name="information-about-dlp-issues"></a><span data-ttu-id="7c08d-102">Teave DLP probleemid</span><span class="sxs-lookup"><span data-stu-id="7c08d-102">Information about DLP issues</span></span>

<span data-ttu-id="7c08d-103">**Oluline**: paljud SharePoint Online ' i ja OneDrive kliendid käivitada Business kriitilised rakendused teenuse, mis töötavad taustal.</span><span class="sxs-lookup"><span data-stu-id="7c08d-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="7c08d-104">Nende hulka kuuluvad sisu migratsioon, andmete kadu vältimine (DLP) ja backup lahendused.</span><span class="sxs-lookup"><span data-stu-id="7c08d-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="7c08d-105">Nendel enneolematul ajal me võtame meetmeid, et tagada SharePoint Online ' i ja OneDrive teenused on väga kättesaadav ja usaldusväärne oma kasutajatele, kes sõltuvad teenuse rohkem kui kunagi varem kaugtöö stsenaariume.</span><span class="sxs-lookup"><span data-stu-id="7c08d-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="7c08d-106">Selle eesmärgi toetuseks oleme rakendanud ranget ahendamise piiranguid taustal olevatele rakendustele (migratsioon, DLP ja backup lahendused) tööpäeval päeva jooksul.</span><span class="sxs-lookup"><span data-stu-id="7c08d-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="7c08d-107">Te peaksite ootama, et need rakendused saavutavad nende aegade jooksul väga piiratud läbilaskevõime.</span><span class="sxs-lookup"><span data-stu-id="7c08d-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="7c08d-108">Aga, õhtuti ja nädalavahetusel tundi piirkonna, teenus on valmis töötlema oluliselt suurem hulk taotlusi taustal apps.</span><span class="sxs-lookup"><span data-stu-id="7c08d-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="7c08d-109">**Teave DLP poliitika kohta**</span><span class="sxs-lookup"><span data-stu-id="7c08d-109">**Information on DLP policy**</span></span>

<span data-ttu-id="7c08d-110">DLP poliitika, saate tuvastada, jälgida ja automaatselt kaitsta tundlikku teavet kogu Office 365.</span><span class="sxs-lookup"><span data-stu-id="7c08d-110">With a DLP policy, you can identify, monitor, and automatically protect sensitive information across Office 365.</span></span>

<span data-ttu-id="7c08d-111">Lisateabe saamiseks külastage neid linke:</span><span class="sxs-lookup"><span data-stu-id="7c08d-111">Please visit these links for more information:</span></span>

- [<span data-ttu-id="7c08d-112">Andmete kaotsimineku vältimise ülevaade</span><span class="sxs-lookup"><span data-stu-id="7c08d-112">Overview of data loss prevention</span></span>](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies)
- [<span data-ttu-id="7c08d-113">Millised tundlikud teabetüübid otsida</span><span class="sxs-lookup"><span data-stu-id="7c08d-113">What the sensitive information types look for</span></span>](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
- [<span data-ttu-id="7c08d-114">Kohandatud tundliku teabe tüübi loomine</span><span class="sxs-lookup"><span data-stu-id="7c08d-114">Create a custom sensitive information type</span></span>](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)
- [<span data-ttu-id="7c08d-115">Saatke meiliteatised ja näidake poliitikaspikreid</span><span class="sxs-lookup"><span data-stu-id="7c08d-115">Send email notifications and show policy tips</span></span>](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)
- [<span data-ttu-id="7c08d-116">Kaitse SharePoint Online faile Säilitussildid ja DLP</span><span class="sxs-lookup"><span data-stu-id="7c08d-116">Protect SharePoint Online files with retention labels and DLP</span></span>](https://docs.microsoft.com/office365/securitycompliance/protect-sharepoint-online-files-with-office-365-labels-and-dlp)
- [<span data-ttu-id="7c08d-117">DLP ja Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="7c08d-117">DLP and Microsoft Teams</span></span>](https://docs.microsoft.com/office365/securitycompliance/dlp-microsoft-teams)

<span data-ttu-id="7c08d-118">Oma andmete testimiseks sisseehitatud või kohandatud tundliku teabe tüübiga kasutage suvandit **testi tüüp jaotises liigitustundlikud** **Classifications** > **teabetüübid**.</span><span class="sxs-lookup"><span data-stu-id="7c08d-118">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="7c08d-119">Lisateabe saamiseks vt teemat [kohandatud tundliku teabe tüüpide testimine](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="7c08d-119">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>