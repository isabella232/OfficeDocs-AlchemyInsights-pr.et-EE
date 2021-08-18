---
title: Intune'i tingimusjuurdepääsu jälgimine
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: 2c3a382671ac95ecbaec1b374bd8c474cf9690a2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327553"
---
# <a name="monitor-intune-conditional-access"></a>Intune'i tingimusjuurdepääsu jälgimine

Tingimusjuurdepääsuga kasutajatele saadetakse teavitusmeil, kui nad ei vasta teie ettevõtte juurdepääsunõuetele. Probleemi lahendamiseks soovitame ühte või enamat järgmistest lahendustest.

1. Kui eeldatakse, et seade on registreeritud, soovitame kasutajal minna Company Portal rakendusse ja veenduda, et see kuvatakse Company Portal. Kui see nii ei ole, peab kasutaja seadme registreerima.
1. Avage Azure'i portaalis **Intune'i**  >  **seadme nõuetele vastavus.** 
1. Seadme nõuetele vastavuse aruande vaatamiseks veendumaks, et kasutaja seade on märgitud nõuetele vastavaks, klõpsake jaotises **Kuvar** nuppu **Seadme nõuetele vastavus**.
1. Avage Azure'i portaalis **Intune'i**  >  **seadme nõuetele vastavus.** Klõpsake **jaotises Haldamine nuppu** **Poliitikad.** Kontrollige vastavuspoliitikate loendis, kas teie kasutaja seadmele on määratud profiil. Kui profiili pole määratud, ei saa Intune seadme nõuetele vastavuse olekut kinnitada.
1. Redigeerige kasutaja tingimusjuurdepääsu ülesannet.
1. Liikuge Azure'i portaalis valikule Intune Conditional access Policies **(Intune'i** tingimusjuurdepääsu poliitikad), valige loendist poliitika ja  >    >  klõpsake **nuppu Kasutajad ja rühmad**.
1. Kindla poliitika sihtimiseks kellelegi lisage ta loendisse **Kaasa**. Kui soovite, et isik poliitikast välja jäetakse, lisage ta loendisse **Välista**.

**Kasulikud lingid:**

- [Seadme nõuetele vastavuse ülevaade](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Ca tõrkeotsing](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Tõrkeotsingupoliitika](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Intune'i seadme nõuetele vastavuse jälgimine](https://docs.microsoft.com/intune/compliance-policy-monitor)

**Märkus.** Nendest juhistest on abi ainult tingimusjuurdepääsu Azure Active Directory tõrkeotsingul. Samuti on võimalik karantiini panna seade, mis blokeerib selle meilijuurdepääsu Exchange poliitikaga. Lisateavet seadmehalduse Exchange leiate [**siit.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))
