---
title: Päevane e-posti limiit on ületatud. Töövoog on peatatud.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731559"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="a0b4d-103">Päevane e-posti limiit on ületatud.</span><span class="sxs-lookup"><span data-stu-id="a0b4d-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="a0b4d-104">Töövoog on peatatud.</span><span class="sxs-lookup"><span data-stu-id="a0b4d-104">Workflow is suspended.</span></span>

<span data-ttu-id="a0b4d-105">Selle tõrke võib vastu võtta järgmistel juhtudel.</span><span class="sxs-lookup"><span data-stu-id="a0b4d-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="a0b4d-106">Teil on SharePoint Online ' is töövoog, mis kasutab SharePoint 2010 või SharePoint 2013 töövoo platvormi tüüpi.</span><span class="sxs-lookup"><span data-stu-id="a0b4d-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="a0b4d-107">Töövoog on konfigureeritud saatma kohandatud meilisõnumeid rohkem kui 200 kasutajale korraga, üle 10 000 adressaadi päevas või rohkem kui 30 sõnumit minutis.</span><span class="sxs-lookup"><span data-stu-id="a0b4d-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="a0b4d-108">Töövoo käivitamisel meilisõnumit ei saadeta ja te märkate järgmist käitumist.</span><span class="sxs-lookup"><span data-stu-id="a0b4d-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="a0b4d-109">SharePointi 2013 platvormi tüübiga töövoo korral sirvige lehe **töövoo olek** kaudu.</span><span class="sxs-lookup"><span data-stu-id="a0b4d-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="a0b4d-110">Töövoo oleku lehel on **sisemine olekuks** seatud **Alustatud**ja teabe jutumull **ei saa adressaadile saata**.</span><span class="sxs-lookup"><span data-stu-id="a0b4d-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="a0b4d-111">Selle probleemi lahendamiseks konfigureerige oma töövoog meilisõnumite saatmiseks, ületamata seejuures [Exchange Online ' i saatja limiite](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="a0b4d-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="a0b4d-112">Näiteks saate töövoos kasutada pausi, saata meilisõnumi Microsoft 365 rühmale, levirühma või e-posti loaga turberühma või saata sõnumi korraga vähem kui 200 adressaadile.</span><span class="sxs-lookup"><span data-stu-id="a0b4d-112">For example, use a pause in the workflow, send the email to a Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="a0b4d-113">Lisateavet leiate järgmisest [artiklist](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="a0b4d-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="a0b4d-114">Seotud teemad</span><span class="sxs-lookup"><span data-stu-id="a0b4d-114">Related topics</span></span>
- [<span data-ttu-id="a0b4d-115">Voo loomine</span><span class="sxs-lookup"><span data-stu-id="a0b4d-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="a0b4d-116">SharePoint ja voog</span><span class="sxs-lookup"><span data-stu-id="a0b4d-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 