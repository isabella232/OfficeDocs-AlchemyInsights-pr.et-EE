---
title: DLP reegel, et krediitkaardi number ei tööta
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
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679437"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="e0728-102">Krediitkaardi numbritega seotud DLP</span><span class="sxs-lookup"><span data-stu-id="e0728-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="e0728-103">**Tähtis**! Nende enneolematude aegade jooksul võtame kasutusele meetmed, et säilitada SharePoint Online’i ja OneDrive’i teenuste hea kättesadavus. Lisateabe saamiseks vaadake teemat [SharePoint Online’i ajutised funktsioonide muudatused](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="e0728-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="e0728-104">**Krediitkaardi numbritega seotud DLP**</span><span class="sxs-lookup"><span data-stu-id="e0728-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="e0728-105">Kas teil on probleeme **andmete kaotsimineku vältimisega (DLP)** , mis ei tööta **krediitkaardi numbrit** sisaldava sisuga, kui kasutate O365 DLP tundliku teabe tüüpi?</span><span class="sxs-lookup"><span data-stu-id="e0728-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="e0728-106">Kui jah, siis veenduge, et teie sisu sisaldaks vajalikku teavet, et käivitada DLP poliitika, kui seda hinnatakse.</span><span class="sxs-lookup"><span data-stu-id="e0728-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="e0728-107">Näiteks, kui teie **krediitkaardi poliitika** on konfigureeritud 85%, hinnatakse ja see tuleb reegli käivitamiseks tuvastada järgmiselt.</span><span class="sxs-lookup"><span data-stu-id="e0728-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="e0728-108">**[Vorming:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 numbrit, mis võivad olla vormindatud või vormindamata (dddddddddddddddd) ja peavad läbima Luhn testi.</span><span class="sxs-lookup"><span data-stu-id="e0728-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="e0728-109">**[Muster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Väga keerukas ja jõuline muster, mis tuvastab kogu maailmas kaarte, sh Visa, MasterCard, Discover Card, JCB, American Express, Kinkekaardid ja söökla kaardid.</span><span class="sxs-lookup"><span data-stu-id="e0728-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="e0728-110">**[Kontrollsumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Jah, Luhn kontrollsumma</span><span class="sxs-lookup"><span data-stu-id="e0728-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="e0728-111">**[Definitsioon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** DLP poliitika on 85% kindel, et see on tuvastanud seda tüüpi tundliku teabe, kui 300 märkide lähedusse jääb:</span><span class="sxs-lookup"><span data-stu-id="e0728-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="e0728-112">Funktsioon Func_credit_card otsib mustriga kattuvat sisu.</span><span class="sxs-lookup"><span data-stu-id="e0728-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="e0728-113">Kehtib mõni järgmistest.</span><span class="sxs-lookup"><span data-stu-id="e0728-113">One of the following is true:</span></span>

  - <span data-ttu-id="e0728-114">Leitakse Keyword_cc_verification märksõna.</span><span class="sxs-lookup"><span data-stu-id="e0728-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="e0728-115">Leitakse Keyword_cc_name märksõna</span><span class="sxs-lookup"><span data-stu-id="e0728-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="e0728-116">Funktsioon Func_expiration_date leiab kuupäeva õigel kuupäevavorming.</span><span class="sxs-lookup"><span data-stu-id="e0728-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="e0728-117">Kontrollsumma läbib</span><span class="sxs-lookup"><span data-stu-id="e0728-117">The checksum passes</span></span>

    <span data-ttu-id="e0728-118">Näiteks käivitatakse järgmise valimi korral DLP krediitkaardi numbri poliitika.</span><span class="sxs-lookup"><span data-stu-id="e0728-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="e0728-119">Visa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="e0728-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="e0728-120">Aegub: 2/2009</span><span class="sxs-lookup"><span data-stu-id="e0728-120">Expires: 2/2009</span></span>

<span data-ttu-id="e0728-121">Lisateavet selle kohta, mida on vaja teie **teabesisu tuvastamiseks** , leiate selle artikli jaotisest [Kuidas tundlikud andmetüübid välja näevad?](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="e0728-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span></span>
  
<span data-ttu-id="e0728-122">Mõne muu sisseehitatud tundliku teabe tüübi abil leiate lisateavet selle kohta, mida on vaja muude tüüpide jaoks: [millist tüüpi tundlikud teabe tüübid otsivad](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="e0728-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  