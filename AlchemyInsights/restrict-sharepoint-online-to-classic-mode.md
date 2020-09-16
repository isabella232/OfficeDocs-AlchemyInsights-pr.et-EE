---
title: SharePoint Online ' i piiramine klassikalises režiimis
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751418"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="119a0-102">SharePoint Online ' i piiramine klassikalises režiimis</span><span class="sxs-lookup"><span data-stu-id="119a0-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="119a0-103">Mõned organisatsioonid vajavad endiselt klassikalist režiimi kogemust.</span><span class="sxs-lookup"><span data-stu-id="119a0-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="119a0-104">Ehkki klassikalise režiimi eemaldamine granuleeritud tasemel pole kavas, pole enam võimalik piirata kogu organisatsiooni (rentniku) loendites ja teekides klassikalise režiimini.</span><span class="sxs-lookup"><span data-stu-id="119a0-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="119a0-105">Administraatoril on järgmised võimalused üksikute loendite ja teekide haldamiseks klassikalises režiimis, kasutades granuleeritud opt-Outi lüliteid, mida pakume järgmistes tasemetes.</span><span class="sxs-lookup"><span data-stu-id="119a0-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="119a0-106">saidikogum</span><span class="sxs-lookup"><span data-stu-id="119a0-106">site collection</span></span>
- <span data-ttu-id="119a0-107">saidi</span><span class="sxs-lookup"><span data-stu-id="119a0-107">site</span></span>
- <span data-ttu-id="119a0-108">lisanud</span><span class="sxs-lookup"><span data-stu-id="119a0-108">list</span></span>
- <span data-ttu-id="119a0-109">Raamatukogu</span><span class="sxs-lookup"><span data-stu-id="119a0-109">library</span></span>

<span data-ttu-id="119a0-110">Lisaks on loendid, mis kasutavad teatud funktsioone ja kohandusi, mida Modern ei toeta, endiselt automaatselt Klassikaliseks režiimis.</span><span class="sxs-lookup"><span data-stu-id="119a0-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="119a0-111">Alates aprillist 1, 2019, protsess, mis keelab rentniku taseme, loobumine kaasaegsest loendist ja teekidest algab ja jätkub kuni 31 mai 2019.</span><span class="sxs-lookup"><span data-stu-id="119a0-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="119a0-112">Rentniku loobumise tõttu klassikalises režiimis olevad loendid ja teegid nihkuvad automaatselt moodsaks.</span><span class="sxs-lookup"><span data-stu-id="119a0-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="119a0-113">Kui vajate klassikalist režiimi, leiate [siit](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) lisateavet ja PnP PowerShelli [juhiseid,](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) mis kirjeldavad suvandeid ja tööriistu, mida saate kasutada klassikalise režiimi kogemuse kasutamiseks.</span><span class="sxs-lookup"><span data-stu-id="119a0-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
