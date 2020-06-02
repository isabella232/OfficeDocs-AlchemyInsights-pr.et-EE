---
title: DLP võib vajada kohandatud tüüpi
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1ec8959a479f1a8f7bfcffb55f440e8c4ab435fb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507510"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="5058a-102">DLP võib vajada kohandatud tüüpi</span><span class="sxs-lookup"><span data-stu-id="5058a-102">DLP might need a custom type</span></span>

<span data-ttu-id="5058a-103">**Tähtis**! Nende enneolematude aegade jooksul võtame kasutusele meetmed, et säilitada SharePoint Online’i ja OneDrive’i teenuste hea kättesadavus. Lisateabe saamiseks vaadake teemat [SharePoint Online’i ajutised funktsioonide muudatused](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="5058a-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="5058a-104">**DLP võib nõuda kohandatud teabe tüüp**</span><span class="sxs-lookup"><span data-stu-id="5058a-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="5058a-105">Andmete kadu vältimine (DLP) poliitika, saate tuvastada ja kaitsta tundliku loomuga andmeid oma organisatsioonis.</span><span class="sxs-lookup"><span data-stu-id="5058a-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="5058a-106">Mõnel juhul peate võib-olla looma oma **kohandatud** tundliku teabe tüübi, et kaitsta oma organisatsiooni andmeid.</span><span class="sxs-lookup"><span data-stu-id="5058a-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="5058a-107">Näiteks võib teie organisatsioonil olla vaja tuvastada ja kaitsta töötaja ID-sid või muid andmeid mõnes teie organisatsioonile eriomas vormingus. Kui jah, lugege lisateabe saamiseks järgmisi artikleid.</span><span class="sxs-lookup"><span data-stu-id="5058a-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="5058a-108">**Sisseehitatud tundliku teabe tüübi kohandamine**</span><span class="sxs-lookup"><span data-stu-id="5058a-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="5058a-109">Kui sisseehitatud tundlik teabetüüp rahuldaks teie vajadused vaid mõne tweaks, saate [kohandada sisseehitatud tundliku teabe tüüpi](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="5058a-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="5058a-110">Näiteks saate märksõnu lisada või eemaldada või lisada või eemaldada täiendavaid tõendeid (nt kuupäev või aadress).</span><span class="sxs-lookup"><span data-stu-id="5058a-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="5058a-111">**Kohandatud tundliku teabe tüübi loomine**</span><span class="sxs-lookup"><span data-stu-id="5058a-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="5058a-112">Kuid kui teil on vaja tuvastada ja kaitsta erinevat tüüpi tundlikku teavet, saate [luua kohandatud tundliku teabe tüübi](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) Security & vastavuse keskus UI.</span><span class="sxs-lookup"><span data-stu-id="5058a-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="5058a-113">**Luua kohandatud tundliku teabe tüüp Security & vastavuse keskus PowerShelli**</span><span class="sxs-lookup"><span data-stu-id="5058a-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="5058a-114">Lõpuks, kui UI ei paku kõik vajalikud suvandid, saate [luua kohandatud tundliku teabe tüüp Security & vastavuse keskus PowerShelli](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="5058a-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="5058a-115">Alustades XML-failist, saate kasutada igat saadaolevat suvandit.</span><span class="sxs-lookup"><span data-stu-id="5058a-115">By starting with an XML file, you can use every option available.</span></span>
