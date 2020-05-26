---
title: 618 kalendri ühiskasutuse poliitika
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/26/2020
ms.locfileid: "44372995"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="7a055-102">Poliitika tõrge kalendri ühiskasutusse andmine</span><span class="sxs-lookup"><span data-stu-id="7a055-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="7a055-103">Tehke vastavalt oma olukorrale ühte järgmistest.</span><span class="sxs-lookup"><span data-stu-id="7a055-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="7a055-104">Kaugtöölaua PowerShelli abil ühendust Exchange Online ' i.</span><span class="sxs-lookup"><span data-stu-id="7a055-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="7a055-105">Lisateabe saamiseks vaadake [ühendamine Exchange Online ' i kaugtöölaua PowerShelli abil](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="7a055-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="7a055-106">Avage asutusesisese serveri Exchange Management shelli.</span><span class="sxs-lookup"><span data-stu-id="7a055-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="7a055-107">Määratlege ühiskasutuse poliitika, mis on määratud kasutajale.</span><span class="sxs-lookup"><span data-stu-id="7a055-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="7a055-108">Selleks käivitage järgmine käsk ja Märkus tagastatud poliitika:</span><span class="sxs-lookup"><span data-stu-id="7a055-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="7a055-109">Värskendage kasutaja ühiskasutuse poliitika.</span><span class="sxs-lookup"><span data-stu-id="7a055-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="7a055-110">Selleks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="7a055-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="7a055-111">Avage Exchange ' i halduskeskus.</span><span class="sxs-lookup"><span data-stu-id="7a055-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="7a055-112">Klõpsake **organisatsioonija**seejärel topeltklõpsake poliitika, mis on määratud kasutaja **eraldi ühiskasutus**.</span><span class="sxs-lookup"><span data-stu-id="7a055-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="7a055-113">See on poliitika, mis tagastati juhises 2.</span><span class="sxs-lookup"><span data-stu-id="7a055-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="7a055-114">Valige lehel ühiskasutuse reegel kalendri ühiskasutuse tase, mida soovite lubada jaotises **Määrake, millist teavet soovite jagada**; Klikkige nupul **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="7a055-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="7a055-115">Lisateabe saamiseks vaadake: ["poliitika ei luba anda õigusi sel tasemel ühe või mitme adressaadi (te)" tõrge, kui kasutaja proovib jagada kalendrit](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="7a055-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
