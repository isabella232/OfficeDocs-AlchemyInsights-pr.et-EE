---
title: DLP reegel USA / UK passi Number ei tööta
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
ms.openlocfilehash: 0567e9521507bcc192b187d0e5a8a0658332ff99
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389537"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="767a1-102">DLP - probleemid U.S. / UK passi numbrid</span><span class="sxs-lookup"><span data-stu-id="767a1-102">Problems with DLP - US/UK Passport Numbers</span></span>

<span data-ttu-id="767a1-103">On teil probleeme **Andmete kaotsimineku vältimise (DLP)** ei tööta sisu sisaldava puhul on **U.S. / UK passi Number** kasutades DLP tundliku teabe tüüp O365?</span><span class="sxs-lookup"><span data-stu-id="767a1-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK Passport Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="767a1-104">Sellisel juhul veenduge, et sisu sisaldab vajalikku teavet kui hinnatakse seda, mida otsib DLP poliitika.</span><span class="sxs-lookup"><span data-stu-id="767a1-104">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="767a1-105">Näiteks on **U.S. / UK passi Number** konfigureeritud 75% usaldusnivoo, järgmine hinnatakse ja reegli käivitamiseks tuleb kindlaks</span><span class="sxs-lookup"><span data-stu-id="767a1-105">For example, for a **US/UK Passport Number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="767a1-106">**[Formaat:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Üheksa numbrit</span><span class="sxs-lookup"><span data-stu-id="767a1-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="767a1-107">**[Puhul:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Üheksa järjestikust numbrit</span><span class="sxs-lookup"><span data-stu-id="767a1-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="767a1-108">**[Kontrollsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ei, ei ole kontrollsumma</span><span class="sxs-lookup"><span data-stu-id="767a1-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="767a1-109">**[Määratlus:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP poliitika on 75% kindel, et ta ei avastanud seda tüüpi tundlikku teavet kui raadiuses 300 tähemärki:</span><span class="sxs-lookup"><span data-stu-id="767a1-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="767a1-110">Funktsiooni Func_usa_uk_passport leiab sisu, mis ühtiks.</span><span class="sxs-lookup"><span data-stu-id="767a1-110">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="767a1-111">Märksõna: Keyword_passport ei leitud.</span><span class="sxs-lookup"><span data-stu-id="767a1-111">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="767a1-112">Näiteks peale tingiksid jaoks on **U.S. / UK passinumber** poliitika: USA passi number 123456789</span><span class="sxs-lookup"><span data-stu-id="767a1-112">For example, the following sample would trigger for the **US/UK Passport Number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="767a1-113">Rohkem infot mis tuleb USA / UK passi Number tuvastada sisu, vt käesoleva artikli järgmist osa: [mida the tundliku teabe tüübid vaadata USA / UK passi Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="767a1-113">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="767a1-114">Kasutades erinevaid sisseehitatud tundliku teabe tüüp, lugege järgmist teabe kohta, mida nõutakse muude: [mida the tundlik tüüpi teavet otsida](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="767a1-114">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  