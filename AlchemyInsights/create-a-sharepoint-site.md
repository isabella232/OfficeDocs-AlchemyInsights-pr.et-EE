---
title: SharePointi saidi loomine
ms.author: efrene
author: efrene
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 30c51d84005534cc1de9e8b8136da1a07be57b73
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/18/2019
ms.locfileid: "36738193"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="be6ec-102">SharePointi saidi loomine</span><span class="sxs-lookup"><span data-stu-id="be6ec-102">Create a SharePoint site</span></span>

<span data-ttu-id="be6ec-103">SharePointi saidiloome kohta teabe saamiseks lugege järgmist:</span><span class="sxs-lookup"><span data-stu-id="be6ec-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="be6ec-104">[Halda saite uues SharePointi administreerimiskeskuses](https://docs.microsoft.com/sharepoint/manage-site-creation): teave saidi loomise suvandite kohta, sh kuidas luua klassikalist saiti või meeskondi, mis ei sisalda Office 365 gruppi.</span><span class="sxs-lookup"><span data-stu-id="be6ec-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="be6ec-105">[Meeskonnatöö saidi loomine SharePointis](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Vaadake, kuidas meeskonnatöö saiti luua.</span><span class="sxs-lookup"><span data-stu-id="be6ec-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Learn how to create a team site.</span></span>
- <span data-ttu-id="be6ec-106">[SharePoint Online ' i suhtlussaidi loomine](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Vaadake, kuidas luua suhtlussaiti.</span><span class="sxs-lookup"><span data-stu-id="be6ec-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="be6ec-107">[Saitide haldamine uues SharePointi administreerimiskeskuses](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): Vaadake, kuidas luua klassikaline sait või meeskonnatöö sait, mis ei sisalda Office 365 rühma.</span><span class="sxs-lookup"><span data-stu-id="be6ec-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> <span data-ttu-id="be6ec-108">[! Näpunäiteid</span><span class="sxs-lookup"><span data-stu-id="be6ec-108">[!Tips]</span></span>
> - <span data-ttu-id="be6ec-109">Te ei saa luua saiti, millel on sama URL-i olemasolev sait.</span><span class="sxs-lookup"><span data-stu-id="be6ec-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="be6ec-110">Kui kustutasite saidi ja soovite URL-i uuesti kasutada, on võimalik, et kustutatud sait on **Kustutatud saitide**puhul endiselt olemas.</span><span class="sxs-lookup"><span data-stu-id="be6ec-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="be6ec-111">Kustutatud saitide haldamiseks vaadake [saidi kustutamist](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="be6ec-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="be6ec-112">Täielikult eemaldada saidi PowerShelli, vt [Eemalda SPSite cmdlet-](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) i näide.</span><span class="sxs-lookup"><span data-stu-id="be6ec-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="be6ec-113">Mõnel kasutajal ei pruugi olla võimalik saiti luua.</span><span class="sxs-lookup"><span data-stu-id="be6ec-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="be6ec-114">Vt teemat [SharePoint Online ' i saidi loomise haldamine](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="be6ec-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="be6ec-115">On võimalik, et sait kuvatakse kinni **luua** oodatust kauem aega.</span><span class="sxs-lookup"><span data-stu-id="be6ec-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="be6ec-116">Kui teil on möödunud rohkem kui 24 tundi pärast seda, kui te esimest korda seda probleemi, Palun logige tugiteenuse pilet.</span><span class="sxs-lookup"><span data-stu-id="be6ec-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="be6ec-117">Paljudel juhtudel oleme juba lahenduse kallal töötanud.</span><span class="sxs-lookup"><span data-stu-id="be6ec-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="be6ec-118">Palun andke meile vähemalt 24 tundi, et lahendus lõpule viia.</span><span class="sxs-lookup"><span data-stu-id="be6ec-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="be6ec-119">Kui teil on vaja luua uus meeskonnatöö sait, mis ei sisalda Office 365 rühma,</span><span class="sxs-lookup"><span data-stu-id="be6ec-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


