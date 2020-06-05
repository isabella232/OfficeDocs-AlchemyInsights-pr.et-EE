---
title: 1332 OWA-sisendkausta reegli (s) ei ole tööd postkasti
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 9abdcdcb33d39b8b9fe2df80f0c15a8b55e465fd
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/05/2020
ms.locfileid: "44576556"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="4772c-102">Sisendkausta reegel ei tööta ootuspäraselt</span><span class="sxs-lookup"><span data-stu-id="4772c-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="4772c-103">Kontrollige Outlooki veebis järgmisi sätteid:</span><span class="sxs-lookup"><span data-stu-id="4772c-103">Verify the following settings in Outlook on the web:</span></span>

- <span data-ttu-id="4772c-104">Sõnumit saab ümber suunata, edastada või vastas automaatselt sisendkausta reeglite alusel ainult üks kord.</span><span class="sxs-lookup"><span data-stu-id="4772c-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="4772c-105">Ümbersuunamisreegel (sisendkausta reegel või meilivoo reegel, tuntud ka kui transpordireegel) saab sõnumile lisada kuni kümme edasisaatmise adressaati.</span><span class="sxs-lookup"><span data-stu-id="4772c-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="4772c-106">Lisateabe saamiseks vaadake [töölehte, transport ja sisendkausta reegli piirangud](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="4772c-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="4772c-107">Sisendkausta reeglid ei tööta alternatiivse päevikuna postkasti.</span><span class="sxs-lookup"><span data-stu-id="4772c-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="4772c-108">Alternatiivse päevikuva postkasti kohta lisateabe saamiseks vaadake [alternatiivse päevikust postkasti](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="4772c-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="4772c-109">Nende probleemide lahendamiseks vaadake [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="4772c-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="4772c-110">Kui eelmised probleemid ei kehti, käivitage sisendkausta reegli diagnostika aruande enne, kui edastate probleemi Microsoft Support:</span><span class="sxs-lookup"><span data-stu-id="4772c-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="4772c-111">Avage postkast Outlook Web ja klõpsake</span><span class="sxs-lookup"><span data-stu-id="4772c-111">Open the mailbox in Outlook on the web, and click</span></span> <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 <span data-ttu-id="4772c-112">**Seadistusi**  >  **Kuva kõik Outlooki sätted**  >  **Posti**  >  **Eeskirjadega**.</span><span class="sxs-lookup"><span data-stu-id="4772c-112">**Settings** > **View all Outlook Settings** > **Mail** > **Rules**.</span></span>

2. <span data-ttu-id="4772c-113">Klõpsake lehe allosas, **kui teie reeglid ei tööta, klõpsake diagnostika aruande loomiseks**.</span><span class="sxs-lookup"><span data-stu-id="4772c-113">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
