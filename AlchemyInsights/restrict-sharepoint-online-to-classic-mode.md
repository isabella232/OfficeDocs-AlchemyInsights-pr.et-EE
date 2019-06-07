---
title: Klassikalises režiimis SharePoint Online piiramiseks
ms.author: kirks
author: Techwriter40
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.openlocfilehash: 76f0b5ed67d3220559d25dfd72c7535181a4513b
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34761755"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="a52ba-102">Klassikalises režiimis SharePoint Online piiramiseks</span><span class="sxs-lookup"><span data-stu-id="a52ba-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="a52ba-103">Mõned organisatsioonid vajavad ikka klassikaline režiimi kogemus.</span><span class="sxs-lookup"><span data-stu-id="a52ba-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="a52ba-104">Kui ei ole plaanis eemaldada klassikalises režiimis granuleeritud tasandil, ei ole enam võimalik piirata klassikaliste režiim loendite ja teekide terve organisatsiooni (rentnik).</span><span class="sxs-lookup"><span data-stu-id="a52ba-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="a52ba-105">Admin on hallata üksikute loendite ja teekide abil granuleeritud loobuda lülitid, et pakume järgmiste huvigruppide classic mode valida järgmist:</span><span class="sxs-lookup"><span data-stu-id="a52ba-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="a52ba-106">saidikogumi</span><span class="sxs-lookup"><span data-stu-id="a52ba-106">site collection</span></span>
- <span data-ttu-id="a52ba-107">saidi</span><span class="sxs-lookup"><span data-stu-id="a52ba-107">site</span></span>
- <span data-ttu-id="a52ba-108">nimekiri</span><span class="sxs-lookup"><span data-stu-id="a52ba-108">list</span></span>
- <span data-ttu-id="a52ba-109">Raamatukogu</span><span class="sxs-lookup"><span data-stu-id="a52ba-109">library</span></span>

<span data-ttu-id="a52ba-110">Lisaks loendite, et teatud funktsioonide kasutamiseks ja kohandused, mis ei toeta modern viiakse ikka automaatselt üle klassikalises režiimis.</span><span class="sxs-lookup"><span data-stu-id="a52ba-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="a52ba-111">Alates 1 aprill 2019, keelata rentniku tasandil protsessi loobuda kaasaegne nimekirja ja raamatukogude alustada ja jätkata läbi 31 mai 2019.</span><span class="sxs-lookup"><span data-stu-id="a52ba-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="a52ba-112">Loendid ja teegid, mis on klassikalise režiimi tõttu rentniku loobuda on nihkunud automaatselt kaasaegne.</span><span class="sxs-lookup"><span data-stu-id="a52ba-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="a52ba-113">Kui vajate klassikalises režiimis leiate rohkem teavet [siin](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) ja PnP PowerShelli juhiseid [siin](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) kirjeldatud võimalusi ja vahendeid, mida saate kasutada klassikalise režiimi kogemus täna.</span><span class="sxs-lookup"><span data-stu-id="a52ba-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
