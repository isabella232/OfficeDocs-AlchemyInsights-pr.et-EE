---
title: DLP võib vajada kohandatud tüüpi
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 72b16d437f97de27cbdc364f022c3e2059b31ef0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712180"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="0ee55-102">DLP võib vajada kohandatud tüüpi</span><span class="sxs-lookup"><span data-stu-id="0ee55-102">DLP might need a custom type</span></span>

<span data-ttu-id="0ee55-103">**Tähtis**! Nende enneolematude aegade jooksul võtame kasutusele meetmed, et säilitada SharePoint Online’i ja OneDrive’i teenuste hea kättesadavus. Lisateabe saamiseks vaadake teemat [SharePoint Online’i ajutised funktsioonide muudatused](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="0ee55-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="0ee55-104">**DLP võib nõuda kohandatud teabe tüüpi**</span><span class="sxs-lookup"><span data-stu-id="0ee55-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="0ee55-105">Andmete kaotsimineku vältimise (DLP) poliitika abil saate oma ettevõttes tuvastada ja kaitsta tundlikke andmeid.</span><span class="sxs-lookup"><span data-stu-id="0ee55-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="0ee55-106">Mõne stsenaariumi korral peate oma asutuse andmete kaitsmiseks võib-olla looma **kohandatud** tundliku teabe tüübi.</span><span class="sxs-lookup"><span data-stu-id="0ee55-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="0ee55-107">Näiteks võib teie asutusel olla vaja tuvastada ja kaitsta töötajate ID-sid või muid andmeid mõnes teie organisatsioonis olevas vormingus. Kui jah, leiate lisateavet järgmistest artiklitest.</span><span class="sxs-lookup"><span data-stu-id="0ee55-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="0ee55-108">**Sisemise tundliku teabe tüübi kohandamine**</span><span class="sxs-lookup"><span data-stu-id="0ee55-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="0ee55-109">Kui sisseehitatud tundliku teabe tüüp vastab teie vajadustele vaid mõne tweaks, saate [kohandada sisseehitatud tundliku teabe tüüpi](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="0ee55-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="0ee55-110">Näiteks saate märksõnu lisada või eemaldada või lisada või eemaldada tõendusmaterjale (nt kuupäev või aadress).</span><span class="sxs-lookup"><span data-stu-id="0ee55-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="0ee55-111">**Kohandatud tundliku teabe tüübi loomine**</span><span class="sxs-lookup"><span data-stu-id="0ee55-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="0ee55-112">Kui teil on vaja tuvastada ja kaitsta erinevat tüüpi tundlikku teavet, saate luua turbe & nõuetele vastavuse keskuse KASUTAJALIIDESes [kohandatud tundliku teabe tüübi](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) .</span><span class="sxs-lookup"><span data-stu-id="0ee55-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="0ee55-113">**Kohandatud tundliku teabe tüübi loomine turbe & nõuetele vastavuse keskuses PowerShell**</span><span class="sxs-lookup"><span data-stu-id="0ee55-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="0ee55-114">Kui kasutajaliides ei paku kõiki vajalikke suvandeid, saate [turvalisuse & täitmise keskuses PowerShell luua kohandatud tundliku teabe tüübi](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="0ee55-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="0ee55-115">Alustades XML-failiga, saate kasutada kõiki saadaolevaid võimalusi.</span><span class="sxs-lookup"><span data-stu-id="0ee55-115">By starting with an XML file, you can use every option available.</span></span>
