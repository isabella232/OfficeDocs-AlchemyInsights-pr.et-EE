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
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Pettuste tuvastamise kontrollide ohutusvihje veaotsing

Kui teil on ohutu vihje, mis ütleb: "saatja ebaõnnestus meie pettuste tuvastamise kontrolli ja ei pruugi olla, kes nad tunduvad olevat", siis saatja ei läbinud kas DKIM või SPF autentimise kontrollid. Parim meetod selle lahendamiseks on saatja lubada end. Kui saatja saadab teie nimel, peate need lubama, lisades saatja IP-aadressi oma SPF-kirjele.
  
Vaadake lisateavet [punase (kahtlase) ohutusvihje kohta pettuste tuvastamise kontrollimiseks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .
  
Siin on mõned muud lingid, mis aitavad:
  
- [Kuidas Microsoft kasutab saatja poliitika raamistik (SPF) vältida tüssamine](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [Seadista SPF, et aidata vältida tüssamist](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
