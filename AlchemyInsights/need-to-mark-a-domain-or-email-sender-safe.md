---
title: Kas soovite märkida domeeni või meili saatja turvaliseks?
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
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803241"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="0193a-102">Kas soovite märkida domeeni või meili saatja turvaliseks?</span><span class="sxs-lookup"><span data-stu-id="0193a-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="0193a-103">**Turvaliste saatjate loendite kasutamine pole soovitatav** , kuna see avab teie organisatsiooni rämpsmeili, Phish ja kelmuse rünnakute eest.</span><span class="sxs-lookup"><span data-stu-id="0193a-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="0193a-104">Kui aga tegemist on ärivajadusega, **soovitame** selle jaoks kasutada **[meilivoo reegleid](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** .</span><span class="sxs-lookup"><span data-stu-id="0193a-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="0193a-105">Meie juhised tagavad saatja autentimise (kinnitatakse, et domeeni saatmine ei ole võltsitud).</span><span class="sxs-lookup"><span data-stu-id="0193a-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="0193a-106">**Märkus**: me ei soovita turvaliste saatjate loendite abil valede positiivsete funktsioonide haldamist, kuna rämpsposti filtreerimise erandid võivad avada teie asutuse turbe rünnakute jaoks.</span><span class="sxs-lookup"><span data-stu-id="0193a-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="0193a-107">Kui teie kasutaja (d) saab rämpspostina või rämpspostina märgitud sõnumeid valesti, **[teavitage sellest Microsofti sõnumeid ja faile](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="0193a-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="0193a-108">Turvalised saatjad Outlookis, lubatud saatja loendis või lubatud domeenide loend anti-spam poliitikas **tuleks vältida** , sest saatjad ümbersõit kogu rämpsposti, paroodia ja Phish kaitse ning saatja autentimine (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="0193a-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="0193a-109">Seda meetodit on kõige parem kasutada ainult ajutiseks testimiseks.</span><span class="sxs-lookup"><span data-stu-id="0193a-109">This method is best used for temporary testing only.</span></span>
