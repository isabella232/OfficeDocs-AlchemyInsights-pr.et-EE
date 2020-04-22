---
title: Töövoog ei käivitatav
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 941e6349c98278a1a8cdac77457ec1cc72cdef8b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766093"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="1c63c-102">Töövoog ei käivitatav</span><span class="sxs-lookup"><span data-stu-id="1c63c-102">Workflow is not starting</span></span>

- <span data-ttu-id="1c63c-103">SharePoint 2010 ja SharePoint 2013 töövoogude ei käivitamata.</span><span class="sxs-lookup"><span data-stu-id="1c63c-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="1c63c-104">Kui teie töövoog ei käivitust, võib olla ajutine teenuse probleem, kus kasutajad võivad kogeda vahelduva viivitusi töövoo edenemise.</span><span class="sxs-lookup"><span data-stu-id="1c63c-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="1c63c-105">Kontrollige [teenuse tervise armatuurlauda](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) , et näha, kas teie organisatsioon on mõjutatud.</span><span class="sxs-lookup"><span data-stu-id="1c63c-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="1c63c-106">Kui teil on möödunud rohkem kui 24 tundi pärast seda, kui te esimest korda seda probleemi, Palun logige tugiteenuse pilet.</span><span class="sxs-lookup"><span data-stu-id="1c63c-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="1c63c-107">Paljudel juhtudel oleme juba lahenduse kallal töötanud.</span><span class="sxs-lookup"><span data-stu-id="1c63c-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="1c63c-108">Palun andke meile vähemalt 24 tundi, et lahendus lõpule viia.</span><span class="sxs-lookup"><span data-stu-id="1c63c-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="1c63c-109">SharePoint 2010 töövood viivitusega käivitamisel.</span><span class="sxs-lookup"><span data-stu-id="1c63c-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="1c63c-110">See juhtub, kui töövoog käivitatakse suur partiide.</span><span class="sxs-lookup"><span data-stu-id="1c63c-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="1c63c-111">(näiteks kui korraga lisatakse mitu üksust).</span><span class="sxs-lookup"><span data-stu-id="1c63c-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="1c63c-112">Töövoogude ei ole mõeldud töötama reaalajas, nii viivitus on-Design käitumist.</span><span class="sxs-lookup"><span data-stu-id="1c63c-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="1c63c-113">Kui töövoog on keerukas laiendatav objekti märgistuskeel (XMOL), võib Kompileerimine olla aeglane.</span><span class="sxs-lookup"><span data-stu-id="1c63c-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="1c63c-114">Vaadake [seda](https://support.microsoft.com//kb/3043697) artiklit.</span><span class="sxs-lookup"><span data-stu-id="1c63c-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="1c63c-115">Töövoogu tuleks lihtsustada või selle ümber kujundada, kasutades Microsoft SharePoint 2013 töövoo platvormi tüüp.</span><span class="sxs-lookup"><span data-stu-id="1c63c-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="1c63c-116">Kui teie töövoo ajalugu on kasvanud suureks, võite soovida üksused puhastada või luua uue ajalooloendi.</span><span class="sxs-lookup"><span data-stu-id="1c63c-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="1c63c-117">Lisateave: [Likvideeri töövoo ajalugu](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="1c63c-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="1c63c-118">Seotud teemad</span><span class="sxs-lookup"><span data-stu-id="1c63c-118">Related topics</span></span>
<span data-ttu-id="1c63c-119">Soovite proovida Microsoft Flow SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="1c63c-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="1c63c-120">Voo loomine</span><span class="sxs-lookup"><span data-stu-id="1c63c-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="1c63c-121">SharePointi ja voog</span><span class="sxs-lookup"><span data-stu-id="1c63c-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


