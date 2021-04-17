---
title: Pettuse tuvastamise kontrollimiseks ohutussed näpunäited
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834727"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="7acdf-102">Pettuse tuvastamise kontrollimiseks ohutussed näpunäited</span><span class="sxs-lookup"><span data-stu-id="7acdf-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="7acdf-103">Kui saate ohutussed näpunäited, mis ütleb "Saatja ei kontrollinud meie pettuste tuvastamist ega pruugi olla see, kes nad näivad olevat", siis ei saanud saatja läbida DKIM-i ega SPF-autentimiskontrolle.</span><span class="sxs-lookup"><span data-stu-id="7acdf-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="7acdf-104">Parim viis selle lahendamiseks on see, et saatja lubab end ise.</span><span class="sxs-lookup"><span data-stu-id="7acdf-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="7acdf-105">Kui saatja saadab teie nimel, peate selle autoriseerima, lisades saatja IP-aadressi oma SPF-kirjesse.</span><span class="sxs-lookup"><span data-stu-id="7acdf-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="7acdf-106">Lisateavet [leiate teemast Punase (kahtlase) ohutusste näpunäidete](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) tõrkeotsing pettuse tuvastamise kontrollimiseks.</span><span class="sxs-lookup"><span data-stu-id="7acdf-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="7acdf-107">Siin on mõned muud lingid, mis võivad aidata.</span><span class="sxs-lookup"><span data-stu-id="7acdf-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="7acdf-108">Kuidas Microsoft kasutab tüssamise vältimiseks saatjapoliitika raamistikku (SPF)</span><span class="sxs-lookup"><span data-stu-id="7acdf-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="7acdf-109">SPF-i häälestamine tüssamise vältimiseks</span><span class="sxs-lookup"><span data-stu-id="7acdf-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
