---
title: Pettuste tuvastamise kontrollide ohutusvihje veaotsing
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 61159391f7a9876750cd7fefc40c54054fb9bec9
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759508"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="5581e-102">Pettuste tuvastamise kontrollide ohutusvihje veaotsing</span><span class="sxs-lookup"><span data-stu-id="5581e-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="5581e-103">Kui teil on ohutu vihje, mis ütleb: "saatja ebaõnnestus meie pettuste tuvastamise kontrolli ja ei pruugi olla, kes nad tunduvad olevat", siis saatja ei läbinud kas DKIM või SPF autentimise kontrollid.</span><span class="sxs-lookup"><span data-stu-id="5581e-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="5581e-104">Parim meetod selle lahendamiseks on saatja lubada end.</span><span class="sxs-lookup"><span data-stu-id="5581e-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="5581e-105">Kui saatja saadab teie nimel, peate need lubama, lisades saatja IP-aadressi oma SPF-kirjele.</span><span class="sxs-lookup"><span data-stu-id="5581e-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="5581e-106">Vaadake lisateavet [punase (kahtlase) ohutusvihje kohta pettuste tuvastamise kontrollimiseks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .</span><span class="sxs-lookup"><span data-stu-id="5581e-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="5581e-107">Siin on mõned muud lingid, mis aitavad:</span><span class="sxs-lookup"><span data-stu-id="5581e-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="5581e-108">Kuidas Microsoft kasutab saatja poliitika raamistik (SPF) vältida tüssamine</span><span class="sxs-lookup"><span data-stu-id="5581e-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="5581e-109">Seadista SPF, et aidata vältida tüssamist</span><span class="sxs-lookup"><span data-stu-id="5581e-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
