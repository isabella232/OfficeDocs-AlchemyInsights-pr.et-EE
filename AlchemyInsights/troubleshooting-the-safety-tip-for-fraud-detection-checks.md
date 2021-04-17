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
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Pettuse tuvastamise kontrollimiseks ohutussed näpunäited

Kui saate ohutussed näpunäited, mis ütleb "Saatja ei kontrollinud meie pettuste tuvastamist ega pruugi olla see, kes nad näivad olevat", siis ei saanud saatja läbida DKIM-i ega SPF-autentimiskontrolle. Parim viis selle lahendamiseks on see, et saatja lubab end ise. Kui saatja saadab teie nimel, peate selle autoriseerima, lisades saatja IP-aadressi oma SPF-kirjesse.
  
Lisateavet [leiate teemast Punase (kahtlase) ohutusste näpunäidete](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) tõrkeotsing pettuse tuvastamise kontrollimiseks.
  
Siin on mõned muud lingid, mis võivad aidata.
  
- [Kuidas Microsoft kasutab tüssamise vältimiseks saatjapoliitika raamistikku (SPF)](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [SPF-i häälestamine tüssamise vältimiseks](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
