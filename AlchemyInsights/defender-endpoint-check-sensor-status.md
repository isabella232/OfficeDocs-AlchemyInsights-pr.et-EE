---
title: Defenderi lõpp-punkti kontrolli anduri olek
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676182"
---
# <a name="defender-endpoint-check-sensor-status"></a>Defenderi lõpp-punkti kontrolli anduri olek

**Anduriprobleemidega seadmed** asuvad turbetoimingute armatuurlaual. See paan annab teavet selle kohta, kuidas seade saab anda anduriandmeid ja suhelda Teenusega Defender for Endpoint. Selles kirjeldatakse, kui palju seadmeid vajab tähelepanu ja aitab teil probleemsed seadmed tuvastada ja teadaolevate probleemide lahendamiseks midagi ette võtta.

Paanil on kaks olekunäidikut, mis annavad teavet selle kohta, kui palju seadmeid ei teavitata teenusest õigesti.

- **Valesti konfigureeritud** Seadmed, mis võivad osaliselt anduriandmeid teenusele Defender for Endpoint esitada ja mis võivad konfiguratsioonivigu parandada.
- **Passiivne** Seadmed, mis on viimase kuu jooksul lõpetanud aruandluse Teenusele Defender for Endpoint rohkem kui seitse päeva.

Kui klõpsate mõnda rühma, suunab see teid loendisse Seadmed, mis on filtreeritud vastavalt teie valikutele. Loendis Seadmed saate seisundioleku loendit filtreerida järgmise oleku järgi.

- **Aktiivne** Seadmed, mis suhtlevad aktiivselt teenusega Defender for Endpoint.
- **Valesti konfigureeritud** Seadmed, mis võivad osaliselt anduriandmeid teenusele Defender for Endpoint esitada, kuid mille konfiguratsioonitõrked tuleb parandada. Valesti konfigureeritud seadmetel võib olla üks või mitme järgmise probleemi kombinatsioon.

    - Anduriandmeid pole . Seadmed on sensorandmete saatmise lõpetanud. Piiratud teatisi saab seadmest käivitada.
    - Kommunikatsioonihäired – seadmega suhtlemine on häiritud. Failide saatmine süvaanalüüsiks, failide blokeerimiseks, seadme isoleerimiseks võrgust ja muud toimingud, mis nõuavad seadmega suhtlemist, ei pruugi töötada.
- **Passiivne** Seadmed, mis on lõpetanud aruandluse Teenusele Defender for Endpoint.

Kogu loendi saate alla laadida CSV-vormingus, kasutades ekspordifunktsiooni.

Lisateavet leiate teemast [Sensori seisundi seisundi kontrollimine rakenduses Microsoft Defender for Endpoint.](/microsoft-365/security/defender-endpoint/check-sensor-status)

Lisateavet selle kohta, mis põhjustas seadme passiivseks või valesti konfigureerimise, leiate teemast Ebatervislike andurite lahendus [Rakenduses Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).
