---
title: SharePointi või OneDrive ' is ei saa üksusi kustutada
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: cc19fcb6603160032dac52b1ec9e194a90b7891f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049513"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="fe7af-102">Üksusi ei saa kustutada</span><span class="sxs-lookup"><span data-stu-id="fe7af-102">Unable to delete items</span></span>

<span data-ttu-id="fe7af-103">Kas SharePointi üksuste kustutamisel on probleeme?</span><span class="sxs-lookup"><span data-stu-id="fe7af-103">Having issues deleting SharePoint items?</span></span>

- <span data-ttu-id="fe7af-104">Veenduge alati, et teil on üksuse kustutamiseks [vajalikud õigused](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) või kui [saidikogumi administraator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) proovib üksust eemaldada.</span><span class="sxs-lookup"><span data-stu-id="fe7af-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="fe7af-105">Veenduge, et üksusel pole [säilituspoliitika](https://docs.microsoft.com/office365/securitycompliance/retention-policies) seadistust.</span><span class="sxs-lookup"><span data-stu-id="fe7af-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="fe7af-106">Veenduge, et üksus on [välja möllitud](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) teisele kasutajale.</span><span class="sxs-lookup"><span data-stu-id="fe7af-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="fe7af-107">Lõpuks administraatorid saavad kasutada [SharePointi mustrid ja tavad](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), mis sisaldab teegi PowerShelli käske, mis võimaldavad teil sooritada keerukaid haldustoiminguid, näiteks jõu kustutamine kangekaelsed üksused.</span><span class="sxs-lookup"><span data-stu-id="fe7af-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="fe7af-108">Eemalda PNP-fail</span><span class="sxs-lookup"><span data-stu-id="fe7af-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="fe7af-109">Eemalda PNP-kaust</span><span class="sxs-lookup"><span data-stu-id="fe7af-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="fe7af-110">PNP-loendi üksuse eemaldamine</span><span class="sxs-lookup"><span data-stu-id="fe7af-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="fe7af-111">Eemalda PNP-loend</span><span class="sxs-lookup"><span data-stu-id="fe7af-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="fe7af-112">Eemalda PNP-väli (veerg)</span><span class="sxs-lookup"><span data-stu-id="fe7af-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)