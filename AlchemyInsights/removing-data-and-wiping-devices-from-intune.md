---
title: Andmete eemaldamine ja seadmete tühjendamine Intune‘i kaudu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: 92673c4a2a0e0faa98d3ade5ca1f6aa687d4c94a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331037"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Andmete eemaldamine ja seadmete tühjendamine Intune‘i kaudu

Seadme kasutuselt kõrvaldamise ja seadme tühjendamise kaugtoimingutega saab eemaldada Intune‘i hallatavad ettevõtteandmed või lähtestada seadme vaikesätted.

1. Logige sisse Microsoft 365 seadmehaldusesse ja valige **Seadmed** > **Kõik seadmed**.
2. Valige seade, millest soovite sisu kustutada.
3. Valige soovitud kaugkustutamise tüüp. Kasutuselt kõrvaldamise korral kustutatakse ainult asutuse teave; täielikul tühjendamisel taastatakse seadmes algsätted.
4. Kinnitamiseks valige **Jah**. Kuni tühjenduse lõpulejõudmiseni kuvatakse seadme toimingu olekuna *Kasutuselt kõrvaldamise ootel*.
    Pärast toimingu lõpulejõudmist ei kuvata seda nutiseadet enam hallatavate seadmete loendis.

**Märkus.** Ettevõtte andmeid ei saa azure AD-ga liidetud seadmetest eemaldada. 

Kasutuselt kõrvaldamise ja tühjendamise toimingute täielikud üksikasjad (sh teabe selle kohta, mis hoitakse alles ja mis kustutatakse) leiate järgmisest dokumentatsioonist:

- [Seadmete eemaldamine tühjendamise, kasutuselt kõrvaldamise või registrist käsitsi kustutamisega](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).
- [Ainult ettevõtteandmete kustutamine Intune‘i hallatavatest rakendustest](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [Kõigi andmete kustutamine macOS-i seadmest](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).