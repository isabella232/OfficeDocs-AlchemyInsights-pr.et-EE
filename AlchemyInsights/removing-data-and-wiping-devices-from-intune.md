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
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416309"
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