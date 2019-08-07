---
title: 1332 OWA - sisendkausta reeglid ei täidavad postkasti
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 218a05a8d321b76dd07345ea48d6b3e158cc120e
ms.sourcegitcommit: 77f704672b7c7de541899e25c022ff10c111e304
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2019
ms.locfileid: "36204056"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="a994b-102">Sisendkausta reegel ei tööta ootuspäraselt</span><span class="sxs-lookup"><span data-stu-id="a994b-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="a994b-103">Kontrollige järgmisi sätteid:</span><span class="sxs-lookup"><span data-stu-id="a994b-103">Verify the following settings:</span></span>

- <span data-ttu-id="a994b-104">Sõnumi saab ümber, saata või vastatavate automaatselt vastavalt sisendkaustareeglid ainult üks kord.</span><span class="sxs-lookup"><span data-stu-id="a994b-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="a994b-105">Ümbersuunamine reegli (reegel või ka Transpordireegli voolu meilireegel) lisada maksimaalselt kümme edastamine adressaadile sõnumi.</span><span class="sxs-lookup"><span data-stu-id="a994b-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="a994b-106">Lisateavet [töölehe, Transport, ja sisse piiratud](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="a994b-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="a994b-107">Sisendkausta reeglid ei tööta alternatiivse päevikupidamise postkasti.</span><span class="sxs-lookup"><span data-stu-id="a994b-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="a994b-108">Alternatiivne päevikupidamise postkasti kohta lisateabe saamiseks vt [alternatiivse päevikupidamise postkasti](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="a994b-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="a994b-109">Nende probleemide lahendamiseks Vaata [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="a994b-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="a994b-110">Kui eelmistest ei rakenda, aruannet sisendkausta reegel diagnostika enne te edastage probleemi Microsoft Support:</span><span class="sxs-lookup"><span data-stu-id="a994b-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="a994b-111">Avage Outlook Web postkast ja klõpsake</span><span class="sxs-lookup"><span data-stu-id="a994b-111">Open the mailbox in Outlook on the web, and click</span></span> <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 <span data-ttu-id="a994b-112">**Seaded** > **kõik Outlooki sätete vaatamine** > **Mail** > **reeglid**.</span><span class="sxs-lookup"><span data-stu-id="a994b-112">**Settings** > **View all Outlook Settings** > **Mail** > **Rules**.</span></span>

2. <span data-ttu-id="a994b-113">Lehe allosas nuppu, **kui teie reeglid ei tööta diagnostika aruande loomiseks klõpsake siin**.</span><span class="sxs-lookup"><span data-stu-id="a994b-113">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
