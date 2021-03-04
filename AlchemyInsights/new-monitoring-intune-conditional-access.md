---
title: Tingimusjuurdepääsu Intune Accessi jälgimine
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
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427425"
---
# <a name="monitor-intune-conditional-access"></a>Tingimusjuurdepääsu Intune Accessi jälgimine

Juurdepääsuõigusega kasutajatele antakse teatise meilisõnum, kui need ei vasta teie asutuse juurdepääsu nõuetele. Lahendamiseks soovitame teha ühte või mitut järgmistest lahendustest.

1. Kui eeldatakse, et seade on registreeritud, Soovitage kasutajal minna ettevõtte portaali rakendusse ja veenduge, et see kuvatakse ettevõtte portaalis. Kui seda ei juhtu, peab kasutaja seadme registreerima.
1. Avage Azure ' i portaalis   >  **seadme nõuetele vastavuse** häälestamine. 
1. Seadme nõuetele vastavuse aruannete vaatamiseks veendumaks, et kasutaja seade on märgitud nõuetele vastavaks, klõpsake jaotises **kuvar** nuppu **seadme vastavus**.
1. Avage Azure ' i portaalis   >  **seadme nõuetele vastavuse** häälestamine. Klõpsake jaotises **haldamine** nuppu **poliitikad**. Veenduge, et nõuetele vastavuse poliitikate loendis oleks teie kasutaja seadmele määratud profiil. Kui profiili pole määratud, ei saa Intune kinnitada seadme nõuetele vastavuse olekut.
1. Kasutaja tingimusliku juurdepääsu määramise redigeerimine.
1. Liikuge Azure ' i portaalis lehele  >  **tingimusjuurdepääsu**  >  **poliitikate** häälestamine, valige loendist poliitika ja klõpsake nuppu **kasutajad ja rühmad**.
1. Kellegile teatud poliitika suunamiseks lisage need **loendisse kaasa**. Kui soovite tagada, et isik on poliitikast välja jäetud, lisage need loendisse **välista**.

**Kasulikud lingid:**

- [Seadme nõuetele vastavuse ülevaade](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Tõrkeotsing CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Tõrkeotsingu poliitika](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Seadme nõuetele vastavuse jälgimine](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> Need toimingud on abiks ainult Azure Active Directory tõrkeotsingul. Samuti on võimalik sulgeda seade, mis blokeerib juurdepääsu Exchange ' i poliitikaga. Lisateavet Exchange ' i seadmete halduse kohta leiate [**siit**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).
