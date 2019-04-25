---
title: DLP reegel numbrid ei tööta
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e1d60c493a27efb7f724d57051e21fad5bd0242f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404484"
---
<span data-ttu-id="f75ac-102">On teil probleeme **Andmete kaotsimineku vältimise (DLP)** , mis sisaldab **Krediitkaardi numbrit** kasutades DLP tundliku teabe tüüp O365 sisu ei tööta?</span><span class="sxs-lookup"><span data-stu-id="f75ac-102">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="f75ac-103">Sellisel juhul veenduge, et sisu sisaldab käivitamiseks vajalik teave ning kui seda hinnatakse DLP poliitika.</span><span class="sxs-lookup"><span data-stu-id="f75ac-103">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="f75ac-104">Näiteks **krediitkaardi poliitika** konfigureeritud 85% usaldusnivoo, järgnev hinnatakse ja peavad avastama reegli käivitamiseks:</span><span class="sxs-lookup"><span data-stu-id="f75ac-104">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="f75ac-105">**[Formaat:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16-kohaline, mida saab vormindada või vormindamata (dddddddddddddddd) ja peab läbima Luhn testi.</span><span class="sxs-lookup"><span data-stu-id="f75ac-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span> 
    
- <span data-ttu-id="f75ac-106">**[Puhul:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Väga keeruline ja tugev muster, mis tuvastab kõik suure brändi üle maailma, sealhulgas Visa, Mastercard, Discover Card, JCB, American Express, Kinkekaardid ja söökla kaardid kaardid.</span><span class="sxs-lookup"><span data-stu-id="f75ac-106">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span> 
    
- <span data-ttu-id="f75ac-107">**[Kontrollsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Jah, Luhn kontrollsumma</span><span class="sxs-lookup"><span data-stu-id="f75ac-107">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span> 
    
- <span data-ttu-id="f75ac-108">**[Määratlus:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP poliitika on 85% kindel, et ta ei avastanud seda tüüpi tundlikku teavet kui raadiuses 300 tähemärki:</span><span class="sxs-lookup"><span data-stu-id="f75ac-108">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="f75ac-109">Funktsiooni Func_credit_card leiab sisu, mis ühtiks.</span><span class="sxs-lookup"><span data-stu-id="f75ac-109">The function Func_credit_card finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="f75ac-110">Üks järgmistest on tõsi:</span><span class="sxs-lookup"><span data-stu-id="f75ac-110">One of the following is true:</span></span> 
    
  - <span data-ttu-id="f75ac-111">Märksõna: Keyword_cc_verification ei leitud.</span><span class="sxs-lookup"><span data-stu-id="f75ac-111">A keyword from Keyword_cc_verification is found.</span></span>
    
  - <span data-ttu-id="f75ac-112">Märksõna: Keyword_cc_name on leitud</span><span class="sxs-lookup"><span data-stu-id="f75ac-112">A keyword from Keyword_cc_name is found</span></span>
    
  - <span data-ttu-id="f75ac-113">Funktsiooni Func_expiration_date leiab õige kuupäev vormingus kuupäev.</span><span class="sxs-lookup"><span data-stu-id="f75ac-113">The function Func_expiration_date finds a date in the right date format.</span></span>
    
  - <span data-ttu-id="f75ac-114">Kontrollsumma läheb</span><span class="sxs-lookup"><span data-stu-id="f75ac-114">The checksum passes</span></span>
    
    <span data-ttu-id="f75ac-115">Näiteks peale tingiksid DLP krediitkaardi Number poliitika:</span><span class="sxs-lookup"><span data-stu-id="f75ac-115">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>
    
  - <span data-ttu-id="f75ac-116">Viisa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="f75ac-116">Visa: 4485 3647 3952 7352</span></span> 
    
  - <span data-ttu-id="f75ac-117">Aegub: 2/2009</span><span class="sxs-lookup"><span data-stu-id="f75ac-117">Expires: 2/2009</span></span>
    
<span data-ttu-id="f75ac-118">Mis tuleb **Numbrid** tuvastada sisu kohta lisateabe saamiseks vt käesoleva artikli järgmist osa: [Mida the tundliku teabe tüübid otsima krediitkaardi #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="f75ac-118">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="f75ac-119">Kasutades erinevaid sisseehitatud tundliku teabe tüüp, lugege järgmist teabe kohta, mida nõutakse muude: [mida the tundlik tüüpi teavet otsida](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="f75ac-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

