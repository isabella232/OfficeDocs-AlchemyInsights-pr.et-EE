---
title: SharePointi või OneDrive ' is ei saa üksusi kustutada
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: db45aa8df40484fdcda7c430f1ca27482a1dd4ce
ms.sourcegitcommit: a9415f3ae8c7ba267b5134bcbdc1e070cea41a0f
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 11/12/2020
ms.locfileid: "49019579"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="dd10b-102">Üksusi ei saa kustutada</span><span class="sxs-lookup"><span data-stu-id="dd10b-102">Unable to delete items</span></span>

- <span data-ttu-id="dd10b-103">Säilituspoliitika võib seda põhjustada, peate kas keelama või välistama vastava ootelepaneku, mis seda probleemi põhjustab.</span><span class="sxs-lookup"><span data-stu-id="dd10b-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="dd10b-104">Pärast säilituspoliitika või ootelepaneku eemaldamist võib muudatuse jõustumiseks kuluda kuni 24 tundi.</span><span class="sxs-lookup"><span data-stu-id="dd10b-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="dd10b-105">Veenduge, et üksusel poleks [säilituspoliitika](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) seadistust.</span><span class="sxs-lookup"><span data-stu-id="dd10b-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="dd10b-106">Võimalik, et sait on ületanud salvestusruumi piirmäära, suurendama [saidi kvooti](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) ja kustutama üksuse.</span><span class="sxs-lookup"><span data-stu-id="dd10b-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

- <span data-ttu-id="dd10b-107">Veenduge, et üksus poleks teise kasutaja jaoks [välja möllitud](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) .</span><span class="sxs-lookup"><span data-stu-id="dd10b-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="dd10b-108">Administraatorid saavad kasutada [SharePointi mustreid ja tavasid](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), mis sisaldab PowerShelli käskude teeki, mis võimaldavad teil sooritada keerulisi haldus-toiminguid (nt jõu kustutamine kangekaelne üksused).</span><span class="sxs-lookup"><span data-stu-id="dd10b-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="dd10b-109">PNP-failis eemaldamine</span><span class="sxs-lookup"><span data-stu-id="dd10b-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="dd10b-110">Kausta PNP eemaldamine</span><span class="sxs-lookup"><span data-stu-id="dd10b-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="dd10b-111">PNP-loendiüksuse eemaldamine</span><span class="sxs-lookup"><span data-stu-id="dd10b-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="dd10b-112">PNP-loendi eemaldamine</span><span class="sxs-lookup"><span data-stu-id="dd10b-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="dd10b-113">Eemalda PNP väli (veerg)</span><span class="sxs-lookup"><span data-stu-id="dd10b-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)