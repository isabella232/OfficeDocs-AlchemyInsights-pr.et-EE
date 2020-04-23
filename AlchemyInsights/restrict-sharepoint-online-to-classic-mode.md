---
title: SharePoint Online ' i piiramine klassikalise režiimiga
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: c5ea5d264b62e4c349623bd431776207b38da470
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742465"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="db3a0-102">SharePoint Online ' i piiramine klassikalise režiimiga</span><span class="sxs-lookup"><span data-stu-id="db3a0-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="db3a0-103">Mõned organisatsioonid vajavad endiselt klassikalise režiimi kogemust.</span><span class="sxs-lookup"><span data-stu-id="db3a0-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="db3a0-104">Kuigi ei ole plaanid eemaldada klassikalise režiimi granuleeritud tasemel, ei ole enam võimalik piirata kogu organisatsiooni (rentniku) klassikaline režiim loendid ja teegid.</span><span class="sxs-lookup"><span data-stu-id="db3a0-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="db3a0-105">Administraatoril on järgmised võimalused üksikute loendite ja teekide haldamiseks klassikalises režiimis, kasutades granuleeritud loobumislüliteid, mida pakume järgmistel tasemetel:</span><span class="sxs-lookup"><span data-stu-id="db3a0-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="db3a0-106">saidikogumi</span><span class="sxs-lookup"><span data-stu-id="db3a0-106">site collection</span></span>
- <span data-ttu-id="db3a0-107">Saidi</span><span class="sxs-lookup"><span data-stu-id="db3a0-107">site</span></span>
- <span data-ttu-id="db3a0-108">Nimekiri</span><span class="sxs-lookup"><span data-stu-id="db3a0-108">list</span></span>
- <span data-ttu-id="db3a0-109">Raamatukogu</span><span class="sxs-lookup"><span data-stu-id="db3a0-109">library</span></span>

<span data-ttu-id="db3a0-110">Lisaks on loendid, mis kasutavad teatud funktsioone ja kohandused, mis ei toeta kaasaegne ikka automaatselt sisse klassikaline režiim.</span><span class="sxs-lookup"><span data-stu-id="db3a0-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="db3a0-111">Alates aprill 1, 2019, protsess keelata rentniku tase loobuda kaasaegne nimekiri ja teegid algavad ja jätkavad mai 31, 2019.</span><span class="sxs-lookup"><span data-stu-id="db3a0-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="db3a0-112">Loendid ja teegid, mis on klassikalise režiimi tulemusena rentniku loobumine-out automaatselt nihkunud kaasaegne.</span><span class="sxs-lookup"><span data-stu-id="db3a0-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="db3a0-113">Kui vajate klassikalist režiimi, vaadake lisateavet [siit](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) ja PnP PowerShelli juhis [siin](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) , mis kirjeldab võimalusi ja tööriistu, mida saate kasutada tänapäeval klassikalise režiimi kogemuse kasutamiseks.</span><span class="sxs-lookup"><span data-stu-id="db3a0-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
