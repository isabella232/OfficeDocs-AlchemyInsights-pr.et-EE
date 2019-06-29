---
title: 1491-Search-Not-returning-Expected-Results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d25c1ef2e0e746432472a436cb11d25b5db5596c
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35355873"
---
# <a name="content-search-not-returning-expected-results"></a>Otsing ei tagasta oodatavad tulemused

Sõites sisu otsingud: Office 365 turvalisus & vastavuse Center, saate ootamatu Otsingu tulemused. Kaaluge järgmist asjad, mis võib mõjutada teie otsingu tulemused:

- **Sisu kohtades ja Otsi tingimustes**: Veenduge, et valitud sisu ettenähtud kohas ja otsingu tingimused. Kui käivitasite annab suur otsing (paljudes kohtades), kaaluda mitmeks mitu otsinguid.

- **Osaliselt indekseeritud üksuste**: [osaliselt indekseeritud üksuste](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) postkastidest sisalduvad hinnanguline Otsingu tulemused. Siiski osaliselt indekseeritud üksuste SharePointis või OneDrive saidid pole lisatud Otsi hinnang.

- **Otsi vead**: palju postkaste (üle 100 000 postkastid) otsimisel võite saada Otsi tõrkeid, tõrkekoodide nagu CS008-009 ja CS012-002). Sel juhul proovige uuesti otsida ainult ebaõnnestunud sisu asukohad. Vaata [see artikkel](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) rohkem teavet.
