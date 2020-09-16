---
title: SharePoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: d90b60de72cf87a56e3b7f6a792708693f31af00
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770835"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="cdb99-102">SharePoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="cdb99-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="cdb99-103">Kas töötate SharePoint Online ' is PowerShelli või skriptide abil?</span><span class="sxs-lookup"><span data-stu-id="cdb99-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="cdb99-104">Lisateavet leiate allpool olevatest linkidest.</span><span class="sxs-lookup"><span data-stu-id="cdb99-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="cdb99-105">SharePoint Online ' i Management shelliga töötamise alustamine</span><span class="sxs-lookup"><span data-stu-id="cdb99-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="cdb99-106">SPO PowerShelliga ühenduse loomine (MFA)</span><span class="sxs-lookup"><span data-stu-id="cdb99-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="cdb99-107">[SharePointi mustrid ja tavad (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) sisaldab PowerShelli käskude teeki, mis võimaldab teil teha KEERULISI toiminguid SPO suunas.</span><span class="sxs-lookup"><span data-stu-id="cdb99-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="cdb99-108">Kui teil on probleeme SPO Management shelliga, veenduge, et olete uusima versiooni värskendanud ja proovite [uuesti importida moodulit](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) *"import-Module Microsoft. online. SharePoint. PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="cdb99-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="cdb99-109">Kui proovite käivitada kliendipoolse objektimudeli skripte, peab teil olema kohalikule seadmele installitud SharePoint Online ' i [klientrakenduse SDK](https://www.microsoft.com/download/details.aspx?id=42038) -s.</span><span class="sxs-lookup"><span data-stu-id="cdb99-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="cdb99-110">Kui teil on PowerShelli skriptide skriptimisega probleeme, võiksite kaaluda PowerShelli käitamist administraatorina ja [täitmise poliitika](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)muutmist.</span><span class="sxs-lookup"><span data-stu-id="cdb99-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>