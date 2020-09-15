---
title: DLP reegel SSN ei tööta
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679365"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="90f2e-102">DLP seotud probleemid</span><span class="sxs-lookup"><span data-stu-id="90f2e-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="90f2e-103">**Tähtis**! Nende enneolematude aegade jooksul võtame kasutusele meetmed, et säilitada SharePoint Online’i ja OneDrive’i teenuste hea kättesadavus. Lisateabe saamiseks vaadake teemat [SharePoint Online’i ajutised funktsioonide muudatused](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="90f2e-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="90f2e-104">**Vorminguga SSN DLP probleemid**</span><span class="sxs-lookup"><span data-stu-id="90f2e-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="90f2e-105">Kas teil on probleeme **andmete kaotsimineku vältimisega (DLP)** , mis ei tööta Microsoft 365 tundliku teabe tippimise korral **sotsiaalkindlustuse numbrit (SSN)** sisaldava sisuga?</span><span class="sxs-lookup"><span data-stu-id="90f2e-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="90f2e-106">Kui jah, siis veenduge, et teie sisu sisaldaks vajalikku teavet selle kohta, mida DLP poliitika otsib.</span><span class="sxs-lookup"><span data-stu-id="90f2e-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="90f2e-107">Näiteks SSN poliitika jaoks, mis on konfigureeritud 85%-ga, hinnatakse ja see tuleb reegli käivitamiseks tuvastada järgmiselt.</span><span class="sxs-lookup"><span data-stu-id="90f2e-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="90f2e-108">**[Vorming:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 numbrit, mis võivad olla vormindatud või vormindamata mustriga.</span><span class="sxs-lookup"><span data-stu-id="90f2e-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="90f2e-109">**[Muster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Neli funktsiooni otsivad vorminguga SSN neljast erinevast etalonist.</span><span class="sxs-lookup"><span data-stu-id="90f2e-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="90f2e-110">Func_ssn leiab vorminguga SSN, 2011 kus on DDD, kus on vormindatud kriipsud või tühikud (-DD-dddd või DDD DD dddd).</span><span class="sxs-lookup"><span data-stu-id="90f2e-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="90f2e-111">Func_unformatted_ssn leiab vorminguga SSN 2011, kus on ddddddddd tugev vorming, mis on vormindamata üheksa järjestikust numbrit ().</span><span class="sxs-lookup"><span data-stu-id="90f2e-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="90f2e-112">Func_randomized_formatted_ssn leiab post-2011 vorminguga SSN, mis on vormindatud sidekriipsude või tühikutega (DDD-DD-dddd või DDD DD dddd)</span><span class="sxs-lookup"><span data-stu-id="90f2e-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="90f2e-113">Func_randomized_unformatted_ssn leiab post-2011 vorminguga SSN, mis on vormindamata üheksa järjestikuseks numbriks (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="90f2e-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="90f2e-114">**[Kontrollsumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Ei, pole kontrollsummat</span><span class="sxs-lookup"><span data-stu-id="90f2e-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="90f2e-115">**[Definitsioon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** DLP poliitika on 85% kindel, et see on tuvastanud seda tüüpi tundliku teabe, kui 300 märkide lähedusse jääb:</span><span class="sxs-lookup"><span data-stu-id="90f2e-115">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="90f2e-116">[Funktsioon Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) otsib mustriga kattuvat sisu.</span><span class="sxs-lookup"><span data-stu-id="90f2e-116">The [function Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="90f2e-117">Leitakse [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) märksõna.</span><span class="sxs-lookup"><span data-stu-id="90f2e-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found.</span></span> <span data-ttu-id="90f2e-118">Märksõnade näited on:  *sotsiaalkindlustus, sotsiaalkindlustus #, SOC SEC, SSN*  .</span><span class="sxs-lookup"><span data-stu-id="90f2e-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="90f2e-119">Näiteks käivitatakse DLP SSN poliitika jaoks järgmine näidis: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="90f2e-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="90f2e-120">Lisateavet selle kohta, mida on vaja sisu tuvastamiseks vorminguga SSN, leiate selle artikli jaotisest [Kuidas tundlikud andmetüübid vorminguga SSN otsivad?](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="90f2e-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="90f2e-121">Mõne muu sisseehitatud tundliku teabe tüübi abil leiate lisateavet selle kohta, mida on vaja muude tüüpide jaoks: [millist tüüpi tundlikud teabe tüübid otsivad](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="90f2e-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  