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
ms.openlocfilehash: bb7d8ca91af73fa4ebed5992ec848128beb18830
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977158"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="15f7c-102">DLP probleemid USA pangakonto numbrid</span><span class="sxs-lookup"><span data-stu-id="15f7c-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="15f7c-103">**Oluline**: nendel enneolematul ajal me võtame meetmeid, et tagada SharePoint Online ' i ja OneDrive teenused on väga kättesaadavad-Palun külastage [SharePoint Online ajutised funktsiooni kohandused](https://aka.ms/ODSPAdjustments) lisateabe saamiseks.</span><span class="sxs-lookup"><span data-stu-id="15f7c-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="15f7c-104">**DLP probleemid USA pangakonto numbrid**</span><span class="sxs-lookup"><span data-stu-id="15f7c-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="15f7c-105">Kas teil on probleeme **andmete kadu vältimine (DLP)** ei tööta sisu, mis sisaldab **USA pangakonto number** , kui kasutate DLP tundliku teabe tüüp O365?</span><span class="sxs-lookup"><span data-stu-id="15f7c-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="15f7c-106">Kui jah, veenduge, et teie sisu sisaldab vajalikku teavet selle kohta, mida DLP poliitika otsib, kui seda hinnatakse.</span><span class="sxs-lookup"><span data-stu-id="15f7c-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="15f7c-107">Näiteks **USA pangakonto number** poliitika konfigureeritud usalduse tase 85%, hinnatakse järgmist ja tuleb tuvastada reegli käivitamiseks:</span><span class="sxs-lookup"><span data-stu-id="15f7c-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="15f7c-108">**[Formaat:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 numbrit</span><span class="sxs-lookup"><span data-stu-id="15f7c-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="15f7c-109">**[Muster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 järjestikust numbrit.</span><span class="sxs-lookup"><span data-stu-id="15f7c-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="15f7c-110">**[Kontrollsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ei, kontrollsumma puudub</span><span class="sxs-lookup"><span data-stu-id="15f7c-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="15f7c-111">**[Määratlus:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** DLP poliitika on 75% kindel, et see on avastatud seda tüüpi tundlik teave, kui lähedus 300 tähemärki:</span><span class="sxs-lookup"><span data-stu-id="15f7c-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="15f7c-112">Regulaarne avaldis Regex_usa_bank_account_number otsib sisu, mis vastab muster</span><span class="sxs-lookup"><span data-stu-id="15f7c-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="15f7c-113">Leitakse märksõna Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="15f7c-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="15f7c-114">Näiteks järgmine näidis käivitab **USA pangakonto number** poliitika: konto 78344011 kontrollimine</span><span class="sxs-lookup"><span data-stu-id="15f7c-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="15f7c-115">Lisateabe saamiseks selle kohta, mida on vaja **USA pangakonto number** tuvastatav teie sisu, lugege järgmist jaotist selles artiklis: [mida tundliku teabe tüübid otsida USA pangakonto number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="15f7c-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="15f7c-116">Kasutades muu sisseehitatud tundliku teabe tüüp, lugege järgmist artiklit teavet, mida on vaja muud tüüpi: [mida tundliku teabe tüübid otsida](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="15f7c-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  