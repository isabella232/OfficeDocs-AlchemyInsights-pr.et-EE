---
title: DLP reegel USA pangakonto number ei tööta
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 0b5c1fb175275028c56e47080708520fe115fb38
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932526"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="dc05d-102">DLP probleemid USA pangakonto numbrid</span><span class="sxs-lookup"><span data-stu-id="dc05d-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="dc05d-103">**Oluline**: paljud SharePoint Online ' i ja OneDrive kliendid käivitada Business kriitilised rakendused teenuse, mis töötavad taustal.</span><span class="sxs-lookup"><span data-stu-id="dc05d-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="dc05d-104">Nende hulka kuuluvad sisu migratsioon, andmete kadu vältimine (DLP) ja backup lahendused.</span><span class="sxs-lookup"><span data-stu-id="dc05d-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="dc05d-105">Nendel enneolematul ajal me võtame meetmeid, et tagada SharePoint Online ' i ja OneDrive teenused on väga kättesaadav ja usaldusväärne oma kasutajatele, kes sõltuvad teenuse rohkem kui kunagi varem kaugtöö stsenaariume.</span><span class="sxs-lookup"><span data-stu-id="dc05d-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="dc05d-106">Selle eesmärgi toetuseks oleme rakendanud ranget ahendamise piiranguid taustal olevatele rakendustele (migratsioon, DLP ja backup lahendused) tööpäeval päeva jooksul.</span><span class="sxs-lookup"><span data-stu-id="dc05d-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="dc05d-107">Te peaksite ootama, et need rakendused saavutavad nende aegade jooksul väga piiratud läbilaskevõime.</span><span class="sxs-lookup"><span data-stu-id="dc05d-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="dc05d-108">Aga, õhtuti ja nädalavahetusel tundi piirkonna, teenus on valmis töötlema oluliselt suurem hulk taotlusi taustal apps.</span><span class="sxs-lookup"><span data-stu-id="dc05d-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="dc05d-109">**DLP probleemid USA pangakonto numbrid**</span><span class="sxs-lookup"><span data-stu-id="dc05d-109">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="dc05d-110">Kas teil on probleeme **andmete kadu vältimine (DLP)** ei tööta sisu, mis sisaldab **USA pangakonto number** , kui kasutate DLP tundliku teabe tüüp O365?</span><span class="sxs-lookup"><span data-stu-id="dc05d-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="dc05d-111">Kui jah, veenduge, et teie sisu sisaldab vajalikku teavet selle kohta, mida DLP poliitika otsib, kui seda hinnatakse.</span><span class="sxs-lookup"><span data-stu-id="dc05d-111">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="dc05d-112">Näiteks **USA pangakonto number** poliitika konfigureeritud usalduse tase 85%, hinnatakse järgmist ja tuleb tuvastada reegli käivitamiseks:</span><span class="sxs-lookup"><span data-stu-id="dc05d-112">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="dc05d-113">**[Formaat:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 numbrit</span><span class="sxs-lookup"><span data-stu-id="dc05d-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="dc05d-114">**[Muster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 järjestikust numbrit.</span><span class="sxs-lookup"><span data-stu-id="dc05d-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="dc05d-115">**[Kontrollsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ei, kontrollsumma puudub</span><span class="sxs-lookup"><span data-stu-id="dc05d-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="dc05d-116">**[Määratlus:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** DLP poliitika on 75% kindel, et see on avastatud seda tüüpi tundlik teave, kui lähedus 300 tähemärki:</span><span class="sxs-lookup"><span data-stu-id="dc05d-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="dc05d-117">Regulaarne avaldis Regex_usa_bank_account_number otsib sisu, mis vastab muster</span><span class="sxs-lookup"><span data-stu-id="dc05d-117">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="dc05d-118">Leitakse märksõna Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="dc05d-118">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="dc05d-119">Näiteks järgmine näidis käivitab **USA pangakonto number** poliitika: konto 78344011 kontrollimine</span><span class="sxs-lookup"><span data-stu-id="dc05d-119">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="dc05d-120">Lisateabe saamiseks selle kohta, mida on vaja **USA pangakonto number** tuvastatav teie sisu, lugege järgmist jaotist selles artiklis: [mida tundliku teabe tüübid otsida USA pangakonto number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="dc05d-120">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="dc05d-121">Kasutades muu sisseehitatud tundliku teabe tüüp, lugege järgmist artiklit teavet, mida on vaja muud tüüpi: [mida tundliku teabe tüübid otsida](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="dc05d-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  