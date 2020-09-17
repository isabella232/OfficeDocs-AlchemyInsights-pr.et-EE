---
title: SharePointi saidi loomine
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 5ebaa342ca9864bc31a9ef26eebcf42d96523871
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806935"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="94bd5-102">SharePointi saidi loomine</span><span class="sxs-lookup"><span data-stu-id="94bd5-102">Create a SharePoint site</span></span>

<span data-ttu-id="94bd5-103">SharePointi administreerimiskeskuse saitide loomine või haldamine [aktiivsete saitide](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) kaudu.</span><span class="sxs-lookup"><span data-stu-id="94bd5-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="94bd5-104">Lisateavet leiate teemast [saitide haldamine uues SharePointi administreerimiskeskuses](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="94bd5-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="94bd5-105">Näpunäited</span><span class="sxs-lookup"><span data-stu-id="94bd5-105">Tips:</span></span>

- <span data-ttu-id="94bd5-106">Te **ei saa** luua saiti olemasoleva saidi sama URL-iga.</span><span class="sxs-lookup"><span data-stu-id="94bd5-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="94bd5-107">Kui kustutasite saidi ja soovite URL-i uuesti kasutada, on võimalik, et kustutatud sait on kustutatud [saitide](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true)korral endiselt olemas.</span><span class="sxs-lookup"><span data-stu-id="94bd5-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="94bd5-108">URL-i uuesti kasutamiseks peab sait olema jäädavalt kustutatud.</span><span class="sxs-lookup"><span data-stu-id="94bd5-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="94bd5-109">Saidi täielikuks eemaldamiseks PowerShelli abil lugege teemat cmdlet [-käsu eemaldamine-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="94bd5-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="94bd5-110">Võimalik, et mõni kasutaja ei saa saiti luua.</span><span class="sxs-lookup"><span data-stu-id="94bd5-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="94bd5-111">[Lugege teemat saidi loomise haldamine SharePoint Online ' is](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="94bd5-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="94bd5-112">Võimalik, et sait näib olevat ummikus, kui **loodab** oodatust kauem aega.</span><span class="sxs-lookup"><span data-stu-id="94bd5-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="94bd5-113">Kui sellest probleemist on möödunud rohkem kui 24 tundi, logige sisse tugiteenuse pilet.</span><span class="sxs-lookup"><span data-stu-id="94bd5-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="94bd5-114">Paljudel juhtudel oleme juba lahendusega töötanud.</span><span class="sxs-lookup"><span data-stu-id="94bd5-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="94bd5-115">Lahenduse lõpetamiseks andke meile vähemalt 24 tundi.</span><span class="sxs-lookup"><span data-stu-id="94bd5-115">Please give us at least 24 hours to complete a solution.</span></span>
