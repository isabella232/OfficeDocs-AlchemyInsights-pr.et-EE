---
title: SharePoint Online ' i PowerShelli
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 00ec337ce34da9d3c3fba0a71602c3078a556552
ms.sourcegitcommit: 6b102e079a7d30298105fd811a67efb707d6d5bf
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/23/2019
ms.locfileid: "37122995"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="1bbca-102">SharePoint Online ' i PowerShelli</span><span class="sxs-lookup"><span data-stu-id="1bbca-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="1bbca-103">Töötamine PowerShelli või skriptidega SharePoint Online ' i raames?</span><span class="sxs-lookup"><span data-stu-id="1bbca-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="1bbca-104">Lisateabe saamiseks külastage allolevaid linke.</span><span class="sxs-lookup"><span data-stu-id="1bbca-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="1bbca-105">Alustamine SharePoint Online Management shelli</span><span class="sxs-lookup"><span data-stu-id="1bbca-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="1bbca-106">Ühendamine SPO PowerShelli mitme teguriga autentimine (MFA)</span><span class="sxs-lookup"><span data-stu-id="1bbca-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="1bbca-107">[SharePointi mustrid ja tavad (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) sisaldab teegi PowerShelli käsud, mis võimaldab teil sooritada keerukaid juhtimise toiminguid suunas spo.</span><span class="sxs-lookup"><span data-stu-id="1bbca-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="1bbca-108">Kui teil on probleeme ühendamisel SPO Management shelli, veenduge, et olete värskendatud uusimale versioonile ja proovige [uuesti importida moodul](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) *"Import-moodul Microsoft. online. SharePoint. PowerShell" abil.*</span><span class="sxs-lookup"><span data-stu-id="1bbca-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="1bbca-109">Kui proovite käivitada kliendipoolne objektimudeli skripte, peate oma kohalikku arvutisse installitud [SharePoint Online ' i kliendi komponendid SDK](https://www.microsoft.com/download/details.aspx?id=42038) .</span><span class="sxs-lookup"><span data-stu-id="1bbca-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="1bbca-110">Kui teil on probleeme, töötab PowerShelli skripte, võiksite kaaluda töötab PowerShelli administraatorina ja muuta [täitmise poliitika](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="1bbca-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>