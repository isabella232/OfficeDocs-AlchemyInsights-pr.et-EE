---
title: 1491-Search-Not-returning-Expected-Results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 1491
ms.assetid: ''
ms.openlocfilehash: 517d9b75fc3aef09c0c2d5870aa695cc0ab10f06
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/22/2019
ms.locfileid: "30776078"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="d2c49-102">Otsing ei tagasta oodatavad tulemused</span><span class="sxs-lookup"><span data-stu-id="d2c49-102">Content Search not returning expected results</span></span>

<span data-ttu-id="d2c49-103">Sõites sisu otsingud: Office 365 turvalisus & vastavuse Center, saate ootamatu Otsingu tulemused.</span><span class="sxs-lookup"><span data-stu-id="d2c49-103">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="d2c49-104">Kaaluge järgmist asjad, mis võib mõjutada teie otsingu tulemused:</span><span class="sxs-lookup"><span data-stu-id="d2c49-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="d2c49-105">**Sisu kohtades ja Otsi tingimustes**: Veenduge, et valitud sisu ettenähtud kohas ja otsingu tingimused.</span><span class="sxs-lookup"><span data-stu-id="d2c49-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="d2c49-106">Kui käivitasite annab suur otsing (paljudes kohtades), kaaluda mitmeks mitu otsinguid.</span><span class="sxs-lookup"><span data-stu-id="d2c49-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="d2c49-107">**Osaliselt indekseeritud üksuste**: [osaliselt indekseeritud üksuste](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) postkastidest sisalduvad hinnanguline Otsingu tulemused.</span><span class="sxs-lookup"><span data-stu-id="d2c49-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="d2c49-108">Siiski osaliselt indekseeritud üksuste SharePointis või OneDrive saidid pole lisatud Otsi hinnang.</span><span class="sxs-lookup"><span data-stu-id="d2c49-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="d2c49-109">**Otsi vead**: palju postkaste (üle 100 000 postkastid) otsimisel võite saada Otsi tõrkeid, tõrkekoodide nagu CS008-009 ja CS012-002).</span><span class="sxs-lookup"><span data-stu-id="d2c49-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="d2c49-110">Sel juhul proovige uuesti otsida ainult ebaõnnestunud sisu asukohad.</span><span class="sxs-lookup"><span data-stu-id="d2c49-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="d2c49-111">Vaata [see artikkel](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) rohkem teavet.</span><span class="sxs-lookup"><span data-stu-id="d2c49-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
