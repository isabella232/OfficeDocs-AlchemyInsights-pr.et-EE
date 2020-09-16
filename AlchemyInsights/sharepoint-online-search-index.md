---
title: SharePoint Online ' is otsimine
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f790efbe6ed445786933efa3fc980f974693d1d9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770763"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="45bea-102">Sisu analüüsimine ja indekseerimine SharePoint Online ' is</span><span class="sxs-lookup"><span data-stu-id="45bea-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="45bea-103">Sisu tuleb analüüsida ja lisada kasutajate otsingu indeksisse, et leida, mida ta SharePoint Online ' is otsib.</span><span class="sxs-lookup"><span data-stu-id="45bea-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span>

- <span data-ttu-id="45bea-104">Veenduge, et sisu oleks leitav, [muutes saidi sisu otsitavaks](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="45bea-104">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="45bea-105">Kui olete hallatavat atribuuti muutnud või kui olete analüüsinud ja hallatavate atribuutide vastendust muutnud, tuleb sait uuesti analüüsida, enne kui teie muudatused kajastuvad otsingu registris.</span><span class="sxs-lookup"><span data-stu-id="45bea-105">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span>

- <span data-ttu-id="45bea-106">Lisateavet leiate teemast [saidi, teegi või loendi analüüsimise ja uuesti indekseerimise taotlemine käsitsi](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="45bea-106">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span>

- <span data-ttu-id="45bea-107">Oodake vähemalt 24 tundi pärast analüüsi ja täieliku uuesti indekseerimise taotlemist, et näha, kas teil on endiselt probleeme.</span><span class="sxs-lookup"><span data-stu-id="45bea-107">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span>

- <span data-ttu-id="45bea-108">Kui olete analüüsi ja täieliku uuesti indekseerimise algatamisest möödunud rohkem kui 24 tundi, logige sisse tugiteenuse juhtumi korral.</span><span class="sxs-lookup"><span data-stu-id="45bea-108">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="45bea-109">Paljudel juhtudel oleme juba lahendusega töötanud.</span><span class="sxs-lookup"><span data-stu-id="45bea-109">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="45bea-110">Lahenduse lõpetamiseks andke meile vähemalt 24 tundi.</span><span class="sxs-lookup"><span data-stu-id="45bea-110">Please give us at least 24 hours to complete a solution.</span></span>

<span data-ttu-id="45bea-111">**Oluline**: kui sait, dokument (teek) või loend on kustutatud ja kuvatakse otsingutulemite hulgas endiselt, tuleks kasutajatele kuvada **tõrketeade 404 faili ei leitud** , kui proovite sellele juurde pääseda.</span><span class="sxs-lookup"><span data-stu-id="45bea-111">**Important**: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="45bea-112">See probleem tuleks sisse logida täiendava uurimise jaoks mõeldud tugiteenuste juhtumina.</span><span class="sxs-lookup"><span data-stu-id="45bea-112">This issue should be logged as a support case for further investigation.</span></span>



