---
title: Otsi SharePoint Online ' is
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c4ff98f0cf928834c803542340b32da15a40d583
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40044039"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="2a740-102">Sisu analüüsimine ja indekseerimine SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="2a740-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="2a740-103">Sisu tuleb analüüsida ja lisada kasutajate otsinguregistrisse, et leida, mida nad otsivad SharePoint Online ' is.</span><span class="sxs-lookup"><span data-stu-id="2a740-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="2a740-104">Sisu indekseerida automaatselt eelnevalt määratletud analüüsigraafiku alusel (analüüsigraafikut ei saa muuta).</span><span class="sxs-lookup"><span data-stu-id="2a740-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="2a740-105">Ämblik valib sisu, mis on muutunud pärast viimast analüüsi ja uuendab indeksit.</span><span class="sxs-lookup"><span data-stu-id="2a740-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="2a740-106">Et tagada sisu analüüsimine ja indeks värskendatakse, arvestage järgmist.</span><span class="sxs-lookup"><span data-stu-id="2a740-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="2a740-107">Veenduge, et sisu saab otsida, [muutes saidi sisu otsitavaks](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="2a740-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="2a740-108">Kui olete muutnud Hallatava atribuudi või kui olete muutnud analüüsitud ja hallatavate atribuutide vastendust, tuleb sait enne muudatuste kajastamist otsinguregistris uuesti indekseerida.</span><span class="sxs-lookup"><span data-stu-id="2a740-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="2a740-109">Kuna muudatused tehakse otsinguskeemis ja mitte tegeliku saidiga, ei Indekseeri ämblik saiti automaatselt ümber.</span><span class="sxs-lookup"><span data-stu-id="2a740-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="2a740-110">Lisateabe saamiseks vaadake [käsitsi päringu analüüsimine ja uuesti indekseerimine saidi, teegi või loendi](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="2a740-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="2a740-111">Oodake vähemalt 24 tundi pärast käsitsi analüüsi ja täielik uuesti indeks, et näha, kas teil on endiselt probleeme.</span><span class="sxs-lookup"><span data-stu-id="2a740-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="2a740-112">Kui pärast analüüsi algatamist ja täielikku uuesti indeksit on möödunud rohkem kui 24 tundi, logige palun tugiteenuse Teenindusjuhtumit.</span><span class="sxs-lookup"><span data-stu-id="2a740-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="2a740-113">Paljudel juhtudel oleme juba lahenduse kallal töötanud.</span><span class="sxs-lookup"><span data-stu-id="2a740-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="2a740-114">Palun andke meile vähemalt 24 tundi, et lahendus lõpule viia.</span><span class="sxs-lookup"><span data-stu-id="2a740-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="2a740-115">Kui sait, dokument (teek) või loend on kustutatud ja endiselt kuvatakse otsingutulemustes, kasutajad peaksid saama **tõrketeate 404 faili ei leitud** , kui proovite sellele juurde pääseda.</span><span class="sxs-lookup"><span data-stu-id="2a740-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="2a740-116">See probleem tuleks sisse logitud tugiteenuse juhtumi edasiseks uurimiseks.</span><span class="sxs-lookup"><span data-stu-id="2a740-116">This issue should be logged as a support case for further investigation.</span></span> 



