---
title: Apple'i automaatse seadme registreerimise sünkroonimistõrked
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 1664a26b313c4a38c9c6d78cdb89997749ba175fd3dd72f278e99bbd50b0ee84
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013744"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Apple'i automaatse seadme registreerimise sünkroonimistõrked

"Oleme tuvastanud, et teil on üks või mitu ADE/DEP-tõend, mis on tõrke olekus. Kuni iga mõjutatud loa tõrke olek on lahendatud, ei tööta ADE-funktsioon ootuspäraselt."

See tõrge võib ilmneda mitmel viisil, sh:

1. Seadmed ei pruugi sünkroonida ABM-/ASM-ilt Intune'ile
2. Registreerimisprofiilide määramised võivad nurjuda
3. Seadmed ei pruugi ADE registreerimist edukalt lõpule viia

Kontrollige, kas Intune'i konsoolis on teatatud sünkroonimistõrge jaotises Seadmed > Registreeri seadmed > Apple'i > registreerimisprogrammi **märkides.**

Üks levinumaid sünkroonimistõrgete põhjuseid on praeguse loa aegumine. Paljudel juhtudel lahendab probleemi mõjutatud loa pikendamine.

Kui üks või mitu teie tõend on aegunud, lugege järgmisi dokumente, mis aitavad teil neid vastavalt vajadusele uuendada.

[Automaatse seadme registreerimise loa uuendamine](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Lisaks saate vaadata järgmist dokumentatsiooni, et näha võimalikke tõrkeid, mis võivad põhjustada loasünkroonimistõrkeid.

[ABM/ASM-i sünkroonimistõrked iOS-i/iPadOS-i ja macOS-i automaatsete seadmete registreerimise märkide korral](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[ABM/ASM-i sünkroonimistõrked iOS-i/iPadOS-i ja macOS-i automaatsete seadmete registreerimise märkide korral](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
