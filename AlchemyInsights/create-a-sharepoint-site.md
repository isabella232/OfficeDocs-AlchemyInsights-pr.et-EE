---
title: SharePointi saidi loomine
ms.author: pebaum
author: todmccoy
ms.audience: Admin
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: e1e71ae9401448ed18058f6307302dcbaf773649
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770851"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="f124b-102">SharePointi saidi loomine</span><span class="sxs-lookup"><span data-stu-id="f124b-102">Create a SharePoint site</span></span>

<span data-ttu-id="f124b-103">Saate luua või hallata SharePointi administreerimiskeskuse [aktiivsete saitide](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) saite.</span><span class="sxs-lookup"><span data-stu-id="f124b-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="f124b-104">Lisateavet leiate jaotisest [uute SharePointi administreerimiskeskuse saitide haldamine](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="f124b-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="f124b-105">Nõuanded:</span><span class="sxs-lookup"><span data-stu-id="f124b-105">Tips:</span></span>

- <span data-ttu-id="f124b-106">Te **ei saa** luua saiti, millel on sama URL-i olemasolev sait.</span><span class="sxs-lookup"><span data-stu-id="f124b-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="f124b-107">Kui kustutasite saidi ja soovite URL-i uuesti kasutada, on võimalik, et kustutatud sait on [Kustutatud saitide](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true)puhul endiselt olemas.</span><span class="sxs-lookup"><span data-stu-id="f124b-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="f124b-108">Sait tuleb URL-i uuesti kasutamiseks jäädavalt kustutada.</span><span class="sxs-lookup"><span data-stu-id="f124b-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="f124b-109">Täielikult eemaldada saidi PowerShelli, vt [Eemalda SPSite cmdlet-](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) i näide.</span><span class="sxs-lookup"><span data-stu-id="f124b-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="f124b-110">Mõnel kasutajal ei pruugi olla võimalik saiti luua.</span><span class="sxs-lookup"><span data-stu-id="f124b-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="f124b-111">[Vt teemat SharePoint Online ' i saidi loomise haldamine](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="f124b-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="f124b-112">On võimalik, et sait kuvatakse kinni **luua** oodatust kauem aega.</span><span class="sxs-lookup"><span data-stu-id="f124b-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="f124b-113">Kui teil on möödunud rohkem kui 24 tundi pärast seda, kui te esimest korda seda probleemi, Palun logige tugiteenuse pilet.</span><span class="sxs-lookup"><span data-stu-id="f124b-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="f124b-114">Paljudel juhtudel oleme juba lahenduse kallal töötanud.</span><span class="sxs-lookup"><span data-stu-id="f124b-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="f124b-115">Palun andke meile vähemalt 24 tundi, et lahendus lõpule viia.</span><span class="sxs-lookup"><span data-stu-id="f124b-115">Please give us at least 24 hours to complete a solution.</span></span>
