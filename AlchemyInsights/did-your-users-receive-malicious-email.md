---
title: Kas teie kasutajad on saanud ründesisuga meilisõnumeid?
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
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 2197e7f195d789193798b80cb092d8046eb6e0be
ms.sourcegitcommit: 3c708a4a349b60b59bc623c44fb78674c685f3c2
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291788"
---
# <a name="did-your-users-receive-malicious-email"></a>Kas teie kasutajad on saanud ründesisuga meilisõnumeid?

- Ründemeilidest saate nüüd Microsoftile teada anda [turbe- ja vastavuskeskuse edastuste lehel](https://sip.protection.office.com/reportsubmission).

[Administraatori edastuste](https://sip.protection.office.com/reportsubmission) lehe kaudu edastatud sõnumeid kontrollitakse ja **üksikasjade** hüpikus kuvatakse järgmine teave:

- kas saatja meiliaadressi autentimisel ilmnes kohaletoimetamise ajal probleeme;
- kas leidub poliitikatabamusi, mis oleksid võinud sõnumiga seotud otsust mingil viisil mõjutada või selle alistada;
- praegused ohutustamise tulemused, et saaksite vaadata, kas sõnumis sisaldunud URL-id või failid olid ründesisuga või mitte;
- hindajate tagasiside.

Alistuse leidmise korral peaks uus kontroll lõpule jõudma mõne minutiga. Kui probleem polnud seotud meiliaadressi autentimisega või kui kohaletoimetamist ei mõjutanud poliitikast tulenev alistamine, võib hindajate tagasiside saamiseks kuluda kuni üks päev.

Kui te pole sõnumi, URL-i või faili osas tehtud lõpliku otsusega (blokeerida või mitte blokeerida) nõus, esitage sõnum ühe päeva möödumisel uuesti kontrollimiseks. Suure tõenäosusega toob sõnumi uuesti esitamine kaasa otsuse muutumise.

Seni saate ründesisuga meilisõnumid kasutajate postkastidest eemaldada [selle artikli](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization) juhiste järgi.

- Kliendid, kellel on Microsoft Defender for Office 365, saavad:
    - kasutada [ohu-uurijat kahtlaste meilisõnumite leidmiseks ja kustutamiseks](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered);
    - kasutada [ohutute linkide funktsiooni juurdepääsu blokeerimiseks](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) ründesisule viivale URL-ile;
    - jälgida kasutajaid, kes on ründesisule viivaid URL-e klõpsanud ja neile liikunud: [Andmepüügi-URL-ide ja klõpsude otsuseandmete vaatamine](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace);
    - käsitsi [käivitada automaatuurimise](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office).

Samuti saate end ründesisuga failide ja URL-ide eest kaitsta artikli [Kaitse ründesisuga URL-ide ja failide eest](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats) juhiste järgi.