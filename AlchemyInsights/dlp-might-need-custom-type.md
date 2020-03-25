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
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932654"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="0e3c2-102">DLP võib vajada kohandatud tüüpi</span><span class="sxs-lookup"><span data-stu-id="0e3c2-102">DLP might need a custom type</span></span>

<span data-ttu-id="0e3c2-103">**Oluline**: paljud SharePoint Online ' i ja OneDrive kliendid käivitada Business kriitilised rakendused teenuse, mis töötavad taustal.</span><span class="sxs-lookup"><span data-stu-id="0e3c2-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="0e3c2-104">Nende hulka kuuluvad sisu migratsioon, andmete kadu vältimine (DLP) ja backup lahendused.</span><span class="sxs-lookup"><span data-stu-id="0e3c2-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="0e3c2-105">Nendel enneolematul ajal me võtame meetmeid, et tagada SharePoint Online ' i ja OneDrive teenused on väga kättesaadav ja usaldusväärne oma kasutajatele, kes sõltuvad teenuse rohkem kui kunagi varem kaugtöö stsenaariume.</span><span class="sxs-lookup"><span data-stu-id="0e3c2-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="0e3c2-106">Selle eesmärgi toetuseks oleme rakendanud ranget ahendamise piiranguid taustal olevatele rakendustele (migratsioon, DLP ja backup lahendused) tööpäeval päeva jooksul.</span><span class="sxs-lookup"><span data-stu-id="0e3c2-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="0e3c2-107">Te peaksite ootama, et need rakendused saavutavad nende aegade jooksul väga piiratud läbilaskevõime.</span><span class="sxs-lookup"><span data-stu-id="0e3c2-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="0e3c2-108">Aga, õhtuti ja nädalavahetusel tundi piirkonna, teenus on valmis töötlema oluliselt suurem hulk taotlusi taustal apps.</span><span class="sxs-lookup"><span data-stu-id="0e3c2-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="0e3c2-109">**DLP võib nõuda kohandatud teabe tüüp**</span><span class="sxs-lookup"><span data-stu-id="0e3c2-109">**DLP may require a custom information type**</span></span>

<span data-ttu-id="0e3c2-110">Andmete kadu vältimine (DLP) poliitika, saate tuvastada ja kaitsta tundliku loomuga andmeid oma organisatsioonis.</span><span class="sxs-lookup"><span data-stu-id="0e3c2-110">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="0e3c2-111">Mõnel juhul peate võib-olla looma oma **kohandatud** tundliku teabe tüübi, et kaitsta oma organisatsiooni andmeid.</span><span class="sxs-lookup"><span data-stu-id="0e3c2-111">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="0e3c2-112">Näiteks võib teie organisatsioonil olla vaja tuvastada ja kaitsta töötaja ID-sid või muid andmeid mõnes teie organisatsioonile eriomas vormingus. Kui jah, lugege lisateabe saamiseks järgmisi artikleid.</span><span class="sxs-lookup"><span data-stu-id="0e3c2-112">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="0e3c2-113">**Sisseehitatud tundliku teabe tüübi kohandamine**</span><span class="sxs-lookup"><span data-stu-id="0e3c2-113">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="0e3c2-114">Kui sisseehitatud tundlik teabetüüp rahuldaks teie vajadused vaid mõne tweaks, saate [kohandada sisseehitatud tundliku teabe tüüpi](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="0e3c2-114">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="0e3c2-115">Näiteks saate märksõnu lisada või eemaldada või lisada või eemaldada täiendavaid tõendeid (nt kuupäev või aadress).</span><span class="sxs-lookup"><span data-stu-id="0e3c2-115">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="0e3c2-116">**Kohandatud tundliku teabe tüübi loomine**</span><span class="sxs-lookup"><span data-stu-id="0e3c2-116">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="0e3c2-117">Kuid kui teil on vaja tuvastada ja kaitsta erinevat tüüpi tundlikku teavet, saate [luua kohandatud tundliku teabe tüübi](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) Security & vastavuse keskus UI.</span><span class="sxs-lookup"><span data-stu-id="0e3c2-117">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="0e3c2-118">**Luua kohandatud tundliku teabe tüüp Security & vastavuse keskus PowerShelli**</span><span class="sxs-lookup"><span data-stu-id="0e3c2-118">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="0e3c2-119">Lõpuks, kui UI ei paku kõik vajalikud suvandid, saate [luua kohandatud tundliku teabe tüüp Security & vastavuse keskus PowerShelli](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="0e3c2-119">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="0e3c2-120">Alustades XML-failist, saate kasutada igat saadaolevat suvandit.</span><span class="sxs-lookup"><span data-stu-id="0e3c2-120">By starting with an XML file, you can use every option available.</span></span>
