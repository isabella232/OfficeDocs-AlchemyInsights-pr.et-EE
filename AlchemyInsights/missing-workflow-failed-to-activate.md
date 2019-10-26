---
title: Töövoo puudub aktiveerimine nurjus
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: f03d7e1441465050c4b0608f4100f217b183d2e2
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/25/2019
ms.locfileid: "36753792"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="0b3e2-102">Töövoo puudub aktiveerimine nurjus</span><span class="sxs-lookup"><span data-stu-id="0b3e2-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="0b3e2-103">Microsoft SharePointi saidikogumi, ei saa lisada globaalselt korduvkasutatav töövoog (nt "kinnitamine-SharePoint 2010") loendisse või teeki.</span><span class="sxs-lookup"><span data-stu-id="0b3e2-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="0b3e2-104">Selle probleemi lahendamiseks toimige järgmiselt.</span><span class="sxs-lookup"><span data-stu-id="0b3e2-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="0b3e2-105">Avage saidikogumi juursait SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="0b3e2-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="0b3e2-106">Valige jaotises **saidi objektid** **töövoogude**.</span><span class="sxs-lookup"><span data-stu-id="0b3e2-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="0b3e2-107">Valige lindi **töövoogude** **Uus** jaotis **korduvkasutatav töövoog**.</span><span class="sxs-lookup"><span data-stu-id="0b3e2-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="0b3e2-108">Sisestage vormil **Loo korduvkasutatav töövoog** nimi \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="0b3e2-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="0b3e2-109">**Platvormi tüüp**, klõpsake **SharePoint 2010 töövooja**seejärel klõpsake nuppu **OK**.</span><span class="sxs-lookup"><span data-stu-id="0b3e2-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="0b3e2-110">**Töövoo** lindi jaotises **Salvesta** , valige **Avalda**.</span><span class="sxs-lookup"><span data-stu-id="0b3e2-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="0b3e2-111">**Töövoo** lindi jaotises **Halda** valige **Avalda globaalselt**.</span><span class="sxs-lookup"><span data-stu-id="0b3e2-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="0b3e2-112">Valige kuvatavas kinnitusdialoogiboksis nupp **OK**.</span><span class="sxs-lookup"><span data-stu-id="0b3e2-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="0b3e2-113">Veebibrauseri, leidke saidikogumi root kodulehel ja seejärel juurdepääsu **saidi sätted** \> **saidikogumi funktsioonid**.</span><span class="sxs-lookup"><span data-stu-id="0b3e2-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="0b3e2-114">Seejärel lülitage **töövoogude** funktsioon:</span><span class="sxs-lookup"><span data-stu-id="0b3e2-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="0b3e2-115">· Kui funktsioon on *aktiveeritud* , klõpsake nuppu **Desaktiveeri** ja seejärel nuppu **Aktiveeri**.</span><span class="sxs-lookup"><span data-stu-id="0b3e2-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="0b3e2-116">· Kui funktsioon on *desaktiveeritud* , klõpsake nuppu **Aktiveeri**.</span><span class="sxs-lookup"><span data-stu-id="0b3e2-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="0b3e2-117">Lisateabe saamiseks lugege järgmist [artiklit](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="0b3e2-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

