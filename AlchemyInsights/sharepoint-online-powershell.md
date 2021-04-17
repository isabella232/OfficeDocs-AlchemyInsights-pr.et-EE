---
title: Sharepoint Online'i PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 839a70282b4dd619e9dbe8167ef0e409e468b1ad
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830578"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="6c7f0-102">Sharepoint Online'i PowerShell</span><span class="sxs-lookup"><span data-stu-id="6c7f0-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="6c7f0-103">Kas töötate PowerShelli või Skriptidega Sharepoint Online'is?</span><span class="sxs-lookup"><span data-stu-id="6c7f0-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="6c7f0-104">Lisateabe saamiseks külastage allolevaid linke.</span><span class="sxs-lookup"><span data-stu-id="6c7f0-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="6c7f0-105">SharePoint Online'i halduskestaga alustamine</span><span class="sxs-lookup"><span data-stu-id="6c7f0-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="6c7f0-106">SPO PowerShelliga ühenduse loomine mitme osalejaga autentimisega (MFA)</span><span class="sxs-lookup"><span data-stu-id="6c7f0-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="6c7f0-107">[SharePointi mustrid ja tavad (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) sisaldab PowerShelli käskude teeki, mis võimaldab SPO-ga teha keerukaid haldustoiminguid.</span><span class="sxs-lookup"><span data-stu-id="6c7f0-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="6c7f0-108">Kui teil on SPO halduskestaga ühenduse loomisel probleeme, veenduge, et [](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) olete uusimale versioonile üle võtnud ja proovige moodul uuesti importida *funktsiooni "Import-Module Microsoft.Online.SharePoint.PowerShell" abil.*</span><span class="sxs-lookup"><span data-stu-id="6c7f0-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="6c7f0-109">Kui proovite käitada kliendipoolseid objektimudeli skripte, peab kohalikusse arvutisse olema installitud Sharepoint Online'i kliendikomponentide [SDK.](https://www.microsoft.com/download/details.aspx?id=42038)</span><span class="sxs-lookup"><span data-stu-id="6c7f0-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="6c7f0-110">Kui teil on probleeme PowerShelli skriptide käivitamisega, võiksite kaaluda PowerShelli käivitamist administraatorina ja muuta [käivitamispoliitikat.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)</span><span class="sxs-lookup"><span data-stu-id="6c7f0-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>