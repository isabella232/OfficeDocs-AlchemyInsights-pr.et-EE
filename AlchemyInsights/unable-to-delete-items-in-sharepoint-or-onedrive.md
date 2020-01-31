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
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571244"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="e5a7d-102">Üksusi ei saa kustutada</span><span class="sxs-lookup"><span data-stu-id="e5a7d-102">Unable to delete items</span></span>

<span data-ttu-id="e5a7d-103">Säilituspoliitikad võivad seda põhjustada, peate kas keelata või välistada vastava Hold, mis põhjustab probleemi.</span><span class="sxs-lookup"><span data-stu-id="e5a7d-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="e5a7d-104">Pärast säilituspoliitika või hoidke eemaldamist, võib kuluda kuni 24 tundi muudatuse jõustumiseks.</span><span class="sxs-lookup"><span data-stu-id="e5a7d-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="e5a7d-105">Veenduge, et üksusel pole [säilituspoliitika](https://docs.microsoft.com/office365/securitycompliance/retention-policies) seadistust.</span><span class="sxs-lookup"><span data-stu-id="e5a7d-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="e5a7d-106">Sait võib olla ületanud salvestuslimiidi, suurendada [saidikvooti](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) ja kustutada üksuse.</span><span class="sxs-lookup"><span data-stu-id="e5a7d-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="e5a7d-107">Veenduge, et üksus on [välja möllitud](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) teisele kasutajale.</span><span class="sxs-lookup"><span data-stu-id="e5a7d-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="e5a7d-108">Lõpuks administraatorid saavad kasutada [SharePointi mustrid ja tavad](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), mis sisaldab teegi PowerShelli käske, mis võimaldavad teil sooritada keerukaid haldustoiminguid, näiteks jõu kustutamine kangekaelsed üksused.</span><span class="sxs-lookup"><span data-stu-id="e5a7d-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="e5a7d-109">Eemalda PNP-fail</span><span class="sxs-lookup"><span data-stu-id="e5a7d-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="e5a7d-110">Eemalda PNP-kaust</span><span class="sxs-lookup"><span data-stu-id="e5a7d-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="e5a7d-111">PNP-loendi üksuse eemaldamine</span><span class="sxs-lookup"><span data-stu-id="e5a7d-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="e5a7d-112">Eemalda PNP-loend</span><span class="sxs-lookup"><span data-stu-id="e5a7d-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="e5a7d-113">Eemalda PNP-väli (veerg)</span><span class="sxs-lookup"><span data-stu-id="e5a7d-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)