---
title: Saidi jäädavalt kustutamine SharePointis
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: 263317339d965d173a5a038fa006e0ce6f8476cc
ms.sourcegitcommit: da04e79b6072321caa16a6ceea6eb5f15de22394
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 03/25/2020
ms.locfileid: "42955128"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a><span data-ttu-id="39804-102">Saidi jäädavalt kustutamine SharePointis</span><span class="sxs-lookup"><span data-stu-id="39804-102">Permanently delete a site in SharePoint</span></span>

<span data-ttu-id="39804-103">Kustutatud saidi URL-i uuesti kasutamiseks (saidi taasloomiseks) või saidi jäädavalt kustutamiseks, kuna see pole enam kasutusel, saate kasutada uue SharePointi halduskeskuse suvandit **Kustuta jäädavalt**.</span><span class="sxs-lookup"><span data-stu-id="39804-103">To reuse a URL from a deleted site (to recreate a site), or to permanently delete a site because it's no longer in use, you can use **Permanently Delete** from the New SharePoint Admin Center.</span></span> 

1. <span data-ttu-id="39804-104">Avage [uue SharePointi halduskeskuse kustutatud saitide leht](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) ja logige sisse kontoga, millel on teie organisatsiooni administraatoriõigused.</span><span class="sxs-lookup"><span data-stu-id="39804-104">Go to the [Deleted sites page of the new SharePoint admin center](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) and sign in with an account that has admin permissions for your organization.</span></span> 

2. <span data-ttu-id="39804-105">Valige vasakpoolses veerus sait.</span><span class="sxs-lookup"><span data-stu-id="39804-105">In the left column, select a site.</span></span> 

3. <span data-ttu-id="39804-106">Klõpsake valikut **Kustuta lõplikult**.</span><span class="sxs-lookup"><span data-stu-id="39804-106">Click **Permanently Delete**.</span></span> 

<span data-ttu-id="39804-107">**Märkus**: rühmadega seotud saite ei saa uues SharePointi halduskeskuses jäädavalt kustutada.</span><span class="sxs-lookup"><span data-stu-id="39804-107">**Note**: Group-connected sites cannot be permanently deleted from the New SharePoint Admin Center.</span></span> <span data-ttu-id="39804-108">Selle asemel tuleb kasutada atribuuti [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite).</span><span class="sxs-lookup"><span data-stu-id="39804-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) will need to be used instead.</span></span>  

<span data-ttu-id="39804-109">Lisateavet vaadake teemast [Saidi jäädavalt kustutamine](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="39804-109">For more info, see [Permanently delete a site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span></span> 
