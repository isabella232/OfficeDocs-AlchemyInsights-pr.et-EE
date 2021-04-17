---
title: Sündmuste tõrkeotsing meili teel
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
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834835"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="19b09-102">Sündmuste tõrkeotsing meili teel</span><span class="sxs-lookup"><span data-stu-id="19b09-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="19b09-103">Veenduge, et funktsioon on postkasti jaoks lubatud: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span><span class="sxs-lookup"><span data-stu-id="19b09-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="19b09-104">Seejärel vaadake logi "Sündmused meilist" **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="19b09-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="19b09-105">Otsige logidest "Sündmused meilist" üles InternetMessageId, mis vastab postkasti üksusele.</span><span class="sxs-lookup"><span data-stu-id="19b09-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="19b09-106">TrustScore määratleb, kas üksus on lisatud või mitte.</span><span class="sxs-lookup"><span data-stu-id="19b09-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="19b09-107">Sündmused lisatakse ainult siis, kui TrustScore = "Trusted" (Usaldusväärne).</span><span class="sxs-lookup"><span data-stu-id="19b09-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="19b09-108">TrustScore määratakse kindlaks atribuutidega SPF, Dkim või Dmarc, mis asuvad sõnumipäises.</span><span class="sxs-lookup"><span data-stu-id="19b09-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="19b09-109">Nende atribuutide kuvamiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="19b09-109">To view these properties:</span></span>

<span data-ttu-id="19b09-110">**Outlooki töölauaversioon**</span><span class="sxs-lookup"><span data-stu-id="19b09-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="19b09-111">Üksuse avamine</span><span class="sxs-lookup"><span data-stu-id="19b09-111">Open the item</span></span>
- <span data-ttu-id="19b09-112">File -> Properties -> Internet Headers</span><span class="sxs-lookup"><span data-stu-id="19b09-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="19b09-113">VÕI</span><span class="sxs-lookup"><span data-stu-id="19b09-113">or</span></span>

<span data-ttu-id="19b09-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="19b09-114">**MFCMapi**</span></span>

- <span data-ttu-id="19b09-115">Sisendkaustas üksusele liikumine</span><span class="sxs-lookup"><span data-stu-id="19b09-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="19b09-116">Otsige PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="19b09-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="19b09-117">Need atribuudid määratakse kindlaks ja registreeritakse transpordi ja marsruutimise ajal.</span><span class="sxs-lookup"><span data-stu-id="19b09-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="19b09-118">Edasiseks tõrkeotsinguks peate võib-olla spf-, DKIM-i ja.või DMARC-i tõrgete kohta transporditoe poole järele järgnema.</span><span class="sxs-lookup"><span data-stu-id="19b09-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>