---
title: Rühma lisamine SharePointi saidile
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: b54457427ffa563b6a6323d85e1c8800191eca11
ms.sourcegitcommit: d1aad215f8aa636ba89c93a13a0c9d90e997f752
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/06/2020
ms.locfileid: "44064389"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="f9cca-102">Probleemid rühma ühendatud saidi loomisel SharePointis</span><span class="sxs-lookup"><span data-stu-id="f9cca-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="f9cca-103">Mõne rühma ühendatud saidi loomisel või uuesti loomisel ilmnesid tavalised probleemid.</span><span class="sxs-lookup"><span data-stu-id="f9cca-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="f9cca-104">Kui olete kustutanud rühma ja selle ühendatud saidi ning soovite luua sama URL-iga mõne muu saidi, peate eelmise saidi jäädavalt eemaldama.</span><span class="sxs-lookup"><span data-stu-id="f9cca-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="f9cca-105">Lae alla [SPO Management shelli](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="f9cca-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="f9cca-106">Lisateavet PowerShelli kohta alustamine, vaadake alustamine [SharePoint Online Management shelli](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="f9cca-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="f9cca-107">Eemaldage saidi kustutatud saidid kasutades [Eemalda SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShelli cmdlet-käsu.</span><span class="sxs-lookup"><span data-stu-id="f9cca-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="f9cca-108">Rühma saitide jäädavalt kustutamiseks on vaja PowerShelli.</span><span class="sxs-lookup"><span data-stu-id="f9cca-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="f9cca-109">Kui loote rühma ühendatud saidi ja kuvatakse hoiatus: **teine sama pseudonüümiga rühm on juba olemas**, kontrollige olemasolevaid rühmi [Microsoft 365 administreerimiskeskusest](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="f9cca-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="f9cca-110">Probleemi lahendamiseks kustutage olemasolev rühm, kui see ei ole enam vajalik või luua saidi teise alias määratud.</span><span class="sxs-lookup"><span data-stu-id="f9cca-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="f9cca-111">On erinevaid viise, kuidas luua ja kasutada tänapäevaseid rühmi SharePointiga.</span><span class="sxs-lookup"><span data-stu-id="f9cca-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="f9cca-112">Saate ühendada olemasolevad saidid Microsoft 365 rühma.</span><span class="sxs-lookup"><span data-stu-id="f9cca-112">You can connect existing sites to an Microsoft 365 group.</span></span> <span data-ttu-id="f9cca-113">Lisateavet leiate teemast [Microsoft 365 rühma ühendamine SharePointi kasutajaliidese abil](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="f9cca-113">For more info, see [Connect an Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="f9cca-114">Microsoft 365 rühma ühendatud saidi loomiseks peate looma [meeskonnatöö saidi](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="f9cca-114">To create an Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
