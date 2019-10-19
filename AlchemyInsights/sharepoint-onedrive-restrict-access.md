---
title: SharePointi või OneDrive ' i juurdepääsu piiramine
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/18/2019
ms.locfileid: "36750660"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="4c5dc-102">SharePointi või OneDrive ' i juurdepääsu piiramine</span><span class="sxs-lookup"><span data-stu-id="4c5dc-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="4c5dc-103">On palju viise, kuidas piirata juurdepääsu SharePoint Online/OneDrive teenused.</span><span class="sxs-lookup"><span data-stu-id="4c5dc-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="4c5dc-104">Need erinevad juurdepääsupiirangu meetodid on toodud allpool.</span><span class="sxs-lookup"><span data-stu-id="4c5dc-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="4c5dc-105">**Õiguste piirang**</span><span class="sxs-lookup"><span data-stu-id="4c5dc-105">**Permission Restriction**</span></span>

<span data-ttu-id="4c5dc-106">SharePoint Online ' i ja OneDrive for Business, piirame juurdepääsu üksustele nagu saidid, failid ja kaustad, ainult andes juurdepääsu neile rühmadele/isikutele, kellel peaks olema juurdepääs.</span><span class="sxs-lookup"><span data-stu-id="4c5dc-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="4c5dc-107">SharePointi loendi või teegi õiguste kohandamine</span><span class="sxs-lookup"><span data-stu-id="4c5dc-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="4c5dc-108">SharePointi saidiga õiguste kohandamine</span><span class="sxs-lookup"><span data-stu-id="4c5dc-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="4c5dc-109">Alamkausta õiguste muutmine</span><span class="sxs-lookup"><span data-stu-id="4c5dc-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="4c5dc-110">Haldamata seadmete juurdepääsu kontrollimine</span><span class="sxs-lookup"><span data-stu-id="4c5dc-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="4c5dc-111">SharePointi või globaalse admin Office 365, saate blokeerida või piirata juurdepääsu SharePointi ja OneDrive ' i sisu haldamata seadmete (need ei ole hübriid AD ühendatud või Intune).</span><span class="sxs-lookup"><span data-stu-id="4c5dc-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="4c5dc-112">**Võrguasukoha piirang**</span><span class="sxs-lookup"><span data-stu-id="4c5dc-112">**Network Location Restriction**</span></span>

<span data-ttu-id="4c5dc-113">IT-administraatoriks saate reguleerida juurdepääsu SharePointi ja OneDrive ' i ressurssidele, mis põhinevad määratletud võrguasukohtadele, mida te usaldate.</span><span class="sxs-lookup"><span data-stu-id="4c5dc-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="4c5dc-114">Seda nimetatakse ka asukohapõhise poliitika.</span><span class="sxs-lookup"><span data-stu-id="4c5dc-114">This is also known as location-based policy.</span></span> <span data-ttu-id="4c5dc-115">Lisateabe saamiseks vaadake [juurdepääsu SharePoint Online ' i ja OneDrive andmed võrgu asukoha järgi](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="4c5dc-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="4c5dc-116">**Saidideluku piirang**</span><span class="sxs-lookup"><span data-stu-id="4c5dc-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="4c5dc-117">SharePoint Online ' i sees on teil võimalus saidikogumi lukustada, nii et keegi ei pääse juurde.</span><span class="sxs-lookup"><span data-stu-id="4c5dc-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="4c5dc-118">See on seatud PowerShelli ja [SharePoint Online Management shelli](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) abil [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate atribuut.</span><span class="sxs-lookup"><span data-stu-id="4c5dc-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="4c5dc-119">**Kasutajate piiramine saitide või alamsaitide loomisega**</span><span class="sxs-lookup"><span data-stu-id="4c5dc-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="4c5dc-120">SharePointi administraator või Office 365 globaalse admin, saate lasta oma kasutajatel luua ja hallata oma SharePointi saite, määratleda, milliseid saite nad saavad luua ja määrata saitide asukoht.</span><span class="sxs-lookup"><span data-stu-id="4c5dc-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="4c5dc-121">Lisateabe saamiseks lugege [saidi loomine SharePoint Online ' i haldamine](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="4c5dc-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

