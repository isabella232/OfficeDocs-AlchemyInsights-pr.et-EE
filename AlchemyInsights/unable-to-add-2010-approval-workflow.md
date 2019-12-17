---
title: Ei saa lisada 2010 kinnitamise töövoog
ms.author: pebaum
author: pebaum
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 11ba9bf04f826b0d7465a9a81a36c327e79f4d13
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049549"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="86b99-102">Ei saa lisada 2010 kinnitamise töövoog</span><span class="sxs-lookup"><span data-stu-id="86b99-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="86b99-103">Microsoft SharePointi saidikogumi, ei saa lisada globaalselt korduvkasutatav töövoog (nt "kinnitamine-SharePoint 2010") loendisse või teeki.</span><span class="sxs-lookup"><span data-stu-id="86b99-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="86b99-104">Selle probleemi lahendamiseks toimige järgmiselt.</span><span class="sxs-lookup"><span data-stu-id="86b99-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="86b99-105">Avage saidikogumi juursait SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="86b99-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="86b99-106">Valige jaotises **saidi objektid** **töövoogude**.</span><span class="sxs-lookup"><span data-stu-id="86b99-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="86b99-107">Valige lindi **töövoogude** **Uus** jaotis **korduvkasutatav töövoog**.</span><span class="sxs-lookup"><span data-stu-id="86b99-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="86b99-108">Sisestage vormil **Loo korduvkasutatav töövoog** nimi \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="86b99-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="86b99-109">**Platvormi tüüp**, klõpsake **SharePoint 2010 töövooja**seejärel klõpsake nuppu **OK**.</span><span class="sxs-lookup"><span data-stu-id="86b99-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="86b99-110">**Töövoo** lindi jaotises **Salvesta** , valige **Avalda**.</span><span class="sxs-lookup"><span data-stu-id="86b99-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="86b99-111">**Töövoo** lindi jaotises **Halda** valige **Avalda globaalselt**.</span><span class="sxs-lookup"><span data-stu-id="86b99-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="86b99-112">Valige kuvatavas kinnitusdialoogiboksis nupp **OK**.</span><span class="sxs-lookup"><span data-stu-id="86b99-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="86b99-113">Veebibrauseri, leidke saidikogumi root kodulehel ja seejärel juurdepääsu **saidi sätted** \> **saidikogumi funktsioonid**.</span><span class="sxs-lookup"><span data-stu-id="86b99-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="86b99-114">Lülita **töövoogude** funktsioon sisse:</span><span class="sxs-lookup"><span data-stu-id="86b99-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="86b99-115">· Kui funktsioon on *aktiveeritud* , klõpsake nuppu **Desaktiveeri** ja seejärel nuppu **Aktiveeri**.</span><span class="sxs-lookup"><span data-stu-id="86b99-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="86b99-116">· Kui funktsioon on *desaktiveeritud* , klõpsake nuppu **Aktiveeri**.</span><span class="sxs-lookup"><span data-stu-id="86b99-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="86b99-117">Lisateabe saamiseks lugege järgmist [artiklit](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="86b99-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

