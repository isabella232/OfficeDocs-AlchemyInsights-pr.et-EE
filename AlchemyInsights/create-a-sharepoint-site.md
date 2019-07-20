---
title: SharePointi saidi loomine
ms.author: kirks
author: Techwriter40
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1386"
- "2303"
- "5200004"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 022f572aadae3b4d9f6665f9f8be871d79b51817
ms.sourcegitcommit: f81c56dd4ae7cb2eedc383dd671b9012f3089286
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/19/2019
ms.locfileid: "35802962"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="3f688-102">SharePointi saidi loomine</span><span class="sxs-lookup"><span data-stu-id="3f688-102">Create a SharePoint site</span></span>

<span data-ttu-id="3f688-103">Näete järgmise SharePointi saidi loomise kohta:</span><span class="sxs-lookup"><span data-stu-id="3f688-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="3f688-104">[Halda saite uue SharePointi administreerimiskeskuses](https://docs.microsoft.com/sharepoint/manage-site-creation): teave saidi loomise võimalusi, sealhulgas klassikaline saidi või meeskonnad saidi, mis ei sisalda Office 365 rühma loomine.</span><span class="sxs-lookup"><span data-stu-id="3f688-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="3f688-105">[SharePointi meeskonnatöö veebisaidi loomine](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): saate luua meeskonnatöö veebisaidi.</span><span class="sxs-lookup"><span data-stu-id="3f688-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Learn how to create a team site.</span></span>
- <span data-ttu-id="3f688-106">[Loo side saidi SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): saate luua side saidi.</span><span class="sxs-lookup"><span data-stu-id="3f688-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="3f688-107">[Halda saite uue SharePointi administreerimiskeskuses](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): saate luua klassikaline saidi või meeskonna sait, mis ei sisalda Office 365 rühma.</span><span class="sxs-lookup"><span data-stu-id="3f688-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> [! Näpunäiteid]
> - <span data-ttu-id="3f688-109">Ei saa luua sama URL-iga olemasoleva saidi sait.</span><span class="sxs-lookup"><span data-stu-id="3f688-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="3f688-110">Kui saidi kustutada ja kes soovib kasutada URL-i, on võimalik kustutatud ala, mis on endiselt olemas **Kustutatud saidid**.</span><span class="sxs-lookup"><span data-stu-id="3f688-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="3f688-111">Juhtida kustutatud saidid vt [saiti kustutada](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="3f688-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="3f688-112">Täielikult eemaldada saidi PowerShelli abil, vaadake [Eemalda-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet-i näites.</span><span class="sxs-lookup"><span data-stu-id="3f688-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="3f688-113">Mõned kasutajad ei saa luua saidi.</span><span class="sxs-lookup"><span data-stu-id="3f688-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="3f688-114">Vaata [Halda saidi loomist SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="3f688-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="3f688-115">On võimalik, et sait kuvatakse jäänud kell **loomine** oodatust kauem aega.</span><span class="sxs-lookup"><span data-stu-id="3f688-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="3f688-116">Kui te esimest korda nägin see probleem on möödunud üle 24 tunni, logi palun toetust pilet.</span><span class="sxs-lookup"><span data-stu-id="3f688-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="3f688-117">Paljudel juhtudel arendame juba lahenduse.</span><span class="sxs-lookup"><span data-stu-id="3f688-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="3f688-118">Palun anna meile vähemalt 24 tundi, lahendus.</span><span class="sxs-lookup"><span data-stu-id="3f688-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="3f688-119">Kui peate looma uue meeskonnasaidi, mis ei sisalda Office 365 rühma,</span><span class="sxs-lookup"><span data-stu-id="3f688-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


