---
title: DLP võib vajada kohandatud tüüpi
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 87fcb5c3cc9ccd525265097b66d9d9b3a85c5feb
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977266"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="47d55-102">DLP võib vajada kohandatud tüüpi</span><span class="sxs-lookup"><span data-stu-id="47d55-102">DLP might need a custom type</span></span>

<span data-ttu-id="47d55-103">**Oluline**: nendel enneolematul ajal me võtame meetmeid, et tagada SharePoint Online ' i ja OneDrive teenused on väga kättesaadavad-Palun külastage [SharePoint Online ajutised funktsiooni kohandused](https://aka.ms/ODSPAdjustments) lisateabe saamiseks.</span><span class="sxs-lookup"><span data-stu-id="47d55-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="47d55-104">**DLP võib nõuda kohandatud teabe tüüp**</span><span class="sxs-lookup"><span data-stu-id="47d55-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="47d55-105">Andmete kadu vältimine (DLP) poliitika, saate tuvastada ja kaitsta tundliku loomuga andmeid oma organisatsioonis.</span><span class="sxs-lookup"><span data-stu-id="47d55-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="47d55-106">Mõnel juhul peate võib-olla looma oma **kohandatud** tundliku teabe tüübi, et kaitsta oma organisatsiooni andmeid.</span><span class="sxs-lookup"><span data-stu-id="47d55-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="47d55-107">Näiteks võib teie organisatsioonil olla vaja tuvastada ja kaitsta töötaja ID-sid või muid andmeid mõnes teie organisatsioonile eriomas vormingus. Kui jah, lugege lisateabe saamiseks järgmisi artikleid.</span><span class="sxs-lookup"><span data-stu-id="47d55-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="47d55-108">**Sisseehitatud tundliku teabe tüübi kohandamine**</span><span class="sxs-lookup"><span data-stu-id="47d55-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="47d55-109">Kui sisseehitatud tundlik teabetüüp rahuldaks teie vajadused vaid mõne tweaks, saate [kohandada sisseehitatud tundliku teabe tüüpi](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="47d55-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="47d55-110">Näiteks saate märksõnu lisada või eemaldada või lisada või eemaldada täiendavaid tõendeid (nt kuupäev või aadress).</span><span class="sxs-lookup"><span data-stu-id="47d55-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="47d55-111">**Kohandatud tundliku teabe tüübi loomine**</span><span class="sxs-lookup"><span data-stu-id="47d55-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="47d55-112">Kuid kui teil on vaja tuvastada ja kaitsta erinevat tüüpi tundlikku teavet, saate [luua kohandatud tundliku teabe tüübi](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) Security & vastavuse keskus UI.</span><span class="sxs-lookup"><span data-stu-id="47d55-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="47d55-113">**Luua kohandatud tundliku teabe tüüp Security & vastavuse keskus PowerShelli**</span><span class="sxs-lookup"><span data-stu-id="47d55-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="47d55-114">Lõpuks, kui UI ei paku kõik vajalikud suvandid, saate [luua kohandatud tundliku teabe tüüp Security & vastavuse keskus PowerShelli](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="47d55-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="47d55-115">Alustades XML-failist, saate kasutada igat saadaolevat suvandit.</span><span class="sxs-lookup"><span data-stu-id="47d55-115">By starting with an XML file, you can use every option available.</span></span>
