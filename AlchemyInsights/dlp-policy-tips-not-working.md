---
title: DLP poliitika nõuanded ei tööta
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932582"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="0285f-102">DLP poliitika Näpunäide probleemid</span><span class="sxs-lookup"><span data-stu-id="0285f-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="0285f-103">**Oluline**: paljud SharePoint Online ' i ja OneDrive kliendid käivitada Business kriitilised rakendused teenuse, mis töötavad taustal.</span><span class="sxs-lookup"><span data-stu-id="0285f-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="0285f-104">Nende hulka kuuluvad sisu migratsioon, andmete kadu vältimine (DLP) ja backup lahendused.</span><span class="sxs-lookup"><span data-stu-id="0285f-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="0285f-105">Nendel enneolematul ajal me võtame meetmeid, et tagada SharePoint Online ' i ja OneDrive teenused on väga kättesaadav ja usaldusväärne oma kasutajatele, kes sõltuvad teenuse rohkem kui kunagi varem kaugtöö stsenaariume.</span><span class="sxs-lookup"><span data-stu-id="0285f-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="0285f-106">Selle eesmärgi toetuseks oleme rakendanud ranget ahendamise piiranguid taustal olevatele rakendustele (migratsioon, DLP ja backup lahendused) tööpäeval päeva jooksul.</span><span class="sxs-lookup"><span data-stu-id="0285f-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="0285f-107">Te peaksite ootama, et need rakendused saavutavad nende aegade jooksul väga piiratud läbilaskevõime.</span><span class="sxs-lookup"><span data-stu-id="0285f-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="0285f-108">Aga, õhtuti ja nädalavahetusel tundi piirkonna, teenus on valmis töötlema oluliselt suurem hulk taotlusi taustal apps.</span><span class="sxs-lookup"><span data-stu-id="0285f-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="0285f-109">**DLP poliitika nõuanded**</span><span class="sxs-lookup"><span data-stu-id="0285f-109">**DLP policy tips**</span></span>

<span data-ttu-id="0285f-110">**DLP poliitika**kasutamisel saavad kasutajad teavitada poliitika rikkumise **poliitika nõuanded**.</span><span class="sxs-lookup"><span data-stu-id="0285f-110">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="0285f-111">Administraatorid saate konfigureerida poliitikaspikrid testides oma DLP poliitika või kui poliitika on täielik jõustamine režiimis.</span><span class="sxs-lookup"><span data-stu-id="0285f-111">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="0285f-112">Poliitika näpunäited oma DLP poliitika turvalisuse ja vastavuse keskus täieliku jõustamise režiimis konfigureerimiseks toimige järgmiselt.</span><span class="sxs-lookup"><span data-stu-id="0285f-112">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="0285f-113">Veenduge, et poliitikaspikrid on **lubatud** DLP reegel, kasutades juhiseid [siin](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="0285f-113">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="0285f-114">Veenduge, et teie **sisu vastaks** [selles artiklis kirjeldatud](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)reegli käivitamiseks **nõutavale** .</span><span class="sxs-lookup"><span data-stu-id="0285f-114">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="0285f-115">Poliitikaspikrid kuvada nii OWA ja Outlook.</span><span class="sxs-lookup"><span data-stu-id="0285f-115">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="0285f-116">Siiski, kui kasutate **Outlook 2013 või uuem**, poliitikaspikrid kuvatakse ainult teatud tingimustel.</span><span class="sxs-lookup"><span data-stu-id="0285f-116">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="0285f-117">Need tingimused on loetletud siin: [toetatud tingimused Outlook 2013 või uuem poliitika näpunäited kuvamiseks](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span><span class="sxs-lookup"><span data-stu-id="0285f-117">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span></span>

<span data-ttu-id="0285f-118">DLP poliitika näpunäited kohta lisateabe saamiseks vaadake: [Kuva poliitikaspikrid DLP poliitika](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="0285f-118">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span></span>
  