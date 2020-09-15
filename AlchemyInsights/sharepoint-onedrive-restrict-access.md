---
title: Juurdepääsu piiramine SharePointis või OneDrive ' is
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700451"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="04b8c-102">Juurdepääsu piiramine SharePointis või OneDrive ' is</span><span class="sxs-lookup"><span data-stu-id="04b8c-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="04b8c-103">SharePoint Online ' i/OneDrive ' i teenustele juurdepääsu piiramiseks on mitu võimalust.</span><span class="sxs-lookup"><span data-stu-id="04b8c-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="04b8c-104">Allpool on kirjeldatud järgmisi Accessi piirangute meetodeid.</span><span class="sxs-lookup"><span data-stu-id="04b8c-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="04b8c-105">**Õiguste piirang**</span><span class="sxs-lookup"><span data-stu-id="04b8c-105">**Permission Restriction**</span></span>

<span data-ttu-id="04b8c-106">SharePoint Online ' is ja OneDrive for Businessis piirame juurdepääsu sellistele üksustele nagu saidid, failid ja kaustad, võimaldades juurdepääsu ainult nendele rühmadele/isikutele, kellel on juurdepääs.</span><span class="sxs-lookup"><span data-stu-id="04b8c-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="04b8c-107">SharePointi loendi või teegi õiguse kohandamine</span><span class="sxs-lookup"><span data-stu-id="04b8c-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="04b8c-108">SharePointi saidi kasutusõiguste kohandamine</span><span class="sxs-lookup"><span data-stu-id="04b8c-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="04b8c-109">Alamkausta õiguse muutmine</span><span class="sxs-lookup"><span data-stu-id="04b8c-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="04b8c-110">Haldamata seadmetest juurdepääsu reguleerimine</span><span class="sxs-lookup"><span data-stu-id="04b8c-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="04b8c-111">SharePointi või üldadministraatori saate hallata või piirata juurdepääsu SharePointi ja OneDrive ' i sisule haldamata seadmetest (need ei ole hübriid ad liitunud või ühilduvad Intune ' is).</span><span class="sxs-lookup"><span data-stu-id="04b8c-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="04b8c-112">**Võrgukoha piirang**</span><span class="sxs-lookup"><span data-stu-id="04b8c-112">**Network Location Restriction**</span></span>

<span data-ttu-id="04b8c-113">IT-administraatorina saate reguleerida juurdepääsu SharePointi ja OneDrive ' i ressurssidele, mis põhinevad teie usaldusväärsel võrgu asukohal.</span><span class="sxs-lookup"><span data-stu-id="04b8c-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="04b8c-114">Seda tuntakse ka asukoha-põhise poliitikana.</span><span class="sxs-lookup"><span data-stu-id="04b8c-114">This is also known as location-based policy.</span></span> <span data-ttu-id="04b8c-115">Lisateavet leiate teemast [SharePoint Online ' i ja OneDrive ' i andmetele juurdepääsu reguleerimine võrgu asukoha põhjal](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="04b8c-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="04b8c-116">**Saidi lukustuse piirang**</span><span class="sxs-lookup"><span data-stu-id="04b8c-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="04b8c-117">SharePoint Online ' is saate saidikogumi lukustada, nii et keegi ei pääseks sellele juurde.</span><span class="sxs-lookup"><span data-stu-id="04b8c-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="04b8c-118">See on määratud PowerShelli ja [SharePoint Online ' i halduse kesta](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) kaudu, kasutades atribuuti [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.</span><span class="sxs-lookup"><span data-stu-id="04b8c-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="04b8c-119">**Kasutajate ja alamsaitide loomise piiramine**</span><span class="sxs-lookup"><span data-stu-id="04b8c-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="04b8c-120">Kui olete SharePointi administraator või üldadministraator, saate lubada kasutajatel luua ja hallata oma SharePointi saite, määrata kindlaks, millist tüüpi saite nad saavad luua, ja määrata saitide asukoha.</span><span class="sxs-lookup"><span data-stu-id="04b8c-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="04b8c-121">Lisateavet leiate teemast [saidi loomise haldamine SharePoint Online ' is](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="04b8c-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

