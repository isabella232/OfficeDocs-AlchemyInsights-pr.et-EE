---
title: DLP reegel US Bank Account number ei tööta
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679292"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="a7874-102">DLP probleemid US Banki konto numbritega</span><span class="sxs-lookup"><span data-stu-id="a7874-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="a7874-103">**Tähtis**! Nende enneolematude aegade jooksul võtame kasutusele meetmed, et säilitada SharePoint Online’i ja OneDrive’i teenuste hea kättesadavus. Lisateabe saamiseks vaadake teemat [SharePoint Online’i ajutised funktsioonide muudatused](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="a7874-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="a7874-104">**DLP probleemid US Banki konto numbritega**</span><span class="sxs-lookup"><span data-stu-id="a7874-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="a7874-105">Kas teil on probleeme **andmete kaotsimineku vältimisega (DLP)** , mis ei tööta **USA** kontonumbrit sisaldava sisuga, kui kasutate O365 DLP tundliku teabe tüüpi?</span><span class="sxs-lookup"><span data-stu-id="a7874-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="a7874-106">Kui jah, siis veenduge, et teie sisu sisaldaks vajalikku teavet selle kohta, mida DLP poliitika selle hindamisel otsib.</span><span class="sxs-lookup"><span data-stu-id="a7874-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="a7874-107">Näiteks kui **US Bank Account number** on konfigureeritud 85% usaldusväärsusega, hinnatakse ja tuleb reegli käivitamise korral tuvastada järgmist.</span><span class="sxs-lookup"><span data-stu-id="a7874-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="a7874-108">**[Vorming:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 numbrit</span><span class="sxs-lookup"><span data-stu-id="a7874-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="a7874-109">**[Muster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 järjestikused numbrid.</span><span class="sxs-lookup"><span data-stu-id="a7874-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="a7874-110">**[Kontrollsumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ei, pole kontrollsummat</span><span class="sxs-lookup"><span data-stu-id="a7874-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="a7874-111">**[Definitsioon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** DLP poliitika on 75% kindel, et see on tuvastanud seda tüüpi tundliku teabe, kui 300 märkide lähedusse jääb:</span><span class="sxs-lookup"><span data-stu-id="a7874-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="a7874-112">Tavaline avaldis Regex_usa_bank_account_number otsib mustriga kattuvat sisu.</span><span class="sxs-lookup"><span data-stu-id="a7874-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="a7874-113">Leitakse Keyword_usa_Bank_Account märksõna.</span><span class="sxs-lookup"><span data-stu-id="a7874-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="a7874-114">Näiteks käivitab Järgmine näidis **USA pangakonto numbripoliitika** : konto 78344011</span><span class="sxs-lookup"><span data-stu-id="a7874-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="a7874-115">Lisateavet selle kohta, mis on vajalik selle kohta, mis on vajalik teie sisu tuvastamiseks **USA pangakonto numbri** kohta, leiate selle artikli jaotisest [Kuidas tundlikud teabe liigid meie pangakonto numbrit näevad](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number) ?</span><span class="sxs-lookup"><span data-stu-id="a7874-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span></span>
  
<span data-ttu-id="a7874-116">Mõne muu sisseehitatud tundliku teabe tüübi abil leiate lisateavet selle kohta, mida on vaja muude tüüpide jaoks: [millist tüüpi tundlikud teabe tüübid otsivad](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="a7874-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  