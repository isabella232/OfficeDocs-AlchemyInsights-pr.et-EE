---
title: Postkasti vastuvõtmise piirangu jõustamine
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/31/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13711"
- "9008580"
ms.openlocfilehash: c1ba5ab10b102680cec52f4e0740c3dd2ceaccbd
ms.sourcegitcommit: a36ec7eda49536933dc8c6f9319cf7320e8aa04d
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/31/2021
ms.locfileid: "59315903"
---
# <a name="mailbox-receiving-limit-enforcement"></a>Postkasti vastuvõtmise piirangu jõustamine

Microsoft on hiljuti alustanud postkasti läve 3600 sõnumit tunnis. Lisateavet leiate teemast [Exchange Online piirangud.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-limits) Microsoft 365, mis saavad tunni jooksul üle 3600 sõnumi, aheneb järgmise 60 minuti jooksul. 

Lisaks rakendatakse saatja ja adressaadi paaride (SRP) piirang, mis blokeerib teatud Microsoft 365 saadetud sõnumid. Kui üks saatja saadab konkreetsele adressaadile üle 33% kogulävest või 1200 sõnumit jooksva tunni kohta, algab SRP-limiit ja postkast ei saa enam sellelt saatjalt sõnumeid vastu võtta. Pange tähele, et:

- See piirang on rakendus teistelt rentnikelt, kohapealt või Interneti-saatjalt saadud meilisõnumitele.
- Meilisõnumite kohaletoimetamine postkasti blokeeritakse järgmise 60 minuti jooksul. 
- Nende postkastide saatjad saavad kättetoimetamisaruande (5.2.121 või 5.2.122), mis kinnitab, et postkast on ületanud maksimaalse kohaletoimetamisläve. Rentnikusisene (sama rentnikusisene meilisõnum) toimetatakse edasi.
- Kui rakendatakse SRP-limiit, jätkab vastuvõttev postkast teistelt saatjatelt saadud sõnumite aktsepteerimist.

Administraatorid saavad jälgida praegust postkastitegevust, pääsedes juurde uuele aruandele ja ülevaatele Exchange halduskeskuses nimega "Postkastid, mis ületavad vastuvõtupiiranguid". Ülevaade kuvatakse ainult juhul, kui rentnikul on riknevad postkastid, kuid aruanne kuvatakse alati armatuurlaual, kuid see on tühi, välja arvatud juhul, kui rentnik on postkaste solvanud.

Lisateavet ülevaate saamise piirangute kohta leiate teemast Postkastid, mis ületavad uues [EAC-s piiranguid.](https://docs.microsoft.com/exchange/monitoring/mail-flow-insights/mailboxes-exceeding-receiving-limits-insights)

Vastuvõtupiirangute ületamise aruande kohta leiate lisateavet teemast Postkastid, mis ületavad vastuvõtulimiitide aruande uues [EAC-s.](https://docs.microsoft.com/exchange/monitoring/mail-flow-reports/mailboxes-exceeding-receiving-limits-report)