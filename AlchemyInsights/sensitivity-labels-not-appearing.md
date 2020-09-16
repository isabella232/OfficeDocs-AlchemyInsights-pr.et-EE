---
title: Tundlikkuse sildid, mida ei esine
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 6a64e001be115c8e5553a0d8c97b8cb815922c69
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801180"
---
# <a name="sensitivity-labels-not-appearing"></a>Tundlikkuse sildid, mida ei esine

Tundlikkuse siltide abil saate oma tundliku sisu klassifitseerida ja kaitsta. Neid saab luua Microsoft 365 nõuetele vastavuse keskuses, Microsoft 365 Turvakeskus või Microsoft 365 turbe & nõuetele vastavuse Center jaotises klassifitseerimine > tundlikkuse sildid. Lisateavet selle funktsiooni kohta leiate teemast [tundlikkuse siltide ülevaade](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).

Kui olete konfigureerinud oma tundlikkuse sildid, kuid neid ei kuvata Microsoft 365 rakendustes, kontrollige järgmist.

- Kontrollige, kas tundlikkuse silt on teie soovitud kasutajatele ja rühmadele [avaldatud](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) .

- Veenduge, et kasutaja kasutab tundlikke silte toetavat rakendust – vt [dokumendis olevaid tundlikkuse silte](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).

- Kui [migreerite Azure ' i teabe kaitse silte](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), pidage silmas [siin](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)loetletud kaalutlusi.

- Andmete kaotsimineku vältimise (DLP) tugi: praegu saab DLP poliitika tingimusena kasutada ainult säilituse silte.  DLP poliitikale mõeldud tundlikkuse siltide tugi pole veel saadaval, kuid me töötame selle kallal.

- Kui krüptimine on lubatud tundlikkuse sildil, saate valida, kas soovite teha järgmist.
    - Õiguse määramine kohe
    - Kasutajatele õiguse määramise lubamine


Võimalike probleemide kohta leiate lisateavet teemast [teadaolevad probleemid tundlikkuse siltidega](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).