---
title: Mitu aktiivset seanssi samale postkastile
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1836"
- "9000248"
ms.openlocfilehash: d2fd3f20346012baed21efd4900ca4cf73391d91
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438936"
---
# <a name="multiple-active-sessions-to-the-same-mailbox"></a><span data-ttu-id="ec16e-102">Mitu aktiivset seanssi samale postkastile</span><span class="sxs-lookup"><span data-stu-id="ec16e-102">Multiple active sessions to the same mailbox</span></span>

<span data-ttu-id="ec16e-103">Exchange ' i ressursside kasutuse juhtimiseks on postkastis "eelarve".</span><span class="sxs-lookup"><span data-stu-id="ec16e-103">To control usage of Exchange resources, a mailbox has a "budget."</span></span>

<span data-ttu-id="ec16e-104">Üle-eelarve erandi saab käivitada, kuid see ei tohi olla piiratud järgmiste asjaoludega.</span><span class="sxs-lookup"><span data-stu-id="ec16e-104">The over-budget exception can be triggered by, but is not limited to, the following circumstances:</span></span>

- <span data-ttu-id="ec16e-105">Sama Outlook Web Appi seansi ajal avatakse mõne brauseri vahekaardid.</span><span class="sxs-lookup"><span data-stu-id="ec16e-105">A few browser tabs are opened within the same Outlook Web App session.</span></span>

- <span data-ttu-id="ec16e-106">Mõned aktiivsed Outlook Web Appi seansid samale postkastile.</span><span class="sxs-lookup"><span data-stu-id="ec16e-106">A few active Outlook Web App sessions to the same mailbox.</span></span>

- <span data-ttu-id="ec16e-107">Mõned teised klientrakendused (Outlook, Outlook Mobile, kolmanda osapoole klientrakendus) pääsevad postkastile juurde samal ajal.</span><span class="sxs-lookup"><span data-stu-id="ec16e-107">A few other client applications (Outlook, Outlook Mobile, a third party client app) access the mailbox at the same time.</span></span>

- <span data-ttu-id="ec16e-108">Pikad töötavad toimingud (nt päringute täitmine) tehakse mõnest muust aktiivsest postkasti seansist.</span><span class="sxs-lookup"><span data-stu-id="ec16e-108">Long running operations, such as executing search requests, are performed from another active mailbox session.</span></span>

