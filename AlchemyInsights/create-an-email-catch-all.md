---
title: Loo e-posti saagi kõik
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286106"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="c7064-102">Loo e-posti saagi kõik</span><span class="sxs-lookup"><span data-stu-id="c7064-102">Create an email catch all</span></span>

<span data-ttu-id="c7064-103">Saagi kasutamine on tugevalt heidutatud.</span><span class="sxs-lookup"><span data-stu-id="c7064-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="c7064-104">Parem on anda tagasilöök saatjale, kes laseb saatjatel teada, et nende sõnumit ei saanud saata nii, et nad saaksid tegutseda.</span><span class="sxs-lookup"><span data-stu-id="c7064-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="c7064-105">Samuti saate piirata jälgida postkasti ainult püüda varem kehtiv e-posti aadressid.</span><span class="sxs-lookup"><span data-stu-id="c7064-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="c7064-106">Iga saagi kõik postkast saab palju rämpsposti ja võib lõpuks täita, kui ei ole tähelepanelikult jälgida.</span><span class="sxs-lookup"><span data-stu-id="c7064-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="c7064-107">(On olemas piirangud.)</span><span class="sxs-lookup"><span data-stu-id="c7064-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="c7064-108">Kui otsustate jätkata, toimige järgmiselt.</span><span class="sxs-lookup"><span data-stu-id="c7064-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="c7064-109">Dünaamilise levirühma & loomiseks lisage "kõik adressaadi tüübid".</span><span class="sxs-lookup"><span data-stu-id="c7064-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="c7064-110">Looge spetsiaalne postkast püüda e-kirju, näiteks catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="c7064-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="c7064-111">Konkreetse domeeni, seadke DomainType "Internalrelee".</span><span class="sxs-lookup"><span data-stu-id="c7064-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="c7064-112">Kui te hiljem eemaldada saagi kõik, kindlasti seadke domeeni tagasi autoriteetne.</span><span class="sxs-lookup"><span data-stu-id="c7064-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="c7064-113">Loo Mailflow transport reegel järgmiselt:</span><span class="sxs-lookup"><span data-stu-id="c7064-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="c7064-114">Kui saatja on "väljaspool organisatsiooni"</span><span class="sxs-lookup"><span data-stu-id="c7064-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="c7064-115">Suuna sõnum Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="c7064-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="c7064-116">Välja arvatud juhul, kui adressaat on allusers@domain.com liige (levirühm sisaldab kõiki liikmeid)</span><span class="sxs-lookup"><span data-stu-id="c7064-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="c7064-117">Veenduge, et uus postkastid lisatakse dünaamiline jaotus rühma kinnitada</span><span class="sxs-lookup"><span data-stu-id="c7064-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
