---
title: DLP reegel SSN ei tööta
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 0b83a858975ffe1bb70f16a7452a13d57dff5340
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932517"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="156c3-102">DLP probleemid sotsiaalkindlustuse numbrid</span><span class="sxs-lookup"><span data-stu-id="156c3-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="156c3-103">**Oluline**: paljud SharePoint Online ' i ja OneDrive kliendid käivitada Business kriitilised rakendused teenuse, mis töötavad taustal.</span><span class="sxs-lookup"><span data-stu-id="156c3-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="156c3-104">Nende hulka kuuluvad sisu migratsioon, andmete kadu vältimine (DLP) ja backup lahendused.</span><span class="sxs-lookup"><span data-stu-id="156c3-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="156c3-105">Nendel enneolematul ajal me võtame meetmeid, et tagada SharePoint Online ' i ja OneDrive teenused on väga kättesaadav ja usaldusväärne oma kasutajatele, kes sõltuvad teenuse rohkem kui kunagi varem kaugtöö stsenaariume.</span><span class="sxs-lookup"><span data-stu-id="156c3-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="156c3-106">Selle eesmärgi toetuseks oleme rakendanud ranget ahendamise piiranguid taustal olevatele rakendustele (migratsioon, DLP ja backup lahendused) tööpäeval päeva jooksul.</span><span class="sxs-lookup"><span data-stu-id="156c3-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="156c3-107">Te peaksite ootama, et need rakendused saavutavad nende aegade jooksul väga piiratud läbilaskevõime.</span><span class="sxs-lookup"><span data-stu-id="156c3-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="156c3-108">Aga, õhtuti ja nädalavahetusel tundi piirkonna, teenus on valmis töötlema oluliselt suurem hulk taotlusi taustal apps.</span><span class="sxs-lookup"><span data-stu-id="156c3-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="156c3-109">**DLP probleemid SSNs**</span><span class="sxs-lookup"><span data-stu-id="156c3-109">**DLP issues with SSNs**</span></span>

<span data-ttu-id="156c3-110">Kas teil on probleeme **andmete kadu vältimine (DLP)** ei tööta sisu, mis sisaldab **sotsiaalse turvalisuse number (SSN)** tundliku teabe tüüp Office 365 kasutamisel?</span><span class="sxs-lookup"><span data-stu-id="156c3-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="156c3-111">Kui jah, veenduge, et teie sisu sisaldab vajalikku teavet DLP poliitika otsib.</span><span class="sxs-lookup"><span data-stu-id="156c3-111">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="156c3-112">Näiteks SSN poliitika konfigureeritud usalduse tase 85%, hinnatakse ja tuleb tuvastada reegli käivitamiseks:</span><span class="sxs-lookup"><span data-stu-id="156c3-112">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="156c3-113">**[Formaat:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 numbrit, mis võib olla vormindatud või vormindamata muster</span><span class="sxs-lookup"><span data-stu-id="156c3-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="156c3-114">**[Muster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Neli funktsiooni otsima SSNs neljas erinevas struktuuris:</span><span class="sxs-lookup"><span data-stu-id="156c3-114">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="156c3-115">Func_ssn leiab SSNs pre-2011 tugeva vormingu, mis on vormindatud kriipsu või tühikuid (DDD-DD-dddd või DDD DD dddd)</span><span class="sxs-lookup"><span data-stu-id="156c3-115">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="156c3-116">Func_unformatted_ssn leiab SSNs pre-2011 tugev vormindamine, mis on vormindamata üheksa järjestikust numbrit (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="156c3-116">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="156c3-117">Func_randomized_formatted_ssn leiab post-2011 SSNs, mis on vormindatud kriipsude või tühikute (DDD-DD-dddd või DDD DD dddd)</span><span class="sxs-lookup"><span data-stu-id="156c3-117">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="156c3-118">Func_randomized_unformatted_ssn leiab post-2011 SSNs, mis on vormindamata üheksa järjestikust numbrit (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="156c3-118">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="156c3-119">**[Kontrollsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Ei, kontrollsumma puudub</span><span class="sxs-lookup"><span data-stu-id="156c3-119">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="156c3-120">**[Määratlus:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP poliitika on 85% kindel, et see on avastatud seda tüüpi tundlik teave, kui lähedus 300 tähemärki:</span><span class="sxs-lookup"><span data-stu-id="156c3-120">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="156c3-121">[Funktsioon Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) otsib sisu, mis vastab mustrile.</span><span class="sxs-lookup"><span data-stu-id="156c3-121">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="156c3-122">Leitakse märksõna [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) .</span><span class="sxs-lookup"><span data-stu-id="156c3-122">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="156c3-123">Märksõnade näited on: *sotsiaalkindlustus, sotsiaalkindlustus #, SOC SEC, SSN* .</span><span class="sxs-lookup"><span data-stu-id="156c3-123">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="156c3-124">Näiteks järgmine näidis käivitab DLP SSN poliitika: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="156c3-124">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="156c3-125">Lisateabe saamiseks selle kohta, mida on vaja SSNs tuvastatav sisu, lugege järgmist jaotist selles artiklis: [mida tundliku teabe tüübid otsida SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="156c3-125">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="156c3-126">Kasutades muu sisseehitatud tundliku teabe tüüp, lugege järgmist artiklit teavet, mida on vaja muud tüüpi: [mida tundliku teabe tüübid otsida](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="156c3-126">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  