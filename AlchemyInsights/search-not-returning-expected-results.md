---
title: 1491-otsing-mitte-tagasi oodatud-tulemused
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 57421d459ef03049d6f931db659a5f9b253f5002
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510568"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="483c0-102">Sisu otsing ei tagasta oodatud tulemusi</span><span class="sxs-lookup"><span data-stu-id="483c0-102">Content Search not returning expected results</span></span>

<span data-ttu-id="483c0-103">Microsoft 365 Security & vastavuse Center sisu otsingud käivitamisel võidakse kuvada ootamatuid otsingutulemeid.</span><span class="sxs-lookup"><span data-stu-id="483c0-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="483c0-104">Kaaluge järgmisi toiminguid, mis võivad teie otsingutulemeid mõjutada:</span><span class="sxs-lookup"><span data-stu-id="483c0-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="483c0-105">**Sisu asukohad ja otsingutingimused**: Veenduge, et olete valinud õiged sisu asukohad ja otsingutingimused.</span><span class="sxs-lookup"><span data-stu-id="483c0-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="483c0-106">Kui te käivitasite suure otsingu (paljude asukohtadest), kaaluge selle tükeldamist mitmesse otsingusse.</span><span class="sxs-lookup"><span data-stu-id="483c0-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="483c0-107">**Osaliselt indekseeritud üksused**: postkastidest [osaliselt indekseeritud üksused](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) kaasatakse hinnangulisest otsingutulemustest.</span><span class="sxs-lookup"><span data-stu-id="483c0-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="483c0-108">Kuid osaliselt indekseeritud üksused SharePoint ja OneDrive saidid ei sisaldu otsingu hinnang.</span><span class="sxs-lookup"><span data-stu-id="483c0-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="483c0-109">**Otsingu tõrked**: otsides suur hulk postkastid (üle 100 000 postkastid), võite saada otsingu tõrked, TÕRKEKOODIDEST nagu CS008-009 ja CS012-002).</span><span class="sxs-lookup"><span data-stu-id="483c0-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="483c0-110">Sel juhul proovige otsingut ainult nurjunud sisu asukohtade puhul.</span><span class="sxs-lookup"><span data-stu-id="483c0-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="483c0-111">Vaadake [seda artiklit](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) lisateabe saamiseks.</span><span class="sxs-lookup"><span data-stu-id="483c0-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
