---
title: SharePoint Online PowerShell
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 300c07e7f0010eae2bd4fe893ece9d09aab93ba5
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786885"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="f9776-102">SharePoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="f9776-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="f9776-103">Kas töötate SharePoint Online ' is PowerShelli või skriptide abil?</span><span class="sxs-lookup"><span data-stu-id="f9776-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="f9776-104">Lisateavet leiate allpool olevatest linkidest.</span><span class="sxs-lookup"><span data-stu-id="f9776-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="f9776-105">SharePoint Online ' i Management shelliga töötamise alustamine</span><span class="sxs-lookup"><span data-stu-id="f9776-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="f9776-106">SPO PowerShelliga ühenduse loomine (MFA)</span><span class="sxs-lookup"><span data-stu-id="f9776-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="f9776-107">[SharePointi mustrid ja tavad (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) sisaldab PowerShelli käskude teeki, mis võimaldab teil teha KEERULISI toiminguid SPO suunas.</span><span class="sxs-lookup"><span data-stu-id="f9776-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="f9776-108">Kui teil on probleeme SPO Management shelliga, veenduge, et olete uusima versiooni värskendanud ja proovite [uuesti importida moodulit](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) *"import-Module Microsoft. online. SharePoint. PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="f9776-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="f9776-109">Kui proovite käivitada kliendipoolse objektimudeli skripte, peab teil olema kohalikule seadmele installitud SharePoint Online ' i [klientrakenduse SDK](https://www.microsoft.com/download/details.aspx?id=42038) -s.</span><span class="sxs-lookup"><span data-stu-id="f9776-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="f9776-110">Kui teil on PowerShelli skriptide skriptimisega probleeme, võiksite kaaluda PowerShelli käitamist administraatorina ja [täitmise poliitika](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)muutmist.</span><span class="sxs-lookup"><span data-stu-id="f9776-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>