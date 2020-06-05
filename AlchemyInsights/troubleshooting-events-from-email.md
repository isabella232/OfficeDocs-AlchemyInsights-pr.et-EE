---
title: Sündmuste tõrkeotsing e-posti teel
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569005"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="aa383-102">Sündmuste tõrkeotsing e-posti teel</span><span class="sxs-lookup"><span data-stu-id="aa383-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="aa383-103">Veenduge, et funktsioon on lubatud postkasti: \*\*Get-EventsFromEmailConfiguration-identiteedi <mailbox> \*\*</span><span class="sxs-lookup"><span data-stu-id="aa383-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="aa383-104">Siis vaadake "sündmused e-posti" logid **eksport-MailboxDiagnosticLogs <mailbox> -komponendi timeprofile**</span><span class="sxs-lookup"><span data-stu-id="aa383-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="aa383-105">Leidke "sündmused e-posti" logisid InternetMessageId, mis vastab üksuse postkasti.</span><span class="sxs-lookup"><span data-stu-id="aa383-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="aa383-106">TrustScore määratleb, kas üksus on lisatud või mitte.</span><span class="sxs-lookup"><span data-stu-id="aa383-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="aa383-107">Sündmusi saab lisada ainult siis, kui TrustScore = "usaldusväärne".</span><span class="sxs-lookup"><span data-stu-id="aa383-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="aa383-108">TrustScore on määratud SPF, DKIM või Dmarc atribuudid, mis on sõnumi päises.</span><span class="sxs-lookup"><span data-stu-id="aa383-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="aa383-109">Nende atribuutide vaatamiseks toimige järgmiselt.</span><span class="sxs-lookup"><span data-stu-id="aa383-109">To view these properties:</span></span>

<span data-ttu-id="aa383-110">**Töölaua Outlook**</span><span class="sxs-lookup"><span data-stu-id="aa383-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="aa383-111">Ava üksus</span><span class="sxs-lookup"><span data-stu-id="aa383-111">Open the item</span></span>
- <span data-ttu-id="aa383-112">Fail-> atribuudid-> Interneti-päised</span><span class="sxs-lookup"><span data-stu-id="aa383-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="aa383-113">Või</span><span class="sxs-lookup"><span data-stu-id="aa383-113">or</span></span>

<span data-ttu-id="aa383-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="aa383-114">**MFCMapi**</span></span>

- <span data-ttu-id="aa383-115">Liikuge sisendkausta üksusele</span><span class="sxs-lookup"><span data-stu-id="aa383-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="aa383-116">Otsi PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="aa383-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="aa383-117">Need omadused määratakse kindlaks ja registreeritakse transpordi ja marsruudi ajal.</span><span class="sxs-lookup"><span data-stu-id="aa383-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="aa383-118">Edasise tõrkeotsingu puhul peate võib-olla jälgima transpordi Tugiteenusi SPF-i, DKIM-i ja DMARC-i tõrgete kohta.</span><span class="sxs-lookup"><span data-stu-id="aa383-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>