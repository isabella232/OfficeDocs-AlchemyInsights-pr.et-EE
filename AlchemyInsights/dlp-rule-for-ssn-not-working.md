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
ms.openlocfilehash: 4ec0df9d4954a8c65f0c34188d285dd8cf44a4f2
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977302"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="a2e42-102">DLP probleemid sotsiaalkindlustuse numbrid</span><span class="sxs-lookup"><span data-stu-id="a2e42-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="a2e42-103">**Oluline**: nendel enneolematul ajal me võtame meetmeid, et tagada SharePoint Online ' i ja OneDrive teenused on väga kättesaadavad-Palun külastage [SharePoint Online ajutised funktsiooni kohandused](https://aka.ms/ODSPAdjustments) lisateabe saamiseks.</span><span class="sxs-lookup"><span data-stu-id="a2e42-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="a2e42-104">**DLP probleemid SSNs**</span><span class="sxs-lookup"><span data-stu-id="a2e42-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="a2e42-105">Kas teil on probleeme **andmete kadu vältimine (DLP)** ei tööta sisu, mis sisaldab **sotsiaalse turvalisuse number (SSN)** tundliku teabe tüüp Office 365 kasutamisel?</span><span class="sxs-lookup"><span data-stu-id="a2e42-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="a2e42-106">Kui jah, veenduge, et teie sisu sisaldab vajalikku teavet DLP poliitika otsib.</span><span class="sxs-lookup"><span data-stu-id="a2e42-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="a2e42-107">Näiteks SSN poliitika konfigureeritud usalduse tase 85%, hinnatakse ja tuleb tuvastada reegli käivitamiseks:</span><span class="sxs-lookup"><span data-stu-id="a2e42-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="a2e42-108">**[Formaat:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 numbrit, mis võib olla vormindatud või vormindamata muster</span><span class="sxs-lookup"><span data-stu-id="a2e42-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="a2e42-109">**[Muster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Neli funktsiooni otsima SSNs neljas erinevas struktuuris:</span><span class="sxs-lookup"><span data-stu-id="a2e42-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="a2e42-110">Func_ssn leiab SSNs pre-2011 tugeva vormingu, mis on vormindatud kriipsu või tühikuid (DDD-DD-dddd või DDD DD dddd)</span><span class="sxs-lookup"><span data-stu-id="a2e42-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="a2e42-111">Func_unformatted_ssn leiab SSNs pre-2011 tugev vormindamine, mis on vormindamata üheksa järjestikust numbrit (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="a2e42-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="a2e42-112">Func_randomized_formatted_ssn leiab post-2011 SSNs, mis on vormindatud kriipsude või tühikute (DDD-DD-dddd või DDD DD dddd)</span><span class="sxs-lookup"><span data-stu-id="a2e42-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="a2e42-113">Func_randomized_unformatted_ssn leiab post-2011 SSNs, mis on vormindamata üheksa järjestikust numbrit (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="a2e42-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="a2e42-114">**[Kontrollsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Ei, kontrollsumma puudub</span><span class="sxs-lookup"><span data-stu-id="a2e42-114">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="a2e42-115">**[Määratlus:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP poliitika on 85% kindel, et see on avastatud seda tüüpi tundlik teave, kui lähedus 300 tähemärki:</span><span class="sxs-lookup"><span data-stu-id="a2e42-115">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="a2e42-116">[Funktsioon Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) otsib sisu, mis vastab mustrile.</span><span class="sxs-lookup"><span data-stu-id="a2e42-116">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="a2e42-117">Leitakse märksõna [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) .</span><span class="sxs-lookup"><span data-stu-id="a2e42-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="a2e42-118">Märksõnade näited on: *sotsiaalkindlustus, sotsiaalkindlustus #, SOC SEC, SSN* .</span><span class="sxs-lookup"><span data-stu-id="a2e42-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="a2e42-119">Näiteks järgmine näidis käivitab DLP SSN poliitika: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="a2e42-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="a2e42-120">Lisateabe saamiseks selle kohta, mida on vaja SSNs tuvastatav sisu, lugege järgmist jaotist selles artiklis: [mida tundliku teabe tüübid otsida SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="a2e42-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="a2e42-121">Kasutades muu sisseehitatud tundliku teabe tüüp, lugege järgmist artiklit teavet, mida on vaja muud tüüpi: [mida tundliku teabe tüübid otsida](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="a2e42-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  