---
title: Tingimusjuurdepääsu jälgimine
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: 80e8cc72db8ae32445d48e5c8a411d5ccd538626653260b3dbd28a247561e888
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975097"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Tingimusjuurdepääsu jälgimine Exchange

Tingimusjuurdepääsuga kasutajatele saadetakse teavitusmeil, kui nad ei vasta teie ettevõtte juurdepääsunõuetele. Probleemi lahendamiseks soovitame ühte või enamat järgmistest lahendustest.

- Kui eeldatakse, et seade on registreeritud, soovitame kasutajal minna Company Portal ja veenduda, et see kuvatakse Company Portal. Kui see nii ei ole, peaks kasutaja seadme registreerima.
- Avage Azure'i portaalis Intune'i > seadme nõuetele vastavus. Klõpsake jaotises Jälgi nuppu Seadme nõuetele vastavus. Vaadake oma seadme nõuetele vastavuse aruannet veendumaks, et kasutaja seade on märgitud nõuetele vastavaks.
- Avage Azure'i portaalis Intune'i > seadme nõuetele vastavus. Klõpsake jaotises Haldamine nuppu Poliitikad. Kontrollige vastavuspoliitikate loendis, kas teie kasutaja seadmele on määratud profiil. Kui profiili pole määratud, ei saa Intune seadme nõuetele vastavuse olekut kinnitada.
- Redigeerige kasutaja tingimusjuurdepääsu ülesannet.

1. Avage Azure'i portaalis **Intune'i**  >  **tingimusjuurdepääsu**  >  **poliitikad.**
2. Valige loendist poliitika.
3. Klõpsake nuppu Kasutajad ja rühmad.
4. Kindla poliitika sihtimiseks kellelegi lisage ta loendisse Kaasa. Tagamaks, et isik poliitikast välja jäetakse, lisage ta loendisse Välista.

Kasulikud lingid:

[Seadme nõuetele vastavuse ülevaade](https://docs.microsoft.com/intune/device-compliance-get-started)

[Ca tõrkeotsing](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Tõrkeotsingupoliitika](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Intune'i seadme nõuetele vastavuse jälgimine](https://docs.microsoft.com/intune/compliance-policy-monitor)

Märkus. Nendest juhistest on abi ainult tingimusjuurdepääsu Azure Active Directory tõrkeotsingul. Samuti on võimalik karantiini panna seade, mis blokeerib selle meilijuurdepääsu Exchange poliitikaga. Lisateavet seadmehalduse Exchange leiate [siit]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
