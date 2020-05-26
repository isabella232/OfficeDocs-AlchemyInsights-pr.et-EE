---
title: Blokeeri allalaadimise lingid
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000213"
- "5715"
ms.openlocfilehash: 8cb53754125cedf4a3d0426d6c3bf70297eb3d74
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/23/2020
ms.locfileid: "44357630"
---
# <a name="block-download-on-sharing-links"></a><span data-ttu-id="6d788-102">Blokeeri allalaadimise lingid</span><span class="sxs-lookup"><span data-stu-id="6d788-102">Block download on sharing links</span></span>

<span data-ttu-id="6d788-103">**Blokeeri allalaadimine** on saadaval ainult Office ' i dokumentidele mõeldud **linkide kuvamiseks** .</span><span class="sxs-lookup"><span data-stu-id="6d788-103">**Block download** is available for **view-only links** to Office documents.</span></span> <span data-ttu-id="6d788-104">Selle suvandi valimisel ei näe inimesed, kes pääsevad failile juurde teie loodud lingi kaudu, suvandeid alla laadida, printida ega kopeerida.</span><span class="sxs-lookup"><span data-stu-id="6d788-104">When you select this option, people who gain access to the file via the link you created will not see options to download, print, or copy the file.</span></span>

<span data-ttu-id="6d788-105">Administraatorid saavad kontrollida, kas "Block alla" säte kuvatakse ainult Office ' i failid või mitte, muutes `BlockDownloadLinksFileType` sätet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) või [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShelli cmdlet-käsud.</span><span class="sxs-lookup"><span data-stu-id="6d788-105">Administrators can control whether the "block download" setting appears only for Office files or not by changing the `BlockDownloadLinksFileType` setting in the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) or [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell cmdlets.</span></span>
