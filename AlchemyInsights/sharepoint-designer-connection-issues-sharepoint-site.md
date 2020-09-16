---
title: SharePoint Designeri ühenduste probleemid
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727167"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="9468d-102">SharePoint Designeri ühenduste probleemid</span><span class="sxs-lookup"><span data-stu-id="9468d-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="9468d-103">Kui SharePoint Designeris esineb SharePointi saitidel probleeme, proovige järgmisi levinud lahendusi.</span><span class="sxs-lookup"><span data-stu-id="9468d-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="9468d-104">1. juhis: Veenduge, et SharePoint Designer 2013 oleks värskendatud SharePoint Designeri [hoolduspaketiga Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) ja sharepoint [Designer 2013, August 2, 2016 värskendus](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="9468d-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="9468d-105">2. juhis: tühjendage kohaliku vahemälu failid.</span><span class="sxs-lookup"><span data-stu-id="9468d-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="9468d-106">Sulgege SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="9468d-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="9468d-107">Eemaldage kohalikus arvutis kõik järgmistest kaustadest leitud failid.</span><span class="sxs-lookup"><span data-stu-id="9468d-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="9468d-108">%APPDATA%\Microsoft\Web serveri Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="9468d-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="9468d-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="9468d-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="9468d-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="9468d-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="9468d-111">Avage SharePoint Designer 2013 ja sisestage konto uuesti, et näha, kas see töötab.</span><span class="sxs-lookup"><span data-stu-id="9468d-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="9468d-112">3. juhis: [Windowsi seadmetes Office 2013 kaasaegse autentimise lubamine](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="9468d-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>

<span data-ttu-id="9468d-113">4. juhis: Administraatorid peavad **lubama kohandatud skripti** SharePointi administreerimiskeskuse sätetes, et lubada SharePoint Designeri ühendust.</span><span class="sxs-lookup"><span data-stu-id="9468d-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="9468d-114">Lisateavet leiate teemast [kohandatud skripti lubamine või keelamine](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .</span><span class="sxs-lookup"><span data-stu-id="9468d-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


