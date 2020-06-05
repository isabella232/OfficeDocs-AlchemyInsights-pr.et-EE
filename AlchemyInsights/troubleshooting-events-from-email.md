---
title: Sündmuste tõrkeotsing e-posti teel
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569005"
---
# <a name="troubleshooting-events-from-email"></a>Sündmuste tõrkeotsing e-posti teel

1. Veenduge, et funktsioon on lubatud postkasti: **Get-EventsFromEmailConfiguration-identiteedi <mailbox> **

2. Siis vaadake "sündmused e-posti" logid **eksport-MailboxDiagnosticLogs <mailbox> -komponendi timeprofile**

3. Leidke "sündmused e-posti" logisid InternetMessageId, mis vastab üksuse postkasti.  

4. TrustScore määratleb, kas üksus on lisatud või mitte. Sündmusi saab lisada ainult siis, kui TrustScore = "usaldusväärne".

TrustScore on määratud SPF, DKIM või Dmarc atribuudid, mis on sõnumi päises.

Nende atribuutide vaatamiseks toimige järgmiselt.

**Töölaua Outlook**

- Ava üksus
- Fail-> atribuudid-> Interneti-päised

Või

**MFCMapi**

- Liikuge sisendkausta üksusele
- Otsi PR_TRANSPORT_MESSAGE_HEADERS_W

Need omadused määratakse kindlaks ja registreeritakse transpordi ja marsruudi ajal. Edasise tõrkeotsingu puhul peate võib-olla jälgima transpordi Tugiteenusi SPF-i, DKIM-i ja DMARC-i tõrgete kohta.