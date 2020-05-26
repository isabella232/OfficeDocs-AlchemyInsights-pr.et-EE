---
title: Kas vajate abi meili saatmise piirangutega?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 7f563df313c869d18c3e4240d271c649a74914af
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357545"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="c42cd-102">Kas vajate abi meili saatmise piirangutega?</span><span class="sxs-lookup"><span data-stu-id="c42cd-102">Need help with email sending limits?</span></span>

<span data-ttu-id="c42cd-103">Allpool on teenuse **poolt täidetavad saatmispiirangud** .</span><span class="sxs-lookup"><span data-stu-id="c42cd-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="c42cd-104">Rohkem infot nende piiride kohta on dokumenteeritud [siin](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="c42cd-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="c42cd-105">Soovimatute hulgisõnumite kohaletoimetamise tõkestamiseks rakendame **kõigi väljaminevate ja sisemiste sõnumite puhul kasutaja adressaadi intressimäära limiite**.</span><span class="sxs-lookup"><span data-stu-id="c42cd-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="c42cd-106">Kogu SKUs, see piirang on **10 000 adressaadid päevas**.</span><span class="sxs-lookup"><span data-stu-id="c42cd-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="c42cd-107">Kliendid, kes peavad saatma seadusliku hulgikaubandusliku meili (nt kliendi uudiskirjad), peaksid kasutama neid teenuseid spetsialiseerunud kolmandate osapoolte pakkujaid.</span><span class="sxs-lookup"><span data-stu-id="c42cd-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="c42cd-108">**Märkus**: kui adressaadi määra piirang on saavutatud, sõnumeid ei saa saata postkasti kuni adressaatide arv, mis saadeti sõnumeid viimase 24 tunni jooksul langeb alla piiri.</span><span class="sxs-lookup"><span data-stu-id="c42cd-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="c42cd-109">Kasutaja ei saa sõnumeid saata kuni selle hetkeni.</span><span class="sxs-lookup"><span data-stu-id="c42cd-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="c42cd-110">Sõnumi määra piirang **30 sõnumit minutis** rakendatakse kõigis SKU-dele.</span><span class="sxs-lookup"><span data-stu-id="c42cd-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="c42cd-111">See määrab, mitu sõnumit kasutaja saab saata oma Exchange Online ' i konto määratud aja jooksul.</span><span class="sxs-lookup"><span data-stu-id="c42cd-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="c42cd-112">**Maksimaalne adressaatide arv, mis on lubatud väljal Adressaat, koopia ja Salakoopia** ühe meilisõnumi puhul kõigis SKU-s, on **1000 adressaadid**.</span><span class="sxs-lookup"><span data-stu-id="c42cd-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="c42cd-113">Selle piirangu kohandamiseks [siia](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="c42cd-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
