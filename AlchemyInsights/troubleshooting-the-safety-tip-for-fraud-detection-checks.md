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
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Pettuste tuvastamise kontrolli turvalisuse näpunäidete tõrkeotsing

Kui kuvatakse ohutusteave, mis ütleb, et "saatja ei ole meie pettuste tuvastamise kontrollinud ja ei pruugi olla see, kes nad näivad olevat", siis ei saanud Saatja DKIM ega SPF-i autentimise kontrollimist. Parim viis selle lahendamiseks on saatjal endale loa andmine. Kui saatja on teie nimel saadetud, peate neile loa andma, lisades oma SPF-kirjele saatja IP-aadressi.
  
Lisateavet leiate teemast [pettuste tuvastamise jaoks mõeldud punase (kahtlaste) turvalisuse näpunäidete tõrkeotsing](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .
  
Siin on mõned muud lingid, mis aitavad teil järgmist.
  
- [Kuidas Microsoft kasutab saatja poliitika raamistikku (SPF), et vältida võltsitud](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [SPF-i häälestamine võltsimise takistamiseks](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
