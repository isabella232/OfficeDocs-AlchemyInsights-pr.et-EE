---
title: Kas teie kasutajad on saanud ründesisuga meilisõnumeid?
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
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 525af0b29ffa291ddf69f6f2d97f505e93342989
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326661"
---
# <a name="did-your-users-receive-malicious-email"></a>Kas teie kasutajad on saanud ründesisuga meilisõnumeid?

Nüüd saate microsoftile pahatahtliku meili edastamiseks kasutada [Microsoft 365 Defender.](https://sip.security.microsoft.com/reportsubmission?viewid=admin)

Administraatorite [edastustes esitatud sõnumid](https://security.microsoft.com/reportsubmission?viewid=admin) skannitakse ja üksikasjalikus hüpikus kuvatakse järgmised tulemid.

- kas saatja meiliaadressi autentimisel ilmnes kohaletoimetamise ajal probleeme;
- kas leidub poliitikatabamusi, mis oleksid võinud sõnumiga seotud otsust mingil viisil mõjutada või selle alistada;
- praegused ohutustamise tulemused, et saaksite vaadata, kas sõnumis sisaldunud URL-id või failid olid ründesisuga või mitte;
- hindajate tagasiside.

Alistuse leidmise korral peaks uus kontroll lõpule jõudma mõne minutiga. Kui probleem polnud seotud meiliaadressi autentimisega või kui kohaletoimetamist ei mõjutanud poliitikast tulenev alistamine, võib hindajate tagasiside saamiseks kuluda kuni üks päev.

Kui te pole sõnumi, URL-i või faili osas tehtud lõpliku otsusega (blokeerida või mitte blokeerida) nõus, esitage sõnum ühe päeva möödumisel uuesti kontrollimiseks. Suure tõenäosusega toob sõnumi uuesti esitamine kaasa otsuse muutumise.

Seni saate ründesisuga meilisõnumid kasutajate postkastidest eemaldada [selle artikli](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization) juhiste järgi.

- Kliendid, kellel on Microsoft Defender for Office 365, saavad:
  - Ohu [exploreri kasutamine kahtlase meili otsimiseks ja kustutamiseks](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
  - [Seif linkide kasutamine pahatahtliku URL-i](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-links) juurdepääsu blokeerimiseks
  - Jälitage kasutajaid, kes klõpsasid ja pääsesid juurde pahatahtlike URL-ide klõpsamisel: vaadake andmepüügi [URL-i](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer)ja klõpsake käsku Võta andmed  &  [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
  - Automaatse [uurimise käsitsi käivitamine](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Samuti saate end ründesisuga failide ja URL-ide eest kaitsta artikli [Kaitse ründesisuga URL-ide ja failide eest](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats) juhiste järgi.
