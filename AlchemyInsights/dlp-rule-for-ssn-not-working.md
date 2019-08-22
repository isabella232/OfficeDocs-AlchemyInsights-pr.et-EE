---
title: DLP reegel ei tööta SSN
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
ms.openlocfilehash: 757136c39700f12f40f839b29277a59b0e436f03
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529846"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="8d58d-102">DLP küsimusi isikukoodidega</span><span class="sxs-lookup"><span data-stu-id="8d58d-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="8d58d-103">On sul probleeme ei tööta sisu sisaldava **Isikukood (SSN)** , kasutades teatud tundlikku teavet Office 365 **Andmete kaotsimineku vältimise (DLP)** ?</span><span class="sxs-lookup"><span data-stu-id="8d58d-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="8d58d-104">Sellisel juhul veenduge, et sisu sisaldab vajalikku teavet DLP poliitika turist.</span><span class="sxs-lookup"><span data-stu-id="8d58d-104">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="8d58d-105">Nt SSN poliitikat konfigureeritud 85% usaldusnivoo, järgnev hinnatakse ja peavad avastama reegli käivitamiseks:</span><span class="sxs-lookup"><span data-stu-id="8d58d-105">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="8d58d-106">**[Formaat:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 numbrit, mis võib olla vormindatud või vormindamata muster</span><span class="sxs-lookup"><span data-stu-id="8d58d-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="8d58d-107">**[Puhul:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Neli funktsiooni otsima SSNs neli erinevat tasandit:</span><span class="sxs-lookup"><span data-stu-id="8d58d-107">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="8d58d-108">Func_ssn leiab SSNs eel-2011 tugev disain kriipse ega tühikuid (ddd-dd-dddd OR ddd dd dddd) vormindatud</span><span class="sxs-lookup"><span data-stu-id="8d58d-108">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="8d58d-109">Func_unformatted_ssn leiab SSNs eel-2011 tugev disain on vormindamata, nagu üheksa järjestikust numbrit (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="8d58d-109">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="8d58d-110">Func_randomized_formatted_ssn leiab post-2011 SSNs, mis on vormindatud kriipse ega tühikuid (ddd-dd-dddd OR ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="8d58d-110">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="8d58d-111">Func_randomized_unformatted_ssn leiab post-2011 SSNs, mis on vormindamata, nagu üheksa järjestikust numbrit (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="8d58d-111">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="8d58d-112">**[Kontrollsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Ei, ei ole kontrollsumma</span><span class="sxs-lookup"><span data-stu-id="8d58d-112">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="8d58d-113">**[Määratlus:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP poliitika on 85% kindel, et ta ei avastanud seda tüüpi tundlikku teavet kui raadiuses 300 tähemärki:</span><span class="sxs-lookup"><span data-stu-id="8d58d-113">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="8d58d-114">[Funktsiooni Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) leiab sisu, mis ühtiks.</span><span class="sxs-lookup"><span data-stu-id="8d58d-114">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="8d58d-115">Märksõna: [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) ei leitud.</span><span class="sxs-lookup"><span data-stu-id="8d58d-115">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="8d58d-116">Sisaldab näiteks märksõnu: *sotsiaalse turvalisuse, sotsiaalkindlustuse #, Soc Sec, SSN* .</span><span class="sxs-lookup"><span data-stu-id="8d58d-116">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="8d58d-117">Näiteks peale tingiksid DLP SSN poliitika: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="8d58d-117">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="8d58d-118">Lisateavet selle kohta, mis tuleb SSNs sisu tuvastada, leiate järgnevalt selles artiklis: [Mida the tundlik tüüpi teavet otsida SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="8d58d-118">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="8d58d-119">Kasutades erinevaid sisseehitatud tundliku teabe tüüp, lugege järgmist teabe kohta, mida nõutakse muude: [mida the tundlik tüüpi teavet otsida](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="8d58d-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  