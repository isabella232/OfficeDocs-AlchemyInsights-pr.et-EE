---
title: Ei saa kustutada OneDrive'i või SharePointi üksuste
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: b25e6d144dcefcfed4258e78ad5cfd4089ba7d1e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36558649"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="9e9c4-102">Ei saa üksusi kustutada</span><span class="sxs-lookup"><span data-stu-id="9e9c4-102">Unable to delete items</span></span>

<span data-ttu-id="9e9c4-103">SharePointi üksuste kustutamine probleeme?</span><span class="sxs-lookup"><span data-stu-id="9e9c4-103">Having issues deleting SharePoint items?</span></span>

- <span data-ttu-id="9e9c4-104">Alati veenduge, et teil on [vastavad õigused](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) kustutada üksuse või [saidikogumi administraator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) katse üksuse eemaldada.</span><span class="sxs-lookup"><span data-stu-id="9e9c4-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="9e9c4-105">Tagada, et üksusel ei ole [säilituspoliitika](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup.</span><span class="sxs-lookup"><span data-stu-id="9e9c4-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="9e9c4-106">Tagada, et kaup ei ole mõnele teisele kasutajale [välja möllitud](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) .</span><span class="sxs-lookup"><span data-stu-id="9e9c4-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="9e9c4-107">Administraatorid saavad kasutada [SharePoint ja tavasid](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) mis sisaldab Raamatukogu PowerShelli käsud, mille abil saab keerulisi juhtimise toiminguid nagu sundida kangekaelne üksuste kustutamine.</span><span class="sxs-lookup"><span data-stu-id="9e9c4-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="9e9c4-108">PNP faili eemaldamiseks</span><span class="sxs-lookup"><span data-stu-id="9e9c4-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="9e9c4-109">PNP kausta eemaldamine</span><span class="sxs-lookup"><span data-stu-id="9e9c4-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="9e9c4-110">PNP loendiüksuse eemaldada</span><span class="sxs-lookup"><span data-stu-id="9e9c4-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="9e9c4-111">Eemalda PNP loend</span><span class="sxs-lookup"><span data-stu-id="9e9c4-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="9e9c4-112">Eemalda PNP väli (veerg)</span><span class="sxs-lookup"><span data-stu-id="9e9c4-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)