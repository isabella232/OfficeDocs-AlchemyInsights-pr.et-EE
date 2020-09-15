---
title: DLP reegel US/UK passi number ei tööta
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679220"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="0801b-102">Probleemid DLP-US/UK Passporti numbritega</span><span class="sxs-lookup"><span data-stu-id="0801b-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="0801b-103">**Tähtis**! Nende enneolematude aegade jooksul võtame kasutusele meetmed, et säilitada SharePoint Online’i ja OneDrive’i teenuste hea kättesadavus. Lisateabe saamiseks vaadake teemat [SharePoint Online’i ajutised funktsioonide muudatused](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="0801b-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="0801b-104">**DLP probleemid US/UK Passporti numbritega**</span><span class="sxs-lookup"><span data-stu-id="0801b-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="0801b-105">Kas teil on probleeme **andmete kaotsimineku vältimisega (DLP)** , mis ei tööta, kui teil on DLP tundliku teabe tüüpi O365 kasutamisel **US/UK Passporti numbrit** sisaldav sisu?</span><span class="sxs-lookup"><span data-stu-id="0801b-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="0801b-106">Kui jah, siis veenduge, et teie sisu sisaldaks vajalikku teavet selle kohta, mida DLP poliitika selle hindamisel otsib.</span><span class="sxs-lookup"><span data-stu-id="0801b-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="0801b-107">Näiteks kui **US/UK Passporti kood** , mis on konfigureeritud 75% usalduse tasemega, hinnatakse ja seda tuleb reegli käivitamiseks tuvastada</span><span class="sxs-lookup"><span data-stu-id="0801b-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="0801b-108">**[Vorming:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Üheksa numbrit</span><span class="sxs-lookup"><span data-stu-id="0801b-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nine digits</span></span>

- <span data-ttu-id="0801b-109">**[Muster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Üheksa järjestikust numbrit</span><span class="sxs-lookup"><span data-stu-id="0801b-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="0801b-110">**[Kontrollsumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ei, pole kontrollsummat</span><span class="sxs-lookup"><span data-stu-id="0801b-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="0801b-111">**[Definitsioon:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** DLP poliitika on 75% kindel, et see on tuvastanud seda tüüpi tundliku teabe, kui 300 märkide lähedusse jääb:</span><span class="sxs-lookup"><span data-stu-id="0801b-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="0801b-112">Funktsioon Func_usa_uk_passport otsib mustriga kattuvat sisu.</span><span class="sxs-lookup"><span data-stu-id="0801b-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="0801b-113">Leitakse Keyword_passport märksõna.</span><span class="sxs-lookup"><span data-stu-id="0801b-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="0801b-114">Näiteks käivitab järgmine valim **USA/Ühendkuningriigi passi numbripoliitika** : USA passi number 123456789</span><span class="sxs-lookup"><span data-stu-id="0801b-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="0801b-115">Lisateavet selle kohta, mida on vaja teie sisu tuvastamiseks US/UK Passporti numbri kohta, leiate selle artikli jaotisest [mis on tundlikud ANDMETÜÜBID meie/Ühendkuningriigi passi numbri](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number) järgi.</span><span class="sxs-lookup"><span data-stu-id="0801b-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span></span>
  
<span data-ttu-id="0801b-116">Mõne muu sisseehitatud tundliku teabe tüübi abil leiate lisateavet selle kohta, mida on vaja muude tüüpide jaoks: [millist tüüpi tundlikud teabe tüübid otsivad](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="0801b-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  