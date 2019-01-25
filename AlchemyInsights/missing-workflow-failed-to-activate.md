---
title: Kadunud töövoogu ei saanud aktiveerida
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 33b92c2cae1f641b0cd88c82fd4ae5e8632d76c2
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29466001"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="8bf03-102">Kadunud töövoogu ei saanud aktiveerida</span><span class="sxs-lookup"><span data-stu-id="8bf03-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="8bf03-103">Microsoft SharePointi saidikogumi, ei saa lisada (nt "kinnitamine - SharePoint 2010") ülemaailmselt korduvkasutatava töövoo loendi või teegi.</span><span class="sxs-lookup"><span data-stu-id="8bf03-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="8bf03-104">Probleemi lahendamiseks toimige järgmiselt.</span><span class="sxs-lookup"><span data-stu-id="8bf03-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="8bf03-105">Avage root saidikogumi SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="8bf03-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="8bf03-106">Valige jaotises **Saidi Objekte**, **töövood**.</span><span class="sxs-lookup"><span data-stu-id="8bf03-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="8bf03-107">**Töövoogude** lindi jaotises **Uus** valik **Korduvkasutatava töövoo**.</span><span class="sxs-lookup"><span data-stu-id="8bf03-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="8bf03-p101">Sisestage vormil **Luua korduvkasutatava töövoo** nimi \*\* *Repair2010* \*\*. **Platvormi tüüp**, klõpsake nuppu **SharePoint 2010 töövoo**ja klõpsake nuppu **OK**.</span><span class="sxs-lookup"><span data-stu-id="8bf03-p101">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*. For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="8bf03-110">Valige **Save** jaotises **töövoo** lindi, **Avalda**.</span><span class="sxs-lookup"><span data-stu-id="8bf03-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="8bf03-p102">**Töövoo** lindi jaotises **Halda** valige **Avaldavad kogu maailmas**. Kuvatavas dialoogiboksis kinnitust valige **OK**.</span><span class="sxs-lookup"><span data-stu-id="8bf03-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="8bf03-p103">Veebibrauseri, otsige saidikogumi kodulehel root, ja siis juurdepääsu **Saidi sätted** \> **Saidikogumi funktsioonid**. Seejärel Lülita **töövood** funktsioon:</span><span class="sxs-lookup"><span data-stu-id="8bf03-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="8bf03-115">· Kui funktsioon on *aktiveeritud* , klõpsake nuppu **Desaktiveeri,** ja seejärel klõpsake nuppu **Aktiveeri**.</span><span class="sxs-lookup"><span data-stu-id="8bf03-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="8bf03-116">· Kui funktsioon on *deaktiveeritud* , klõpsake nuppu **Aktiveeri**.</span><span class="sxs-lookup"><span data-stu-id="8bf03-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="8bf03-117">Lisateabe saamiseks vaadake [artikli](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="8bf03-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

