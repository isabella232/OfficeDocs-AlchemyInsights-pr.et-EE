---
title: Meilisõnumite tõrkeotsing
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658730"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="c09cb-102">Meilisõnumite tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="c09cb-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="c09cb-103">Veenduge, et funktsioon on postkasti jaoks lubatud: \*\*Get-EventsFromEmailConfiguration-Identity <mailbox> \*\*</span><span class="sxs-lookup"><span data-stu-id="c09cb-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="c09cb-104">Seejärel Vaata "sündmusi e-posti" logid **ekspordi-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="c09cb-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="c09cb-105">Otsige jaotisest "e-posti logid" välja InternetMessageId, mis vastab postkastis olevale üksusele.</span><span class="sxs-lookup"><span data-stu-id="c09cb-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="c09cb-106">TrustScore määratleb, kas üksus on lisatud või mitte.</span><span class="sxs-lookup"><span data-stu-id="c09cb-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="c09cb-107">Sündmusi lisatakse ainult juhul, kui TrustScore = "usaldusväärne".</span><span class="sxs-lookup"><span data-stu-id="c09cb-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="c09cb-108">TrustScore on määratud SPF-, DKIM-või Dmarc atribuudid, mis asuvad sõnumi päises.</span><span class="sxs-lookup"><span data-stu-id="c09cb-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="c09cb-109">Nende atribuutide kuvamiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="c09cb-109">To view these properties:</span></span>

<span data-ttu-id="c09cb-110">**Töölaua Outlook**</span><span class="sxs-lookup"><span data-stu-id="c09cb-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="c09cb-111">Üksuse avamine</span><span class="sxs-lookup"><span data-stu-id="c09cb-111">Open the item</span></span>
- <span data-ttu-id="c09cb-112">Failid > atribuudid – > Interneti-päised</span><span class="sxs-lookup"><span data-stu-id="c09cb-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="c09cb-113">või</span><span class="sxs-lookup"><span data-stu-id="c09cb-113">or</span></span>

<span data-ttu-id="c09cb-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="c09cb-114">**MFCMapi**</span></span>

- <span data-ttu-id="c09cb-115">Sisendkausta üksusele liikumine</span><span class="sxs-lookup"><span data-stu-id="c09cb-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="c09cb-116">Otsi PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="c09cb-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="c09cb-117">Need atribuudid määratakse ja salvestatakse veo ja marsruutimise ajal.</span><span class="sxs-lookup"><span data-stu-id="c09cb-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="c09cb-118">Edasiseks tõrkeotsinguks võib juhtuda, et peate jälgima transpordi tuge SPF-, DKIM-ja DMARC tõrgete kohta.</span><span class="sxs-lookup"><span data-stu-id="c09cb-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>