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
ms.openlocfilehash: 7d1848830847fc6722da20e09a4875f49bf02bd3
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35360913"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="6b891-102">Sisendkausta reegel ei tööta ootuspäraselt</span><span class="sxs-lookup"><span data-stu-id="6b891-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="6b891-103">Kontrollige järgmisi sätteid:</span><span class="sxs-lookup"><span data-stu-id="6b891-103">Verify the following settings:</span></span>

- <span data-ttu-id="6b891-104">Sõnumi saab ümber, saata või vastatavate automaatselt vastavalt sisendkaustareeglid ainult üks kord.</span><span class="sxs-lookup"><span data-stu-id="6b891-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="6b891-105">Ümbersuunamine reegli (reegel või ka Transpordireegli voolu meilireegel) lisada maksimaalselt kümme edastamine adressaadile sõnumi.</span><span class="sxs-lookup"><span data-stu-id="6b891-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="6b891-106">Lisateavet [töölehe, Transport, ja sisse piiratud](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="6b891-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="6b891-107">Sisendkausta reeglid ei tööta alternatiivse päevikupidamise postkasti.</span><span class="sxs-lookup"><span data-stu-id="6b891-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="6b891-108">Alternatiivne päevikupidamise postkasti kohta lisateabe saamiseks vt [alternatiivse päevikupidamise postkasti](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="6b891-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="6b891-109">Nende probleemide lahendamiseks Vaata [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="6b891-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="6b891-110">Kui eelmistest ei rakenda, aruannet sisendkausta reegel diagnostika enne te edastage probleemi Microsoft Support:</span><span class="sxs-lookup"><span data-stu-id="6b891-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="6b891-111">Postkasti Outlook Web avada, ja klõpsake nuppu **sätted** \> **Valikud** \> **Korralda e-posti** \> **sisendkausta reeglid**.</span><span class="sxs-lookup"><span data-stu-id="6b891-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>

2. <span data-ttu-id="6b891-112">Lehe allosas nuppu, **kui teie reeglid ei tööta diagnostika aruande loomiseks klõpsake siin**.</span><span class="sxs-lookup"><span data-stu-id="6b891-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
