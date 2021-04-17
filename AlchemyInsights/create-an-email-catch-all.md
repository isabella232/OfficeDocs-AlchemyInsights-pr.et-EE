---
title: Meilisõnumite püüdmise loomine
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816196"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="3b60b-102">Meilisõnumite püüdmise loomine</span><span class="sxs-lookup"><span data-stu-id="3b60b-102">Create an email catch all</span></span>

<span data-ttu-id="3b60b-103">Saagi kasutamist ei soovitata.</span><span class="sxs-lookup"><span data-stu-id="3b60b-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="3b60b-104">Parem on pakkuda saatjale tagasisaatmine, andes saatjale teada, et tema sõnumit ei saanud adressaadina kohale toimetada, et nad saaksid midagi ette võtta.</span><span class="sxs-lookup"><span data-stu-id="3b60b-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="3b60b-105">Samuti saate jälgitud postkasti piirata ainult varem kehtivate meiliaadresside püüdmisega.</span><span class="sxs-lookup"><span data-stu-id="3b60b-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="3b60b-106">Iga postkast saab palju rämpsposti ja võib lõpuks täita, kui seda ei jälgita hoolikalt.</span><span class="sxs-lookup"><span data-stu-id="3b60b-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="3b60b-107">(Piirangud on olemas.)</span><span class="sxs-lookup"><span data-stu-id="3b60b-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="3b60b-108">Kui otsustate jätkata, tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="3b60b-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="3b60b-109">Dünaamilise levirühma loomine & "Kõik adressaaditüübid".</span><span class="sxs-lookup"><span data-stu-id="3b60b-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="3b60b-110">Looge spetsiaalne postkast meilisõnumite püüdmiseks , näiteks catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="3b60b-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="3b60b-111">Määrake konkreetse domeeni domeenitüübiks "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="3b60b-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="3b60b-112">Kui eemaldate hiljem kogu saagi, määrake domeen kindlasti uuesti autoriteetseks.</span><span class="sxs-lookup"><span data-stu-id="3b60b-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="3b60b-113">Looge meilivoo transpordireegel järgmiselt.</span><span class="sxs-lookup"><span data-stu-id="3b60b-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="3b60b-114">Kui saatja on "Väljaspool asutust"</span><span class="sxs-lookup"><span data-stu-id="3b60b-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="3b60b-115">Sõnumi ümbersuunamine Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="3b60b-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="3b60b-116">Välja arvatud juhul, kui adressaat on allusers@domain.com liige (levirühm sisaldab kõiki liikmeid)</span><span class="sxs-lookup"><span data-stu-id="3b60b-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="3b60b-117">Kontrollige, kas dünaamilise levirühma lisatakse uusi postkaste.</span><span class="sxs-lookup"><span data-stu-id="3b60b-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
