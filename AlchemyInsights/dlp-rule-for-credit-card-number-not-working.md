---
title: DLP reegel numbrid ei tööta
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 875afb47175a78c22894720cb0db8222f6f41614
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529951"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="88b55-102">DLP probleeme numbrite</span><span class="sxs-lookup"><span data-stu-id="88b55-102">DLP issues with Credit Card Numbers</span></span>

<span data-ttu-id="88b55-103">On teil probleeme **Andmete kaotsimineku vältimise (DLP)** , mis sisaldab **Krediitkaardi numbrit** kasutades DLP tundliku teabe tüüp O365 sisu ei tööta?</span><span class="sxs-lookup"><span data-stu-id="88b55-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="88b55-104">Sellisel juhul veenduge, et sisu sisaldab käivitamiseks vajalik teave ning kui seda hinnatakse DLP poliitika.</span><span class="sxs-lookup"><span data-stu-id="88b55-104">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="88b55-105">Näiteks **krediitkaardi poliitika** konfigureeritud 85% usaldusnivoo, järgnev hinnatakse ja peavad avastama reegli käivitamiseks:</span><span class="sxs-lookup"><span data-stu-id="88b55-105">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="88b55-106">**[Formaat:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16-kohaline, mida saab vormindada või vormindamata (dddddddddddddddd) ja peab läbima Luhn testi.</span><span class="sxs-lookup"><span data-stu-id="88b55-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="88b55-107">**[Puhul:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Väga keeruline ja tugev muster, mis tuvastab kõik suure brändi üle maailma, sealhulgas Visa, MasterCard, Discover Card, JCB, American Express, Kinkekaardid ja söökla kaardid kaardid.</span><span class="sxs-lookup"><span data-stu-id="88b55-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="88b55-108">**[Kontrollsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Jah, Luhn kontrollsumma</span><span class="sxs-lookup"><span data-stu-id="88b55-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="88b55-109">**[Määratlus:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP poliitika on 85% kindel, et ta ei avastanud seda tüüpi tundlikku teavet kui raadiuses 300 tähemärki:</span><span class="sxs-lookup"><span data-stu-id="88b55-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="88b55-110">Funktsiooni Func_credit_card leiab sisu, mis ühtiks.</span><span class="sxs-lookup"><span data-stu-id="88b55-110">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="88b55-111">Üks järgmistest on tõsi:</span><span class="sxs-lookup"><span data-stu-id="88b55-111">One of the following is true:</span></span>

  - <span data-ttu-id="88b55-112">Märksõna: Keyword_cc_verification ei leitud.</span><span class="sxs-lookup"><span data-stu-id="88b55-112">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="88b55-113">Märksõna: Keyword_cc_name on leitud</span><span class="sxs-lookup"><span data-stu-id="88b55-113">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="88b55-114">Funktsiooni Func_expiration_date leiab õige kuupäev vormingus kuupäev.</span><span class="sxs-lookup"><span data-stu-id="88b55-114">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="88b55-115">Kontrollsumma läheb</span><span class="sxs-lookup"><span data-stu-id="88b55-115">The checksum passes</span></span>

    <span data-ttu-id="88b55-116">Näiteks peale tingiksid DLP krediitkaardi Number poliitika:</span><span class="sxs-lookup"><span data-stu-id="88b55-116">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="88b55-117">Viisa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="88b55-117">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="88b55-118">Aegub: 2/2009</span><span class="sxs-lookup"><span data-stu-id="88b55-118">Expires: 2/2009</span></span>

<span data-ttu-id="88b55-119">Mis tuleb **Numbrid** tuvastada sisu kohta lisateabe saamiseks vt käesoleva artikli järgmist osa: [Mida the tundliku teabe tüübid otsima krediitkaardi #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="88b55-119">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="88b55-120">Kasutades erinevaid sisseehitatud tundliku teabe tüüp, lugege järgmist teabe kohta, mida nõutakse muude: [mida the tundlik tüüpi teavet otsida](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="88b55-120">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  