---
title: Otsi SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: fc49978fbd2c07381dae83061b1a1868cd1df0d0
ms.sourcegitcommit: 327a2c77afc2ff3d67d3aaaea1a92068a3c4bb1f
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/06/2019
ms.locfileid: "36059248"
---
# <a name="search-in-sharepoint-online"></a><span data-ttu-id="6b08a-102">Otsi SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="6b08a-102">Search in SharePoint Online</span></span>

<span data-ttu-id="6b08a-103">Sisu peab olema analüüsitud ja kasutajatel leida, mida nad otsivad SharePoint Online otsinguregistrisse lisatud.</span><span class="sxs-lookup"><span data-stu-id="6b08a-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="6b08a-104">Sisu automaatselt analüüsimisel vastavalt eelmääratletud indekseerimise ajakava (indekseerimise ajakava ei saa muuta).</span><span class="sxs-lookup"><span data-stu-id="6b08a-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="6b08a-105">Ämblik kirkad, mis on muutunud pärast viimast analüüsi ja uuendab indeks.</span><span class="sxs-lookup"><span data-stu-id="6b08a-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="6b08a-106">Et sisu analüüsimisel ja registrit värskendatakse, võtke arvesse järgmist.</span><span class="sxs-lookup"><span data-stu-id="6b08a-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="6b08a-107">Veenduge, et sisu leiate [saidi sisu otsida](https://docs.microsoft.com/sharepoint/make-site-content-searchable)tehes.</span><span class="sxs-lookup"><span data-stu-id="6b08a-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="6b08a-108">Hallatava atribuudi muutmist või muutmist kaardistamine analüüsitud ja õnnestus omadused, saidil tuleb uuesti analüüsitud enne tehtud muudatused kajastuvad nii.</span><span class="sxs-lookup"><span data-stu-id="6b08a-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="6b08a-109">Kuna muudatused tehakse otsingu skeemi ning mitte tegelik saidi ämblik hakkab automaatselt uuesti indekseerida saidi.</span><span class="sxs-lookup"><span data-stu-id="6b08a-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="6b08a-110">Lisateavet vt [indekseerimise ja uuesti indekseerimise saidi, teegi või loendi käsitsi taotleda](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="6b08a-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="6b08a-111">Oota vähemalt 24 tundi pärast analüüsi ja täieliku uuesti indekseerida näha, kui ei kao probleemi käsitsi taotleda.</span><span class="sxs-lookup"><span data-stu-id="6b08a-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="6b08a-112">Kui üle 24 tunni on möödunud tegemisest analüüsi ja täieliku uuesti indekseerida, logige esitamist.</span><span class="sxs-lookup"><span data-stu-id="6b08a-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="6b08a-113">Paljudel juhtudel arendame juba lahenduse.</span><span class="sxs-lookup"><span data-stu-id="6b08a-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="6b08a-114">Palun anna meile vähemalt 24 tundi, lahendus.</span><span class="sxs-lookup"><span data-stu-id="6b08a-114">Please give us at least 24 hours to complete a solution.</span></span>

>[! Oluline!]<span data-ttu-id="6b08a-115">: saidi, dokumendi (Raamatukogu) või nimekiri oli kustutatud ja ikka näitab tulemusi, kui kasutajatele tuleks on **Error 404 faili ei leitud** katsel kuvatakse juurdepääs.</span><span class="sxs-lookup"><span data-stu-id="6b08a-115">: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="6b08a-116">See probleem peaks olema logitud esitamist palusid.</span><span class="sxs-lookup"><span data-stu-id="6b08a-116">This issue should be logged as a support case for further investigation.</span></span> 



