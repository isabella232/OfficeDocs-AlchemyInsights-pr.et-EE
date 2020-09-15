---
title: Kõigi meilisõnumite loomine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712982"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="1a684-102">Kõigi meilisõnumite loomine</span><span class="sxs-lookup"><span data-stu-id="1a684-102">Create an email catch all</span></span>

<span data-ttu-id="1a684-103">Saagi kasutamine on tugevalt heidutav.</span><span class="sxs-lookup"><span data-stu-id="1a684-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="1a684-104">Parem on anda põrge tagasi saatjale, et saatjad saaksid teada, et nende sõnumit ei saanud esitada nii, et nad saaksid tegutseda.</span><span class="sxs-lookup"><span data-stu-id="1a684-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="1a684-105">Samuti saate jälgida postkasti piirata ainult varem kehtivate meiliaadresside järgi.</span><span class="sxs-lookup"><span data-stu-id="1a684-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="1a684-106">Kõik postkastid saavad palju rämpsposti ja võivad lõpuks täita, kui neid hoolikalt ei jälgita.</span><span class="sxs-lookup"><span data-stu-id="1a684-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="1a684-107">(Seal saab limiite.)</span><span class="sxs-lookup"><span data-stu-id="1a684-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="1a684-108">Kui otsustate jätkata, järgige järgmisi juhiseid.</span><span class="sxs-lookup"><span data-stu-id="1a684-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="1a684-109">Saate luua dünaamilise levirühma & kaasata "kõik adressaadi tüübid".</span><span class="sxs-lookup"><span data-stu-id="1a684-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="1a684-110">Saate luua spetsiaalse postkasti meilisõnumite püüdmiseks (nt catchall@domain.com).</span><span class="sxs-lookup"><span data-stu-id="1a684-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="1a684-111">Määrake konkreetse domeeni jaoks DomainType väärtuseks "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="1a684-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="1a684-112">Kui eemaldate selle hiljem, veenduge, et Domeen oleks uuesti autoriteetseks määratud.</span><span class="sxs-lookup"><span data-stu-id="1a684-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="1a684-113">Meilivoogude transpordi reegli loomiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="1a684-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="1a684-114">Kui saatja on "väljaspool asutust"</span><span class="sxs-lookup"><span data-stu-id="1a684-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="1a684-115">Sõnumi ümbersuunamine Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="1a684-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="1a684-116">Välja arvatud juhul, kui adressaat on allusers@domain.com liige (levirühma sisaldab kõiki liikmeid)</span><span class="sxs-lookup"><span data-stu-id="1a684-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="1a684-117">Veenduge, et valideerite, et uued postkastid lisatakse dünaamilisse levirühma.</span><span class="sxs-lookup"><span data-stu-id="1a684-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
