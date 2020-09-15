---
title: IP-aadressi ja kliendi tuvastamine auditi logides
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668306"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>IP-aadressi ja kliendi tuvastamine auditi logides

Auditi logides kuvatakse Microsoft 365 kasutaja või administraatori tegevusele vastav IP-aadress. Kliendiinfo on ka logitud. Selle teabe tuvastamiseks tehke järgmist.

1. Logige sisse [Microsoft 365 turbe & nõuetele vastavuse keskuses](https://protection.office.com/).

2. Avage leht **Otsingu**  >  **auditilogi otsing** .

   Kui olete huvitatud konkreetsest tegevusest, valige see **tegevuste** loendist. Kui ei, siis tagastatakse kõik tegevused valitud kasutaja jaoks (vaikesäte).

   **Märkus**: teatud tegevused ei pruugi olla saadaval menüüs **Tegevused** ; need auditi üksused tagastatakse siis, kui valitud on **kõigi tegevuste tulemid** (vaikesäte).

3. Määrake väljal **Kasutajad** kasutajanimi, valige tegevuse jaoks sobiv kuupäevavahemik ja klõpsake siis nuppu **Otsi**.

Tulemites näete paanil tulemid selle tegevuse IP-aadressi. Valige auditi kirje, et **näha üksikasjalikku teavet hüpik (** nt klient, toimingu sooritanud kasutaja jne).

Lisateavet leiate teemast [ohustatud kontole juurdepääsemiseks kasutatava arvuti IP-aadressi leidmine](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
