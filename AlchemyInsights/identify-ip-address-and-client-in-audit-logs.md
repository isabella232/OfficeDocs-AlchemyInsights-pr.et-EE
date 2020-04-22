---
title: IP-aadressi ja kliendi tuvastamine auditiloogides
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d1a0d412fc0c6d79e50b101ca759127522f45dcd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716384"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>IP-aadressi ja kliendi tuvastamine auditiloogides

Auditilogi kuvatakse IP-aadress, mis vastab tegevusele Microsoft 365 kasutaja või administraator. Samuti logitakse klienditeave. Siin on juhised sellise teabe tuvastamiseks

1. Logige sisse [Microsoft 365 Security & vastavuse Center](https://protection.office.com/).

2. **otsingulehele otsingu** > **auditilogi** .

   Kui olete huvitatud konkreetsest tegevusest, valige see **tegevuste** loendist. Kui ei, siis tagastatakse kõik tegevused valitud kasutajale (vaikesäte).

   **Märkus**: teatud tegevused ei pruugi olla saadaval menüüs **Tegevused** ; kuid need auditiüksused tagastatakse, kui on valitud **kõigi tegevuste Kuva tulemid** (vaikesäte).

3. Määrake kasutajanimi väljal **Kasutajad** , valige tegevuse jaoks sobiv kuupäevavahemik ja klõpsake suvandit **Otsing**.

Tulemustes näete tulemuste paanil selle tegevuse IP-aadressi. Valige auditiloend üksikasjaliku teabe kuvamiseks **üksikasjade** hüpik (nt. Klient, kasutaja, kes tegi toimingu vms).

Lisateabe saamiseks vaadake [kahjustatud kontole juurdepääsuks kasutatava arvuti IP-aadressi leidmist](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
