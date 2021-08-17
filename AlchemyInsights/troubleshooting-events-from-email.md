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
ms.openlocfilehash: b6a8b2a1174f04a1e0ed0fdee9a954bb3bf108038f0804353d84755e490f5f47
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105348"
---
# <a name="troubleshooting-events-from-email"></a>Sündmuste tõrkeotsing meili teel

1. Veenduge, et funktsioon on postkasti jaoks lubatud: **Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. Seejärel vaadake logi "Sündmused meilist" **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. Otsige logidest "Sündmused meilist" üles InternetMessageId, mis vastab postkasti üksusele.  

4. TrustScore määratleb, kas üksus on lisatud või mitte. Sündmused lisatakse ainult siis, kui TrustScore = "Trusted" (Usaldusväärne).

TrustScore määratakse kindlaks atribuutidega SPF, Dkim või Dmarc, mis asuvad sõnumipäises.

Nende atribuutide kuvamiseks tehke järgmist.

**Töölaua Outlook**

- Üksuse avamine
- File -> Properties -> Internet Headers

VÕI

**MFCMapi**

- Sisendkaustas üksusele liikumine
- Otsige PR_TRANSPORT_MESSAGE_HEADERS_W

Need atribuudid määratakse kindlaks ja registreeritakse transpordi ja marsruutimise ajal. Edasiseks tõrkeotsinguks peate võib-olla spf-, DKIM-i ja.või DMARC-i tõrgete kohta transporditoe poole järele järgnema.