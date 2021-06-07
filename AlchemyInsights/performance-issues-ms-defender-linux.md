---
title: Microsoft Defender for Endpointi jõudlusprobleemid Linuxis
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793759"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a>Microsoft Defender for Endpointi jõudlusprobleemid Linuxis

Selles artiklis juhendatakse teid Microsoft Defender for Endpointi jõudlusprobleemide tuvastamise juhistest Linuxis.

Oluline on esmalt veenduda, et teie probleem on lahendatud uusima [versiooniga.](/microsoft-365/security/defender-endpoint/linux-whatsnew) 

Uurimise alustamiseks lugege teemat Microsoft [Defender for Endpointi jõudlusprobleemide tõrkeotsing Linuxis.](/microsoft-365/security/defender-endpoint/linux-support-perf)

## <a name="exclusions"></a>Välistamised

Välistamised võivad aidata jõudlusprobleeme leevendada. Vaadake oma välistamised üle enne alustamist, et mis tahes täiendav risk oleks teada ja dokumenteeritud.

Lisateavet leiate teemast Microsoft Defenderi välistamiste konfigureerimine ja [valideerimine Lõpp-punkti jaoks Linuxis.](/microsoft-365/security/defender-endpoint/linux-exclusions)

Kui teil on mitu & kausta, mille soovite välistada ja need on kõik samas ühenduspunktis, võib ühenduspunkti välistamine olla lihtsam. Alates veebruari väljaandest 101.22.80 saate välistada kogu ühenduspunkti.

Näiteks kui /mnt/backup on mountpoint, saate välistamisloendisse lisada /mnt/backup, käivitades selle käsu.

`$ mdatp exclusion folder add –path /mnt/backup`

**Märkus.** Välistamiste lisamine suurendab ründevara tuvastamata jätmise ohtu ning seda tuleks käsitleda ja rakendada hoolikalt.

## <a name="need-help"></a>Kas vajate abi?

Selleks et teid kõige tõhusamal viisil aidata, koguge diagnostikaandmed enne tugiteenuse juhtumi avamist.
