---
title: DLP ei tööta ootuspäraselt
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932618"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="a07f2-102">DLP ei tööta ootuspäraselt</span><span class="sxs-lookup"><span data-stu-id="a07f2-102">DLP not working as expected</span></span>

<span data-ttu-id="a07f2-103">**Oluline**: paljud SharePoint Online ' i ja OneDrive kliendid käivitada Business kriitilised rakendused teenuse, mis töötavad taustal.</span><span class="sxs-lookup"><span data-stu-id="a07f2-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="a07f2-104">Nende hulka kuuluvad sisu migratsioon, andmete kadu vältimine (DLP) ja backup lahendused.</span><span class="sxs-lookup"><span data-stu-id="a07f2-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="a07f2-105">Nendel enneolematul ajal me võtame meetmeid, et tagada SharePoint Online ' i ja OneDrive teenused on väga kättesaadav ja usaldusväärne oma kasutajatele, kes sõltuvad teenuse rohkem kui kunagi varem kaugtöö stsenaariume.</span><span class="sxs-lookup"><span data-stu-id="a07f2-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="a07f2-106">Selle eesmärgi toetuseks oleme rakendanud ranget ahendamise piiranguid taustal olevatele rakendustele (migratsioon, DLP ja backup lahendused) tööpäeval päeva jooksul.</span><span class="sxs-lookup"><span data-stu-id="a07f2-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="a07f2-107">Te peaksite ootama, et need rakendused saavutavad nende aegade jooksul väga piiratud läbilaskevõime.</span><span class="sxs-lookup"><span data-stu-id="a07f2-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="a07f2-108">Aga, õhtuti ja nädalavahetusel tundi piirkonna, teenus on valmis töötlema oluliselt suurem hulk taotlusi taustal apps.</span><span class="sxs-lookup"><span data-stu-id="a07f2-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

 <span data-ttu-id="a07f2-109">**DLP seadistamine**</span><span class="sxs-lookup"><span data-stu-id="a07f2-109">**Setting up DLP**</span></span>

<span data-ttu-id="a07f2-110">Kas teil on probleeme **andmete kadu vältimine (DLP)** Office 365 ei tööta ootuspäraselt?</span><span class="sxs-lookup"><span data-stu-id="a07f2-110">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="a07f2-111">Kui jah, veenduge, et teie **DLP poliitika** on õigesti seadistatud ja et teie andmed sisaldavad seda, mida **DLP poliitika** otsib, kui seda hinnatakse.</span><span class="sxs-lookup"><span data-stu-id="a07f2-111">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="a07f2-112">DLP poliitika võimaldab teil tuvastada ja kaitsta tundliku loomuga teavet oma organisatsioonis.</span><span class="sxs-lookup"><span data-stu-id="a07f2-112">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="a07f2-113">DLP poliitikate häälestamise puhul kasutage [siin](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)olevat teavet.</span><span class="sxs-lookup"><span data-stu-id="a07f2-113">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="a07f2-114">**Mida DLP poliitikad otsida**</span><span class="sxs-lookup"><span data-stu-id="a07f2-114">**What DLP policies look for**</span></span>
  
<span data-ttu-id="a07f2-115">**Sisseehitatud tundliku teabe tüüpide** kasutamisel Office 365 turvalisuse ja vastavuse keskus, DLP poliitika otsida konkreetseid mustreid ja elemente, kui need tundlikud tüübid tuvastada.</span><span class="sxs-lookup"><span data-stu-id="a07f2-115">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="a07f2-116">**Sisseehitatud tundlikud teabetüübid**</span><span class="sxs-lookup"><span data-stu-id="a07f2-116">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="a07f2-117">Teave sisseehitatud tundlik tüübid ja mida DLP poliitika otsib kui tuvastamine tundlik tüüp, vaadake: [mida tundliku teabe tüübid otsida](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="a07f2-117">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="a07f2-118">**Kohandatud tundliku teabe tüübid**</span><span class="sxs-lookup"><span data-stu-id="a07f2-118">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="a07f2-119">Kui proovite luua kohandatud tundliku teabe tüüpe, kasutage järgmist artiklit teabe saamiseks kohandatud tundliku tüübi loomise kohta: [kohandatud tundliku teabe tüübi loomine](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="a07f2-119">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="a07f2-120">**DLP poliitika testimine**</span><span class="sxs-lookup"><span data-stu-id="a07f2-120">**Test a DLP policy**</span></span>

<span data-ttu-id="a07f2-121">Oma andmete testimiseks sisseehitatud või kohandatud tundliku teabe tüübiga kasutage suvandit **testi tüüp jaotises liigitustundlikud** **Classifications** > **teabetüübid**.</span><span class="sxs-lookup"><span data-stu-id="a07f2-121">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="a07f2-122">Lisateabe saamiseks vt teemat [kohandatud tundliku teabe tüüpide testimine](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="a07f2-122">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="a07f2-123">**Aruanded**</span><span class="sxs-lookup"><span data-stu-id="a07f2-123">**Reports**</span></span>
  
- <span data-ttu-id="a07f2-124">Hankige tundlikud andmete ülevaated [DLP aruannetega.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="a07f2-124">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="a07f2-125">Vaadake juhtumi konkreetseid üksikasju [intsidendi aruandega](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="a07f2-125">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
