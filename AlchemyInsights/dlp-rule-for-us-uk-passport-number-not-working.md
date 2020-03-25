---
title: DLP reegel USA/UK passi number ei tööta
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c63e814059c897531109aa78725e9811b311fb27
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931258"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="e50b7-102">Probleemid DLP-USA/UK passi numbritega</span><span class="sxs-lookup"><span data-stu-id="e50b7-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="e50b7-103">**Oluline**: paljud SharePoint Online ' i ja OneDrive kliendid käivitada Business kriitilised rakendused teenuse, mis töötavad taustal.</span><span class="sxs-lookup"><span data-stu-id="e50b7-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="e50b7-104">Nende hulka kuuluvad sisu migratsioon, andmete kadu vältimine (DLP) ja backup lahendused.</span><span class="sxs-lookup"><span data-stu-id="e50b7-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="e50b7-105">Nendel enneolematul ajal me võtame meetmeid, et tagada SharePoint Online ' i ja OneDrive teenused on väga kättesaadav ja usaldusväärne oma kasutajatele, kes sõltuvad teenuse rohkem kui kunagi varem kaugtöö stsenaariume.</span><span class="sxs-lookup"><span data-stu-id="e50b7-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="e50b7-106">Selle eesmärgi toetuseks oleme rakendanud ranget ahendamise piiranguid taustal olevatele rakendustele (migratsioon, DLP ja backup lahendused) tööpäeval päeva jooksul.</span><span class="sxs-lookup"><span data-stu-id="e50b7-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="e50b7-107">Te peaksite ootama, et need rakendused saavutavad nende aegade jooksul väga piiratud läbilaskevõime.</span><span class="sxs-lookup"><span data-stu-id="e50b7-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="e50b7-108">Aga, õhtuti ja nädalavahetusel tundi piirkonna, teenus on valmis töötlema oluliselt suurem hulk taotlusi taustal apps.</span><span class="sxs-lookup"><span data-stu-id="e50b7-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="e50b7-109">**DLP probleemid USA/UK passi numbrid**</span><span class="sxs-lookup"><span data-stu-id="e50b7-109">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="e50b7-110">Kas teil on probleeme **andmete kadu vältimine (DLP)** ei tööta sisu, mis sisaldab **USA/UK passi number** , kui kasutate DLP tundliku teabe tüüp O365?</span><span class="sxs-lookup"><span data-stu-id="e50b7-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="e50b7-111">Kui jah, veenduge, et teie sisu sisaldab vajalikku teavet selle kohta, mida DLP poliitika otsib, kui seda hinnatakse.</span><span class="sxs-lookup"><span data-stu-id="e50b7-111">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="e50b7-112">Näiteks **USA/UK passi number** poliitika konfigureeritud usalduse tase 75%, hinnatakse ja tuleb tuvastada reegli käivitamiseks</span><span class="sxs-lookup"><span data-stu-id="e50b7-112">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="e50b7-113">**[Formaat:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Üheksa numbrit</span><span class="sxs-lookup"><span data-stu-id="e50b7-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="e50b7-114">**[Muster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Üheksa järjestikust numbrit</span><span class="sxs-lookup"><span data-stu-id="e50b7-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="e50b7-115">**[Kontrollsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ei, kontrollsumma puudub</span><span class="sxs-lookup"><span data-stu-id="e50b7-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="e50b7-116">**[Määratlus:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP poliitika on 75% kindel, et see on avastatud seda tüüpi tundlik teave, kui lähedus 300 tähemärki:</span><span class="sxs-lookup"><span data-stu-id="e50b7-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="e50b7-117">Funktsioon Func_usa_uk_passport otsib sisu, mis vastab mustrile.</span><span class="sxs-lookup"><span data-stu-id="e50b7-117">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="e50b7-118">Leitakse märksõna Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="e50b7-118">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="e50b7-119">Näiteks käivitab Järgmine näidis **USA/Ühendkuningriigi passi numbri** poliitika: USA passporti number 123456789</span><span class="sxs-lookup"><span data-stu-id="e50b7-119">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="e50b7-120">Lisateabe saamiseks selle kohta, mida on vaja USA/UK Passporti numbri avastamiseks teie sisu, lugege järgmist jaotist selles artiklis: [mida tundliku teabe tüübid otsida USA/UK passi number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="e50b7-120">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="e50b7-121">Kasutades muu sisseehitatud tundliku teabe tüüp, lugege järgmist artiklit teavet, mida on vaja muud tüüpi: [mida tundliku teabe tüübid otsida](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="e50b7-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  