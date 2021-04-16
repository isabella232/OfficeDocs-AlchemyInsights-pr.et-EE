---
title: Kas peate domeeni või meili saatja turvaliseks märkima?
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
- "9002921"
- "5673"
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792128"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="11ebb-102">Kas peate domeeni või meili saatja turvaliseks märkima?</span><span class="sxs-lookup"><span data-stu-id="11ebb-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="11ebb-103">Turvaliste **saatjate loendite kasutamine pole soovitatav,** kuna see avab teie asutuse rämpsposti, andmepüügi ja tüssamisrünnakute jaoks.</span><span class="sxs-lookup"><span data-stu-id="11ebb-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="11ebb-104">Kui aga on olemas ärinõue, **soovitame selleks** kasutada **[meilivoo](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** reegleid.</span><span class="sxs-lookup"><span data-stu-id="11ebb-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="11ebb-105">Meie juhised tagavad saatja autentimise (kontrollib, et saatmisdomeeni ei tüssata).</span><span class="sxs-lookup"><span data-stu-id="11ebb-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="11ebb-106">**Märkus.** Me ei soovita turvaliste saatjate loendite abil valepositiivseid andmeid hallata, kuna rämpsposti filtreerimise erandid võivad teie asutuse avada turberünnetele.</span><span class="sxs-lookup"><span data-stu-id="11ebb-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="11ebb-107">Kui teie kasutaja(d) saavad valesti rämpsposti või rämpspostina märgitud sõnumeid, **[teatage sõnumitest ja failidest Microsoftile.](https://protection.office.com/reportsubmission)**</span><span class="sxs-lookup"><span data-stu-id="11ebb-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="11ebb-108">Turvaliste saatjate kasutamist Outlookis, lubatud saatjate loendit  või lubatud domeeniloendit rämpspostitõrjepoliitikates tuleks vältida, kuna saatjad väldivad kogu rämpsposti, tüssamis- ja andmepüügikaitset ning saatja autentimist (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="11ebb-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="11ebb-109">Seda meetodit on kõige parem kasutada ainult ajutiseks testimiseks.</span><span class="sxs-lookup"><span data-stu-id="11ebb-109">This method is best used for temporary testing only.</span></span>
