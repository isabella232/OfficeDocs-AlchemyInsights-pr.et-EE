---
title: Kasutajate poliitikate/postkasti sätete parandamine
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746732"
---
# <a name="fix-user-policymailbox-settings"></a><span data-ttu-id="87823-102">Kasutajate poliitikate/postkasti sätete parandamine</span><span class="sxs-lookup"><span data-stu-id="87823-102">Fix user policy/mailbox settings</span></span>

<span data-ttu-id="87823-103">Postkasti rämpsmeili sätted mõjutasid seda sõnumit.</span><span class="sxs-lookup"><span data-stu-id="87823-103">The junk mail settings on the mailbox affected this message.</span></span> <span data-ttu-id="87823-104">Sätete läbivaatamiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="87823-104">To review the settings, do the following:</span></span>

1. <span data-ttu-id="87823-105">Käivitage Exchange Management shell.</span><span class="sxs-lookup"><span data-stu-id="87823-105">Launch Exchange Management Shell.</span></span> <span data-ttu-id="87823-106">Lisateavet leiate teemast [Exchange ' i halduse kesta avamine](https://go.microsoft.com/fwlink/?linkid=2101432).</span><span class="sxs-lookup"><span data-stu-id="87823-106">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
2. <span data-ttu-id="87823-107">Käivitage see käsk (kasutaja meiliaadressi kasutamine):  **Get-mailboxjunkmailconfiguration-Identity "User@domain.com"**</span><span class="sxs-lookup"><span data-stu-id="87823-107">Run this command (using the user's email address):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span></span>
3. <span data-ttu-id="87823-108">Kontrollige, kas saatja meiliaadress on osa **TrustedSendersAndDomains** või **BlockedSendersAndDomains**.</span><span class="sxs-lookup"><span data-stu-id="87823-108">Check if the sender's email address is part of **TrustedSendersAndDomains** or **BlockedSendersAndDomains**.</span></span> <span data-ttu-id="87823-109">Kui meiliaadress on ühes loenditest, peate selle võib-olla eemaldama.</span><span class="sxs-lookup"><span data-stu-id="87823-109">If the email address is in one of the lists, you may have to remove it.</span></span> <span data-ttu-id="87823-110">Lisateavet leiate teemast [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span><span class="sxs-lookup"><span data-stu-id="87823-110">To learn more, see [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span></span>
