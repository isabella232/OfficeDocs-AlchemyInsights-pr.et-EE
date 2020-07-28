---
title: Andmete eemaldamine ja seadmete eemaldamine Intune kaudu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439155"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Andmete eemaldamine ja seadmete eemaldamine Intune kaudu

Seade on kasutuselt kõrvaldatud ja seadme tühjendamiseks saab kasutada ettevõtte andmeid, mida hallatakse Intune abil või tehase lähtestamiseks ja seadme vaikesätetele tagastamiseks.

1. Logige sisse rakendusse Microsoft 365 Device Management ja valige **seadmed**  >  **kõigis seadmetes**.
2. Valige seade, mille soovite kustutada.
3. Valige eemaldatava kaugjuhtimispuldi tüüp. Pensionile kustutab ainult ettevõtte andmed, samal ajal kui täielikud salvrätikud taastavad seadme tehase seadetesse.
4. Kinnitamiseks valige **Jah** . Kui pühkimine on lõpule jõudnud, kuvatakse seadme toimingu olekuks Ootel.</br>
    Kui toiming on lõpule viidud, ei näe te hallatava seadme loendis enam mobiilsideseadmet.

**Märkus** Ettevõtte andmeid ei saa eemaldada Azure AD-ga ühendatud seadmetest.

Lisateavet selle kohta, kuidas eemaldada ja kustutada toiminguid, sealhulgas seda, mis jääb alles ja mis kustutatakse, leiate teemast [seadmete eemaldamine, kui kasutate seadme tühjendamise, pensionile jäämist või käsitsi registreerimise tühistamist](https://docs.microsoft.com/intune/devices-wipe).

Kui soovite kustutada kõik macOS-seadme andmed, lugege teemat [kõigi andmete kustutamine MacOS-seadmest](https://docs.microsoft.com/intune/device-erase).