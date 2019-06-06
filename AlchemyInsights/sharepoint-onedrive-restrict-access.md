---
title: Piirata juurdepääsu SharePointi või OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 5101366ff65f477c19b9c7f2c0d7065cf88501b0
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/05/2019
ms.locfileid: "34735139"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="f6a66-102">Piirata juurdepääsu SharePointi või OneDrive</span><span class="sxs-lookup"><span data-stu-id="f6a66-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="f6a66-103">On palju võimalusi piirata juurdepääsu SharePoint Online/OneDrive teenuseid.</span><span class="sxs-lookup"><span data-stu-id="f6a66-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="f6a66-104">Need erinevate juurdepääsu piiramise meetodid on toodud allpool.</span><span class="sxs-lookup"><span data-stu-id="f6a66-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="f6a66-105">Luba piirangut</span><span class="sxs-lookup"><span data-stu-id="f6a66-105">Permission Restriction</span></span>

<span data-ttu-id="f6a66-106">SharePoint Online ja OneDrive for Business, piirame juurdepääsu üksuste saidid, failid ja kaustad nende rühmade/isikute, kes peaks olema juurdepääs ainult andes.</span><span class="sxs-lookup"><span data-stu-id="f6a66-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

[<span data-ttu-id="f6a66-107">Saate kohandada SharePointi loendi või teegi õiguste</span><span class="sxs-lookup"><span data-stu-id="f6a66-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/en-us/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

[<span data-ttu-id="f6a66-108">Saate kohandada SharePointi saidi õigused</span><span class="sxs-lookup"><span data-stu-id="f6a66-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions)

[<span data-ttu-id="f6a66-109">Muutke alamkausta õigusi</span><span class="sxs-lookup"><span data-stu-id="f6a66-109">Change the permissions on a subfolder</span></span>](https://support.office.com/en-us/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

[<span data-ttu-id="f6a66-110">Kasutusõigus haldamata seadmed</span><span class="sxs-lookup"><span data-stu-id="f6a66-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/en-us/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="f6a66-111">SharePointi või teenusekomplekti Office 365 globaalne admin, te saate blokeerida või SharePointis või OneDrive sisu piirata haldamata seadmetest (nende hübriid AD liidetud või ühilduv Intune).</span><span class="sxs-lookup"><span data-stu-id="f6a66-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="f6a66-112">Võrgu asukoht piirang</span><span class="sxs-lookup"><span data-stu-id="f6a66-112">Network Location Restriction</span></span>

<span data-ttu-id="f6a66-113">Nagu IT-administraator, saate kontrollida juurdepääsu SharePointis või OneDrive ressursse vastavalt kindlaksmääratud kohtades, mis on usaldusväärsed.</span><span class="sxs-lookup"><span data-stu-id="f6a66-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="f6a66-114">See on ka asukohapõhised poliitika.</span><span class="sxs-lookup"><span data-stu-id="f6a66-114">This is also known as location-based policy.</span></span> <span data-ttu-id="f6a66-115">Lisateabe saamiseks lugege [SharePoint Online ja OneDrive andmeid sõltuvalt juurdepääsu kontroll](https://docs.microsoft.com/en-us/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="f6a66-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/en-us/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="f6a66-116">Saidipiirangut lukk</span><span class="sxs-lookup"><span data-stu-id="f6a66-116">Site Lock Restriction</span></span> 

<span data-ttu-id="f6a66-117">Jooksul SharePoint Online peate võime lukustada saidikogumi, nii et keegi ei ole juurdepääsu.</span><span class="sxs-lookup"><span data-stu-id="f6a66-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="f6a66-118">See asub PowerShelli ja [Set-SPOSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) - LockState atribuudi [SharePoint Online halduskesta](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) kaudu.</span><span class="sxs-lookup"><span data-stu-id="f6a66-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="f6a66-119">Piirata, saite või alamsaitide loomine</span><span class="sxs-lookup"><span data-stu-id="f6a66-119">Restrict users from creating sites or subsites</span></span>

<span data-ttu-id="f6a66-120">SharePointi admin või Office 365 globaalne admin, võite oma kasutajad luua ja hallata oma SharePointi saitidele, kindlaks määrata, milliseid saite nad luua, ja määrake asukoht saidid.</span><span class="sxs-lookup"><span data-stu-id="f6a66-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="f6a66-121">Lisateabe saamiseks lugege [SharePoint Online Halda saidi loomist](https://docs.microsoft.com/en-us/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="f6a66-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/manage-site-creation)</span></span>

