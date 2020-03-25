---
title: DLP reegel krediitkaardi number ei tööta
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
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932439"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="f7391-102">DLP probleemid krediitkaardi numbrid</span><span class="sxs-lookup"><span data-stu-id="f7391-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="f7391-103">**Oluline**: paljud SharePoint Online ' i ja OneDrive kliendid käivitada Business kriitilised rakendused teenuse, mis töötavad taustal.</span><span class="sxs-lookup"><span data-stu-id="f7391-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="f7391-104">Nende hulka kuuluvad sisu migratsioon, andmete kadu vältimine (DLP) ja backup lahendused.</span><span class="sxs-lookup"><span data-stu-id="f7391-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="f7391-105">Nendel enneolematul ajal me võtame meetmeid, et tagada SharePoint Online ' i ja OneDrive teenused on väga kättesaadav ja usaldusväärne oma kasutajatele, kes sõltuvad teenuse rohkem kui kunagi varem kaugtöö stsenaariume.</span><span class="sxs-lookup"><span data-stu-id="f7391-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="f7391-106">Selle eesmärgi toetuseks oleme rakendanud ranget ahendamise piiranguid taustal olevatele rakendustele (migratsioon, DLP ja backup lahendused) tööpäeval päeva jooksul.</span><span class="sxs-lookup"><span data-stu-id="f7391-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="f7391-107">Te peaksite ootama, et need rakendused saavutavad nende aegade jooksul väga piiratud läbilaskevõime.</span><span class="sxs-lookup"><span data-stu-id="f7391-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="f7391-108">Aga, õhtuti ja nädalavahetusel tundi piirkonna, teenus on valmis töötlema oluliselt suurem hulk taotlusi taustal apps.</span><span class="sxs-lookup"><span data-stu-id="f7391-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="f7391-109">**DLP probleemid krediitkaardi numbrid**</span><span class="sxs-lookup"><span data-stu-id="f7391-109">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="f7391-110">Kas teil on probleeme **andmete kadu vältimine (DLP)** ei tööta sisu, mis sisaldab **krediitkaardi number** , kasutades DLP tundliku teabe tüüp O365?</span><span class="sxs-lookup"><span data-stu-id="f7391-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="f7391-111">Kui jah, veenduge, et teie sisu sisaldab vajalikku teavet, et käivitada DLP poliitika, kui see on hinnatud.</span><span class="sxs-lookup"><span data-stu-id="f7391-111">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="f7391-112">Näiteks **krediitkaardi poliitika** konfigureeritud usalduse tase 85%, hinnatakse ja tuleb tuvastada reegli käivitamiseks:</span><span class="sxs-lookup"><span data-stu-id="f7391-112">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="f7391-113">**[Formaat:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 numbrit, mida saab vormindada või vormindamata (dddddddddddddddd) ja peab läbima Luhn test.</span><span class="sxs-lookup"><span data-stu-id="f7391-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="f7391-114">**[Muster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Väga keeruline ja jõuline muster, mis tuvastab kaarte kõigi suuremate kaubamärkide kogu maailmas, sealhulgas Visa, MasterCard, Discover kaart, JCB, American Express, kinkekaardid, ja söökla kaardid.</span><span class="sxs-lookup"><span data-stu-id="f7391-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="f7391-115">**[Kontrollsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Jah, Luhn-i kontrollsumma</span><span class="sxs-lookup"><span data-stu-id="f7391-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="f7391-116">**[Määratlus:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP poliitika on 85% kindel, et see on avastatud seda tüüpi tundlik teave, kui lähedus 300 tähemärki:</span><span class="sxs-lookup"><span data-stu-id="f7391-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="f7391-117">Funktsioon Func_credit_card otsib sisu, mis vastab mustrile.</span><span class="sxs-lookup"><span data-stu-id="f7391-117">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="f7391-118">Üks järgmistest on täidetud:</span><span class="sxs-lookup"><span data-stu-id="f7391-118">One of the following is true:</span></span>

  - <span data-ttu-id="f7391-119">Leitakse märksõna Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="f7391-119">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="f7391-120">Leitakse märksõna Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="f7391-120">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="f7391-121">Funktsioon Func_expiration_date otsib kuupäeva paremas kuupäevavormingus.</span><span class="sxs-lookup"><span data-stu-id="f7391-121">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="f7391-122">Kontrollsumma möödub</span><span class="sxs-lookup"><span data-stu-id="f7391-122">The checksum passes</span></span>

    <span data-ttu-id="f7391-123">Näiteks järgmine näidis käivitab DLP krediitkaardi number poliitika:</span><span class="sxs-lookup"><span data-stu-id="f7391-123">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="f7391-124">Viisa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="f7391-124">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="f7391-125">Aegub: 2/2009</span><span class="sxs-lookup"><span data-stu-id="f7391-125">Expires: 2/2009</span></span>

<span data-ttu-id="f7391-126">Lisateabe saamiseks selle kohta, mida on vaja teie sisu tuvastada **krediitkaardi number** , lugege järgmist jaotist selles artiklis: [mida tundliku teabe tüübid otsida krediitkaardi #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="f7391-126">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="f7391-127">Kasutades muu sisseehitatud tundliku teabe tüüp, lugege järgmist artiklit teavet, mida on vaja muud tüüpi: [mida tundliku teabe tüübid otsida](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="f7391-127">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  