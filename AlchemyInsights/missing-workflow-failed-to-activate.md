---
title: Töövoo puudub aktiveerimine nurjus
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 2598111005c219c398b63ca374e8e99348efc02c
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762097"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="91788-102">Töövoo puudub aktiveerimine nurjus</span><span class="sxs-lookup"><span data-stu-id="91788-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="91788-103">Microsoft SharePointi saidikogumi, ei saa lisada globaalselt korduvkasutatav töövoog (nt "kinnitamine-SharePoint 2010") loendisse või teeki.</span><span class="sxs-lookup"><span data-stu-id="91788-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="91788-104">Selle probleemi lahendamiseks toimige järgmiselt.</span><span class="sxs-lookup"><span data-stu-id="91788-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="91788-105">Avage saidikogumi juursait SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="91788-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="91788-106">Valige jaotises **saidi objektid** **töövoogude**.</span><span class="sxs-lookup"><span data-stu-id="91788-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="91788-107">Valige lindi **töövoogude** **Uus** jaotis **korduvkasutatav töövoog**.</span><span class="sxs-lookup"><span data-stu-id="91788-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="91788-108">Sisestage vormil **Loo korduvkasutatav töövoog** nimi \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="91788-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="91788-109">**Platvormi tüüp**, klõpsake **SharePoint 2010 töövooja**seejärel klõpsake nuppu **OK**.</span><span class="sxs-lookup"><span data-stu-id="91788-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="91788-110">**Töövoo** lindi jaotises **Salvesta** , valige **Avalda**.</span><span class="sxs-lookup"><span data-stu-id="91788-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="91788-111">**Töövoo** lindi jaotises **Halda** valige **Avalda globaalselt**.</span><span class="sxs-lookup"><span data-stu-id="91788-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="91788-112">Valige kuvatavas kinnitusdialoogiboksis nupp **OK**.</span><span class="sxs-lookup"><span data-stu-id="91788-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="91788-113">Veebibrauseri, leidke saidikogumi root kodulehel ja seejärel juurdepääsu **saidi sätted** \> **saidikogumi funktsioonid**.</span><span class="sxs-lookup"><span data-stu-id="91788-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="91788-114">Seejärel lülitage **töövoogude** funktsioon:</span><span class="sxs-lookup"><span data-stu-id="91788-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="91788-115">· Kui funktsioon on *aktiveeritud* , klõpsake nuppu **Desaktiveeri** ja seejärel nuppu **Aktiveeri**.</span><span class="sxs-lookup"><span data-stu-id="91788-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="91788-116">· Kui funktsioon on *desaktiveeritud* , klõpsake nuppu **Aktiveeri**.</span><span class="sxs-lookup"><span data-stu-id="91788-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="91788-117">Lisateabe saamiseks lugege järgmist [artiklit](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="91788-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

