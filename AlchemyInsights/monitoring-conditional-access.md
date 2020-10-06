---
title: Tingimusliku juurdepääsu jälgimine
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
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366424"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Exchange ' i tingimisi juurdepääsu jälgimine

Juurdepääsuõigusega kasutajatele antakse teatise meilisõnum, kui need ei vasta teie asutuse juurdepääsu nõuetele. Lahendamiseks soovitame teha ühte või mitut järgmistest lahendustest.

- Kui eeldatakse, et seade on registreeritud, Soovitage kasutajal minna ettevõtte portaali rakendusse ja veenduge, et see kuvatakse ettevõtte portaalis. Kui seda ei juhtu, peaks kasutaja seadme registreerima.
- Azure ' i portaalis avage > seadme nõuetele vastavuse häälestamine. Klõpsake jaotises kuvar nuppu seadme nõuetele vastavus. Vaadake seadme nõuetele vastavuse aruandeid, et veenduda, kas kasutaja seade on märgitud nõuetele vastavaks.
- Azure ' i portaalis avage > seadme nõuetele vastavuse häälestamine. Klõpsake jaotises haldamine nuppu poliitikad. Veenduge, et nõuetele vastavuse poliitikate loendis oleks teie kasutaja seadmele määratud profiil. Kui profiili pole määratud, ei saa Intune kinnitada seadme nõuetele vastavuse olekut.
- Kasutaja tingimusliku juurdepääsu määramise redigeerimine.

1. Azure ' i portaalis Avage **Intune**  >  **tingimusjuurdepääsu**  >  **poliitikate**häälestamine.
2. Valige loendist poliitika.
3. Klõpsake nuppu kasutajad ja rühmad.
4. Kellegile teatud poliitika suunamiseks lisage need loendisse kaasa. Kui soovite tagada, et isik on poliitikast välja jäetud, lisage need loendisse välista.

Kasulikud lingid:

[Seadme nõuetele vastavuse ülevaade](https://docs.microsoft.com/intune/device-compliance-get-started)

[Tõrkeotsing CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Tõrkeotsingu poliitika](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[Seadme nõuetele vastavuse jälgimine](https://docs.microsoft.com/intune/compliance-policy-monitor)

Märkus: need toimingud on abiks ainult Azure Active Directory tõrkeotsingul. Samuti on võimalik sulgeda seade, mis blokeerib juurdepääsu Exchange ' i poliitikaga. Lisateavet Exchange ' i seadmete halduse kohta leiate [siit](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).
