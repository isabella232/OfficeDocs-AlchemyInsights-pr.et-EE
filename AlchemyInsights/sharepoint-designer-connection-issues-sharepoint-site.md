---
title: SharePoint Designeri ühenduse probleemid
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 01ccc6bc28148f397fb6cd2b7a0eaaeb5b51973f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511540"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="b56bd-102">SharePoint Designeri ühenduse probleemid</span><span class="sxs-lookup"><span data-stu-id="b56bd-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="b56bd-103">Kui SharePoint Designeri esineb SharePointi saitidele ühenduse probleemid, proovige järgmisi ühiseid lahendusi.</span><span class="sxs-lookup"><span data-stu-id="b56bd-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="b56bd-104">1. samm: Veenduge, et SharePoint Designer 2013 värskendatakse [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) ja [2 August 2016 värskendus SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="b56bd-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="b56bd-105">2. samm: tühjendage kohaliku vahemälu failid:</span><span class="sxs-lookup"><span data-stu-id="b56bd-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="b56bd-106">Sulgege SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="b56bd-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="b56bd-107">Eemaldage kohalikus arvutis kõik failid, mis on leitud igas järgmises kaustas.</span><span class="sxs-lookup"><span data-stu-id="b56bd-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="b56bd-108">%AppData%\microsoft\veebiserveri Ekstensions\cache</span><span class="sxs-lookup"><span data-stu-id="b56bd-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="b56bd-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="b56bd-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="b56bd-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="b56bd-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="b56bd-111">Avage SharePoint Designer 2013 ja sisestage konto uuesti, et näha, kas see töötab.</span><span class="sxs-lookup"><span data-stu-id="b56bd-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="b56bd-112">3. samm: [lubage kaasaegne autentimine Office 2013 Windows Devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="b56bd-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>

<span data-ttu-id="b56bd-113">Samm 4: Administraatorid peavad **lubama kohandatud skripti** SharePointi administreerimiskeskuse sätetes SharePoint Designeri ühenduse lubamiseks.</span><span class="sxs-lookup"><span data-stu-id="b56bd-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="b56bd-114">Lisateavet leiate teemast [kohandatud skripti lubamine või vältimine](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .</span><span class="sxs-lookup"><span data-stu-id="b56bd-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


