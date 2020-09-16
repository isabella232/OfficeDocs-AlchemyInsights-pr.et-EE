---
title: SharePoint Online ' i otsingu skeemi haldamine
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f2d8d3e07fe32d21af484e4c59e0f5ac6fe8081c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770547"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="15d7d-102">SharePoint Online ' i otsingu skeemi haldamine</span><span class="sxs-lookup"><span data-stu-id="15d7d-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="15d7d-103">Otsingu skeem reguleerib seda, mida kasutajad saavad otsida, kuidas kasutajad saavad seda otsida ja kuidas saate oma otsingu veebisaitidel tulemusi esitada.</span><span class="sxs-lookup"><span data-stu-id="15d7d-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="15d7d-104">Lisateavet leiate teemast [SharePoint Online ' i otsingu skeemi haldamine](https://docs.microsoft.com/sharepoint/manage-search-schema) .</span><span class="sxs-lookup"><span data-stu-id="15d7d-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="15d7d-105">Muutke otsingu skeemi.</span><span class="sxs-lookup"><span data-stu-id="15d7d-105">Change the search schema.</span></span>
- <span data-ttu-id="15d7d-106">Hallatavate atribuutide loomine.</span><span class="sxs-lookup"><span data-stu-id="15d7d-106">Create managed properties.</span></span>
- <span data-ttu-id="15d7d-107">Vastendus analüüsitud vastenduse vastendatud atribuutidega hallatavatele atribuutidele.</span><span class="sxs-lookup"><span data-stu-id="15d7d-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="15d7d-108">Uurige oma otsingu skeemi haldamise osas järgmist.</span><span class="sxs-lookup"><span data-stu-id="15d7d-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="15d7d-109">Kui teile kuvatakse hoiatus, mis kinnitab, **et rakendus on** skeemi muutmisel peatatud, on see ainult ajutiselt, sest teenuse hooldust esineb.</span><span class="sxs-lookup"><span data-stu-id="15d7d-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="15d7d-110">Kui möödunud on rohkem kui 24 tundi ja teil esineb endiselt hoiatusi, logige sisse tugiteenuste juhtumi korral.</span><span class="sxs-lookup"><span data-stu-id="15d7d-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="15d7d-111">Kui muudate hallatavaid atribuute või lisate uusi, jõustuvad muudatused alles pärast seda, kui sisu on uuesti analüüsitud.</span><span class="sxs-lookup"><span data-stu-id="15d7d-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="15d7d-112">SharePoint Online ' is toimub analüüsimine automaatselt määratletud analüüsi ajakava põhjal.</span><span class="sxs-lookup"><span data-stu-id="15d7d-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="15d7d-113">Kui soovite veenduda, et muudatused on analüüsitud, saate [taotleda loendi või teegi uuesti indekseerimist.](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="15d7d-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="15d7d-114">Otsingu skeemi põhjaliku ülevaate leiate teemast [Otsingu skeemi tutvustus](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="15d7d-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


