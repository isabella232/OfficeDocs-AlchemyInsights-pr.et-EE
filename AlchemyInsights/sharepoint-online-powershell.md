---
title: SharePoint Online ' i PowerShelli
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 8c270748fc75f929371fbb2856daad3ae61a1540
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764257"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="f2598-102">SharePoint Online ' i PowerShelli</span><span class="sxs-lookup"><span data-stu-id="f2598-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="f2598-103">Töötamine PowerShelli või skriptidega SharePoint Online ' i raames?</span><span class="sxs-lookup"><span data-stu-id="f2598-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="f2598-104">Lisateabe saamiseks külastage allolevaid linke.</span><span class="sxs-lookup"><span data-stu-id="f2598-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="f2598-105">Alustamine SharePoint Online Management shelli</span><span class="sxs-lookup"><span data-stu-id="f2598-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="f2598-106">Ühendamine SPO PowerShelli mitme teguriga autentimine (MFA)</span><span class="sxs-lookup"><span data-stu-id="f2598-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="f2598-107">[SharePointi mustrid ja tavad (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) sisaldab teegi PowerShelli käsud, mis võimaldab teil sooritada keerukaid juhtimise toiminguid suunas spo.</span><span class="sxs-lookup"><span data-stu-id="f2598-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="f2598-108">Kui teil on probleeme ühendamisel SPO Management shelli, veenduge, et olete värskendatud uusimale versioonile ja proovige [uuesti importida moodul](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) *"Import-moodul Microsoft. online. SharePoint. PowerShell" abil.*</span><span class="sxs-lookup"><span data-stu-id="f2598-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="f2598-109">Kui proovite käivitada kliendipoolne objektimudeli skripte, peate oma kohalikku arvutisse installitud [SharePoint Online ' i kliendi komponendid SDK](https://www.microsoft.com/download/details.aspx?id=42038) .</span><span class="sxs-lookup"><span data-stu-id="f2598-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="f2598-110">Kui teil on probleeme, töötab PowerShelli skripte, võiksite kaaluda töötab PowerShelli administraatorina ja muuta [täitmise poliitika](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="f2598-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>