---
title: Kadunud töövoogu ei saanud aktiveerida
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 44fd3c2d1e8b278b47c0fde6d48c7cbcbaa5c324
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543921"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="8e5b8-102">Kadunud töövoogu ei saanud aktiveerida</span><span class="sxs-lookup"><span data-stu-id="8e5b8-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="8e5b8-103">Microsoft SharePointi saidikogumi, ei saa lisada (nt "kinnitamine - SharePoint 2010") ülemaailmselt korduvkasutatava töövoo loendi või teegi.</span><span class="sxs-lookup"><span data-stu-id="8e5b8-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="8e5b8-104">Probleemi lahendamiseks toimige järgmiselt.</span><span class="sxs-lookup"><span data-stu-id="8e5b8-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="8e5b8-105">Avage root saidikogumi SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="8e5b8-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="8e5b8-106">Valige jaotises **Saidi Objekte**, **töövood**.</span><span class="sxs-lookup"><span data-stu-id="8e5b8-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="8e5b8-107">**Töövoogude** lindi jaotises **Uus** valik **Korduvkasutatava töövoo**.</span><span class="sxs-lookup"><span data-stu-id="8e5b8-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="8e5b8-108">Sisestage vormil **Luua korduvkasutatava töövoo** nimi \*\* *Repair2010* \*\*.</span><span class="sxs-lookup"><span data-stu-id="8e5b8-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="8e5b8-109">**Platvormi tüüp**, klõpsake nuppu **SharePoint 2010 töövoo**ja klõpsake nuppu **OK**.</span><span class="sxs-lookup"><span data-stu-id="8e5b8-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="8e5b8-110">Valige **Save** jaotises **töövoo** lindi, **Avalda**.</span><span class="sxs-lookup"><span data-stu-id="8e5b8-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="8e5b8-111">**Töövoo** lindi jaotises **Halda** valige **Avaldavad kogu maailmas**.</span><span class="sxs-lookup"><span data-stu-id="8e5b8-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="8e5b8-112">Kuvatavas dialoogiboksis kinnitust valige **OK**.</span><span class="sxs-lookup"><span data-stu-id="8e5b8-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="8e5b8-113">Veebibrauseri, otsige saidikogumi kodulehel root, ja siis juurdepääsu **Saidi sätted** \> **Saidikogumi funktsioonid**.</span><span class="sxs-lookup"><span data-stu-id="8e5b8-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="8e5b8-114">Seejärel Lülita **töövood** funktsioon:</span><span class="sxs-lookup"><span data-stu-id="8e5b8-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="8e5b8-115">· Kui funktsioon on *aktiveeritud* , klõpsake nuppu **Desaktiveeri,** ja seejärel klõpsake nuppu **Aktiveeri**.</span><span class="sxs-lookup"><span data-stu-id="8e5b8-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="8e5b8-116">· Kui funktsioon on *deaktiveeritud* , klõpsake nuppu **Aktiveeri**.</span><span class="sxs-lookup"><span data-stu-id="8e5b8-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="8e5b8-117">Lisateabe saamiseks vaadake [artikli](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="8e5b8-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

