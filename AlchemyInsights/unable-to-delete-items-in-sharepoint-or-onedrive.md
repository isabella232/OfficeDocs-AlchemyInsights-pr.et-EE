---
title: Üksuste kustutamine SharePoint või OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3601c5eff121e10b6bddace6f7228204a01080a636e24f3a56373fe8d469c799
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038513"
---
# <a name="unable-to-delete-items"></a>Üksusi ei saa kustutada

- Säilituspoliitikad võivad seda põhjustada, peate vastava ootelestuse keelama või välistama, mis seda probleemi põhjustab. Pärast säilituspoliitika või -ooteloleku eemaldamist võib muudatuse jõustumist aega võtta kuni 24 tundi. Veenduge, et üksusel [pole säilituspoliitika](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) häälestust.

- Võimalik, et sait on ületanud salvestuslimiidi, [suurendanud saidi limiiti](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) ja kustutanud üksuse.

- Veenduge, et üksus pole [teisele kasutajale](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) välja registreeritud.

- Administraatorid saavad kasutada [SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) mustreid ja tavasid (PnP), mis sisaldab PowerShelli käskude teeki, mis võimaldab teha keerukaid haldustoiminguid (nt sundida kangekaelseid üksusi kustutama).
- [PNP-faili eemaldamine](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [PNP-kausta eemaldamine](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [PNP loendiüksuse eemaldamine](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [PNP-loendi eemaldamine](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [PNP-välja eemaldamine (veerg)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)