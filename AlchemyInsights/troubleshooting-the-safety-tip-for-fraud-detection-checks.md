---
title: Pettuste tuvastamise kontrolli turvalisuse näpunäidete tõrkeotsing
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: e42b498070bf5d9bfc36110667da8cc0fd431524
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658406"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="85d1f-102">Pettuste tuvastamise kontrolli turvalisuse näpunäidete tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="85d1f-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="85d1f-103">Kui kuvatakse ohutusteave, mis ütleb, et "saatja ei ole meie pettuste tuvastamise kontrollinud ja ei pruugi olla see, kes nad näivad olevat", siis ei saanud Saatja DKIM ega SPF-i autentimise kontrollimist.</span><span class="sxs-lookup"><span data-stu-id="85d1f-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="85d1f-104">Parim viis selle lahendamiseks on saatjal endale loa andmine.</span><span class="sxs-lookup"><span data-stu-id="85d1f-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="85d1f-105">Kui saatja on teie nimel saadetud, peate neile loa andma, lisades oma SPF-kirjele saatja IP-aadressi.</span><span class="sxs-lookup"><span data-stu-id="85d1f-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="85d1f-106">Lisateavet leiate teemast [pettuste tuvastamise jaoks mõeldud punase (kahtlaste) turvalisuse näpunäidete tõrkeotsing](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .</span><span class="sxs-lookup"><span data-stu-id="85d1f-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="85d1f-107">Siin on mõned muud lingid, mis aitavad teil järgmist.</span><span class="sxs-lookup"><span data-stu-id="85d1f-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="85d1f-108">Kuidas Microsoft kasutab saatja poliitika raamistikku (SPF), et vältida võltsitud</span><span class="sxs-lookup"><span data-stu-id="85d1f-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="85d1f-109">SPF-i häälestamine võltsimise takistamiseks</span><span class="sxs-lookup"><span data-stu-id="85d1f-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
