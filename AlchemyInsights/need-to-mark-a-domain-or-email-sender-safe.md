---
title: Kas soovite märkida domeeni või e-posti saatja turvalisuse?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281144"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="7514e-102">Kas soovite märkida domeeni või e-posti saatja turvalisuse?</span><span class="sxs-lookup"><span data-stu-id="7514e-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="7514e-103">**Turvaliste saatjate loendite kasutamine ei ole soovitatav** , kuna see avab teie organisatsiooni rämpsposti, Phish ja tüssamine rünnakud.</span><span class="sxs-lookup"><span data-stu-id="7514e-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="7514e-104">Kui aga on olemas ärivajadus, **soovitame** selle jaoks kasutada **[meilivoo reegleid](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** .</span><span class="sxs-lookup"><span data-stu-id="7514e-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="7514e-105">Meie juhised tagavad saatja autentimise (kontrollib saatmine domeeni ei ole tüssunud).</span><span class="sxs-lookup"><span data-stu-id="7514e-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="7514e-106">**Märkus**: me ei soovita hallata valepositiivseid kasutades turvaliste saatjate loendid, kuna erandid rämpsposti filtreerimine võib avada oma organisatsiooni turvalisuse rünnakute.</span><span class="sxs-lookup"><span data-stu-id="7514e-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="7514e-107">Kui teie kasutaja (d) saab sõnumeid, mis on valesti märgistatud rämpspostiks või rämpspostina, teatage **[Microsoftile sõnumeid ja faile](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="7514e-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="7514e-108">Turvalised saatjad Outlookis, lubatud saatja nimekirja või lubatud domeeni nimekirja rämpspostipoliitika **tuleks vältida** , sest saatjate mööduda kõik rämpsposti, spoof ja Phish kaitse ja saatja autentimine (SPF, DKIM, dmarc).</span><span class="sxs-lookup"><span data-stu-id="7514e-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="7514e-109">Seda meetodit kasutatakse kõige paremini ajutiseks testimiseks.</span><span class="sxs-lookup"><span data-stu-id="7514e-109">This method is best used for temporary testing only.</span></span>
