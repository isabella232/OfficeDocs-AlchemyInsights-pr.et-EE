---
title: Jagamine välistele kasutajatele ei tööta
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 69e290e5a13f40ad045086791189a7d0af88240b
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32369494"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="ad5b7-102">SharePointi sisu jagamine välistele kasutajatele probleemide lahendamine</span><span class="sxs-lookup"><span data-stu-id="ad5b7-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="ad5b7-103">Veenduge, et väline jagamine on lubatud oma organisatsiooni:</span><span class="sxs-lookup"><span data-stu-id="ad5b7-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="ad5b7-104">Mine ning [teenuste &amp; lisandmoodulid Microsoft 365 administreerimiskeskuses lehe](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), ja klõpsake nuppu **saidid**.</span><span class="sxs-lookup"><span data-stu-id="ad5b7-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="ad5b7-105">Veenduge, et seade on sisse lülitatud, "Sees".</span><span class="sxs-lookup"><span data-stu-id="ad5b7-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="ad5b7-106">Kui "Ainult olemasoleva välise kasutajate" on valitud, veenduge, et välise kasutaja on loetletud Microsoft 365 halduskeskus.</span><span class="sxs-lookup"><span data-stu-id="ad5b7-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="ad5b7-107">Veenduge, et väline jagada seda lubatud ala.</span><span class="sxs-lookup"><span data-stu-id="ad5b7-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="ad5b7-108">Klassikaline saidikogumi:</span><span class="sxs-lookup"><span data-stu-id="ad5b7-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="ad5b7-109">Uus SharePointi administreerimiskeskuses, vasakul paanil klõpsake nuppu **saidid**.</span><span class="sxs-lookup"><span data-stu-id="ad5b7-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="ad5b7-110">Valige või kohtadesse ja lindi nuppu **ühiskasutus**.</span><span class="sxs-lookup"><span data-stu-id="ad5b7-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="ad5b7-111">Meeskonnatöö saidi, mis kuulub Office 365 rühma või teatise saidi:</span><span class="sxs-lookup"><span data-stu-id="ad5b7-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="ad5b7-112">Uue saidi selliseid on sama ühiskasutuse säte kui oma kogu asutuses kehtivaid sätteid, kui kogu asutuses kehtivaid säte võimaldab jagada faile, linke, mis ei nõua sisselogimist kasutades.</span><span class="sxs-lookup"><span data-stu-id="ad5b7-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="ad5b7-113">Sel juhul saidid võimaldavad jagada uute ja olemasolevate väliste kasutajate sisselogimine.</span><span class="sxs-lookup"><span data-stu-id="ad5b7-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="ad5b7-114">Konkreetsetele lehekülgedele sätte muutmiseks kasutage uue SharePointi administreerimiskeskuse või PowerShelli.</span><span class="sxs-lookup"><span data-stu-id="ad5b7-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="ad5b7-115">[Lisateave](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="ad5b7-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="ad5b7-116">Välise jagamise säte meetmeid saab rohkem piiranguid kui kogu asutuses kehtivaid keskkonnas, kuid mitte rohkem kui kogu asutuses kehtivaid säte leebe.</span><span class="sxs-lookup"><span data-stu-id="ad5b7-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

