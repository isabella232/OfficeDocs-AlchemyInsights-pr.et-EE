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
ms.openlocfilehash: f3614a41c1bc92184d7f8a11bd224310fef6aa0cabc8e1db1288bde01ca1cb5a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53922207"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Andmete eemaldamine ja seadmete tühjendamine Intune‘i kaudu

Seadme kasutuselt kõrvaldamise ja seadme tühjendamise kaugtoimingutega saab eemaldada Intune‘i hallatavad ettevõtteandmed või lähtestada seadme vaikesätted.

1. Logige sisse Microsoft 365 seadmehaldusesse ja valige **Seadmed** > **Kõik seadmed**.
2. Valige seade, millest soovite sisu kustutada.
3. Valige soovitud kaugkustutamise tüüp. Kasutuselt kõrvaldamise korral kustutatakse ainult asutuse teave; täielikul tühjendamisel taastatakse seadmes algsätted.
4. Kinnitamiseks valige **Jah**. Kuni tühjenduse lõpulejõudmiseni kuvatakse seadme toimingu olekuna *Kasutuselt kõrvaldamise ootel*.
    Pärast toimingu lõpulejõudmist ei kuvata seda nutiseadet enam hallatavate seadmete loendis.

> [!NOTE]
> Ettevõtte andmeid ei saa eemaldada seadmetest, mis on liidetud Azure AD-ga. 

Kasutuselt kõrvaldamise ja tühjendamise toimingute täielikud üksikasjad (sh teabe selle kohta, mis hoitakse alles ja mis kustutatakse) leiate järgmisest dokumentatsioonist:

- [Seadmete eemaldamine tühjendamise, kasutuselt kõrvaldamise või registrist käsitsi kustutamisega](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).
- [Ainult ettevõtteandmete kustutamine Intune‘i hallatavatest rakendustest](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [Kõigi andmete kustutamine macOS-i seadmest](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).