---
title: Ei saa lisada vaikimisi 2010 kinnitamise töövoog
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2060c9a1-e714-4d93-925e-629c82c35986
ms.openlocfilehash: 758b0339b842478f9609eb716b5b4ddab6579c80
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29466039"
---
# <a name="cant-add-default-2010-approval-workflow"></a><span data-ttu-id="bcef3-102">Ei saa lisada vaikimisi 2010 kinnitamise töövoog</span><span class="sxs-lookup"><span data-stu-id="bcef3-102">Can't add default 2010 Approval Workflow</span></span>

<span data-ttu-id="bcef3-103">Microsoft SharePointi saidikogumi, ei saa lisada (nt "kinnitamine - SharePoint 2010") ülemaailmselt korduvkasutatava töövoo loendi või teegi.</span><span class="sxs-lookup"><span data-stu-id="bcef3-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="bcef3-104">Probleemi lahendamiseks toimige järgmiselt.</span><span class="sxs-lookup"><span data-stu-id="bcef3-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="bcef3-105">Avage root saidikogumi SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="bcef3-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="bcef3-106">Valige jaotises **Saidi Objekte**, **töövood**.</span><span class="sxs-lookup"><span data-stu-id="bcef3-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="bcef3-107">**Töövoogude** lindi jaotises **Uus** valik **Korduvkasutatava töövoo**.</span><span class="sxs-lookup"><span data-stu-id="bcef3-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="bcef3-p101">Sisestage vormil **Luua korduvkasutatava töövoo** nimi \* \*\*Repair2010\*\*\*. **Platvormi tüüp**, valige **SharePoint 2010 töövoo**ja seejärel klõpsake **nuppu OK**.</span><span class="sxs-lookup"><span data-stu-id="bcef3-p101">On the **Create Reusable Workflow** form, enter the name  \* **Repair2010**\* . For **Platform Type**, select **SharePoint 2010 Workflow**, and then select **OK**.</span></span> 
  
5. <span data-ttu-id="bcef3-110">Valige **Save** jaotises **töövoo** lindi, **Avalda**.</span><span class="sxs-lookup"><span data-stu-id="bcef3-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
6. <span data-ttu-id="bcef3-p102">**Töövoo** lindi jaotises **Halda** valige **Avaldavad kogu maailmas**. Kuvatavas dialoogiboksis kinnitust valige **OK**.</span><span class="sxs-lookup"><span data-stu-id="bcef3-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
7. <span data-ttu-id="bcef3-p103">Veebibrauseri, otsige saidikogumi kodulehel root, ja siis juurdepääsu **Saidi sätted** \> **Saidikogumi funktsioonid**. Seejärel Lülita **töövood** funktsioon:</span><span class="sxs-lookup"><span data-stu-id="bcef3-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="bcef3-115">· Kui funktsioon on *aktiveeritud* , klõpsake nuppu **Desaktiveeri,** ja seejärel klõpsake nuppu **Aktiveeri**.</span><span class="sxs-lookup"><span data-stu-id="bcef3-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="bcef3-116">· Kui funktsioon on *deaktiveeritud* , klõpsake nuppu **Aktiveeri**.</span><span class="sxs-lookup"><span data-stu-id="bcef3-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="bcef3-117">Lisateabe saamiseks vaadake [artikli](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="bcef3-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

