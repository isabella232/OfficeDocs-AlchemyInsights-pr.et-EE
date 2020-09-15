---
title: Puuduv töövoog ei saanud aktiveerida
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 604dc770c5c14ded6a8de1cec9e311b03b69f094
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667082"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="1c7a7-102">Puuduv töövoog ei saanud aktiveerida</span><span class="sxs-lookup"><span data-stu-id="1c7a7-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="1c7a7-103">Microsoft SharePointi saidikogumis ei saa lisada loendile või teegile globaalselt korduvkasutatavat töövoogu (nt "kinnitamine-SharePoint 2010").</span><span class="sxs-lookup"><span data-stu-id="1c7a7-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="1c7a7-104">Probleemi lahendamiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="1c7a7-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="1c7a7-105">Avage saidikogumi juurkaustas rakenduses SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="1c7a7-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="1c7a7-106">Valige jaotises **saidi objektid**valik **töövood**.</span><span class="sxs-lookup"><span data-stu-id="1c7a7-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="1c7a7-107">Valige lindi **töövood** **uues** jaotises **korduvkasutatavad töövood**.</span><span class="sxs-lookup"><span data-stu-id="1c7a7-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="1c7a7-108">Sisestage vormil **korduvkasutatava töövoo loomine** nimi \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="1c7a7-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="1c7a7-109">Valige **platvormi tüübi**korral **SharePoint 2010 töövoog**ja seejärel klõpsake nuppu **OK**.</span><span class="sxs-lookup"><span data-stu-id="1c7a7-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="1c7a7-110">Klõpsake **töövoo** lindi jaotises **salvestamine** nuppu **Avalda**.</span><span class="sxs-lookup"><span data-stu-id="1c7a7-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="1c7a7-111">Klõpsake **töövoo** lindi jaotises **haldamine** nuppu **Avalda globaalselt**.</span><span class="sxs-lookup"><span data-stu-id="1c7a7-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="1c7a7-112">Valige kuvataval kinnituse dialoogiboksis nupp **OK**.</span><span class="sxs-lookup"><span data-stu-id="1c7a7-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="1c7a7-113">Otsige veebibrauseris üles saidikogumi juurlik veebisait ja seejärel saidi **sätete** saidikogumi \> **funktsioonid**.</span><span class="sxs-lookup"><span data-stu-id="1c7a7-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="1c7a7-114">Seejärel lülitab **töövoode** funktsiooni sisse.</span><span class="sxs-lookup"><span data-stu-id="1c7a7-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="1c7a7-115">· Kui funktsioon on  *aktiveeritud*  , klõpsake nuppu **Desaktiveeri ja seejärel** nuppu **Aktiveeri**.</span><span class="sxs-lookup"><span data-stu-id="1c7a7-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="1c7a7-116">· Kui funktsioon on  *desaktiveeritud*  , klõpsake nuppu **Aktiveeri**.</span><span class="sxs-lookup"><span data-stu-id="1c7a7-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="1c7a7-117">Lisateavet leiate järgmisest [artiklist](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="1c7a7-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

