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
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403739"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="0d8c5-102">Töövoog ei käivitu</span><span class="sxs-lookup"><span data-stu-id="0d8c5-102">Workflow is not starting</span></span>

- <span data-ttu-id="0d8c5-103">SharePoint 2010 ja SharePoint 2013 töövood ei käivitu.</span><span class="sxs-lookup"><span data-stu-id="0d8c5-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="0d8c5-104">Kui töövoog ei käivitu, võib ilmneda ajutine teenuseprobleem, mille korral kasutajad võivad töövoo edenemise korral ilmneda aeg-ajalt viivitusi.</span><span class="sxs-lookup"><span data-stu-id="0d8c5-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="0d8c5-105">Kontrollige [teenuse seisundi armatuurlauda,](https://admin.microsoft.com/AdminPortal/Home/servicehealth) et näha, kas teie ettevõtet mõjutab.</span><span class="sxs-lookup"><span data-stu-id="0d8c5-105">Check the [Service Health Dashboard](https://admin.microsoft.com/AdminPortal/Home/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="0d8c5-106">Kui sellest probleemist on möödunud rohkem kui 24 tundi, logige sisse tugiteenusepilet.</span><span class="sxs-lookup"><span data-stu-id="0d8c5-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="0d8c5-107">Paljudel juhtudel töötame juba lahenduse kallal.</span><span class="sxs-lookup"><span data-stu-id="0d8c5-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="0d8c5-108">Lahenduse lõpuleviimiseks andke meile vähemalt 24 tundi.</span><span class="sxs-lookup"><span data-stu-id="0d8c5-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="0d8c5-109">SharePoint 2010 töövood hilinevad käivitamisel.</span><span class="sxs-lookup"><span data-stu-id="0d8c5-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="0d8c5-110">See juhtub siis, kui töövoog käivitatakse suurtes pakettides.</span><span class="sxs-lookup"><span data-stu-id="0d8c5-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="0d8c5-111">(nt kui korraga lisatakse mitu üksust).</span><span class="sxs-lookup"><span data-stu-id="0d8c5-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="0d8c5-112">Töövood pole loodud reaalajas töötama, nii et viivitus on by-design käitumine.</span><span class="sxs-lookup"><span data-stu-id="0d8c5-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="0d8c5-113">Kui töövoog on keerukas laiendatav objekti märgistuskeel (XMOL), võib kompileerimine olla aeglane.</span><span class="sxs-lookup"><span data-stu-id="0d8c5-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="0d8c5-114">Vaadake [seda](https://support.microsoft.com//kb/3043697) artiklit.</span><span class="sxs-lookup"><span data-stu-id="0d8c5-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="0d8c5-115">Peaksite töövoogu lihtsustama või selle ümber kujundama Microsoft SharePoint 2013 töövooplatvormi tüübi abil.</span><span class="sxs-lookup"><span data-stu-id="0d8c5-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="0d8c5-116">Kui töövoo ajalugu on kasvanud suureks, võite soovida üksused likvideerida või luua uue ajalooloendi.</span><span class="sxs-lookup"><span data-stu-id="0d8c5-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="0d8c5-117">Lisateave: [Töövooajaloo likvideerimine](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="0d8c5-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="0d8c5-118">Seotud teemad</span><span class="sxs-lookup"><span data-stu-id="0d8c5-118">Related topics</span></span>
<span data-ttu-id="0d8c5-119">Kas soovite proovida Microsoft Flow'i SharePoint Online'is?</span><span class="sxs-lookup"><span data-stu-id="0d8c5-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="0d8c5-120">Voo loomine</span><span class="sxs-lookup"><span data-stu-id="0d8c5-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="0d8c5-121">SharePoint ja Flow</span><span class="sxs-lookup"><span data-stu-id="0d8c5-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
