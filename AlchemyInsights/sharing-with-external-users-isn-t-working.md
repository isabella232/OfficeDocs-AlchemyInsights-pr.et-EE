---
title: Ühiskasutus väliste kasutajatega ei tööta
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691571"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="3fea0-102">SharePointi sisu ühiskasutuse probleemide lahendamine väliste kasutajatega</span><span class="sxs-lookup"><span data-stu-id="3fea0-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="3fea0-103">Veenduge, et väline ühiskasutus on teie asutuse jaoks sisse lülitatud.</span><span class="sxs-lookup"><span data-stu-id="3fea0-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="3fea0-104">Avage [ &amp; Microsoft 365 halduskeskus lehel teenuste lisandmoodulid](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)ja klõpsake nuppu **saidid**.</span><span class="sxs-lookup"><span data-stu-id="3fea0-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="3fea0-105">Veenduge, et säte oleks "sees".</span><span class="sxs-lookup"><span data-stu-id="3fea0-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="3fea0-106">Kui valitud on "ainult olemasolevad välised kasutajad", siis veenduge, et väline kasutaja on loetletud Microsoft 365 halduskeskus.</span><span class="sxs-lookup"><span data-stu-id="3fea0-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="3fea0-107">Veenduge, et väline ühiskasutus oleks saidi jaoks sisse lülitatud.</span><span class="sxs-lookup"><span data-stu-id="3fea0-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="3fea0-108">Klassikalise saidikogumi jaoks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="3fea0-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="3fea0-109">Klõpsake uues SharePointi administreerimiskeskuses vasakpoolsel paanil nuppu **saidid**.</span><span class="sxs-lookup"><span data-stu-id="3fea0-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="3fea0-110">Valige sait või saidid ja klõpsake lindil nuppu **ühiskasutus**.</span><span class="sxs-lookup"><span data-stu-id="3fea0-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="3fea0-111">Meeskonnatöö saidi jaoks, mis kuulub mõnele Microsoft 365 rühmale või kommunikatsiooni saidile.</span><span class="sxs-lookup"><span data-stu-id="3fea0-111">For a team site that belongs to a Microsoft 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="3fea0-112">Nendel uutel saidi tüübil on sama ühiskasutuse säte kui teie asutuse kogum, välja arvatud juhul, kui kogu ettevõtte säte võimaldab faile ühiskasutusse anda linkide kaudu, mis ei nõua sisselogimist.</span><span class="sxs-lookup"><span data-stu-id="3fea0-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="3fea0-113">Sel juhul võimaldavad saidid ühiskasutusse anda uute ja olemasolevate väliste kasutajatega, kes sisse logivad.</span><span class="sxs-lookup"><span data-stu-id="3fea0-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="3fea0-114">Kindlate saitide sätete muutmiseks kasutage uut SharePointi administreerimiskeskuset või PowerShelli.</span><span class="sxs-lookup"><span data-stu-id="3fea0-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="3fea0-115">[Lisateave](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="3fea0-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="3fea0-116">Mis tahes saidi väline ühiskasutuse säte võib olla rohkem piiravam kui teie asutuse hõlmav säte, kuid mitte suurem kui organisatsiooni hõlmavas säte.</span><span class="sxs-lookup"><span data-stu-id="3fea0-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

