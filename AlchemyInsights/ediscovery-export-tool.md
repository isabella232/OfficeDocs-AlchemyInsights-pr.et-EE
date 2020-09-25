---
title: e-juurdluse ekspordi tööriist
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277946"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="2da23-102">E-juurdluse ekspordi tööriista ei saa installida või käivitada?</span><span class="sxs-lookup"><span data-stu-id="2da23-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="2da23-103">Kui te ei saa otsingutulemite allalaadimiseks e-juurdluse ekspordi tööriista installida ega käivitada, kontrollige järgmisi asju.</span><span class="sxs-lookup"><span data-stu-id="2da23-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="2da23-104">Arvuti, mida kasutate, vastab järgmistele eeltingimustele:</span><span class="sxs-lookup"><span data-stu-id="2da23-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="2da23-105">32-või 64-bitised versioonid Windows 7 ja uuemad versioonid</span><span class="sxs-lookup"><span data-stu-id="2da23-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="2da23-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="2da23-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="2da23-107">Toetatud brauser.</span><span class="sxs-lookup"><span data-stu-id="2da23-107">A supported browser:</span></span>

  - <span data-ttu-id="2da23-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="2da23-108">Microsoft Edge</span></span>

    <span data-ttu-id="2da23-109">Või</span><span class="sxs-lookup"><span data-stu-id="2da23-109">Or</span></span>

  - <span data-ttu-id="2da23-110">Internet Explorer 10 ja uuemad versioonid</span><span class="sxs-lookup"><span data-stu-id="2da23-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="2da23-111">Muud brauserid (nt Google Chrome ja Mozilla Firefox) ei toeta.</span><span class="sxs-lookup"><span data-stu-id="2da23-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="2da23-112">Teie asutus saab luua ühenduse lõpp-punktiga Azure ' is, mis on \*\* \* . blob.Core.Windows.net\*\* (metamärki tähistab teie eksporditoimingu kordumatut identifikaatorit).</span><span class="sxs-lookup"><span data-stu-id="2da23-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="2da23-113">Olete määranud ekspordi rolli Microsoft 365 turbe &amp; nõuetele vastavuse keskuses.</span><span class="sxs-lookup"><span data-stu-id="2da23-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="2da23-114">Vaikimisi määratakse see roll ainult e-juurdluse halduri rollirühma.</span><span class="sxs-lookup"><span data-stu-id="2da23-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="2da23-115">Vaadake teemat e- [juurdluse õiguse määramine](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span><span class="sxs-lookup"><span data-stu-id="2da23-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="2da23-116">Lisateavet leiate teemast [sisu otsingutulemite eksportimine](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span><span class="sxs-lookup"><span data-stu-id="2da23-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="2da23-117">Kui ekspordite rohkem kui 100K postkaste, peate eksportimise tulemite allalaadimiseks kasutama järgmist PowerShelli, et eksportida  [tulemid enam kui 100k postkastist](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="2da23-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>