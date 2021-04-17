---
title: Kas vajate abi seoses meilisaatmispiirangutega?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: b5bdfbf818328c97ec93b3468aeedcbe88e03913
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836275"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="7757d-102">Kas vajate abi seoses meilisaatmispiirangutega?</span><span class="sxs-lookup"><span data-stu-id="7757d-102">Need help with email sending limits?</span></span>

<span data-ttu-id="7757d-103">Allpool leiate teenuses **teadlikult jõustatud saatmispiirangud**.</span><span class="sxs-lookup"><span data-stu-id="7757d-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="7757d-104">Lisateavet nende piirangute kohta saate [siit](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="7757d-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="7757d-105">Soovimatute hulgipostituste saatmise takistamiseks rakendame igale kasutajale **kõigile väljaminevatele ja sissetulevatele sõnumitele kehtivad adressaatide arvu piirangud**.</span><span class="sxs-lookup"><span data-stu-id="7757d-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="7757d-106">Kõigis SKU-des on see piirang **10 000 adressaati päevas**.</span><span class="sxs-lookup"><span data-stu-id="7757d-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="7757d-107">Kliendid, kellel on õigustatud vajadus saata hulgi kommertssõnumeid (nt klientidele suunatud uudiskirju), peaksid kasutama mõnda kolmandast osapoolest teenusepakkujat, kes spetsialiseerub vastava teenuse osutamisele.</span><span class="sxs-lookup"><span data-stu-id="7757d-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="7757d-108">**Märkus.** Pärast adressaatide arvu piirangu ületamist ei saa sõnumeid postkastist saata enne, kui viimase 24 tunni jooksul saadetud sõnumite adressaatide arv langeb alla selle piirmäära.</span><span class="sxs-lookup"><span data-stu-id="7757d-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="7757d-109">Kuni selle hetkeni ei saa kasutaja rohkem sõnumeid saata.</span><span class="sxs-lookup"><span data-stu-id="7757d-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="7757d-110">Kõigis SKU-des kehtib ka sõnumite arvu piirmäär, milleks on **30 sõnumit minutis**.</span><span class="sxs-lookup"><span data-stu-id="7757d-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="7757d-111">See määrab ära selle, kui palju sõnumeid saab kasutaja oma Exchange Online‘i kontolt määratud ajavahemikus saata.</span><span class="sxs-lookup"><span data-stu-id="7757d-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="7757d-112">Kõigis SKU-des on ühes meilisõnumis **väljadel Adressaat, Koopia ja Salakoopia lubatud adressaatide arv** piiratud ja selleks piirmääraks on **1000 adressaati**.</span><span class="sxs-lookup"><span data-stu-id="7757d-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="7757d-113">Selle piirmäära kohandamiseks minge [siia](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="7757d-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
