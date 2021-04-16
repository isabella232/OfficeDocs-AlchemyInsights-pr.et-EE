---
title: e-juurdluse ekspordi tööriist
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814584"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="20601-102">Kas te ei saa e-juurdluse ekspordi tööriista installida või käivitada?</span><span class="sxs-lookup"><span data-stu-id="20601-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="20601-103">Kui te ei saa otsingutulemite allalaadimiseks e-juurdluse ekspordi tööriista installida ega käivitada, kontrollige järgmist.</span><span class="sxs-lookup"><span data-stu-id="20601-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="20601-104">Arvuti, mida kasutate, vastab rekvisiitide nõuetele.</span><span class="sxs-lookup"><span data-stu-id="20601-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="20601-105">Windows 7 ja uuemate versioonide 32- või 64-bitised versioonid</span><span class="sxs-lookup"><span data-stu-id="20601-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="20601-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="20601-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="20601-107">Toetatud brauser:</span><span class="sxs-lookup"><span data-stu-id="20601-107">A supported browser:</span></span>

  - <span data-ttu-id="20601-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="20601-108">Microsoft Edge</span></span>

    <span data-ttu-id="20601-109">Või</span><span class="sxs-lookup"><span data-stu-id="20601-109">Or</span></span>

  - <span data-ttu-id="20601-110">Internet Explorer 10 ja uuemad versioonid</span><span class="sxs-lookup"><span data-stu-id="20601-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="20601-111">Muid brausereid (nt Google Chrome ja Mozilla Firefox) ei toetata.</span><span class="sxs-lookup"><span data-stu-id="20601-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="20601-112">Teie ettevõte saab luua ühenduse Azure'i lõpp-punktiga, **\* mis on .blob.core.windows.net** (metamärk tähistab teie eksporditöö kordumatut identifikaatorit).</span><span class="sxs-lookup"><span data-stu-id="20601-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="20601-113">Teile määratakse Microsoft 365 turbenõuete keskuses &amp; ekspordiroll.</span><span class="sxs-lookup"><span data-stu-id="20601-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="20601-114">Vaikimisi määratakse see roll ainult e-juurdluse halduri rollirühmale.</span><span class="sxs-lookup"><span data-stu-id="20601-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="20601-115">Lugege [teemat E-juurdluse õiguste määramine.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)</span><span class="sxs-lookup"><span data-stu-id="20601-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="20601-116">Lisateavet leiate teemast [Sisuotsingu tulemite eksportimine.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)</span><span class="sxs-lookup"><span data-stu-id="20601-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="20601-117">Kui ekspordite rohkem kui 100 K postkasti, peate tulemite eksportimiseks kasutama järgmist PowerShelli: tulemite eksportimine rohkem kui [100K postkastidest.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)</span><span class="sxs-lookup"><span data-stu-id="20601-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>