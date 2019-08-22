---
title: Igapäevase e-posti piirmäär on ületatud. Töövoog on peatatud.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: e3fbcd5bfc279847cfb39140c3689f5433b61509
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36514444"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="c6dae-103">Igapäevase e-posti on ületatud.</span><span class="sxs-lookup"><span data-stu-id="c6dae-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="c6dae-104">Töövoog on peatatud.</span><span class="sxs-lookup"><span data-stu-id="c6dae-104">Workflow is suspended.</span></span>

<span data-ttu-id="c6dae-105">See tõrge võib vastu võtta järgmistel juhtudel:</span><span class="sxs-lookup"><span data-stu-id="c6dae-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="c6dae-106">Olete töövoo SharePoint Online, mis kasutab SharePoint 2010 või SharePointi 2013 töövoo platvormi tüüp.</span><span class="sxs-lookup"><span data-stu-id="c6dae-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="c6dae-107">Töövoog on konfigureeritud kohandatud e-kirja saatmiseks üle 200 kasutajatele korraga, üle 10 000 adressaati päevas või üle 30 sõnumites minutis.</span><span class="sxs-lookup"><span data-stu-id="c6dae-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="c6dae-108">Töövoo käivitamisel saadetakse e-kiri ja märkate järgmist käitumist:</span><span class="sxs-lookup"><span data-stu-id="c6dae-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="c6dae-109">Kasutades SharePointi 2013 platvormi tüüp töövoo sirvite **Töövoo oleku** lehel.</span><span class="sxs-lookup"><span data-stu-id="c6dae-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="c6dae-110">Lehe Töövoo olek **Staatusest** on seatud **Alustatud**ja teabe õhupalli kuvab **ei saa adressaadile saata**.</span><span class="sxs-lookup"><span data-stu-id="c6dae-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="c6dae-111">Selle probleemi lahendamiseks konfigureerige oma töövoo saata e-kirju [Exchange Online'i saatja piire](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)ületamata.</span><span class="sxs-lookup"><span data-stu-id="c6dae-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="c6dae-112">Näiteks kasutada töövoo pausi, saada email Office 365 rühma, leviloendi või e-posti lubatud turberühma või saata sõnum alla 200 adressaadile korraga.</span><span class="sxs-lookup"><span data-stu-id="c6dae-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="c6dae-113">Lisateabe saamiseks vaadake [artikli](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="c6dae-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="c6dae-114">Seotud teemad</span><span class="sxs-lookup"><span data-stu-id="c6dae-114">Related topics</span></span>
- [<span data-ttu-id="c6dae-115">Luua voolu</span><span class="sxs-lookup"><span data-stu-id="c6dae-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="c6dae-116">SharePoint ja voolu</span><span class="sxs-lookup"><span data-stu-id="c6dae-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 