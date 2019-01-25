---
title: DLP reegel meid pangakonto Number ei tööta
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 6eae9146d33f5fc307085dbf931d57bdbb28b82e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29466118"
---
<span data-ttu-id="4fb0c-p101">On teil probleeme **Andmete kaotsimineku vältimise (DLP)** mis sisaldab **USA pangakonto numbrit** kasutades DLP tundliku teabe tüüp O365 sisu ei tööta? Sellisel juhul veenduge, et sisu sisaldab vajalikku teavet kui hinnatakse seda, mida otsib DLP poliitika.</span><span class="sxs-lookup"><span data-stu-id="4fb0c-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="4fb0c-104">Näiteks **USA pangakonto Number** poliitika konfigureeritud 85% usaldusnivoo, järgnev hinnatakse ja peavad avastama reegli käivitamiseks:</span><span class="sxs-lookup"><span data-stu-id="4fb0c-104">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="4fb0c-105">**[Formaat:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 numbrit</span><span class="sxs-lookup"><span data-stu-id="4fb0c-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span> 
    
- <span data-ttu-id="4fb0c-106">**[Muster:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 järjestikust numbrit.</span><span class="sxs-lookup"><span data-stu-id="4fb0c-106">**[Pattern:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span> 
    
- <span data-ttu-id="4fb0c-107">**[Kontrollsumma:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ei, ei ole kontrollsumma</span><span class="sxs-lookup"><span data-stu-id="4fb0c-107">**[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="4fb0c-108">**[Määratlus:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)** DLP poliitika on 75% kindel, et ta ei avastanud seda tüüpi tundlikku teavet kui raadiuses 300 tähemärki:</span><span class="sxs-lookup"><span data-stu-id="4fb0c-108">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="4fb0c-109">Regulaaravaldise Regex_usa_bank_account_number leiab sisu, mis ühtiks</span><span class="sxs-lookup"><span data-stu-id="4fb0c-109">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>
    
  - <span data-ttu-id="4fb0c-110">Märksõna: Keyword_usa_Bank_Account ei leitud.</span><span class="sxs-lookup"><span data-stu-id="4fb0c-110">A keyword from Keyword_usa_Bank_Account is found.</span></span>
    
    <span data-ttu-id="4fb0c-111">Näiteks peale tingiksid **USA pangakonto Number** poliitika: pangakonto 78344011</span><span class="sxs-lookup"><span data-stu-id="4fb0c-111">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span> 
    
<span data-ttu-id="4fb0c-112">Lisateavet selle kohta, mida nõutakse **USA pangakonto Number** sisu tuvastada, leiate käesoleva artikli järgnevalt: [Mida the tundlik tüüpi teavet otsida USA pangakonto Number](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="4fb0c-112">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="4fb0c-113">Kasutades erinevaid sisseehitatud tundliku teabe tüüp, lugege järgmist teabe kohta, mida nõutakse muude: [mida the tundlik tüüpi teavet otsida](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="4fb0c-113">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

