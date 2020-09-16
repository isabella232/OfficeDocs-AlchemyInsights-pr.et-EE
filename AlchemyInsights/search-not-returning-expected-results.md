---
title: 1491-Search-Not-tagastamine-oodatud-tulemused
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740470"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="fabb3-102">Sisu otsing ei tagasta oodatud tulemeid</span><span class="sxs-lookup"><span data-stu-id="fabb3-102">Content Search not returning expected results</span></span>

<span data-ttu-id="fabb3-103">Microsoft 365 turbe & nõuetele vastavuse keskuses sisu otsimisel võidakse kuvada ootamatud otsingutulemused.</span><span class="sxs-lookup"><span data-stu-id="fabb3-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="fabb3-104">Arvestage järgmiste asjadega, mis võivad teie otsingutulemusi mõjutada.</span><span class="sxs-lookup"><span data-stu-id="fabb3-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="fabb3-105">**Sisu asukohad ja otsingukriteeriumid**: Veenduge, et olete valinud õige sisu asukohad ja otsingu tingimused.</span><span class="sxs-lookup"><span data-stu-id="fabb3-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="fabb3-106">Kui käivitasite suure otsingu (paljudes asukohtades), kaaluge selle tükeldamist mitmeks otsinguks.</span><span class="sxs-lookup"><span data-stu-id="fabb3-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="fabb3-107">**Osaliselt indekseeritud üksused**: postkastidest  [osaliselt indekseeritud üksused](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) kaasatakse hinnangulise otsingu tulemisse.</span><span class="sxs-lookup"><span data-stu-id="fabb3-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="fabb3-108">Siiski ei kuulu SharePointi ja OneDrive ' i saitidelt osaliselt indekseeritud üksused otsingu hinnangusse.</span><span class="sxs-lookup"><span data-stu-id="fabb3-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="fabb3-109">**Otsingu tõrked**: suurel hulgal postkastidest (üle 100 000 postkasti) otsimisel võite saada tõrketeateid, kus on tõrkekoodid (nt CS008-009 ja CS012-002).</span><span class="sxs-lookup"><span data-stu-id="fabb3-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="fabb3-110">Sellisel juhul proovige otsingut ainult ebaõnnestunud sisu asukohtade korral.</span><span class="sxs-lookup"><span data-stu-id="fabb3-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="fabb3-111">Lisateavet leiate  [sellest artiklist](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .</span><span class="sxs-lookup"><span data-stu-id="fabb3-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
