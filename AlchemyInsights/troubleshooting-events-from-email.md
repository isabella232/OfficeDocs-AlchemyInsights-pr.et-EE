---
title: Sündmuste tõrkeotsing meili teel
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
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834835"
---
# <a name="troubleshooting-events-from-email"></a>Sündmuste tõrkeotsing meili teel

1. Veenduge, et funktsioon on postkasti jaoks lubatud: **Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. Seejärel vaadake logi "Sündmused meilist" **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. Otsige logidest "Sündmused meilist" üles InternetMessageId, mis vastab postkasti üksusele.  

4. TrustScore määratleb, kas üksus on lisatud või mitte. Sündmused lisatakse ainult siis, kui TrustScore = "Trusted" (Usaldusväärne).

TrustScore määratakse kindlaks atribuutidega SPF, Dkim või Dmarc, mis asuvad sõnumipäises.

Nende atribuutide kuvamiseks tehke järgmist.

**Outlooki töölauaversioon**

- Üksuse avamine
- File -> Properties -> Internet Headers

VÕI

**MFCMapi**

- Sisendkaustas üksusele liikumine
- Otsige PR_TRANSPORT_MESSAGE_HEADERS_W

Need atribuudid määratakse kindlaks ja registreeritakse transpordi ja marsruutimise ajal. Edasiseks tõrkeotsinguks peate võib-olla spf-, DKIM-i ja.või DMARC-i tõrgete kohta transporditoe poole järele järgnema.