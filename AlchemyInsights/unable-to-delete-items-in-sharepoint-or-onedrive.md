---
title: SharePointi või OneDrive ' is ei saa üksusi kustutada
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
ms.openlocfilehash: db45aa8df40484fdcda7c430f1ca27482a1dd4ce
ms.sourcegitcommit: a9415f3ae8c7ba267b5134bcbdc1e070cea41a0f
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 11/12/2020
ms.locfileid: "49019579"
---
# <a name="unable-to-delete-items"></a>Üksusi ei saa kustutada

- Säilituspoliitika võib seda põhjustada, peate kas keelama või välistama vastava ootelepaneku, mis seda probleemi põhjustab. Pärast säilituspoliitika või ootelepaneku eemaldamist võib muudatuse jõustumiseks kuluda kuni 24 tundi. Veenduge, et üksusel poleks [säilituspoliitika](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) seadistust.

- Võimalik, et sait on ületanud salvestusruumi piirmäära, suurendama [saidi kvooti](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) ja kustutama üksuse.

- Veenduge, et üksus poleks teise kasutaja jaoks [välja möllitud](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) .

- Administraatorid saavad kasutada [SharePointi mustreid ja tavasid](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), mis sisaldab PowerShelli käskude teeki, mis võimaldavad teil sooritada keerulisi haldus-toiminguid (nt jõu kustutamine kangekaelne üksused).
- [PNP-failis eemaldamine](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Kausta PNP eemaldamine](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [PNP-loendiüksuse eemaldamine](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [PNP-loendi eemaldamine](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Eemalda PNP väli (veerg)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)