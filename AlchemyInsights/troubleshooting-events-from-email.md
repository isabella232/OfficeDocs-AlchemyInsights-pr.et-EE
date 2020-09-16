---
title: Meilisõnumite tõrkeotsing
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
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658730"
---
# <a name="troubleshooting-events-from-email"></a>Meilisõnumite tõrkeotsing

1. Veenduge, et funktsioon on postkasti jaoks lubatud: **Get-EventsFromEmailConfiguration-Identity <mailbox> **

2. Seejärel Vaata "sündmusi e-posti" logid **ekspordi-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. Otsige jaotisest "e-posti logid" välja InternetMessageId, mis vastab postkastis olevale üksusele.  

4. TrustScore määratleb, kas üksus on lisatud või mitte. Sündmusi lisatakse ainult juhul, kui TrustScore = "usaldusväärne".

TrustScore on määratud SPF-, DKIM-või Dmarc atribuudid, mis asuvad sõnumi päises.

Nende atribuutide kuvamiseks tehke järgmist.

**Töölaua Outlook**

- Üksuse avamine
- Failid > atribuudid – > Interneti-päised

või

**MFCMapi**

- Sisendkausta üksusele liikumine
- Otsi PR_TRANSPORT_MESSAGE_HEADERS_W

Need atribuudid määratakse ja salvestatakse veo ja marsruutimise ajal. Edasiseks tõrkeotsinguks võib juhtuda, et peate jälgima transpordi tuge SPF-, DKIM-ja DMARC tõrgete kohta.