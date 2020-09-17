---
title: Töövoog ei käivitu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794763"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="26f6c-102">Töövoog ei käivitu</span><span class="sxs-lookup"><span data-stu-id="26f6c-102">Workflow is not starting</span></span>

- <span data-ttu-id="26f6c-103">SharePoint 2010 ja SharePoint 2013 töövood ei käivitu.</span><span class="sxs-lookup"><span data-stu-id="26f6c-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="26f6c-104">Kui teie töövoog ei käivitu, võib olla ajutine teenuse probleem, mille korral võivad kasutajad töövoo edenemise korral esineda ajutisi viivitusi.</span><span class="sxs-lookup"><span data-stu-id="26f6c-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="26f6c-105">Kontrollige [teenuse tervise armatuurlauda](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) , et näha, kas teie ettevõte on mõjutatud.</span><span class="sxs-lookup"><span data-stu-id="26f6c-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="26f6c-106">Kui sellest probleemist on möödunud rohkem kui 24 tundi, logige sisse tugiteenuse pilet.</span><span class="sxs-lookup"><span data-stu-id="26f6c-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="26f6c-107">Paljudel juhtudel oleme juba lahendusega töötanud.</span><span class="sxs-lookup"><span data-stu-id="26f6c-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="26f6c-108">Lahenduse lõpetamiseks andke meile vähemalt 24 tundi.</span><span class="sxs-lookup"><span data-stu-id="26f6c-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="26f6c-109">SharePointi 2010 töövood on avakuval edasi lükatud.</span><span class="sxs-lookup"><span data-stu-id="26f6c-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="26f6c-110">See juhtub siis, kui töövoog käivitatakse suurte partiidena.</span><span class="sxs-lookup"><span data-stu-id="26f6c-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="26f6c-111">(näiteks kui korraga lisatakse mitu üksust).</span><span class="sxs-lookup"><span data-stu-id="26f6c-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="26f6c-112">Töövood pole loodud reaalajas töötamiseks, nii et viivitus on disainitud käitumist.</span><span class="sxs-lookup"><span data-stu-id="26f6c-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="26f6c-113">Kui töövoog on keerukas Extensible Object Markup Language (XMOL), võib Kompileerimine olla aeglane.</span><span class="sxs-lookup"><span data-stu-id="26f6c-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="26f6c-114">Vaadake [seda](https://support.microsoft.com//kb/3043697) artiklit.</span><span class="sxs-lookup"><span data-stu-id="26f6c-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="26f6c-115">Peate töövoo lihtsustama või selle ümber kujundama Microsoft SharePoint 2013 töövoo platvormi tüübi abil.</span><span class="sxs-lookup"><span data-stu-id="26f6c-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="26f6c-116">Kui teie töövoo ajalugu on suureks kasvanud, soovite võib-olla üksused likvideerida või luua uue ajaloo loendi.</span><span class="sxs-lookup"><span data-stu-id="26f6c-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="26f6c-117">Lisateave: [töövoo ajaloo likvideerimine](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="26f6c-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="26f6c-118">Seotud teemad</span><span class="sxs-lookup"><span data-stu-id="26f6c-118">Related topics</span></span>
<span data-ttu-id="26f6c-119">Kas soovite proovida Microsoft Flow SharePoint Online ' is?</span><span class="sxs-lookup"><span data-stu-id="26f6c-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="26f6c-120">Voo loomine</span><span class="sxs-lookup"><span data-stu-id="26f6c-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="26f6c-121">SharePoint ja voog</span><span class="sxs-lookup"><span data-stu-id="26f6c-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


